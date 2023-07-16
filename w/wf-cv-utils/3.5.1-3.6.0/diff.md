# Comparing `tmp/wf-cv-utils-3.5.1.tar.gz` & `tmp/wf-cv-utils-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-cv-utils-3.5.1.tar", last modified: Sun Jul 16 17:55:28 2023, max compression
+gzip compressed data, was "wf-cv-utils-3.6.0.tar", last modified: Sun Jul 16 23:35:06 2023, max compression
```

## Comparing `wf-cv-utils-3.5.1.tar` & `wf-cv-utils-3.6.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/LICENSE
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1495 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/README.md
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        5 2023-07-16 17:54:46.000000 wf-cv-utils-3.5.1/VERSION
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/cv_utils/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      195 2023-07-16 17:52:59.000000 wf-cv-utils-3.5.1/cv_utils/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    34095 2023-07-16 13:26:52.000000 wf-cv-utils-3.5.1/cv_utils/aruco.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      327 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/color.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    24937 2023-07-16 15:43:51.000000 wf-cv-utils-3.5.1/cv_utils/core.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/cv_utils/drawing/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/drawing/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4150 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/drawing/matplotlib.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    11003 2023-07-16 15:40:10.000000 wf-cv-utils-3.5.1/cv_utils/drawing/opencv.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4966 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/eager_video_capture.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     7160 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/video.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/setup.cfg
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1011 2023-07-16 15:40:14.000000 wf-cv-utils-3.5.1/setup.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      431 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       67 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        9 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-08 20:56:25.000000 wf-cv-utils-3.6.0/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-08 20:56:25.000000 wf-cv-utils-3.6.0/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1495 2022-12-08 20:56:25.000000 wf-cv-utils-3.6.0/README.md
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        5 2023-07-16 23:32:31.000000 wf-cv-utils-3.6.0/VERSION
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/cv_utils/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      225 2023-07-16 22:05:06.000000 wf-cv-utils-3.6.0/cv_utils/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    34095 2023-07-16 22:03:30.000000 wf-cv-utils-3.6.0/cv_utils/aruco.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    16002 2023-07-16 23:25:41.000000 wf-cv-utils-3.6.0/cv_utils/colmap.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      380 2023-07-16 22:03:25.000000 wf-cv-utils-3.6.0/cv_utils/color.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    24991 2023-07-16 22:03:24.000000 wf-cv-utils-3.6.0/cv_utils/core.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/cv_utils/drawing/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-08 20:56:25.000000 wf-cv-utils-3.6.0/cv_utils/drawing/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4204 2023-07-16 22:03:44.000000 wf-cv-utils-3.6.0/cv_utils/drawing/matplotlib.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    11056 2023-07-16 22:03:39.000000 wf-cv-utils-3.6.0/cv_utils/drawing/opencv.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4966 2023-07-16 22:03:21.000000 wf-cv-utils-3.6.0/cv_utils/eager_video_capture.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     7160 2023-07-16 22:03:19.000000 wf-cv-utils-3.6.0/cv_utils/video.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1011 2023-07-16 17:56:52.000000 wf-cv-utils-3.6.0/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:35:05.995186 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 23:35:05.000000 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      450 2023-07-16 23:35:05.000000 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 23:35:05.000000 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       67 2023-07-16 23:35:05.000000 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        9 2023-07-16 23:35:05.000000 wf-cv-utils-3.6.0/wf_cv_utils.egg-info/top_level.txt
```

### Comparing `wf-cv-utils-3.5.1/LICENSE` & `wf-cv-utils-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/PKG-INFO` & `wf-cv-utils-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.5.1
+Version: 3.6.0
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

### Comparing `wf-cv-utils-3.5.1/README.md` & `wf-cv-utils-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/cv_utils/aruco.py` & `wf-cv-utils-3.6.0/cv_utils/aruco.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/cv_utils/core.py` & `wf-cv-utils-3.6.0/cv_utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import cv2 as cv
 import numpy as np
 import os
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 def termination_criteria(
     max_iterations=10000,
     accuracy=1e-9
 ):
     termination_criteria = (cv.TERM_CRITERIA_COUNT & cv.TERM_CRITERIA_EPS, max_iterations, accuracy)
     return termination_criteria
```

### Comparing `wf-cv-utils-3.5.1/cv_utils/drawing/matplotlib.py` & `wf-cv-utils-3.6.0/cv_utils/drawing/matplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import cv2 as cv
 import numpy as np
 import matplotlib.pyplot as plt
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 # Fetch an image from a local image file and return it in OpenCV format
 def fetch_image_from_local_drive(image_path):
     image = cv.imread(image_path)
     return image
 
 def plot_2d_image_points(
```

### Comparing `wf-cv-utils-3.5.1/cv_utils/drawing/opencv.py` & `wf-cv-utils-3.6.0/cv_utils/drawing/opencv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import cv2 as cv
 import cv_utils.color
 import pandas as pd
 import numpy as np
 import math
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 MARKER_DICT = {
     '+': cv.MARKER_CROSS,
     'x': cv.MARKER_TILTED_CROSS,
     '*': cv.MARKER_STAR,
     'd': cv.MARKER_DIAMOND,
```

### Comparing `wf-cv-utils-3.5.1/cv_utils/eager_video_capture.py` & `wf-cv-utils-3.6.0/cv_utils/eager_video_capture.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/cv_utils/video.py` & `wf-cv-utils-3.6.0/cv_utils/video.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/setup.py` & `wf-cv-utils-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.1/wf_cv_utils.egg-info/PKG-INFO` & `wf-cv-utils-3.6.0/wf_cv_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.5.1
+Version: 3.6.0
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

