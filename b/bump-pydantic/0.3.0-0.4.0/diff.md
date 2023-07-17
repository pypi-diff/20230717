# Comparing `tmp/bump_pydantic-0.3.0.tar.gz` & `tmp/bump_pydantic-0.4.0.tar.gz`

## Comparing `bump_pydantic-0.3.0.tar` & `bump_pydantic-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/__main__.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/py.typed
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/__init__.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/add_default_none.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/field.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/mypy_visitor.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/replace_config.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/replace_generic_model.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/replace_imports.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/root_model.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/bump_pydantic/codemods/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/case.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/file.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/folder.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/__init__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/add_none.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/base_settings.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/config_to_model.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/field.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/folder_inside_folder.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/is_base_model.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/replace_validator.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/integration/cases/root_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_add_default_none.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_class_def_visitor.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_field.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_generic_model.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_replace_config.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_replace_imports.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_root_model.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/tests/unit/test_validator.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/README.md
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 bump_pydantic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/__main__.py
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/py.typed
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/__init__.py
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/add_default_none.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/con_func.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/field.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/mypy_visitor.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_config.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_generic_model.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_imports.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/root_model.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/case.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/file.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/folder.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/add_none.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/base_settings.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/con_func.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/config_to_model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/field.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/folder_inside_folder.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/is_base_model.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/replace_validator.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/root_model.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/unicode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_add_default_none.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_class_def_visitor.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_con_func.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_field.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_generic_model.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_replace_config.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_replace_imports.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_root_model.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_validator.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/README.md
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/PKG-INFO
```

### Comparing `bump_pydantic-0.3.0/.github/workflows/main.yml` & `bump_pydantic-0.4.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,24 @@
   push:
     branches:
       - main
     tags:
       - '**'
   pull_request: {}
 
+env:
+  PYTHONWARNDEFAULTENCODING: true
+
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
+
       - name: set up python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: Install hatch
         run: pip install hatch
@@ -34,15 +38,16 @@
     timeout-minutes: 30
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
+
       - name: set up python
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python-version }}"
 
       - name: Install hatch
         run: pip install hatch
@@ -69,15 +74,15 @@
     runs-on: ubuntu-latest
     environment: release
 
     permissions:
       id-token: write
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: set up python
         uses: actions/setup-python@v4
         with:
           python-version: '3.10'
 
       - name: install
```

### Comparing `bump_pydantic-0.3.0/bump_pydantic/.github/workflows/ci.yml` & `bump_pydantic-0.4.0/bump_pydantic/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/__init__.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import List, Type
 
 from libcst.codemod import ContextAwareTransformer
 from libcst.codemod.visitors import AddImportsVisitor, RemoveImportsVisitor
 
 from bump_pydantic.codemods.add_default_none import AddDefaultNoneCommand
+from bump_pydantic.codemods.con_func import ConFuncCallCommand
 from bump_pydantic.codemods.field import FieldCodemod
 from bump_pydantic.codemods.replace_config import ReplaceConfigCodemod
 from bump_pydantic.codemods.replace_generic_model import ReplaceGenericModelCommand
 from bump_pydantic.codemods.replace_imports import ReplaceImportsCodemod
 from bump_pydantic.codemods.root_model import RootModelCommand
 from bump_pydantic.codemods.validator import ValidatorCodemod
 
@@ -24,25 +25,31 @@
     """Replace imports that have been moved."""
     BP005 = "BP005"
     """Replace `GenericModel` with `BaseModel`."""
     BP006 = "BP006"
     """Replace `BaseModel.__root__ = T` with `RootModel[T]`."""
     BP007 = "BP007"
     """Replace `@validator` with `@field_validator`."""
+    BP008 = "BP008"
+    """Replace `constr(<args>)` with `Annotated[str, StringConstraints(<args>)`."""
 
 
 def gather_codemods(disabled: List[Rule]) -> List[Type[ContextAwareTransformer]]:
     codemods: List[Type[ContextAwareTransformer]] = []
 
     if Rule.BP001 not in disabled:
         codemods.append(AddDefaultNoneCommand)
 
     if Rule.BP002 not in disabled:
         codemods.append(ReplaceConfigCodemod)
 
+    # The `ConFuncCallCommand` needs to run before the `FieldCodemod`.
+    if Rule.BP008 not in disabled:
+        codemods.append(ConFuncCallCommand)
+
     if Rule.BP003 not in disabled:
         codemods.append(FieldCodemod)
 
     if Rule.BP004 not in disabled:
         codemods.append(ReplaceImportsCodemod)
 
     if Rule.BP005 not in disabled:
```

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/add_default_none.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/add_default_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/field.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/mypy_visitor.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/mypy_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/replace_config.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/replace_generic_model.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/replace_imports.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/root_model.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/bump_pydantic/codemods/validator.py` & `bump_pydantic-0.4.0/bump_pydantic/codemods/validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/integration/folder.py` & `bump_pydantic-0.4.0/tests/integration/folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         path = root / self.name
         path.mkdir()
 
         for file in self.files:
             if isinstance(file, Folder):
                 file.create_structure(path)
             else:
-                (path / file.name).write_text(file.content)
+                (path / file.name).write_text(file.content, encoding="utf-8")
 
     @classmethod
     def from_structure(cls, root: Path) -> Folder:
         name = root.name
         files: list[File | Folder] = []
 
         for path in root.iterdir():
             if path.is_dir():
                 files.append(cls.from_structure(path))
             else:
-                files.append(File(path.name, path.read_text().splitlines()))
+                files.append(File(path.name, path.read_text(encoding="utf-8").splitlines()))
 
         return Folder(name, *files)
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, File):
             return False
```

### Comparing `bump_pydantic-0.3.0/tests/integration/test_cli.py` & `bump_pydantic-0.4.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/__init__.py` & `bump_pydantic-0.4.0/tests/integration/cases/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from ..case import Case
 from ..file import File
 from ..folder import Folder
 from .add_none import cases as add_none_cases
 from .base_settings import cases as base_settings_cases
+from .con_func import cases as con_func_cases
 from .config_to_model import cases as config_to_model_cases
 from .field import cases as generic_model_cases
 from .folder_inside_folder import cases as folder_inside_folder_cases
 from .is_base_model import cases as is_base_model_cases
 from .replace_validator import cases as replace_validator_cases
 from .root_model import cases as root_model_cases
+from .unicode import cases as unicode_cases
 
 cases = [
     Case(
-        id="empty",
-        input=File("__init__.py", content=[]),
+        name="empty",
+        source=File("__init__.py", content=[]),
         expected=File("__init__.py", content=[]),
     ),
     *base_settings_cases,
     *add_none_cases,
     *is_base_model_cases,
     *replace_validator_cases,
     *config_to_model_cases,
     *root_model_cases,
     *generic_model_cases,
     *folder_inside_folder_cases,
+    *unicode_cases,
+    *con_func_cases,
 ]
-before = Folder("project", *[case.input for case in cases])
+before = Folder("project", *[case.source for case in cases])
 expected = Folder("project", *[case.expected for case in cases])
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/add_none.py` & `bump_pydantic-0.4.0/tests/integration/cases/add_none.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="Add None",
-        input=File(
+        name="Add None",
+        source=File(
             "add_none.py",
             content=[
                 "from typing import Any, Dict, Optional, Union",
                 "",
                 "from pydantic import BaseModel, Field",
                 "",
                 "",
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/base_settings.py` & `bump_pydantic-0.4.0/tests/integration/cases/base_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="BaseSettings import",
-        input=File(
+        name="BaseSettings import",
+        source=File(
             "settings.py",
             content=[
                 "from pydantic import BaseSettings",
                 "",
                 "",
                 "class Settings(BaseSettings):",
                 "    a: int",
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/config_to_model.py` & `bump_pydantic-0.4.0/tests/integration/cases/replace_validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,82 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="Replace Config class to model",
-        input=File(
-            "config_to_model.py",
+        name="Replace validator",
+        source=File(
+            "replace_validator.py",
             content=[
-                "from pydantic import BaseModel",
+                "from pydantic import BaseModel, validator, root_validator",
                 "",
                 "",
                 "class A(BaseModel):",
-                "    class Config:",
-                "        orm_mode = True",
-                "        validate_all = True",
-                "",
-                "",
-                "class BaseConfig:",
-                "    orm_mode = True",
-                "    validate_all = True",
+                "    a: int",
+                "    b: str",
                 "",
-                "",
-                "class B(BaseModel):",
-                "    class Config(BaseConfig):",
-                "        ...",
+                "    @validator('a')",
+                "    def validate_a(cls, v):",
+                "        return v + 1",
+                "",
+                "    @root_validator()",
+                "    def validate_b(cls, values):",
+                "        return values",
             ],
         ),
         expected=File(
-            "config_to_model.py",
+            "replace_validator.py",
             content=[
-                "from pydantic import ConfigDict, BaseModel",
+                "from pydantic import field_validator, model_validator, BaseModel",
                 "",
                 "",
                 "class A(BaseModel):",
-                "    model_config = ConfigDict(from_attributes=True, validate_default=True)",
-                "",
-                "",
-                "class BaseConfig:",
-                "    orm_mode = True",
-                "    validate_all = True",
+                "    a: int",
+                "    b: str",
                 "",
-                "",
-                "class B(BaseModel):",
-                "    # TODO[pydantic]: The `Config` class inherits from another class, please create the `model_config` manually.",  # noqa: E501
-                "    # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.",
-                "    class Config(BaseConfig):",
-                "        ...",
+                "    @field_validator('a')",
+                "    @classmethod",
+                "    def validate_a(cls, v):",
+                "        return v + 1",
+                "",
+                "    @model_validator()",
+                "    @classmethod",
+                "    def validate_b(cls, values):",
+                "        return values",
             ],
         ),
     ),
     Case(
-        id="Replace Config class on BaseSettings",
-        input=File(
-            "config_dict_and_settings.py",
+        name="Replace validator with pre=True",
+        source=File(
+            "const_to_literal.py",
             content=[
-                "from pydantic import BaseModel, BaseSettings",
-                "",
-                "",
-                "class Settings(BaseSettings):",
-                "    sentry_dsn: str",
+                "from enum import Enum",
+                "from pydantic import BaseModel, Field",
                 "",
-                "    class Config:",
-                "        orm_mode = True",
                 "",
+                "class A(str, Enum):",
+                "    a = 'a'",
+                "    b = 'b'",
                 "",
                 "class A(BaseModel):",
-                "    class Config:",
-                "        orm_mode = True",
+                "    a: A = Field(A.a, const=True)",
             ],
         ),
         expected=File(
-            "config_dict_and_settings.py",
+            "const_to_literal.py",
             content=[
-                "from pydantic import ConfigDict, BaseModel",
-                "from pydantic_settings import BaseSettings, SettingsConfigDict",
-                "",
+                "from enum import Enum",
+                "from pydantic import BaseModel",
+                "from typing import Literal",
                 "",
-                "class Settings(BaseSettings):",
-                "    sentry_dsn: str",
-                "    model_config = SettingsConfigDict(from_attributes=True)",
                 "",
+                "class A(str, Enum):",
+                "    a = 'a'",
+                "    b = 'b'",
                 "",
                 "class A(BaseModel):",
-                "    model_config = ConfigDict(from_attributes=True)",
+                "    a: Literal[A.a] = A.a",
             ],
         ),
     ),
 ]
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/field.py` & `bump_pydantic-0.4.0/tests/integration/cases/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="Replace Fields",
-        input=File(
+        name="Replace Fields",
+        source=File(
             "field.py",
             content=[
                 "from pydantic import BaseModel, Field",
                 "",
                 "",
                 "class A(BaseModel):",
                 "    a: List[int] = Field(..., min_items=1, max_items=10)",
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/folder_inside_folder.py` & `bump_pydantic-0.4.0/tests/integration/cases/folder_inside_folder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ..case import Case
 from ..file import File
 from ..folder import Folder
 
 cases = [
     Case(
-        id="Add Folder",
-        input=Folder(
+        name="Add Folder",
+        source=Folder(
             "folder",
             File("__init__.py", content=[]),
             File(
                 "file.py",
                 content=[
                     "from typing import Optional, Union",
                     "",
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/is_base_model.py` & `bump_pydantic-0.4.0/tests/integration/cases/is_base_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="Make sure is BaseModel",
-        input=File(
+        name="Make sure is BaseModel",
+        source=File(
             "a.py",
             content=[
                 "from pydantic import BaseModel",
                 "",
                 "",
                 "class A(BaseModel):",
                 "    a: int",
@@ -30,16 +30,16 @@
                 "",
                 "class D:",
                 "    d: int",
             ],
         ),
     ),
     Case(
-        id="Make sure is BaseModel",
-        input=File(
+        name="Make sure is BaseModel",
+        source=File(
             "b.py",
             content=[
                 "from pydantic import BaseModel",
                 "from .a import A, D",
                 "from typing import Optional",
                 "",
                 "",
@@ -65,16 +65,16 @@
                 "",
                 "class C(D):",
                 "    c: Optional[int]",
             ],
         ),
     ),
     Case(
-        id="Make sure is BaseModel",
-        input=File(
+        name="Make sure is BaseModel",
+        source=File(
             "c.py",
             content=[
                 "from pydantic import BaseModel",
                 "from .d import D",
                 "",
                 "",
                 "class C(D):",
@@ -90,16 +90,16 @@
                 "",
                 "class C(D):",
                 "    c: Optional[int] = None",
             ],
         ),
     ),
     Case(
-        id="Make sure is BaseModel",
-        input=File(
+        name="Make sure is BaseModel",
+        source=File(
             "d.py",
             content=[
                 "from pydantic import BaseModel",
                 "",
                 "",
                 "class D(BaseModel):",
                 "    d: int",
```

### Comparing `bump_pydantic-0.3.0/tests/integration/cases/root_model.py` & `bump_pydantic-0.4.0/tests/integration/cases/root_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..case import Case
 from ..file import File
 
 cases = [
     Case(
-        id="Replace __root__ by RootModel",
-        input=File(
+        name="Replace __root__ by RootModel",
+        source=File(
             "root_model.py",
             content=[
                 "from pydantic import BaseModel",
                 "",
                 "",
                 "class A(BaseModel):",
                 "    __root__ = int",
```

### Comparing `bump_pydantic-0.3.0/tests/unit/test_add_default_none.py` & `bump_pydantic-0.4.0/tests/unit/test_add_default_none.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def test_no_annotations(self) -> None:
         source = textwrap.dedent(
             """class Potato:
             a: Optional[str]
         """
         )
         module = self.add_default_none("some/test/module.py", source)
-        self.assertEqual(module.code, source)
+        assert module.code == source
 
     def test_with_optional(self) -> None:
         module = self.add_default_none(
             "some/test/module.py",
             """
             from pydantic import BaseModel
 
@@ -53,15 +53,15 @@
         expected = textwrap.dedent(
             """from pydantic import BaseModel
 
 class Potato(BaseModel):
     a: Optional[str] = None
 """
         )
-        self.assertEqual(module.code, expected)
+        assert module.code == expected
 
     def test_with_union_none(self) -> None:
         module = self.add_default_none(
             "some/test/module.py",
             """
             from pydantic import BaseModel
             from typing import Union
@@ -74,15 +74,15 @@
             """from pydantic import BaseModel
 from typing import Union
 
 class Potato(BaseModel):
     a: Union[str, None] = None
 """
         )
-        self.assertEqual(module.code, expected)
+        assert module.code == expected
 
     def test_with_multiple_classes(self) -> None:
         module = self.add_default_none(
             "some/test/module.py",
             """
             from pydantic import BaseModel
             from typing import Optional
@@ -101,15 +101,15 @@
 class Potato(BaseModel):
     a: Optional[str] = None
 
 class Carrot(Potato):
     b: Optional[str] = None
             """
         )
-        self.assertEqual(module.code, expected)
+        assert module.code == expected
 
     def test_any(self) -> None:
         module = self.add_default_none(
             "some/test/module.py",
             """
             from pydantic import BaseModel
             from typing import Any
@@ -122,15 +122,15 @@
             """from pydantic import BaseModel
 from typing import Any
 
 class Potato(BaseModel):
     a: Any = None
 """
         )
-        self.assertEqual(module.code, expected)
+        assert module.code == expected
 
     @pytest.mark.xfail(reason="Recursive Union is not supported")
     def test_union_of_union(self) -> None:
         module = self.add_default_none(
             "some/test/module.py",
             """
             from pydantic import BaseModel
@@ -144,8 +144,8 @@
             """from pydantic import BaseModel
 from typing import Union
 
 class Potato(BaseModel):
     a: Union[Union[str, None], int] = None
 """
         )
-        self.assertEqual(module.code, expected)
+        assert module.code == expected
```

### Comparing `bump_pydantic-0.3.0/tests/unit/test_class_def_visitor.py` & `bump_pydantic-0.4.0/tests/unit/test_class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_field.py` & `bump_pydantic-0.4.0/tests/unit/test_field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_generic_model.py` & `bump_pydantic-0.4.0/tests/unit/test_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_replace_config.py` & `bump_pydantic-0.4.0/tests/unit/test_replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_replace_imports.py` & `bump_pydantic-0.4.0/tests/unit/test_replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_root_model.py` & `bump_pydantic-0.4.0/tests/unit/test_root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/tests/unit/test_validator.py` & `bump_pydantic-0.4.0/tests/unit/test_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/.gitignore` & `bump_pydantic-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/LICENSE.txt` & `bump_pydantic-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.3.0/README.md` & `bump_pydantic-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,38 @@
+Metadata-Version: 2.1
+Name: bump-pydantic
+Version: 0.4.0
+Summary: Convert Pydantic from V1 to V2 ♻
+Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
+Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
+Project-URL: Source, https://github.com/pydantic/bump-pydantic
+Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pydantic
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: libcst
+Requires-Dist: mypy
+Requires-Dist: rich
+Requires-Dist: typer>=0.7.0
+Requires-Dist: typing-extensions
+Description-Content-Type: text/markdown
+
 # Bump Pydantic ♻️
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
-[![PyPI - License](https://img.shields.io/pypi/l/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
 Bump Pydantic is a tool to help you migrate your code from Pydantic V1 to V2.
 
 
 > **Note**
 > If you find bugs, please report them on the [issue tracker](https://github.com/pydantic/bump-pydantic/issues/new).
@@ -23,15 +49,15 @@
     - [BP001: Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields](#bp001-add-default-none-to-optionalt-uniont-none-and-any-fields)
     - [BP002: Replace `Config` class by `model_config` attribute](#bp002-replace-config-class-by-model_config-attribute)
     - [BP003: Replace `Field` old parameters to new ones](#bp003-replace-field-old-parameters-to-new-ones)
     - [BP004: Replace imports](#bp004-replace-imports)
     - [BP005: Replace `GenericModel` by `BaseModel`](#bp005-replace-genericmodel-by-basemodel)
     - [BP006: Replace `__root__` by `RootModel`](#bp006-replace-__root__-by-rootmodel)
     - [BP007: Replace decorators](#bp007-replace-decorators)
-    <!-- - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter) -->
+    - [BP008: Replace `con*` functions by `Annotated` versions](#bp008-replace-con-functions-by-annotated-versions)
   - [License](#license)
 
 ---
 
 ## Installation
 
 The installation is as simple as:
@@ -53,23 +79,23 @@
 ```
 
 ### Check diff before applying changes
 
 To check the diff before applying the changes, you can run:
 
 ```bash
-bump-pydantic --diff <package>
+bump-pydantic --diff <path>
 ```
 
 ### Apply changes
 
 To apply the changes, you can run:
 
 ```bash
-bump-pydantic <package>
+bump-pydantic <path>
 ```
 
 ## Rules
 
 You can find below the list of rules that are applied by `bump-pydantic`.
 
 It's also possible to disable rules by using the `--disable` option.
@@ -256,16 +282,47 @@
         return v
 
     @model_validator(mode='before')
     def validate_root(cls, values):
         return values
 ```
 
-<!--
-### BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
+### BP008: Replace `con*` functions by `Annotated` versions
+
+- ✅ Replace `constr(*args)` by `Annotated[str, StringConstraints(*args)]`.
+- ✅ Replace `conint(*args)` by `Annotated[int, Field(*args)]`.
+- ✅ Replace `confloat(*args)` by `Annotated[float, Field(*args)]`.
+- ✅ Replace `conbytes(*args)` by `Annotated[bytes, Field(*args)]`.
+- ✅ Replace `condecimal(*args)` by `Annotated[Decimal, Field(*args)]`.
+- ✅ Replace `conset(T, *args)` by `Annotated[Set[T], Field(*args)]`.
+- ✅ Replace `confrozenset(T, *args)` by `Annotated[Set[T], Field(*args)]`.
+- ✅ Replace `conlist(T, *args)` by `Annotated[List[T], Field(*args)]`.
+
+The following code will be transformed:
+
+```py
+from pydantic import BaseModel, constr
+
+
+class User(BaseModel):
+    name: constr(min_length=1)
+```
+
+Into:
+
+```py
+from pydantic import BaseModel, StringConstraints
+from typing_extensions import Annotated
+
+
+class User(BaseModel):
+    name: Annotated[str, StringConstraints(min_length=1)]
+```
+
+<!-- ### BP009: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
 
 - ✅ Replace `pydantic.parse_obj_as(T, obj)` to `pydantic.TypeAdapter(T).validate_python(obj)`.
 
 
 The following code will be transformed:
 
 ```py
@@ -298,15 +355,38 @@
 
 
 class Users(BaseModel):
     users: List[User]
 
 
 users = TypeAdapter(Users).validate_python({'users': [{'name': 'John'}]})
+``` -->
+
+<!-- ### BP010: Replace `PyObject` by `ImportString`
+
+- ✅ Replace `PyObject` by `ImportString`.
+
+The following code will be transformed:
+
+```py
+from pydantic import BaseModel, PyObject
+
+
+class User(BaseModel):
+    name: PyObject
 ```
--->
+
+Into:
+
+```py
+from pydantic import BaseModel, ImportString
+
+
+class User(BaseModel):
+    name: ImportString
+``` -->
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `bump_pydantic-0.3.0/pyproject.toml` & `bump_pydantic-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,61 +33,62 @@
 bump-pydantic = "bump_pydantic.main:app"
 
 [tool.hatch.version]
 path = "bump_pydantic/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
+  "black>=23.1.0",
   "coverage[toml]>=6.5",
-  "pytest",
-  "rich",
+  "mypy>=1.0.0",
   "pydantic",
   "pytest-xdist",
+  "pytest",
+  "rich",
   "rtoml",
-  "black>=23.1.0",
-  "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
 
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
+cov-report = ["- coverage combine", "coverage report"]
+format = ["black {args:.}", "ruff --fix {args:.}"]
 lint = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mypy {args:bump_pydantic tests}",
 ]
-format = ["black {args:.}", "ruff --fix {args:.}"]
+test = "pytest {args:tests}"
+test-cov = "coverage run -m pytest {args:tests}"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.black]
-target-version = ["py38"]
-skip-string-normalization = true
 line-length = 120
+skip-string-normalization = true
+target-version = ["py38"]
 
 [tool.ruff]
+extend-select = ['A', 'B', 'C4', 'C90', 'I', 'Q', 'PERF', 'PT', 'RUF100', 'UP', 'W']
+ignore = ['B008']  # That's how Typer works.
+isort = { known-first-party = ['bump_pydantic', 'tests'] }
 line-length = 120
-extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
 mccabe = { max-complexity = 14 }
-isort = { known-first-party = ['bump_pydantic', 'tests'] }
 target-version = 'py38'
 
 [tool.pytest.ini_options]
 xfail_strict = true
 
 [tool.coverage.run]
-source_pkgs = ["bump_pydantic"]
 branch = true
+source_pkgs = ["bump_pydantic"]
 
 [tool.coverage.report]
-show_missing = true
-skip_covered = true
 exclude_lines = [
-  "pragma: nocover",
-  "pragma: no cover",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
+  "pragma: no cover",
+  "pragma: nocover",
 ]
+show_missing = true
+skip_covered = true
```

### Comparing `bump_pydantic-0.3.0/PKG-INFO` & `bump_pydantic-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,11 @@
-Metadata-Version: 2.1
-Name: bump-pydantic
-Version: 0.3.0
-Summary: Convert Pydantic from V1 to V2 ♻
-Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
-Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
-Project-URL: Source, https://github.com/pydantic/bump-pydantic
-Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
-License-Expression: MIT
-License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pydantic
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Requires-Dist: libcst
-Requires-Dist: mypy
-Requires-Dist: rich
-Requires-Dist: typer>=0.7.0
-Requires-Dist: typing-extensions
-Description-Content-Type: text/markdown
-
 # Bump Pydantic ♻️
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
-[![PyPI - License](https://img.shields.io/pypi/l/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
 Bump Pydantic is a tool to help you migrate your code from Pydantic V1 to V2.
 
 
 > **Note**
 > If you find bugs, please report them on the [issue tracker](https://github.com/pydantic/bump-pydantic/issues/new).
@@ -50,15 +22,15 @@
     - [BP001: Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields](#bp001-add-default-none-to-optionalt-uniont-none-and-any-fields)
     - [BP002: Replace `Config` class by `model_config` attribute](#bp002-replace-config-class-by-model_config-attribute)
     - [BP003: Replace `Field` old parameters to new ones](#bp003-replace-field-old-parameters-to-new-ones)
     - [BP004: Replace imports](#bp004-replace-imports)
     - [BP005: Replace `GenericModel` by `BaseModel`](#bp005-replace-genericmodel-by-basemodel)
     - [BP006: Replace `__root__` by `RootModel`](#bp006-replace-__root__-by-rootmodel)
     - [BP007: Replace decorators](#bp007-replace-decorators)
-    <!-- - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter) -->
+    - [BP008: Replace `con*` functions by `Annotated` versions](#bp008-replace-con-functions-by-annotated-versions)
   - [License](#license)
 
 ---
 
 ## Installation
 
 The installation is as simple as:
@@ -80,23 +52,23 @@
 ```
 
 ### Check diff before applying changes
 
 To check the diff before applying the changes, you can run:
 
 ```bash
-bump-pydantic --diff <package>
+bump-pydantic --diff <path>
 ```
 
 ### Apply changes
 
 To apply the changes, you can run:
 
 ```bash
-bump-pydantic <package>
+bump-pydantic <path>
 ```
 
 ## Rules
 
 You can find below the list of rules that are applied by `bump-pydantic`.
 
 It's also possible to disable rules by using the `--disable` option.
@@ -283,16 +255,47 @@
         return v
 
     @model_validator(mode='before')
     def validate_root(cls, values):
         return values
 ```
 
-<!--
-### BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
+### BP008: Replace `con*` functions by `Annotated` versions
+
+- ✅ Replace `constr(*args)` by `Annotated[str, StringConstraints(*args)]`.
+- ✅ Replace `conint(*args)` by `Annotated[int, Field(*args)]`.
+- ✅ Replace `confloat(*args)` by `Annotated[float, Field(*args)]`.
+- ✅ Replace `conbytes(*args)` by `Annotated[bytes, Field(*args)]`.
+- ✅ Replace `condecimal(*args)` by `Annotated[Decimal, Field(*args)]`.
+- ✅ Replace `conset(T, *args)` by `Annotated[Set[T], Field(*args)]`.
+- ✅ Replace `confrozenset(T, *args)` by `Annotated[Set[T], Field(*args)]`.
+- ✅ Replace `conlist(T, *args)` by `Annotated[List[T], Field(*args)]`.
+
+The following code will be transformed:
+
+```py
+from pydantic import BaseModel, constr
+
+
+class User(BaseModel):
+    name: constr(min_length=1)
+```
+
+Into:
+
+```py
+from pydantic import BaseModel, StringConstraints
+from typing_extensions import Annotated
+
+
+class User(BaseModel):
+    name: Annotated[str, StringConstraints(min_length=1)]
+```
+
+<!-- ### BP009: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
 
 - ✅ Replace `pydantic.parse_obj_as(T, obj)` to `pydantic.TypeAdapter(T).validate_python(obj)`.
 
 
 The following code will be transformed:
 
 ```py
@@ -325,15 +328,38 @@
 
 
 class Users(BaseModel):
     users: List[User]
 
 
 users = TypeAdapter(Users).validate_python({'users': [{'name': 'John'}]})
+``` -->
+
+<!-- ### BP010: Replace `PyObject` by `ImportString`
+
+- ✅ Replace `PyObject` by `ImportString`.
+
+The following code will be transformed:
+
+```py
+from pydantic import BaseModel, PyObject
+
+
+class User(BaseModel):
+    name: PyObject
 ```
--->
+
+Into:
+
+```py
+from pydantic import BaseModel, ImportString
+
+
+class User(BaseModel):
+    name: ImportString
+``` -->
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

