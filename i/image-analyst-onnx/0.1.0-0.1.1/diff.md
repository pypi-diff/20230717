# Comparing `tmp/image_analyst_onnx-0.1.0.tar.gz` & `tmp/image_analyst_onnx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_onnx-0.1.0.tar", max compression
+gzip compressed data, was "image_analyst_onnx-0.1.1.tar", max compression
```

## Comparing `image_analyst_onnx-0.1.0.tar` & `image_analyst_onnx-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_onnx-0.1.0/LICENSE
--rw-r--r--   0        0        0     1121 2023-07-14 19:44:48.692011 image_analyst_onnx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      883 2023-07-14 19:47:11.642611 image_analyst_onnx-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_onnx-0.1.0/src/image_analyst/onnx/__init__.py
--rw-r--r--   0        0        0    10222 2023-07-14 19:54:32.612650 image_analyst_onnx-0.1.0/src/image_analyst/onnx/models.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 image_analyst_onnx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_onnx-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1121 2023-07-17 12:27:57.975682 image_analyst_onnx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1188 2023-07-17 11:20:58.380078 image_analyst_onnx-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_onnx-0.1.1/src/image_analyst/onnx/__init__.py
+-rw-r--r--   0        0        0    10172 2023-07-17 12:27:15.333068 image_analyst_onnx-0.1.1/src/image_analyst/onnx/models.py
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 image_analyst_onnx-0.1.1/PKG-INFO
```

### Comparing `image_analyst_onnx-0.1.0/LICENSE` & `image_analyst_onnx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_onnx-0.1.0/pyproject.toml` & `image_analyst_onnx-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-onnx"
-version = "0.1.0"
+version = "0.1.1"
 description = "ImageAnalyst ONNX is an extension to the ImageAnalyst library, providing additional models and functions using onnx."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystONNX"
 keywords = ["image", "analysis", "onnx"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
-image-analyst = "^0.1.0"
+image-analyst = "^0.1.2"
 onnxruntime = "^1.15.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
```

### Comparing `image_analyst_onnx-0.1.0/README.md` & `image_analyst_onnx-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) ~= 3.9
 - [pip](https://pip.pypa.io/en/stable/)
 
-## Download
+## Download & Installation
 
-You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystONNX/releases).
+There is two ways to download and install the application.
 
-## Installation
+### Using PyPI
 
-You can install the application by running the following command:
+You can download and install the application using [PyPI](https://pypi.org/project/image-analyst-onnx/). To do so, run the following command:
+
+```bash
+pip install image-analyst-onnx
+```
+
+### Using the GitHub releases
+
+You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystONNX/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst_onnx-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
```

### Comparing `image_analyst_onnx-0.1.0/src/image_analyst/onnx/models.py` & `image_analyst_onnx-0.1.1/src/image_analyst/onnx/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     ModelLoadingFailedException,
     InvalidDtypeException,
     DetectionFailedException,
 )
 from image_analyst.image import (
     ImageFormat,
     BoundingBox,
-    verify_image,
     ImageEmbedder,
     EmbeddingFunction,
 )
 from image_analyst.utils import NmsFunction, NmsPython
 from image_analyst.models import ODModel, Detection
 from typing import Optional, Literal
 import onnxruntime as ort
@@ -63,20 +62,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Onnx: the new YoloV7Onnx.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.0/onnx-yolov7-coco.onnx",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-coco.onnx",  # noqa: E501
                 "onnx-yolov7-coco.onnx",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.0/onnx-yolov7-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-coco.names",  # noqa: E501
                 "onnx-yolov7-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
@@ -124,20 +123,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Onnx: the new YoloV7Onnx.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.0/onnx-yolov7-tiny-coco.onnx",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-tiny-coco.onnx",  # noqa: E501
                 "onnx-yolov7-tiny-coco.onnx",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.0/onnx-yolov7-tiny-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-tiny-coco.names",  # noqa: E501
                 "onnx-yolov7-tiny-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
@@ -213,16 +212,14 @@
         return np.float32
 
     @property
     def supported_format(self) -> ImageFormat:  # noqa: D102
         return ImageFormat.RGB
 
     def __call__(self, image: np.ndarray) -> list[Detection]:  # noqa: D102
-        verify_image(image)
-
         if image.dtype != self.supported_dtype:
             raise InvalidDtypeException("The image dtype is not supported.")
 
         logger.info("Started Image preprocessing")
         embedded_image, bounding_box = self.__embedding_function(
             image, *self.__model_size
         )
```

### Comparing `image_analyst_onnx-0.1.0/PKG-INFO` & `image_analyst_onnx-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: image-analyst-onnx
-Version: 0.1.0
+Version: 0.1.1
 Summary: ImageAnalyst ONNX is an extension to the ImageAnalyst library, providing additional models and functions using onnx.
 Home-page: https://github.com/BergLucas/ImageAnalystONNX
 Keywords: image,analysis,onnx
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: image-analyst (>=0.1.0,<0.2.0)
+Requires-Dist: image-analyst (>=0.1.2,<0.2.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystONNX
 Description-Content-Type: text/markdown
 
 # ImageAnalyst ONNX
 
@@ -26,21 +26,29 @@
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) ~= 3.9
 - [pip](https://pip.pypa.io/en/stable/)
 
-## Download
+## Download & Installation
 
-You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystONNX/releases).
+There is two ways to download and install the application.
 
-## Installation
+### Using PyPI
 
-You can install the application by running the following command:
+You can download and install the application using [PyPI](https://pypi.org/project/image-analyst-onnx/). To do so, run the following command:
+
+```bash
+pip install image-analyst-onnx
+```
+
+### Using the GitHub releases
+
+You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystONNX/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst_onnx-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
```

