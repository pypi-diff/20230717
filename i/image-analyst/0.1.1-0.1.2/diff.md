# Comparing `tmp/image_analyst-0.1.1.tar.gz` & `tmp/image_analyst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst-0.1.1.tar", max compression
+gzip compressed data, was "image_analyst-0.1.2.tar", max compression
```

## Comparing `image_analyst-0.1.1.tar` & `image_analyst-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.1/LICENSE
--rw-r--r--   0        0        0      989 2023-07-14 21:02:14.347031 image_analyst-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      885 2023-07-14 16:43:27.012629 image_analyst-0.1.1/README.md
--rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.1/src/image_analyst/analyzers.py
--rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.1/src/image_analyst/exceptions.py
--rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.1.1/src/image_analyst/image.py
--rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.1/src/image_analyst/models.py
--rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.1/src/image_analyst/trackers.py
--rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.1/src/image_analyst/utils.py
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 image_analyst-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1430 2023-07-16 20:40:07.447385 image_analyst-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      885 2023-07-14 16:43:27.012629 image_analyst-0.1.2/README.md
+-rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.2/src/image_analyst/analyzers.py
+-rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.2/src/image_analyst/exceptions.py
+-rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.1.2/src/image_analyst/image.py
+-rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.2/src/image_analyst/models.py
+-rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.2/src/image_analyst/trackers.py
+-rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.2/src/image_analyst/utils.py
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 image_analyst-0.1.2/PKG-INFO
```

### Comparing `image_analyst-0.1.1/LICENSE` & `image_analyst-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/README.md` & `image_analyst-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/analyzers.py` & `image_analyst-0.1.2/src/image_analyst/analyzers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/exceptions.py` & `image_analyst-0.1.2/src/image_analyst/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/image.py` & `image_analyst-0.1.2/src/image_analyst/image.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/models.py` & `image_analyst-0.1.2/src/image_analyst/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/trackers.py` & `image_analyst-0.1.2/src/image_analyst/trackers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/src/image_analyst/utils.py` & `image_analyst-0.1.2/src/image_analyst/utils.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.1/PKG-INFO` & `image_analyst-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: image-analyst
-Version: 0.1.1
+Version: 0.1.2
 Summary: ImageAnalyst is a library that simplifies image analysis.
 Home-page: https://github.com/BergLucas/ImageAnalyst
 Keywords: image,analysis
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cv2
+Provides-Extra: hf
+Provides-Extra: onnx
+Provides-Extra: tf
+Requires-Dist: image-analyst-cv2[cv2] (>=0.1.0,<0.2.0) ; extra == "cv2"
+Requires-Dist: image-analyst-hf (>=0.1.0,<0.2.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "hf")
+Requires-Dist: image-analyst-onnx (>=0.1.0,<0.2.0) ; extra == "onnx"
+Requires-Dist: image-analyst-tf (>=0.1.1,<0.2.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "tf")
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalyst
 Description-Content-Type: text/markdown
 
 # ImageAnalyst
 
 ImageAnalyst is a library that simplifies image analysis. The library achieves this goal by standardizing the input and output
```

