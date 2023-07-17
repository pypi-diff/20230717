# Comparing `tmp/ortelius-cli-9.3.233.tar.gz` & `tmp/ortelius-cli-9.3.234.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.233.tar", last modified: Tue Apr 18 23:21:59 2023, max compression
+gzip compressed data, was "ortelius-cli-9.3.234.tar", last modified: Mon Jul 17 18:39:46 2023, max compression
```

## Comparing `ortelius-cli-9.3.233.tar` & `ortelius-cli-9.3.234.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.747339 ortelius-cli-9.3.233/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-03-09 18:41:03.000000 ortelius-cli-9.3.233/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2021-05-26 22:33:09.000000 ortelius-cli-9.3.233/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-18 23:21:59.744175 ortelius-cli-9.3.233/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-03-09 18:39:10.000000 ortelius-cli-9.3.233/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.732319 ortelius-cli-9.3.233/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    70590 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/bin/dh
--rwxr-xr-x   0 steve      (502) staff       (20)     3038 2023-03-23 17:39:44.000000 ortelius-cli-9.3.233/bin/helminfo.sh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.736856 ortelius-cli-9.3.233/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    74485 2023-04-18 23:20:46.000000 ortelius-cli-9.3.233/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.739018 ortelius-cli-9.3.233/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23766 2023-03-23 17:39:44.000000 ortelius-cli-9.3.233/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    10508 2023-03-23 17:40:27.000000 ortelius-cli-9.3.233/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.743387 ortelius-cli-9.3.233/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      308 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2023-04-18 23:21:59.747614 ortelius-cli-9.3.233/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1007 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-07-17 18:39:46.697337 ortelius-cli-9.3.234/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-03-09 18:41:03.000000 ortelius-cli-9.3.234/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2021-05-26 22:33:09.000000 ortelius-cli-9.3.234/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    11080 2023-07-17 18:39:46.696608 ortelius-cli-9.3.234/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-03-09 18:39:10.000000 ortelius-cli-9.3.234/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-07-17 18:39:46.678613 ortelius-cli-9.3.234/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70590 2023-07-17 18:38:16.000000 ortelius-cli-9.3.234/bin/dh
+-rwxr-xr-x   0 steve      (502) staff       (20)     3038 2023-03-23 17:39:44.000000 ortelius-cli-9.3.234/bin/helminfo.sh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-07-17 18:39:46.682391 ortelius-cli-9.3.234/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2023-07-17 18:38:16.000000 ortelius-cli-9.3.234/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    74485 2023-04-18 23:20:46.000000 ortelius-cli-9.3.234/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-07-17 18:39:46.687747 ortelius-cli-9.3.234/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23766 2023-03-23 17:39:44.000000 ortelius-cli-9.3.234/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    10508 2023-03-23 17:40:27.000000 ortelius-cli-9.3.234/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-07-17 18:39:46.695774 ortelius-cli-9.3.234/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    11080 2023-07-17 18:39:46.000000 ortelius-cli-9.3.234/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      308 2023-07-17 18:39:46.000000 ortelius-cli-9.3.234/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2023-07-17 18:39:46.000000 ortelius-cli-9.3.234/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       71 2023-07-17 18:39:46.000000 ortelius-cli-9.3.234/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2023-07-17 18:39:46.000000 ortelius-cli-9.3.234/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2023-07-17 18:39:46.697498 ortelius-cli-9.3.234/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1010 2023-07-17 18:38:16.000000 ortelius-cli-9.3.234/setup.py
```

### Comparing `ortelius-cli-9.3.233/LICENSE` & `ortelius-cli-9.3.234/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/PKG-INFO` & `ortelius-cli-9.3.234/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.233
+Version: 9.3.234
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.233/README.md` & `ortelius-cli-9.3.234/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/bin/dh` & `ortelius-cli-9.3.234/bin/dh`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.233"
+__version__ = "9.3.234"
 
 import json
 import os
 from pathlib import Path
 import re
 import stat
 import subprocess
```

### Comparing `ortelius-cli-9.3.233/bin/helminfo.sh` & `ortelius-cli-9.3.234/bin/helminfo.sh`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/deployhub/dhapi.py` & `ortelius-cli-9.3.234/deployhub/dhapi.py`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/doc/deployhub.md` & `ortelius-cli-9.3.234/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/doc/dh.md` & `ortelius-cli-9.3.234/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.233/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.234/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.233
+Version: 9.3.234
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.233/setup.py` & `ortelius-cli-9.3.234/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.233",
+    version="9.3.234",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh", "bin/helminfo.sh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
-    install_requires=["click", "qtoml", "PyYAML", "requests", "configobj", "flatten_dict", "pydantic", "certifi"],
+    install_requires=["click", "qtoml", "pyyaml==6", "requests", "configobj", "flatten_dict", "pydantic", "certifi"],
     include_package_data=True,
 )
```

