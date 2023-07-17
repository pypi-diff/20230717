# Comparing `tmp/s2tutil-0.0.1.tar.gz` & `tmp/s2tutil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2tutil-0.0.1.tar", last modified: Mon Jul 17 16:19:51 2023, max compression
+gzip compressed data, was "s2tutil-0.0.2.tar", last modified: Mon Jul 17 18:26:15 2023, max compression
```

## Comparing `s2tutil-0.0.1.tar` & `s2tutil-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 16:19:51.521390 s2tutil-0.0.1/
--rw-r--r--   0 brainco    (501) staff       (20)     1967 2023-07-17 16:19:51.521068 s2tutil-0.0.1/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)     1272 2023-07-17 16:07:27.000000 s2tutil-0.0.1/README.md
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 16:19:51.516370 s2tutil-0.0.1/s2tutil/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:30:10.000000 s2tutil-0.0.1/s2tutil/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)      256 2023-07-14 20:48:27.000000 s2tutil-0.0.1/s2tutil/__main__.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 16:19:51.519358 s2tutil-0.0.1/s2tutil/transcriber/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:41:56.000000 s2tutil-0.0.1/s2tutil/transcriber/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     2983 2023-07-17 16:14:50.000000 s2tutil-0.0.1/s2tutil/transcriber/transcribe_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 16:19:51.520355 s2tutil-0.0.1/s2tutil/util/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:42:38.000000 s2tutil-0.0.1/s2tutil/util/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     1516 2023-07-17 15:03:06.000000 s2tutil-0.0.1/s2tutil/util/downloader.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 16:19:51.518741 s2tutil-0.0.1/s2tutil.egg-info/
--rw-r--r--   0 brainco    (501) staff       (20)     1967 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)      375 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/SOURCES.txt
--rw-r--r--   0 brainco    (501) staff       (20)        1 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/dependency_links.txt
--rw-r--r--   0 brainco    (501) staff       (20)       50 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/entry_points.txt
--rw-r--r--   0 brainco    (501) staff       (20)       33 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/requires.txt
--rw-r--r--   0 brainco    (501) staff       (20)        8 2023-07-17 16:19:51.000000 s2tutil-0.0.1/s2tutil.egg-info/top_level.txt
--rw-r--r--   0 brainco    (501) staff       (20)       38 2023-07-17 16:19:51.521491 s2tutil-0.0.1/setup.cfg
--rw-r--r--   0 brainco    (501) staff       (20)     1110 2023-07-17 15:00:38.000000 s2tutil-0.0.1/setup.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 18:26:15.931338 s2tutil-0.0.2/
+-rw-r--r--   0 brainco    (501) staff       (20)     1967 2023-07-17 18:26:15.930121 s2tutil-0.0.2/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)     1272 2023-07-17 16:07:27.000000 s2tutil-0.0.2/README.md
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 18:26:15.913244 s2tutil-0.0.2/s2tutil/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:30:10.000000 s2tutil-0.0.2/s2tutil/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)      256 2023-07-14 20:48:27.000000 s2tutil-0.0.2/s2tutil/__main__.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 18:26:15.925410 s2tutil-0.0.2/s2tutil/transcriber/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:41:56.000000 s2tutil-0.0.2/s2tutil/transcriber/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     2983 2023-07-17 16:14:50.000000 s2tutil-0.0.2/s2tutil/transcriber/transcribe_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 18:26:15.928483 s2tutil-0.0.2/s2tutil/util/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-07-14 19:42:38.000000 s2tutil-0.0.2/s2tutil/util/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     1516 2023-07-17 15:03:06.000000 s2tutil-0.0.2/s2tutil/util/downloader.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-07-17 18:26:15.922494 s2tutil-0.0.2/s2tutil.egg-info/
+-rw-r--r--   0 brainco    (501) staff       (20)     1967 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)      375 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/SOURCES.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        1 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/dependency_links.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       50 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/entry_points.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       32 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/requires.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        8 2023-07-17 18:26:15.000000 s2tutil-0.0.2/s2tutil.egg-info/top_level.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       38 2023-07-17 18:26:15.931748 s2tutil-0.0.2/setup.cfg
+-rw-r--r--   0 brainco    (501) staff       (20)     1109 2023-07-17 18:25:24.000000 s2tutil-0.0.2/setup.py
```

### Comparing `s2tutil-0.0.1/PKG-INFO` & `s2tutil-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2tutil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Audio to text transcription utility using whisper.cpp models
 Home-page: https://github.com/DavidSonoda/s2tutil
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `s2tutil-0.0.1/README.md` & `s2tutil-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `s2tutil-0.0.1/s2tutil/transcriber/transcribe_subcommand.py` & `s2tutil-0.0.2/s2tutil/transcriber/transcribe_subcommand.py`

 * *Files identical despite different names*

### Comparing `s2tutil-0.0.1/s2tutil/util/downloader.py` & `s2tutil-0.0.2/s2tutil/util/downloader.py`

 * *Files identical despite different names*

### Comparing `s2tutil-0.0.1/s2tutil.egg-info/PKG-INFO` & `s2tutil-0.0.2/s2tutil.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2tutil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Audio to text transcription utility using whisper.cpp models
 Home-page: https://github.com/DavidSonoda/s2tutil
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `s2tutil-0.0.1/setup.py` & `s2tutil-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="s2tutil",
-    version="0.0.1",
+    version="0.0.2",
     description="Audio to text transcription utility using whisper.cpp models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Juewei Dong",
     author_email="juewei.dong@brainco.tech",
     url="https://github.com/DavidSonoda/s2tutil",
     license="MIT",
@@ -26,9 +26,9 @@
     python_requires=">=3.7",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "s2tutil = s2tutil.__main__:main",
         ],
     },
-    install_requires=["pywhispercpp==1.1.0", "click==8.1.3"],
+    install_requires=["whispercpp==0.0.17", "click==8.1.3"],
 )
```

