# Comparing `tmp/yarrow_diagrams-0.0.3.0.tar.gz` & `tmp/yarrow_diagrams-0.0.3.1.tar.gz`

## Comparing `yarrow_diagrams-0.0.3.0.tar` & `yarrow_diagrams-0.0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/__init__.py
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/bipartite_multigraph.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/cupy.py
--rw-r--r--   0        0        0    12972 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/diagram.py
--rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/finite_function.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/__init__.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/cupy.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/array/numpy.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/decompose/frobenius.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/functor.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/functor/optic.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/numpy/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/numpy/layer.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/__init__.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/finite_function.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/yarrow/segmented/operations.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/__init__.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/bipartite_multigraph.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/cupy.py
+-rw-r--r--   0        0        0    12972 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/diagram.py
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/finite_function.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/array/__init__.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/array/cupy.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/array/numpy.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/decompose/frobenius.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/functor/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/functor/functor.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/functor/optic.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/numpy/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/numpy/layer.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/segmented/__init__.py
+-rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/segmented/finite_function.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/yarrow/segmented/operations.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/README.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.3.1/PKG-INFO
```

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/bipartite_multigraph.py` & `yarrow_diagrams-0.0.3.1/yarrow/bipartite_multigraph.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/cupy.py` & `yarrow_diagrams-0.0.3.1/yarrow/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/diagram.py` & `yarrow_diagrams-0.0.3.1/yarrow/diagram.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/finite_function.py` & `yarrow_diagrams-0.0.3.1/yarrow/finite_function.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/array/__init__.py` & `yarrow_diagrams-0.0.3.1/yarrow/array/__init__.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/array/cupy.py` & `yarrow_diagrams-0.0.3.1/yarrow/array/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/array/numpy.py` & `yarrow_diagrams-0.0.3.1/yarrow/array/numpy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/decompose/frobenius.py` & `yarrow_diagrams-0.0.3.1/yarrow/decompose/frobenius.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/functor/functor.py` & `yarrow_diagrams-0.0.3.1/yarrow/functor/functor.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/functor/optic.py` & `yarrow_diagrams-0.0.3.1/yarrow/functor/optic.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/numpy/__init__.py` & `yarrow_diagrams-0.0.3.1/yarrow/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/numpy/layer.py` & `yarrow_diagrams-0.0.3.1/yarrow/numpy/layer.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/segmented/finite_function.py` & `yarrow_diagrams-0.0.3.1/yarrow/segmented/finite_function.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/yarrow/segmented/operations.py` & `yarrow_diagrams-0.0.3.1/yarrow/segmented/operations.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/LICENSE` & `yarrow_diagrams-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/README.md` & `yarrow_diagrams-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.3.0/pyproject.toml` & `yarrow_diagrams-0.0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "yarrow-diagrams"
-version = "0.0.3.0"
+version = "0.0.3.1"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "yarrow diagrams"
 readme = "README.md"
 requires-python = ">= 3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
   "numpy~=1.23.3",
-  "scipy~=1.9.0",
+  "scipy~=1.10.0",
 ]
 
 [project.urls]
 "Homepage" = "https://yarrow.id"
 "Github" = "https://github.com/yarrow-id/diagrams/"
 "Documentation" = "https://yarrow-diagrams.readthedocs.io/"
```

### Comparing `yarrow_diagrams-0.0.3.0/PKG-INFO` & `yarrow_diagrams-0.0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: yarrow-diagrams
-Version: 0.0.3.0
+Version: 0.0.3.1
 Summary: yarrow diagrams
 Project-URL: Homepage, https://yarrow.id
 Project-URL: Github, https://github.com/yarrow-id/diagrams/
 Project-URL: Documentation, https://yarrow-diagrams.readthedocs.io/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy~=1.23.3
-Requires-Dist: scipy~=1.9.0
+Requires-Dist: scipy~=1.10.0
 Description-Content-Type: text/markdown
 
 # Yarrow Diagrams
 
 [![Documentation Status](https://readthedocs.org/projects/yarrow-diagrams/badge/?version=latest)](https://yarrow-diagrams.readthedocs.io/en/latest/?badge=latest)
 
 **⚠️ yarrow is still early in development ⚠️**: it's missing some features, and not everything is documented. Consider yourself warned!
```

