# Comparing `tmp/motti-0.0.7.tar.gz` & `tmp/motti-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motti-0.0.7.tar", last modified: Mon Jul 17 14:13:18 2023, max compression
+gzip compressed data, was "motti-0.0.8.tar", last modified: Mon Jul 17 16:38:49 2023, max compression
```

## Comparing `motti-0.0.7.tar` & `motti-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.830180 motti-0.0.7/
--rw-rw-rw-   0        0        0      135 2023-07-17 14:13:18.830180 motti-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-17 14:13:01.000000 motti-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.823177 motti-0.0.7/motti/
--rw-rw-rw-   0        0        0      161 2023-07-17 13:52:44.000000 motti-0.0.7/motti/__init__.py
--rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.7/motti/dev.py
--rw-rw-rw-   0        0        0     1149 2023-07-17 14:10:47.000000 motti-0.0.7/motti/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:18.828175 motti-0.0.7/motti.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.7/motti.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-17 14:13:18.000000 motti-0.0.7/motti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 14:13:18.831183 motti-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-07-17 14:12:45.000000 motti-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.230278 motti-0.0.8/
+-rw-rw-rw-   0        0        0      135 2023-07-17 16:38:49.229276 motti-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-17 14:13:01.000000 motti-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.221277 motti-0.0.8/motti/
+-rw-rw-rw-   0        0        0      184 2023-07-17 16:38:11.000000 motti-0.0.8/motti/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.8/motti/dev.py
+-rw-rw-rw-   0        0        0     1625 2023-07-17 16:37:20.000000 motti-0.0.8/motti/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.227284 motti-0.0.8/motti.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:38:49.230278 motti-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-07-17 16:38:37.000000 motti-0.0.8/setup.py
```

### Comparing `motti-0.0.7/motti/tools.py` & `motti-0.0.8/motti/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from datetime import datetime
 import os
 from typing import Optional, Union
 from pathlib import Path
 import argparse
 import yaml
 from dataclasses import dataclass, asdict
+import torch
+import numpy as np
+import random
 
 def pil2str(x):
     buffer = BytesIO()
     x.save(buffer, format='PNG')
     b64 = base64.b64encode(buffer.getvalue())
     res = str(b64, 'utf-8')
     return res
@@ -40,9 +43,15 @@
 def load_yaml(path):
     return yaml.safe_load(open(path, 'r'))
 
 def load_namespace(path):
     D = load_yaml(path)
     return argparse.Namespace(**D)
 
-
-
+def seed_everything(seed):
+    torch.manual_seed(seed)       # Current CPU
+    torch.cuda.manual_seed(seed)  # Current GPU
+    np.random.seed(seed)          # Numpy module
+    random.seed(seed)             # Python random module
+    torch.backends.cudnn.benchmark = False    # Close optimization
+    torch.backends.cudnn.deterministic = True # Close optimization
+    # torch.cuda.manual_seed_all(seed) # All GPU (Optional)
```

