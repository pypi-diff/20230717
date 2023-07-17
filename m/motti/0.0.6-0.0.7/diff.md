# Comparing `tmp/motti-0.0.6.tar.gz` & `tmp/motti-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motti-0.0.6.tar", last modified: Mon Jul 17 12:06:33 2023, max compression
+gzip compressed data, was "motti-0.0.7.tar", last modified: Mon Jul 17 14:13:18 2023, max compression
```

## Comparing `motti-0.0.6.tar` & `motti-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.696720 motti-0.0.6/
--rw-rw-rw-   0        0        0      135 2023-07-17 12:06:33.695721 motti-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-07-17 12:06:03.000000 motti-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.687700 motti-0.0.6/motti/
--rw-rw-rw-   0        0        0      120 2023-07-17 12:00:05.000000 motti-0.0.6/motti/__init__.py
--rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.6/motti/dev.py
--rw-rw-rw-   0        0        0      909 2023-07-17 12:05:19.000000 motti-0.0.6/motti/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:06:33.694720 motti-0.0.6/motti.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.6/motti.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-17 12:06:33.000000 motti-0.0.6/motti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:06:33.696720 motti-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-07-17 12:06:24.000000 motti-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.830180 motti-0.0.7/
+-rw-rw-rw-   0        0        0      135 2023-07-17 14:13:18.830180 motti-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-17 14:13:01.000000 motti-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.823177 motti-0.0.7/motti/
+-rw-rw-rw-   0        0        0      161 2023-07-17 13:52:44.000000 motti-0.0.7/motti/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.7/motti/dev.py
+-rw-rw-rw-   0        0        0     1149 2023-07-17 14:10:47.000000 motti-0.0.7/motti/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.828175 motti-0.0.7/motti.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.7/motti.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:13:18.831183 motti-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-07-17 14:12:45.000000 motti-0.0.7/setup.py
```

### Comparing `motti-0.0.6/motti/tools.py` & `motti-0.0.7/motti/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from io import BytesIO
 import base64
 from PIL import Image
 from datetime import datetime
 import os
 from typing import Optional, Union
 from pathlib import Path
-
+import argparse
+import yaml
+from dataclasses import dataclass, asdict
 
 def pil2str(x):
     buffer = BytesIO()
     x.save(buffer, format='PNG')
     b64 = base64.b64encode(buffer.getvalue())
     res = str(b64, 'utf-8')
     return res
@@ -17,20 +19,30 @@
 def str2pil(s):
     b64 = base64.b64decode(s.encode('utf-8'))
     return Image.open(BytesIO(b64))
 
 def get_datetime():
     return datetime.now().strftime("%Y%m%d-%H%M%S")
 
-def project_dir_with(project_dir="."):
+def init_project_dir_with(project_dir="."):
     def f(*args, **kwargs):
         return os.path.join(project_dir, *args, **kwargs)
     return f
 
 def is_abs_path(path: Union[Path, str]):
     if isinstance(path, Path):
         return path.is_absolute()
     elif isinstance(path, str):
         return os.path.isabs(path)
     else:
         raise NotImplementedError 
         return False
+
+def load_yaml(path):
+    return yaml.safe_load(open(path, 'r'))
+
+def load_namespace(path):
+    D = load_yaml(path)
+    return argparse.Namespace(**D)
+
+
+
```

