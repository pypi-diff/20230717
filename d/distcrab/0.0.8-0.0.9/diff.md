# Comparing `tmp/distcrab-0.0.8.tar.gz` & `tmp/distcrab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distcrab-0.0.8.tar", last modified: Mon Feb  6 03:53:08 2023, max compression
+gzip compressed data, was "distcrab-0.0.9.tar", last modified: Fri Feb 17 09:38:44 2023, max compression
```

## Comparing `distcrab-0.0.8.tar` & `distcrab-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-06 03:53:08.336375 distcrab-0.0.8/
--rw-r--r--   0 debian    (1000) debian    (1000)       18 2022-11-01 05:29:26.000000 distcrab-0.0.8/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)      554 2023-02-06 03:53:08.336375 distcrab-0.0.8/PKG-INFO
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-06 03:53:08.336375 distcrab-0.0.8/distcrab/
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2023-02-03 07:59:32.000000 distcrab-0.0.8/distcrab/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      830 2023-02-06 03:49:49.000000 distcrab-0.0.8/distcrab/__main__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4630 2023-02-06 03:50:10.000000 distcrab-0.0.8/distcrab/main.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-06 03:53:08.336375 distcrab-0.0.8/distcrab.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)      554 2023-02-06 03:53:08.000000 distcrab-0.0.8/distcrab.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      248 2023-02-06 03:53:08.000000 distcrab-0.0.8/distcrab.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-02-06 03:53:08.000000 distcrab-0.0.8/distcrab.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       19 2023-02-06 03:53:08.000000 distcrab-0.0.8/distcrab.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        9 2023-02-06 03:53:08.000000 distcrab-0.0.8/distcrab.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)      188 2023-02-06 01:54:37.000000 distcrab-0.0.8/readme.md
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-02-06 03:53:08.336375 distcrab-0.0.8/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)      649 2023-02-06 03:50:42.000000 distcrab-0.0.8/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-17 09:38:44.125026 distcrab-0.0.9/
+-rw-r--r--   0 debian    (1000) debian    (1000)       18 2022-11-01 05:29:26.000000 distcrab-0.0.9/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)      554 2023-02-17 09:38:44.125026 distcrab-0.0.9/PKG-INFO
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-17 09:38:44.125026 distcrab-0.0.9/distcrab/
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2023-02-03 07:59:32.000000 distcrab-0.0.9/distcrab/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      830 2023-02-06 03:49:49.000000 distcrab-0.0.9/distcrab/__main__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4564 2023-02-17 09:35:48.000000 distcrab-0.0.9/distcrab/main.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-02-17 09:38:44.125026 distcrab-0.0.9/distcrab.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)      554 2023-02-17 09:38:44.000000 distcrab-0.0.9/distcrab.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      248 2023-02-17 09:38:44.000000 distcrab-0.0.9/distcrab.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-02-17 09:38:44.000000 distcrab-0.0.9/distcrab.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       19 2023-02-17 09:38:44.000000 distcrab-0.0.9/distcrab.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        9 2023-02-17 09:38:44.000000 distcrab-0.0.9/distcrab.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      188 2023-02-06 01:54:37.000000 distcrab-0.0.9/readme.md
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-02-17 09:38:44.125026 distcrab-0.0.9/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)      649 2023-02-17 09:35:57.000000 distcrab-0.0.9/setup.py
```

### Comparing `distcrab-0.0.8/PKG-INFO` & `distcrab-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distcrab
-Version: 0.0.8
+Version: 0.0.9
 Summary: distcrab
 Home-page: http://255.255.255.255/
 Author: distcrab
 Author-email: root@localhost.localdomain
 License: UNLISENCED
 Description: ```bash
         python3 -m pip install --upgrade distcrab
```

### Comparing `distcrab-0.0.8/distcrab/__main__.py` & `distcrab-0.0.9/distcrab/__main__.py`

 * *Files identical despite different names*

### Comparing `distcrab-0.0.8/distcrab/main.py` & `distcrab-0.0.9/distcrab/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from io import StringIO, FileIO, BytesIO
 from pathlib import PurePosixPath
 from socket import socket
 from urllib.request import urlopen
 from tarfile import open
 from paramiko import Transport, SSHException, SFTPClient
 from git.cmd import Git
-from git import Repo
 from logging import getLogger
 
 logger = getLogger()
 
 class Tar():
     def __init__(self, **kwargs):
         self.kwargs = kwargs
@@ -21,15 +20,15 @@
         if kwargs.get('version'):
             version = kwargs.get('version')
             src = BytesIO(urlopen(f'''http://192.168.21.1:5080/APP/develop/develop/update/industry/crab/dists/crab-{version}.tar.xz''').read())
         elif kwargs.get('branch'):
             version = BytesIO(urlopen(f'''http://192.168.21.1:5080/APP/develop/develop/update/industry/crab/heads/{kwargs.get('branch')}.txt''').read()).read().decode()
             src = BytesIO(urlopen(f'''http://192.168.21.1:5080/APP/develop/develop/update/industry/crab/dists/crab-{version}.tar.xz''').read())
         else:
-            version = Git().describe(Repo(search_parent_directories=True).head.object.hexsha, tags=True, abbrev=True, always=True, long=True)
+            version = Git().describe(tags=True, abbrev=True, always=True, long=True, dirty=True)
             src = FileIO(f'''var/crab-{version}.tar.xz''')
         self.version = version
         self.src = src
 
     def __iter__(self):
         yield (PurePosixPath(f'''/dev/shm/crab.tar.xz'''), self.src)
```

### Comparing `distcrab-0.0.8/distcrab.egg-info/PKG-INFO` & `distcrab-0.0.9/distcrab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distcrab
-Version: 0.0.8
+Version: 0.0.9
 Summary: distcrab
 Home-page: http://255.255.255.255/
 Author: distcrab
 Author-email: root@localhost.localdomain
 License: UNLISENCED
 Description: ```bash
         python3 -m pip install --upgrade distcrab
```

### Comparing `distcrab-0.0.8/setup.py` & `distcrab-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 name = 'distcrab'
 
 setup(
     name = name,
-    version = '0.0.8',
+    version = '0.0.9',
     keywords = [name],
     description = name,
     long_description=(Path(__file__).parent / 'readme.md').read_text(),
     long_description_content_type='text/markdown',
     license = 'UNLISENCED',
     url = 'http://255.255.255.255/',
     author = name,
```

