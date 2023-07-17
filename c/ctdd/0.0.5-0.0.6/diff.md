# Comparing `tmp/ctdd-0.0.5.tar.gz` & `tmp/ctdd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.5.tar", max compression
+gzip compressed data, was "ctdd-0.0.6.tar", max compression
```

## Comparing `ctdd-0.0.5.tar` & `ctdd-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.5/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.5/README.md
--rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.5/ctdd/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.5/ctdd/__main__.py
--rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.5/ctdd/ffi_factory.py
--rw-r--r--   0        0        0     1663 2023-07-13 11:47:07.434036 ctdd-0.0.5/ctdd/mocker.py
--rw-r--r--   0        0        0     2592 2023-07-11 11:26:17.438280 ctdd-0.0.5/ctdd/tester.py
--rw-r--r--   0        0        0     2979 2023-07-13 11:45:15.551318 ctdd-0.0.5/ctdd/tester_state.py
--rw-r--r--   0        0        0      736 2023-07-13 11:48:01.933872 ctdd-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.6/README.md
+-rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.6/ctdd/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.6/ctdd/__main__.py
+-rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.6/ctdd/ffi_factory.py
+-rw-r--r--   0        0        0     1663 2023-07-13 11:47:07.434036 ctdd-0.0.6/ctdd/mocker.py
+-rw-r--r--   0        0        0     2764 2023-07-17 12:11:04.503502 ctdd-0.0.6/ctdd/tester.py
+-rw-r--r--   0        0        0     3088 2023-07-17 12:11:57.942213 ctdd-0.0.6/ctdd/tester_state.py
+-rw-r--r--   0        0        0      736 2023-07-17 13:15:03.287677 ctdd-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.6/PKG-INFO
```

### Comparing `ctdd-0.0.5/LICENSE` & `ctdd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.5/README.md` & `ctdd-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.5/ctdd/__main__.py` & `ctdd-0.0.6/ctdd/__main__.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.5/ctdd/ffi_factory.py` & `ctdd-0.0.6/ctdd/ffi_factory.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.5/ctdd/mocker.py` & `ctdd-0.0.6/ctdd/mocker.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.5/ctdd/tester.py` & `ctdd-0.0.6/ctdd/tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from john import TestCase
 from .tester_state import TesterState
 
 class Tester(TestCase):
     _state = None
     factory = None
     _source_files = []
+    _header_files = []
 
     @staticmethod
     def _ensure_state(verbose=False):
         if not Tester._state:
-            Tester._state = TesterState('__main__', Tester._source_files, verbose=verbose)
+            Tester._state = TesterState('__main__', Tester._source_files,  Tester._header_files, verbose=verbose)
             Tester.factory = Tester._state.factory
 
         return Tester
 
     @staticmethod
     def help():
         Tester._ensure_state()
@@ -31,14 +32,19 @@
 
     @staticmethod
     def addSourceFile(filename):
         Tester._source_files.append(filename)
         return Tester
 
     @staticmethod
+    def addHeaderFile(filename):
+        Tester._header_files.append(filename)
+        return Tester
+
+    @staticmethod
     def go(verbose=False):
         Tester._ensure_state(verbose=verbose).Runner.run()
         return Tester
 
     @property
     def sut(self):
         return Tester._state.ensure_sut()
```

### Comparing `ctdd-0.0.5/ctdd/tester_state.py` & `ctdd-0.0.6/ctdd/tester_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 def _struct_creator(state, typename):
     struct = state.tube._ffi.new(f'struct {typename} *')
     return struct
 
 class TesterState:
 
-    def __init__(self, module_name: str, source_files=[], verbose=False):
+    def __init__(self, module_name: str, source_files=[], header_files=[], verbose=False):
         self._module_name = module_name
         self._verbose = verbose
         self.factory = FFIFactory()
         self.mocker = Mocker()
         self.externs = []
         self.source_files = source_files
+        self.header_files = header_files
         self.tube = None
         self.sut = None
 
         paste = self.create_tube("introspection").verbose(self._verbose).squeeze()
         if paste is None:
             raise RuntimeError('introspection build failed')
 
@@ -65,14 +66,15 @@
         return CrelmFactory().create_Tube(tube_name) \
             .verbose(self._verbose) \
             .save_compiler_temps() \
             .set_source_folder_relative(test_case_filename) \
             .add_source_file(c_filename) \
             .add_header_file(h_filename) \
             .add_source_files(self.source_files) \
+            .add_header_files(self.header_files) \
             .add_externs(self.externs)
 
     def _ensure_tube(self):
         if not self.tube:
             self.sut = None
             self.tube = self.create_tube()
```

### Comparing `ctdd-0.0.5/pyproject.toml` & `ctdd-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.5"
+version = "0.0.6"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ctdd-0.0.5/PKG-INFO` & `ctdd-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.5
+Version: 0.0.6
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

