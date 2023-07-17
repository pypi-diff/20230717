# Comparing `tmp/streamlitopencvplayer-1.3.6.tar.gz` & `tmp/streamlitopencvplayer-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.6.tar", last modified: Sun Jul 16 23:12:06 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.7.tar", last modified: Mon Jul 17 14:10:46 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.6.tar` & `streamlitopencvplayer-1.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.703078 streamlitopencvplayer-1.3.6/
--rw-rw-rw-   0        0        0      419 2023-07-16 23:12:06.701580 streamlitopencvplayer-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 23:12:06.704076 streamlitopencvplayer-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-16 23:11:35.000000 streamlitopencvplayer-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.665312 streamlitopencvplayer-1.3.6/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6273 2023-07-16 23:11:21.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.686480 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.696533 streamlitopencvplayer-1.3.6/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.6/test/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-07-11 08:43:30.000000 streamlitopencvplayer-1.3.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.943077 streamlitopencvplayer-1.3.7/
+-rw-rw-rw-   0        0        0      419 2023-07-17 14:10:46.941072 streamlitopencvplayer-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:10:46.944073 streamlitopencvplayer-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-17 14:10:21.000000 streamlitopencvplayer-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.914071 streamlitopencvplayer-1.3.7/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6572 2023-07-17 14:10:03.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.930072 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-17 14:10:46.000000 streamlitopencvplayer-1.3.7/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 14:10:46.938071 streamlitopencvplayer-1.3.7/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.7/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.3.7/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.6/README.md` & `streamlitopencvplayer-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.3.6/setup.py` & `streamlitopencvplayer-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.6' 
+VERSION = '1.3.7' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.6/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.7/streamlitopencvplayer/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+import json
 import time
 import urllib.request
-import json
 
 import cv2
 import streamlit as st
 
-
-if "name_vid_sel" not in st.session_state:
-    st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 # Function to display video in the Streamlit app
 
 
 def display_video(video_path, json_file):
     # Open the video file
-    if "capture" not in st.session_state or st.session_state['old_vid_name'] != st.session_state['name_vid_sel']:
-        st.session_state['capture'] = cv2.VideoCapture(video_path)
+    # Check if video_url variables exists in session state
+    if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state :
+        if "capture" not in st.session_state:
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+            # or st.session_state['name_vid_old'] != st.session_state['name_vid_sel']
+    else :
+        if st.session_state['name_vid_old'] != st.session_state['name_vid_sel'] :
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+            st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
+
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
         exit()
     if "resume" not in st.session_state:
```

### Comparing `streamlitopencvplayer-1.3.6/test/test.py` & `streamlitopencvplayer-1.3.7/test/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 import argparse
 import uuid
 
 import streamlit as st
 
 from streamlitopencvplayer.app import display_video
 
-# Initiate all session states used
-if 'counter' not in st.session_state:
-    st.session_state['counter'] = 0
-if 'frames' not in st.session_state:
-    st.session_state['frames'] = []
 
 
 class opencvplayer:
     """Class streamlit opencv player."""
 
     def __init__(self, video_path, json_path):
         self.video_path = video_path
```

