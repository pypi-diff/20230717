# Comparing `tmp/viper_lib-0.5.8.tar.gz` & `tmp/viper_lib-0.6.tar.gz`

## Comparing `viper_lib-0.5.8.tar` & `viper_lib-0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper.pth
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/__init__.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/better_threading.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/exceptions.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/format.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/frozendict.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/interactive.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/pickle_utils.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/warnings.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/abc/__init__.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/abc/connection.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/abc/flux.py
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/abc/io.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/building/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/building/module_tools.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/compress/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/compress/flux.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/debugging/__init__.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/debugging/chrono.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/debugging/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/meta/__init__.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/meta/decorators.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/meta/iterable.py
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/meta/procedural.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.8/Viper/meta/utils.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.8/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.8/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.8/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper.pth
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/__init__.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/better_threading.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/exceptions.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/format.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/frozendict.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/interactive.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/io.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/pickle_utils.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/warnings.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/__init__.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/connection.py
+-rw-r--r--   0        0        0    15818 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/io.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/building/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/building/module_tools.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/compress/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/compress/flux.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/__init__.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/chrono.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/__init__.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/decorators.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/iterable.py
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/procedural.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/utils.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.6/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.6/README.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 viper_lib-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 viper_lib-0.6/PKG-INFO
```

### Comparing `viper_lib-0.5.8/Viper/better_threading.py` & `viper_lib-0.6/Viper/better_threading.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/format.py` & `viper_lib-0.6/Viper/format.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/frozendict.py` & `viper_lib-0.6/Viper/frozendict.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/interactive.py` & `viper_lib-0.6/Viper/interactive.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/pickle_utils.py` & `viper_lib-0.6/Viper/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/warnings.py` & `viper_lib-0.6/Viper/warnings.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/abc/connection.py` & `viper_lib-0.6/Viper/abc/connection.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/building/module_tools.py` & `viper_lib-0.6/Viper/building/module_tools.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/compress/flux.py` & `viper_lib-0.6/Viper/compress/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/debugging/chrono.py` & `viper_lib-0.6/Viper/debugging/chrono.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/debugging/utils.py` & `viper_lib-0.6/Viper/debugging/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/meta/decorators.py` & `viper_lib-0.6/Viper/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/meta/iterable.py` & `viper_lib-0.6/Viper/meta/iterable.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/meta/procedural.py` & `viper_lib-0.6/Viper/meta/procedural.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/Viper/meta/utils.py` & `viper_lib-0.6/Viper/meta/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/.gitignore` & `viper_lib-0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/LICENSE` & `viper_lib-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/README.md` & `viper_lib-0.6/README.md`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.8/pyproject.toml` & `viper_lib-0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "viper_lib"
-version = "0.5.8"
+version = "0.6"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin.n7@gmail.com" },
 ]
 description = "A Python library full of useful Python tools."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `viper_lib-0.5.8/PKG-INFO` & `viper_lib-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viper_lib
-Version: 0.5.8
+Version: 0.6
 Summary: A Python library full of useful Python tools.
 Project-URL: Repository, https://github.com/MrVoustache/Viper
 Project-URL: Bug Tracker, https://github.com/MrVoustache/Viper/issues
 Author-email: Vincent Raulin <vincent.raulin.n7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Vincent Raulin
```

