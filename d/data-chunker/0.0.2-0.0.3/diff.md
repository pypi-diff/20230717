# Comparing `tmp/data_chunker-0.0.2.tar.gz` & `tmp/data_chunker-0.0.3.tar.gz`

## Comparing `data_chunker-0.0.2.tar` & `data_chunker-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 data_chunker-0.0.2/src/data_chunker/__init__.py
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 data_chunker-0.0.2/src/data_chunker/java_code.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 data_chunker-0.0.2/src/data_chunker/parser.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 data_chunker-0.0.2/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 data_chunker-0.0.2/LICENSE
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 data_chunker-0.0.2/README.adoc
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 data_chunker-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 data_chunker-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/__init__.py
+-rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/java_code.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/parser.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 data_chunker-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 data_chunker-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 data_chunker-0.0.3/README.adoc
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 data_chunker-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 data_chunker-0.0.3/PKG-INFO
```

### Comparing `data_chunker-0.0.2/src/data_chunker/java_code.py` & `data_chunker-0.0.3/src/data_chunker/java_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,187 +1,195 @@
-import javalang
-
-# Declare a dict/lookup to abbreviate Java type declarations.
-declaration_types = { 
-    javalang.tree.AnnotationDeclaration: "annotation",
-    javalang.tree.ClassDeclaration: "class", 
-    javalang.tree.EnumDeclaration: "enumeration",
-    javalang.tree.InterfaceDeclaration: "interface"
-}
-
-def get_node_start_end(tree: javalang.tree.CompilationUnit,
-                       d_node: javalang.tree.Declaration) -> int | int | int | int:
-    startpos  = None
-    endpos    = None
-    startline = None
-    endline   = None
-    for path, node in tree:
-        if startpos is not None and d_node not in path:
-            endpos = node.position
-            endline = node.position.line if node.position is not None else None
-            break
-        if startpos is None and node == d_node:
-            startpos = node.position
-            startline = node.position.line if node.position is not None else None
-    return startpos, endpos, startline, endline
-
-def get_node_text(codelines: list, startpos, endpos, startline, endline, 
-                  last_endline_index) -> str | int | int | int:
-
-    if startpos is None:
-        return "", None, None, None
-
-    startline_index = startline - 1 
-    endline_index = endline - 1 if endpos is not None else None 
-
-    # 1. check for and fetch annotations
-    if last_endline_index is not None:
-        for line in codelines[(last_endline_index + 1):(startline_index)]:
-            if "@" in line: 
-                startline_index = startline_index - 1
-    node_text = "<ST>".join(codelines[startline_index:endline_index])
-    if "}" in node_text:
-        node_text = node_text[:node_text.rfind("}") + 1] 
-
-    # 2. remove trailing rbrace for last methods & any external content/comments
-    # if endpos is None and 
-    if not abs(node_text.count("}") - node_text.count("{")) == 0:
-        # imbalanced braces
-        brace_diff = abs(node_text.count("}") - node_text.count("{"))
-
-        for _ in range(brace_diff):
-            node_text  = node_text[:node_text.rfind("}")]    
-            node_text  = node_text[:node_text.rfind("}") + 1]     
-
-    node_lines = node_text.split("<ST>")  
-    node_text  = "".join(node_lines)                   
-    last_endline_index = startline_index + (len(node_lines) - 1) 
-    
-    return node_text, (startline_index + 1), (last_endline_index + 1), last_endline_index
-
-def chunk_constants( tree: javalang.tree.CompilationUnit ) -> list :
-
-    # Initialize return variables
-    chunks = []
-    # Initialize local variables
-    t = None
-    # Check that there is only one type in tree.types otherwise return
-    if len(tree.types) == 1:
-        t = tree.types[0]
-    else:
-        return chunks
-    # Attempt to read the package name (throws an error sometimes)
-    try:
-        p_name = tree.package.name
-    except AttributeError as e:
-        raise ChunkingError("Package name does not exist, raised in " + 
-                         chunk_constants.__name__)
-    # Checks that the tree has constants (TODO: still neede?)
-    if not hasattr(t.body, "constants"):
-        return chunks
-    # Loop through nodes of a given type.
-    for constant in t.body.constants:
-        c_string = constant.name
-        arg_list = []
-        if constant.arguments != None:
-            for arg in constant.arguments:
-                try:
-                    arg_list.append(arg.value)
-                except AttributeError as e:
-                    raise ChunkingError("When adding constants from" + t.name + 
-                                        ", raised in " + 
-                                        chunk_constants.__name__ + 
-                                        ": " + str(e))
-            arg_string = ", ".join(arg_list)
-            code = constant.name + "(" + arg_string + ")"
-            chunks.append({"package": str(p_name),
-                           "type": declaration_types.get(type(t)),
-                           "typename": t.name,
-                           "member": "constant",
-                           "membername": constant.name,
-                           "code": code})
-
-    return chunks
-
-def chunk_constructors(tree: javalang.tree.CompilationUnit,
-                       codelines: list) -> list:
-    node_type = javalang.tree.ConstructorDeclaration
-    return chunk_node_type(tree, node_type, "constructor", codelines)
-
-def chunk_fields(tree: javalang.tree.CompilationUnit,
-                 codelines: list) -> list:
-    node_type = javalang.tree.FieldDeclaration
-    return chunk_node_type(tree, node_type, "field", codelines)
-
-def chunk_methods(tree: javalang.tree.CompilationUnit,
-                  codelines: list) -> list:
-    node_type = javalang.tree.MethodDeclaration
-    return chunk_node_type(tree, node_type, "method", codelines)
-
-
-
-def chunk_node_type(tree: javalang.tree.CompilationUnit,
-                    node_type: javalang.tree.Declaration,
-                    mem_str: str,
-                    codelines: list) -> list:
-    # Initialize return variables
-    chunks = []
-    # Initialize local variables
-    t = None
-    # Check that there is only one type in tree.types otherwise return
-    if len(tree.types) == 1:
-        t = tree.types[0]
-    else:
-        return chunks
-    # Attempt to read the package name (throws an error sometimes)
-    try:
-        p_name = tree.package.name
-    except AttributeError as e:
-        raise ChunkingError("Package name does not exist, raised in " + 
-                         chunk_constants.__name__)
-    # Loop through nodes of a given type.
-    lex = None
-    for _, node in tree.filter(node_type):
-        startp, endp, startl, endl = get_node_start_end(tree, node)
-        code, startl, endl, lex = get_node_text(
-            codelines, startp, endp, startl, endl, lex
-        )
-        # Need this ternary operator since Fields have their names elsewhere
-        mem_name = node.name if mem_str != "field" else node.declarators[0].name
-        chunks.append({"package": p_name,
-                       "type": str(declaration_types.get(type(t))),
-                       "typename": t.name,
-                       "member": mem_str,
-                       "membername": mem_name,
-                       "code": code})
-
-    return chunks
-
-def parse_code(code_path: str, 
-               codelines: list) -> javalang.tree.CompilationUnit:
-    # Initialize return values
-    tree = None
-    # Merge list of code lines into one string
-    code_text = ''.join(codelines)
-    # Attempt to parse file; failures are recorded for return.
-    try:
-        tree = javalang.parse.parse( code_text )
-    except javalang.parser.JavaSyntaxError as e:
-        raise ParseError("Syntax error raised as JavaSyntaxError")
-    # For simplicity, consider files with anything other than one type as 
-    # failed
-    try:
-        if tree != None and len( tree.types ) != 1:
-            raise ParseError("More than one type in file, which is not " +
-                             "allowed, raised in " + str(parse_code.__name__))
-    except AttributeError as e:
-        raise ParseError("Tree's types do not exist, raised in " + 
-                         str(parse_code.__name__) + ", " + str(e))
-    return tree
-
-# Declare a couple of classes to catch exceptions, handled by calling
-# code
-class ChunkingError(Exception):
-    pass
-
-class ParseError(Exception):
-    pass
+import javalang
+
+# Declare a dict/lookup to abbreviate Java type declarations.
+declaration_types = { 
+    javalang.tree.AnnotationDeclaration: "annotation",
+    javalang.tree.ClassDeclaration: "class", 
+    javalang.tree.EnumDeclaration: "enumeration",
+    javalang.tree.InterfaceDeclaration: "interface"
+}
+
+def get_node_start_end(tree: javalang.tree.CompilationUnit,
+                       d_node: javalang.tree.Declaration) -> int | int | int | int:
+    startpos  = None
+    endpos    = None
+    startline = None
+    endline   = None
+    for path, node in tree:
+        if startpos is not None and d_node not in path:
+            endpos = node.position
+            endline = node.position.line if node.position is not None else None
+            break
+        if startpos is None and node == d_node:
+            startpos = node.position
+            startline = node.position.line if node.position is not None else None
+    return startpos, endpos, startline, endline
+
+def get_node_text(codelines: list, startpos, endpos, startline, endline, 
+                  last_endline_index) -> str | int | int | int:
+
+    if startpos is None:
+        return "", None, None, None
+
+    startline_index = startline - 1 
+    endline_index = endline - 1 if endpos is not None else None 
+
+    # 1. check for and fetch annotations
+    if last_endline_index is not None:
+        for line in codelines[(last_endline_index + 1):(startline_index)]:
+            if "@" in line: 
+                startline_index = startline_index - 1
+    node_text = "<ST>".join(codelines[startline_index:endline_index])
+    if "}" in node_text:
+        node_text = node_text[:node_text.rfind("}") + 1] 
+
+    # 2. remove trailing rbrace for last methods & any external content/comments
+    # if endpos is None and 
+    if not abs(node_text.count("}") - node_text.count("{")) == 0:
+        # imbalanced braces
+        brace_diff = abs(node_text.count("}") - node_text.count("{"))
+
+        for _ in range(brace_diff):
+            node_text  = node_text[:node_text.rfind("}")]    
+            node_text  = node_text[:node_text.rfind("}") + 1]     
+
+    node_lines = node_text.split("<ST>")  
+    node_text  = "".join(node_lines)                   
+    last_endline_index = startline_index + (len(node_lines) - 1) 
+    
+    return node_text, (startline_index + 1), (last_endline_index + 1), last_endline_index
+
+def chunk_constants( tree: javalang.tree.CompilationUnit ) -> list :
+
+    # Initialize return variables
+    chunks = []
+    # Initialize local variables
+    t = None
+
+    # Check that there is only one type in tree.types otherwise return
+    if len(tree.types) == 1:
+        t = tree.types[0]
+    else:
+        return chunks
+    # Attempt to read the package name (throws an error sometimes)
+    try:
+        p_name = tree.package.name
+    except AttributeError as e:
+        raise ChunkingError("Package name does not exist, raised in " + 
+                         chunk_constants.__name__)
+    # Checks that the tree has constants (TODO: still neede?)
+    if not hasattr(t.body, "constants"):
+        return chunks
+    # Loop through nodes of a given type.
+    for constant in t.body.constants:
+        c_string = constant.name
+        arg_list = []
+        if constant.arguments != None:
+            for arg in constant.arguments:
+                try:
+                    arg_list.append(arg.value)
+                except AttributeError as e:
+                    raise ChunkingError("When adding constants from" + t.name + 
+                                        ", raised in " + 
+                                        chunk_constants.__name__ + 
+                                        ": " + str(e))
+            arg_string = ", ".join(arg_list)
+            code = constant.name + "(" + arg_string + ")"
+            chunks.append({"package": str(p_name),
+                           "type": declaration_types.get(type(t)),
+                           "typename": t.name,
+                           "member": "constant",
+                           "membername": constant.name,
+                           "code": code})
+
+    return chunks
+
+def chunk_constructors(tree: javalang.tree.CompilationUnit,
+                       codelines: list) -> list:
+    node_type = javalang.tree.ConstructorDeclaration
+    return chunk_node_type(tree, node_type, "constructor", codelines)
+
+def chunk_fields(tree: javalang.tree.CompilationUnit,
+                 codelines: list) -> list:
+    node_type = javalang.tree.FieldDeclaration
+    return chunk_node_type(tree, node_type, "field", codelines)
+
+def chunk_methods(tree: javalang.tree.CompilationUnit,
+                  codelines: list) -> list:
+    node_type = javalang.tree.MethodDeclaration
+    return chunk_node_type(tree, node_type, "method", codelines)
+
+
+
+def chunk_node_type(tree: javalang.tree.CompilationUnit,
+                    node_type: javalang.tree.Declaration,
+                    mem_str: str,
+                    codelines: list) -> list:
+    # Initialize return variables
+    chunks = []
+    # Initialize local variables
+    t = None
+    # Check that there is only one type in tree.types otherwise return
+    if len(tree.types) == 1:
+        t = tree.types[0]
+    else:
+        return chunks
+    # Attempt to read the package name (throws an error sometimes)
+    try:
+        p_name = tree.package.name
+    except AttributeError as e:
+        raise ChunkingError("Package name does not exist, raised in " + 
+                         chunk_constants.__name__)
+    # Loop through nodes of a given type.
+    lex = None
+    for _, node in tree.filter(node_type):
+        startp, endp, startl, endl = get_node_start_end(tree, node)
+        code, startl, endl, lex = get_node_text(
+            codelines, startp, endp, startl, endl, lex
+        )
+        # Need this ternary operator since Fields have their names elsewhere
+        mem_name = node.name if mem_str != "field" else node.declarators[0].name
+        chunks.append({"package": p_name,
+                       "type": str(declaration_types.get(type(t))),
+                       "typename": t.name,
+                       "member": mem_str,
+                       "membername": mem_name,
+                       "code": code})
+
+    return chunks
+
+def parse_code(code_path: str, 
+               codelines: list) -> javalang.tree.CompilationUnit:
+
+    # Initialize return values
+    tree = None
+
+    # Merge list of code lines into one string
+    code_text = ''.join(codelines)
+
+    # Attempt to parse file; failures are recorded for return.
+    #tree = javalang.parse.parse( code_text )
+    try:
+        tree = javalang.parse.parse( code_text )
+    except javalang.parser.JavaSyntaxError as e:
+        raise ParseError("Syntax error raised as JavaSyntaxError")
+    except javalang.tokenizer.LexerError as le:
+        raise ParseError("Tokenizer error raised as LexerError")
+
+    # For simplicity, consider files with anything other than one type as 
+    # failed
+    try:
+        if tree != None and len( tree.types ) != 1:
+            raise ParseError("More than one type in file, which is not " +
+                             "allowed, raised in " + str(parse_code.__name__))
+    except AttributeError as e:
+        raise ParseError("Tree's types do not exist, raised in " + 
+                         str(parse_code.__name__) + ", " + str(e))
+    return tree
+
+# Declare a couple of classes to catch exceptions, handled by calling
+# code
+class ChunkingError(Exception):
+    pass
+
+class ParseError(Exception):
+    pass
```

### Comparing `data_chunker-0.0.2/LICENSE` & `data_chunker-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 BreakFree Solutions
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 BreakFree Solutions
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `data_chunker-0.0.2/README.adoc` & `data_chunker-0.0.3/README.adoc`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-= data-chunker
-
-Python library that chunks code into a Python list consisting of Python dictionaries. This list of dictionaries can then be used for vector-store creation, which can provide granular context for OpenAI queries.
-
-Current list of languages that can be chunked:
-
-* Java (packages, methods, and variables)
-
-== Modules
-=== parser.py
-* Contains functions to read code lines from given files and file paths
-* get_file_list(code_path, file_extension) - returns a list of files from the path passed in
-* get_code_lines(file) - returns the code from the file name passed in
-
-=== java_code.py
-* Contains functions to split java files into smaller chunks
-
-== Contributing
-
-The GitHub repository for this package is https://github.com/break-free/data-chunker.
-
-The `main` branch is protected therefore any contributions require a branch to be created. Branch names should be preprended with either `feat/` or `fix/` to indicate whether new functionality or a refactor/fix is being made (e.g, `fix/update-readme`). Once the branch is complete, it can be merged back into `main`.
-
-The repository includes additional directories, such as `setup`, `info`, and `training`, and files such as `main.py`, that includes additional resources for development and usage examples.
-
-== Packaging
-
-This Python package was produced using https://hatch.pypa.io/latest/config/build/[hatchling]. Refer to the `pyproject.toml` for specifics.
-
-Recommend reading the following sites to get familiar with Python packages and uploading to https://pypi.org.
-
-* https://packaging.python.org/en/latest/tutorials/packaging-projects/[Packaging Python Projects].
-* https://hatch.pypa.io/latest/config/build/[Hatchling - Build Configuration].
-* https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#uploading-your-project-to-pypi[Uploading your Project to PyPI].
-* https://pypi.org/project/keyring/[keyring] (useful for keeping PyPI login safe).
-
-== Notes
-
-This code has been battle-tested with *one* application. If you encounter any issues then please https://github.com/break-free/java-code-chunker/issues[submit an issue ticket here on GitHub].
+= data-chunker
+
+Python library that chunks code into a Python list consisting of Python dictionaries. This list of dictionaries can then be used for vector-store creation, which can provide granular context for OpenAI queries.
+
+Current list of languages that can be chunked:
+
+* Java (packages, methods, and variables)
+
+== Modules
+=== parser.py
+* Contains functions to read code lines from given files and file paths
+* get_file_list(code_path, file_extension) - returns a list of files from the path passed in
+* get_code_lines(file) - returns the code from the file name passed in
+
+=== java_code.py
+* Contains functions to split java files into smaller chunks
+
+== Contributing
+
+The GitHub repository for this package is https://github.com/break-free/data-chunker.
+
+The `main` branch is protected therefore any contributions require a branch to be created. Branch names should be preprended with either `feat/` or `fix/` to indicate whether new functionality or a refactor/fix is being made (e.g, `fix/update-readme`). Once the branch is complete, it can be merged back into `main`.
+
+The repository includes additional directories, such as `setup`, `info`, and `training`, and files such as `main.py`, that includes additional resources for development and usage examples.
+
+== Packaging
+
+This Python package was produced using https://hatch.pypa.io/latest/config/build/[hatchling]. Refer to the `pyproject.toml` for specifics.
+
+Recommend reading the following sites to get familiar with Python packages and uploading to https://pypi.org.
+
+* https://packaging.python.org/en/latest/tutorials/packaging-projects/[Packaging Python Projects].
+* https://hatch.pypa.io/latest/config/build/[Hatchling - Build Configuration].
+* https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#uploading-your-project-to-pypi[Uploading your Project to PyPI].
+* https://pypi.org/project/keyring/[keyring] (useful for keeping PyPI login safe).
+
+== Notes
+
+This code has been battle-tested with *one* application. If you encounter any issues then please https://github.com/break-free/java-code-chunker/issues[submit an issue ticket here on GitHub].
```

### Comparing `data_chunker-0.0.2/PKG-INFO` & `data_chunker-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-chunker
-Version: 0.0.2
+Version: 0.0.3
 Summary: Chunks code into a list made up of indexable dictionaries.
 Project-URL: Homepage, https://github.com/break-free/data-chunker
 Project-URL: Issues, https://github.com/break-free/data-chunker/issues
 Author-email: Chris Mills <cmills@breakfreesolutions.com>, Colin Pitawanakwat <cpitawanakwat@breakfreesolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

