# Comparing `tmp/motti-0.0.5.tar.gz` & `tmp/motti-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motti-0.0.5.tar", last modified: Mon Jul 17 12:02:04 2023, max compression
+gzip compressed data, was "motti-0.0.6.tar", last modified: Mon Jul 17 12:06:33 2023, max compression
```

## Comparing `motti-0.0.5.tar` & `motti-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.494141 motti-0.0.5/
--rw-rw-rw-   0        0        0      135 2023-07-17 12:02:04.493143 motti-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-17 12:01:24.000000 motti-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.485142 motti-0.0.5/motti/
--rw-rw-rw-   0        0        0      120 2023-07-17 12:00:05.000000 motti-0.0.5/motti/__init__.py
--rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.5/motti/dev.py
--rw-rw-rw-   0        0        0      908 2023-07-17 11:49:49.000000 motti-0.0.5/motti/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.492142 motti-0.0.5/motti.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.5/motti.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:02:04.494141 motti-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-07-17 12:00:13.000000 motti-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.696720 motti-0.0.6/
+-rw-rw-rw-   0        0        0      135 2023-07-17 12:06:33.695721 motti-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-07-17 12:06:03.000000 motti-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.687700 motti-0.0.6/motti/
+-rw-rw-rw-   0        0        0      120 2023-07-17 12:00:05.000000 motti-0.0.6/motti/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.6/motti/dev.py
+-rw-rw-rw-   0        0        0      909 2023-07-17 12:05:19.000000 motti-0.0.6/motti/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.694720 motti-0.0.6/motti.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.6/motti.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:06:33.696720 motti-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-07-17 12:06:24.000000 motti-0.0.6/setup.py
```

### Comparing `motti-0.0.5/motti/tools.py` & `motti-0.0.6/motti/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import BytesIO
 import base64
 from PIL import Image
 from datetime import datetime
 import os
-from typing import Optiona, Union
+from typing import Optional, Union
 from pathlib import Path
 
 
 def pil2str(x):
     buffer = BytesIO()
     x.save(buffer, format='PNG')
     b64 = base64.b64encode(buffer.getvalue())
```

