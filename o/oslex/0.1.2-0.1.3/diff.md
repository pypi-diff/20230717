# Comparing `tmp/oslex-0.1.2.tar.gz` & `tmp/oslex-0.1.3.tar.gz`

## Comparing `oslex-0.1.2.tar` & `oslex-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 oslex-0.1.2/.editorconfig
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 oslex-0.1.2/pyproject.toml2
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 oslex-0.1.2/oslex/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oslex-0.1.2/oslex/py.typed
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 oslex-0.1.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oslex-0.1.2/LICENSE
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 oslex-0.1.2/README.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 oslex-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 oslex-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 oslex-0.1.3/.editorconfig
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 oslex-0.1.3/oslex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oslex-0.1.3/oslex/py.typed
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 oslex-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oslex-0.1.3/LICENSE
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 oslex-0.1.3/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 oslex-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 oslex-0.1.3/PKG-INFO
```

### Comparing `oslex-0.1.2/pyproject.toml2` & `oslex-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "oslex"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name="Tamás PEREGI", email="petamas@gmail.com" },
 ]
 description = "OS-independent wrapper for shlex and mslex"
 readme = "README.md"
 # mslex is supposed to support >=3.5, but it has an accidental f-string, making it unusable on 3.5
 # see https://github.com/smoofra/mslex/issues/1
@@ -29,10 +29,7 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/petamas/oslex"
 "Bug Tracker" = "https://github.com/petamas/oslex/issues"
-
-[tool.hatch.build.targets.wheel.force-include]
-"py.typed" = "py.typed"
```

### Comparing `oslex-0.1.2/oslex/__init__.py` & `oslex-0.1.3/oslex/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from typing import List
 
 
 def is_posix() -> bool:
     """
     Returns whether the system running Python is POSIX compatible.
     This is the condition for oslex.underlying being shlex.
     This is also the condition for os.path being posixpath.
@@ -43,23 +44,23 @@
     """
     Return a shell-escaped version of the string s. The returned value is a string that can safely be used as one token in a shell command line, for cases where you cannot use a list.
     This function is safe to use both for POSIX-compatible shells and for Windows's cmd.
     """
     return underlying.quote(s)
 
 
-def split(s: str) -> list[str]:
+def split(s: str) -> List[str]:
     """
     Split the string s using shell-like syntax.
     This function is safe to use both for POSIX-compatible shells and for Windows's cmd.
     """
     return underlying.split(s)
 
 
-def join(split_command: list[str]) -> str:
+def join(split_command: List[str]) -> str:
     """
     Concatenate the tokens of the list split_command and return a string. This function is the inverse of split().
     The returned value is shell-escaped to protect against injection vulnerabilities (see quote()).
     This function is safe to use both for POSIX-compatible shells and for Windows's cmd.
     """
     # shlex only has join() since Python 3.8
     # mslex doesn't have it at all
```

### Comparing `oslex-0.1.2/.gitignore` & `oslex-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oslex-0.1.2/LICENSE` & `oslex-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oslex-0.1.2/README.md` & `oslex-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oslex-0.1.2/PKG-INFO` & `oslex-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslex
-Version: 0.1.2
+Version: 0.1.3
 Summary: OS-independent wrapper for shlex and mslex
 Project-URL: Homepage, https://github.com/petamas/oslex
 Project-URL: Bug Tracker, https://github.com/petamas/oslex/issues
 Author-email: Tamás PEREGI <petamas@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

