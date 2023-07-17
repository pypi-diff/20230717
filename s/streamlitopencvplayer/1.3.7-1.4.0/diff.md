# Comparing `tmp/streamlitopencvplayer-1.3.7.tar.gz` & `tmp/streamlitopencvplayer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.7.tar", last modified: Mon Jul 17 14:10:46 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.4.0.tar", last modified: Mon Jul 17 14:37:34 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.7.tar` & `streamlitopencvplayer-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.943077 streamlitopencvplayer-1.3.7/
--rw-rw-rw-   0        0        0      419 2023-07-17 14:10:46.941072 streamlitopencvplayer-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 14:10:46.944073 streamlitopencvplayer-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-17 14:10:21.000000 streamlitopencvplayer-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.914071 streamlitopencvplayer-1.3.7/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6572 2023-07-17 14:10:03.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.930072 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.938071 streamlitopencvplayer-1.3.7/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.7/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.3.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:37:34.457541 streamlitopencvplayer-1.4.0/
+-rw-rw-rw-   0        0        0      419 2023-07-17 14:37:34.456542 streamlitopencvplayer-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:37:34.458544 streamlitopencvplayer-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-17 14:37:28.000000 streamlitopencvplayer-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:37:34.428548 streamlitopencvplayer-1.4.0/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8011 2023-07-17 14:34:33.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:37:34.445546 streamlitopencvplayer-1.4.0/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-17 14:37:34.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-17 14:37:34.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:37:34.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-17 14:37:34.000000 streamlitopencvplayer-1.4.0/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 14:37:34.452543 streamlitopencvplayer-1.4.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.0/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.7/README.md` & `streamlitopencvplayer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.3.7/setup.py` & `streamlitopencvplayer-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.7' 
+VERSION = '1.4.0' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.7/test/test.py` & `streamlitopencvplayer-1.4.0/test/test.py`

 * *Files identical despite different names*

