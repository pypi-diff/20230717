# Comparing `tmp/streamlinkutils-0.0.1.tar.gz` & `tmp/streamlinkutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlinkutils-0.0.1.tar", max compression
+gzip compressed data, was "streamlinkutils-0.0.2.tar", max compression
```

## Comparing `streamlinkutils-0.0.1.tar` & `streamlinkutils-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    17096 2023-07-16 22:16:38.882339 streamlinkutils-0.0.1/LICENSE
--rw-r--r--   0        0        0      444 2023-07-16 22:24:21.205839 streamlinkutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2337 2023-07-16 22:14:27.723920 streamlinkutils-0.0.1/README.md
--rw-r--r--   0        0        0     8842 2023-07-16 22:12:35.510777 streamlinkutils-0.0.1/src/StreamlinkUtils/__init__.py
--rw-r--r--   0        0        0     2801 1970-01-01 00:00:00.000000 streamlinkutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    17096 2023-07-16 22:16:38.882339 streamlinkutils-0.0.2/LICENSE
+-rw-r--r--   0        0        0      602 2023-07-17 13:17:57.162647 streamlinkutils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2337 2023-07-16 22:14:27.723920 streamlinkutils-0.0.2/README.md
+-rw-r--r--   0        0        0     9258 2023-07-17 12:29:46.847347 streamlinkutils-0.0.2/src/StreamlinkUtils/__init__.py
+-rw-r--r--   0        0        0     2801 1970-01-01 00:00:00.000000 streamlinkutils-0.0.2/PKG-INFO
```

### Comparing `streamlinkutils-0.0.1/LICENSE` & `streamlinkutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlinkutils-0.0.1/README.md` & `streamlinkutils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlinkutils-0.0.1/src/StreamlinkUtils/__init__.py` & `streamlinkutils-0.0.2/src/StreamlinkUtils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import io
 import os
 import sys
 import time
 import platform
 import logging
 import streamlink
+import subprocess
 from typing import Optional
 from streamlink.stream.hls import HLSStream
 
 def dir_up(path: str) -> str:
     '''
     Returns the parent directory of the given path.
 
@@ -310,14 +311,32 @@
     Returns:
         str: The absolute path to the streamlink package folder.
     '''
 
     return os.path.abspath(streamlink.__file__)
 
 
+
+def install_pkg(pkg: str):
+    '''
+    Installs a package using pip into the streamlink pkgs folder.
+
+    Args:
+        pkg (str): The name of the package to install.
+
+    Returns:
+        None
+
+    Raises:
+        subprocess.CalledProcessError: If the pip installation command fails.
+    '''
+
+    subprocess.check_call(["pip", "install", "--target", get_pkgs_folder(), pkg])
+
+
 def get_streamlink_folder() -> str:
     '''
     Retrieves the path to the root streamlink folder.
 
     Returns:
         str: The path to the root streamlink folder.
     '''
```

### Comparing `streamlinkutils-0.0.1/PKG-INFO` & `streamlinkutils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: streamlinkutils
-Version: 0.0.1
-Summary: This module adds extra utilities to Streamlink's API. I am in no way connected with streamlink.
+Version: 0.0.2
+Summary: This module adds extra utilities to Streamlink's API. I am in no way connected with Streamlink.
 Author: Parrot Developers
 Author-email: redacted@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

