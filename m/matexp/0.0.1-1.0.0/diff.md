# Comparing `tmp/matexp-0.0.1.tar.gz` & `tmp/matexp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matexp-0.0.1.tar", last modified: Tue May 30 16:49:03 2023, max compression
+gzip compressed data, was "matexp-1.0.0.tar", last modified: Mon Jul 17 13:36:04 2023, max compression
```

## Comparing `matexp-0.0.1.tar` & `matexp-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-30 16:49:03.607854 matexp-0.0.1/
--rw-rw-r--   0 dm        (1000) dm        (1000)       24 2022-06-07 19:15:44.000000 matexp-0.0.1/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)      110 2022-04-11 19:32:57.000000 matexp-0.0.1/.gitmodules
--rw-rw-r--   0 dm        (1000) dm        (1000)     1094 2023-03-21 16:41:49.000000 matexp-0.0.1/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     2799 2023-05-30 16:49:03.607854 matexp-0.0.1/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     2048 2023-05-21 16:28:38.000000 matexp-0.0.1/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-30 16:49:03.599854 matexp-0.0.1/backward_euler/
--rw-rw-r--   0 dm        (1000) dm        (1000)    79223 2022-06-06 21:22:04.000000 matexp-0.0.1/backward_euler/Accuracy_Comparison.png
--rw-rw-r--   0 dm        (1000) dm        (1000)    13689 2022-04-19 12:55:24.000000 matexp-0.0.1/backward_euler/NMDA.cpp
--rw-rw-r--   0 dm        (1000) dm        (1000)     8313 2022-04-12 22:54:13.000000 matexp-0.0.1/backward_euler/Nav11.cpp
--rw-rw-r--   0 dm        (1000) dm        (1000)    50956 2022-06-07 00:59:22.000000 matexp-0.0.1/backward_euler/Speed-Accuracy_Trade-off.png
--rw-rw-r--   0 dm        (1000) dm        (1000)    32562 2022-06-07 01:05:26.000000 matexp-0.0.1/backward_euler/Speed_Comparison.png
--rw-rw-r--   0 dm        (1000) dm        (1000)    11100 2023-04-28 19:22:17.000000 matexp-0.0.1/backward_euler/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    17861 2022-04-12 21:33:25.000000 matexp-0.0.1/backward_euler/ampa13.cpp
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-30 16:49:03.603854 matexp-0.0.1/matexp/
--rw-rw-r--   0 dm        (1000) dm        (1000)     3843 2023-04-28 19:12:27.000000 matexp-0.0.1/matexp/__init__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2730 2023-05-20 16:11:39.000000 matexp-0.0.1/matexp/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    17509 2023-03-27 15:47:24.000000 matexp-0.0.1/matexp/approx.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    15907 2023-03-30 19:46:04.000000 matexp-0.0.1/matexp/codegen.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     4011 2023-04-28 19:23:50.000000 matexp-0.0.1/matexp/inputs.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1691 2022-09-22 23:15:06.000000 matexp-0.0.1/matexp/lti_model.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    11136 2023-04-19 21:04:25.000000 matexp-0.0.1/matexp/nmodl_compiler.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    13742 2022-06-06 18:35:44.000000 matexp-0.0.1/matexp/optimizer.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     4157 2022-05-30 19:29:53.000000 matexp-0.0.1/matexp/polynomial.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-30 16:49:03.607854 matexp-0.0.1/matexp/tests/
--rw-rw-r--   0 dm        (1000) dm        (1000)     7917 2022-06-22 01:29:32.000000 matexp-0.0.1/matexp/tests/NMDA.mod
--rw-rw-r--   0 dm        (1000) dm        (1000)     2774 2022-06-22 01:29:33.000000 matexp-0.0.1/matexp/tests/Nav11.mod
--rw-rw-r--   0 dm        (1000) dm        (1000)     5637 2022-06-22 01:29:33.000000 matexp-0.0.1/matexp/tests/ampa13.mod
--rw-rw-r--   0 dm        (1000) dm        (1000)      218 2022-04-20 13:49:27.000000 matexp-0.0.1/matexp/tests/nonlinear.mod
--rw-rw-r--   0 dm        (1000) dm        (1000)     3264 2023-04-28 19:09:37.000000 matexp-0.0.1/matexp/tests/test_error.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2331 2023-04-28 19:09:25.000000 matexp-0.0.1/matexp/tests/test_inputs.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1968 2023-04-28 22:00:47.000000 matexp-0.0.1/matexp/tests/test_main.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1882 2023-04-28 19:08:22.000000 matexp-0.0.1/matexp/tests/test_nmodl.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     3655 2023-04-28 19:08:10.000000 matexp-0.0.1/matexp/tests/test_polynomial.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-30 16:49:03.603854 matexp-0.0.1/matexp.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     2799 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      891 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       56 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       29 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        7 2023-05-30 16:49:03.000000 matexp-0.0.1/matexp.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)   615842 2022-07-08 20:00:53.000000 matexp-0.0.1/presentation.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)      963 2023-05-30 16:44:26.000000 matexp-0.0.1/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-05-30 16:49:03.607854 matexp-0.0.1/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-17 13:36:04.458702 matexp-1.0.0/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       24 2022-06-07 19:15:44.000000 matexp-1.0.0/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)      110 2022-04-11 19:32:57.000000 matexp-1.0.0/.gitmodules
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3128 2023-07-17 13:32:17.000000 matexp-1.0.0/DETAILS.md
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1094 2023-03-21 16:41:49.000000 matexp-1.0.0/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2768 2023-07-17 13:36:04.458702 matexp-1.0.0/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2017 2023-07-17 00:44:01.000000 matexp-1.0.0/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-17 13:36:04.454702 matexp-1.0.0/backward_euler/
+-rw-rw-r--   0 dm        (1000) dm        (1000)    79223 2022-06-06 21:22:04.000000 matexp-1.0.0/backward_euler/Accuracy_Comparison.png
+-rw-rw-r--   0 dm        (1000) dm        (1000)    13689 2022-04-19 12:55:24.000000 matexp-1.0.0/backward_euler/NMDA.cpp
+-rw-rw-r--   0 dm        (1000) dm        (1000)     8313 2022-04-12 22:54:13.000000 matexp-1.0.0/backward_euler/Nav11.cpp
+-rw-rw-r--   0 dm        (1000) dm        (1000)    50956 2022-06-07 00:59:22.000000 matexp-1.0.0/backward_euler/Speed-Accuracy_Trade-off.png
+-rw-rw-r--   0 dm        (1000) dm        (1000)    32562 2022-06-07 01:05:26.000000 matexp-1.0.0/backward_euler/Speed_Comparison.png
+-rw-rw-r--   0 dm        (1000) dm        (1000)    11100 2023-04-28 19:22:17.000000 matexp-1.0.0/backward_euler/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    17861 2022-04-12 21:33:25.000000 matexp-1.0.0/backward_euler/ampa13.cpp
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-17 13:36:04.454702 matexp-1.0.0/matexp/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3843 2023-04-28 19:12:27.000000 matexp-1.0.0/matexp/__init__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2730 2023-05-20 16:11:39.000000 matexp-1.0.0/matexp/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    17509 2023-03-27 15:47:24.000000 matexp-1.0.0/matexp/approx.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    15907 2023-03-30 19:46:04.000000 matexp-1.0.0/matexp/codegen.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4011 2023-04-28 19:23:50.000000 matexp-1.0.0/matexp/inputs.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1691 2022-09-22 23:15:06.000000 matexp-1.0.0/matexp/lti_model.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    11136 2023-04-19 21:04:25.000000 matexp-1.0.0/matexp/nmodl_compiler.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    13742 2022-06-06 18:35:44.000000 matexp-1.0.0/matexp/optimizer.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4157 2022-05-30 19:29:53.000000 matexp-1.0.0/matexp/polynomial.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-17 13:36:04.454702 matexp-1.0.0/matexp/tests/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     7917 2022-06-22 01:29:32.000000 matexp-1.0.0/matexp/tests/NMDA.mod
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2774 2022-06-22 01:29:33.000000 matexp-1.0.0/matexp/tests/Nav11.mod
+-rw-rw-r--   0 dm        (1000) dm        (1000)     5637 2022-06-22 01:29:33.000000 matexp-1.0.0/matexp/tests/ampa13.mod
+-rw-rw-r--   0 dm        (1000) dm        (1000)      218 2022-04-20 13:49:27.000000 matexp-1.0.0/matexp/tests/nonlinear.mod
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3264 2023-04-28 19:09:37.000000 matexp-1.0.0/matexp/tests/test_error.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2331 2023-04-28 19:09:25.000000 matexp-1.0.0/matexp/tests/test_inputs.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1968 2023-04-28 22:00:47.000000 matexp-1.0.0/matexp/tests/test_main.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1882 2023-04-28 19:08:22.000000 matexp-1.0.0/matexp/tests/test_nmodl.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3655 2023-04-28 19:08:10.000000 matexp-1.0.0/matexp/tests/test_polynomial.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-17 13:36:04.454702 matexp-1.0.0/matexp.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2768 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      902 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       56 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       29 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        7 2023-07-17 13:36:04.000000 matexp-1.0.0/matexp.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)   615842 2022-07-08 20:00:53.000000 matexp-1.0.0/presentation.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)      963 2023-07-17 01:28:23.000000 matexp-1.0.0/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-07-17 13:36:04.458702 matexp-1.0.0/setup.cfg
```

### Comparing `matexp-0.0.1/LICENSE.txt` & `matexp-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/PKG-INFO` & `matexp-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matexp
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simulator for Linear Time-Invariant Kinetic Models using the NMODL file format.
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/matexp
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -18,32 +18,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # matexp
 
 This program solves systems of differential equations for the NEURON simulator
 using the matrix-exponential method of integration. This is a new method of
-integration. The solution is faster and more accurate than NEURONs built in
-solver. This method is only applicable to systems which are linear and
-time-invariant, such as Markov kinetic models. This method is also limited to
-systems with one or two inputs.
+integration. The solution is faster and more accurate than NEURONs built
+in "sparse" solver. This method is only applicable to systems which are linear
+and time-invariant, such as Markov kinetic models. This method is also limited
+to systems with one or two inputs.
 
 This program uses the
 [NMODL file format](https://www.neuron.yale.edu/neuron/static/py_doc/modelspec/programmatic/mechanisms/nmodl.html)
-(".mod" files) for both its inputs and outputs.  
-The input kinetic model is a .mod file, and the solved equations are written to new .mod file.  
+(".mod" files). 
+The input kinetic model is an NMODL file, and the solution is written to a new NMODL file.
 
 For more information about how this program works see [DETAILS.md](./DETAILS.md).
 
 
 ### Installation
 
 Prerequisites:
 * Compiler for the target system.
-    + Host requires `g++`
+    + CPU requires `g++`
     + Cuda requires the `cupy` python package.
 
 ```
 $ pip install matexp
 ```
```

### Comparing `matexp-0.0.1/README.md` & `matexp-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # matexp
 
 This program solves systems of differential equations for the NEURON simulator
 using the matrix-exponential method of integration. This is a new method of
-integration. The solution is faster and more accurate than NEURONs built in
-solver. This method is only applicable to systems which are linear and
-time-invariant, such as Markov kinetic models. This method is also limited to
-systems with one or two inputs.
+integration. The solution is faster and more accurate than NEURONs built
+in "sparse" solver. This method is only applicable to systems which are linear
+and time-invariant, such as Markov kinetic models. This method is also limited
+to systems with one or two inputs.
 
 This program uses the
 [NMODL file format](https://www.neuron.yale.edu/neuron/static/py_doc/modelspec/programmatic/mechanisms/nmodl.html)
-(".mod" files) for both its inputs and outputs.  
-The input kinetic model is a .mod file, and the solved equations are written to new .mod file.  
+(".mod" files). 
+The input kinetic model is an NMODL file, and the solution is written to a new NMODL file.
 
 For more information about how this program works see [DETAILS.md](./DETAILS.md).
 
 
 ### Installation
 
 Prerequisites:
 * Compiler for the target system.
-    + Host requires `g++`
+    + CPU requires `g++`
     + Cuda requires the `cupy` python package.
 
 ```
 $ pip install matexp
 ```
```

### Comparing `matexp-0.0.1/backward_euler/Accuracy_Comparison.png` & `matexp-1.0.0/backward_euler/Accuracy_Comparison.png`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/NMDA.cpp` & `matexp-1.0.0/backward_euler/NMDA.cpp`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/Nav11.cpp` & `matexp-1.0.0/backward_euler/Nav11.cpp`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/Speed-Accuracy_Trade-off.png` & `matexp-1.0.0/backward_euler/Speed-Accuracy_Trade-off.png`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/Speed_Comparison.png` & `matexp-1.0.0/backward_euler/Speed_Comparison.png`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/__main__.py` & `matexp-1.0.0/backward_euler/__main__.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/backward_euler/ampa13.cpp` & `matexp-1.0.0/backward_euler/ampa13.cpp`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/__init__.py` & `matexp-1.0.0/matexp/__init__.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/__main__.py` & `matexp-1.0.0/matexp/__main__.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/approx.py` & `matexp-1.0.0/matexp/approx.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/codegen.py` & `matexp-1.0.0/matexp/codegen.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/inputs.py` & `matexp-1.0.0/matexp/inputs.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/lti_model.py` & `matexp-1.0.0/matexp/lti_model.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/nmodl_compiler.py` & `matexp-1.0.0/matexp/nmodl_compiler.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/optimizer.py` & `matexp-1.0.0/matexp/optimizer.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/polynomial.py` & `matexp-1.0.0/matexp/polynomial.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/NMDA.mod` & `matexp-1.0.0/matexp/tests/NMDA.mod`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/Nav11.mod` & `matexp-1.0.0/matexp/tests/Nav11.mod`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/ampa13.mod` & `matexp-1.0.0/matexp/tests/ampa13.mod`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/test_error.py` & `matexp-1.0.0/matexp/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/test_inputs.py` & `matexp-1.0.0/matexp/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/test_main.py` & `matexp-1.0.0/matexp/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/test_nmodl.py` & `matexp-1.0.0/matexp/tests/test_nmodl.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp/tests/test_polynomial.py` & `matexp-1.0.0/matexp/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/matexp.egg-info/PKG-INFO` & `matexp-1.0.0/matexp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matexp
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simulator for Linear Time-Invariant Kinetic Models using the NMODL file format.
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/matexp
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -18,32 +18,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # matexp
 
 This program solves systems of differential equations for the NEURON simulator
 using the matrix-exponential method of integration. This is a new method of
-integration. The solution is faster and more accurate than NEURONs built in
-solver. This method is only applicable to systems which are linear and
-time-invariant, such as Markov kinetic models. This method is also limited to
-systems with one or two inputs.
+integration. The solution is faster and more accurate than NEURONs built
+in "sparse" solver. This method is only applicable to systems which are linear
+and time-invariant, such as Markov kinetic models. This method is also limited
+to systems with one or two inputs.
 
 This program uses the
 [NMODL file format](https://www.neuron.yale.edu/neuron/static/py_doc/modelspec/programmatic/mechanisms/nmodl.html)
-(".mod" files) for both its inputs and outputs.  
-The input kinetic model is a .mod file, and the solved equations are written to new .mod file.  
+(".mod" files). 
+The input kinetic model is an NMODL file, and the solution is written to a new NMODL file.
 
 For more information about how this program works see [DETAILS.md](./DETAILS.md).
 
 
 ### Installation
 
 Prerequisites:
 * Compiler for the target system.
-    + Host requires `g++`
+    + CPU requires `g++`
     + Cuda requires the `cupy` python package.
 
 ```
 $ pip install matexp
 ```
```

### Comparing `matexp-0.0.1/matexp.egg-info/SOURCES.txt` & `matexp-1.0.0/matexp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .gitmodules
+DETAILS.md
 LICENSE.txt
 README.md
 presentation.pdf
 pyproject.toml
 backward_euler/Accuracy_Comparison.png
 backward_euler/NMDA.cpp
 backward_euler/Nav11.cpp
```

### Comparing `matexp-0.0.1/presentation.pdf` & `matexp-1.0.0/presentation.pdf`

 * *Files identical despite different names*

### Comparing `matexp-0.0.1/pyproject.toml` & `matexp-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["matexp"]
 
 [project]
 name = "matexp"
-version = "0.0.1"
+version = "1.0.0"
 description = "Simulator for Linear Time-Invariant Kinetic Models using the NMODL file format."
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 urls = {Homepage = "https://github.com/ctrl-z-9000-times/matexp"}
```

