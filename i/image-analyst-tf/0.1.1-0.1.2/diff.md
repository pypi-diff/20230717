# Comparing `tmp/image_analyst_tf-0.1.1.tar.gz` & `tmp/image_analyst_tf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_tf-0.1.1.tar", max compression
+gzip compressed data, was "image_analyst_tf-0.1.2.tar", max compression
```

## Comparing `image_analyst_tf-0.1.1.tar` & `image_analyst_tf-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.1.1/LICENSE
--rw-r--r--   0        0        0     1174 2023-07-16 20:03:50.261260 image_analyst_tf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      884 2023-07-14 20:19:02.371375 image_analyst_tf-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.1.1/src/image_analyst/tf/__init__.py
--rw-r--r--   0        0        0    13634 2023-07-16 19:43:37.542678 image_analyst_tf-0.1.1/src/image_analyst/tf/models.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 image_analyst_tf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1182 2023-07-17 11:29:18.851147 image_analyst_tf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-07-17 11:27:00.632197 image_analyst_tf-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.1.2/src/image_analyst/tf/__init__.py
+-rw-r--r--   0        0        0    13634 2023-07-17 11:28:24.714731 image_analyst_tf-0.1.2/src/image_analyst/tf/models.py
+-rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 image_analyst_tf-0.1.2/PKG-INFO
```

### Comparing `image_analyst_tf-0.1.1/LICENSE` & `image_analyst_tf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_tf-0.1.1/pyproject.toml` & `image_analyst_tf-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "image-analyst-tf"
-version = "0.1.1"
+version = "0.1.2"
 description = "ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystTF"
-keywords = ["image", "analysis", "tf"]
+keywords = ["image", "analysis", "tensorflow"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 numpy = "^1.24.3"
-image-analyst = "^0.1.1"
+image-analyst = "^0.1.2"
 tensorflow = "^2.10.0"
 tensorflow-io-gcs-filesystem = "^0.29, !=0.32.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
```

### Comparing `image_analyst_tf-0.1.1/README.md` & `image_analyst_tf-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) >=3.9, <3.12
 - [pip](https://pip.pypa.io/en/stable/)
 
-## Download
+## Download & Installation
 
-You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystTF/releases).
+There is two ways to download and install the application.
 
-## Installation
+### Using PyPI
 
-You can install the application by running the following command:
+You can download and install the application using [PyPI](https://pypi.org/project/image-analyst-tf/). To do so, run the following command:
+
+```bash
+pip install image-analyst-tf
+```
+
+### Using the GitHub releases
+
+You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystTF/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst_tf-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
```

### Comparing `image_analyst_tf-0.1.1/src/image_analyst/tf/models.py` & `image_analyst_tf-0.1.2/src/image_analyst/tf/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Tflite: the new YoloV7Tflite.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.0/tf-yolov7-coco.tflite",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-coco.tflite",  # noqa: E501
                 "tf-yolov7-coco.tflite",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.0/tf-yolov7-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-coco.names",  # noqa: E501
                 "tf-yolov7-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
@@ -107,20 +107,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Tflite: the new YoloV7Tflite.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.0/tf-yolov7-tiny-coco.tflite",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-tiny-coco.tflite",  # noqa: E501
                 "tf-yolov7-tiny-coco.tflite",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.0/tf-yolov7-tiny-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-tiny-coco.names",  # noqa: E501
                 "tf-yolov7-tiny-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
```

### Comparing `image_analyst_tf-0.1.1/PKG-INFO` & `image_analyst_tf-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: image-analyst-tf
-Version: 0.1.1
+Version: 0.1.2
 Summary: ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow.
 Home-page: https://github.com/BergLucas/ImageAnalystTF
-Keywords: image,analysis,tf
+Keywords: image,analysis,tensorflow
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: image-analyst (>=0.1.1,<0.2.0)
+Requires-Dist: image-analyst (>=0.1.2,<0.2.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: tensorflow (>=2.10.0,<3.0.0)
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.29,<0.30)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystTF
 Description-Content-Type: text/markdown
 
 # ImageAnalyst TF
@@ -27,21 +27,29 @@
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) >=3.9, <3.12
 - [pip](https://pip.pypa.io/en/stable/)
 
-## Download
+## Download & Installation
 
-You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystTF/releases).
+There is two ways to download and install the application.
 
-## Installation
+### Using PyPI
 
-You can install the application by running the following command:
+You can download and install the application using [PyPI](https://pypi.org/project/image-analyst-tf/). To do so, run the following command:
+
+```bash
+pip install image-analyst-tf
+```
+
+### Using the GitHub releases
+
+You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystTF/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst_tf-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
```

