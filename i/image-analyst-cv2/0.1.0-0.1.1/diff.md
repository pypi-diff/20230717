# Comparing `tmp/image_analyst_cv2-0.1.0.tar.gz` & `tmp/image_analyst_cv2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_cv2-0.1.0.tar", max compression
+gzip compressed data, was "image_analyst_cv2-0.1.1.tar", max compression
```

## Comparing `image_analyst_cv2-0.1.0.tar` & `image_analyst_cv2-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_cv2-0.1.0/LICENSE
--rw-r--r--   0        0        0     1548 2023-07-14 17:24:50.674346 image_analyst_cv2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      879 2023-07-14 17:21:58.751142 image_analyst_cv2-0.1.0/README.md
--rw-r--r--   0        0        0      169 2023-07-14 17:26:19.383797 image_analyst_cv2-0.1.0/src/image_analyst/cv2/__init__.py
--rw-r--r--   0        0        0      923 2023-07-14 17:26:29.985398 image_analyst_cv2-0.1.0/src/image_analyst/cv2/image.py
--rw-r--r--   0        0        0     9621 2023-07-14 17:32:32.537162 image_analyst_cv2-0.1.0/src/image_analyst/cv2/models.py
--rw-r--r--   0        0        0     4189 2023-07-14 17:33:56.616784 image_analyst_cv2-0.1.0/src/image_analyst/cv2/utils.py
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 image_analyst_cv2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_cv2-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1339 2023-07-17 12:44:00.452585 image_analyst_cv2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1282 2023-07-17 11:16:30.761026 image_analyst_cv2-0.1.1/README.md
+-rw-r--r--   0        0        0      203 2023-07-14 17:57:00.279840 image_analyst_cv2-0.1.1/src/image_analyst/cv2/__init__.py
+-rw-r--r--   0        0        0      923 2023-07-14 17:26:29.985398 image_analyst_cv2-0.1.1/src/image_analyst/cv2/image.py
+-rw-r--r--   0        0        0     9621 2023-07-17 12:43:43.910829 image_analyst_cv2-0.1.1/src/image_analyst/cv2/models.py
+-rw-r--r--   0        0        0     4189 2023-07-14 17:33:56.616784 image_analyst_cv2-0.1.1/src/image_analyst/cv2/utils.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 image_analyst_cv2-0.1.1/PKG-INFO
```

### Comparing `image_analyst_cv2-0.1.0/LICENSE` & `image_analyst_cv2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.0/pyproject.toml` & `image_analyst_cv2-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-cv2"
-version = "0.1.0"
+version = "0.1.1"
 description = "ImageAnalyst CV2 is an extension to the ImageAnalyst library, providing additional models and functions using cv2."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystCV2"
 keywords = ["image", "analysis", "cv2"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,32 +12,28 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
-image-analyst = "^0.1.0"
-opencv-python = {version = "^4.8.0.74", optional = true}
+image-analyst = "^0.1.2"
 opencv-contrib-python = {version = "^4.8.0.74", optional = true}
-opencv-python-headless = {version = "^4.8.0.74", optional = true}
 opencv-contrib-python-headless = {version = "^4.8.0.74", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
 
 [tool.poetry.extras]
-cv2 = ["opencv-python"]
-cv2-contrib = ["opencv-contrib-python"]
-cv2-headless = ["opencv-python-headless"]
-cv2-contrib-headless = ["opencv-contrib-python-headless"]
+cv2 = ["opencv-contrib-python"]
+cv2-headless = ["opencv-contrib-python-headless"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 relative_files = true
```

### Comparing `image_analyst_cv2-0.1.0/README.md` & `image_analyst_cv2-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,21 +5,36 @@
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) ~= 3.9
 - [pip](https://pip.pypa.io/en/stable/)
 
-## Download
+## Extras
 
-You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystCV2/releases).
+The application has some extras that can be installed:
 
-## Installation
+- `cv2`
+- `cv2-headless`
 
-You can install the application by running the following command:
+## Download & Installation
+
+There is two ways to download and install the application.
+
+### Using PyPI
+
+You can download and install the application using [PyPI](https://pypi.org/project/image-analyst-cv2/). To do so, run the following command:
+
+```bash
+pip install image-analyst-cv2
+```
+
+### Using the GitHub releases
+
+You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalystCV2/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst_cv2-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
```

### Comparing `image_analyst_cv2-0.1.0/src/image_analyst/cv2/image.py` & `image_analyst_cv2-0.1.1/src/image_analyst/cv2/image.py`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.0/src/image_analyst/cv2/models.py` & `image_analyst_cv2-0.1.1/src/image_analyst/cv2/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,25 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV3OpenCV: the new YoloV3OpenCV.
         """
         try:
             weights_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-coco.weights",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-coco.weights",  # noqa: E501
                 "cv2-yolov3-coco.weights",
                 report_callback,
             )
             config_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-coco.cfg",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-coco.cfg",  # noqa: E501
                 "cv2-yolov3-coco.cfg",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-coco.names",  # noqa: E501
                 "cv2-yolov3-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV3 model."
             ) from e
@@ -98,25 +98,25 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV3OpenCV: the new YoloV3OpenCV.
         """
         try:
             weights_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-tiny-coco.weights",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-tiny-coco.weights",  # noqa: E501
                 "cv2-yolov3-tiny-coco.weights",
                 report_callback,
             )
             config_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-tiny-coco.cfg",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-tiny-coco.cfg",  # noqa: E501
                 "cv2-yolov3-tiny-coco.cfg",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.0/cv2-yolov3-tiny-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystCV2/releases/download/v0.1.1/cv2-yolov3-tiny-coco.names",  # noqa: E501
                 "cv2-yolov3-tiny-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV3 model."
             ) from e
```

### Comparing `image_analyst_cv2-0.1.0/src/image_analyst/cv2/utils.py` & `image_analyst_cv2-0.1.1/src/image_analyst/cv2/utils.py`

 * *Files identical despite different names*

