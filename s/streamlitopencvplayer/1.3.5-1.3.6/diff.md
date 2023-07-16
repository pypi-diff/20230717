# Comparing `tmp/streamlitopencvplayer-1.3.5.tar.gz` & `tmp/streamlitopencvplayer-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.5.tar", last modified: Thu Jul 13 13:06:02 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.6.tar", last modified: Sun Jul 16 23:12:06 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.5.tar` & `streamlitopencvplayer-1.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.478446 streamlitopencvplayer-1.3.5/
--rw-rw-rw-   0        0        0      419 2023-07-13 13:06:02.476444 streamlitopencvplayer-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 13:06:02.479447 streamlitopencvplayer-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-13 13:05:56.000000 streamlitopencvplayer-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.452445 streamlitopencvplayer-1.3.5/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-07-13 13:05:38.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.467446 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.473444 streamlitopencvplayer-1.3.5/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.5/test/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-07-11 08:43:30.000000 streamlitopencvplayer-1.3.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.703078 streamlitopencvplayer-1.3.6/
+-rw-rw-rw-   0        0        0      419 2023-07-16 23:12:06.701580 streamlitopencvplayer-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:12:06.704076 streamlitopencvplayer-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-16 23:11:35.000000 streamlitopencvplayer-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.665312 streamlitopencvplayer-1.3.6/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6273 2023-07-16 23:11:21.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.686480 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-16 23:12:06.000000 streamlitopencvplayer-1.3.6/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 23:12:06.696533 streamlitopencvplayer-1.3.6/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.6/test/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-07-11 08:43:30.000000 streamlitopencvplayer-1.3.6/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.5/README.md` & `streamlitopencvplayer-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.3.5/setup.py` & `streamlitopencvplayer-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.5' 
+VERSION = '1.3.6' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.5/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.6/streamlitopencvplayer/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 import streamlit as st
 
 
 if "name_vid_sel" not in st.session_state:
     st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 # Function to display video in the Streamlit app
 
+
 def display_video(video_path, json_file):
     # Open the video file
     if "capture" not in st.session_state or st.session_state['old_vid_name'] != st.session_state['name_vid_sel']:
         st.session_state['capture'] = cv2.VideoCapture(video_path)
     if "fps" not in st.session_state:
-        st.session_state['fps'] = st.session_state['capture'].get(cv2.CAP_PROP_FPS)
+        st.session_state['fps'] = st.session_state['capture'].get(
+            cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
         exit()
     if "resume" not in st.session_state:
         st.session_state["resume"] = False
     if "frame" not in st.session_state:
         ret, frame = st.session_state["capture"].read()
@@ -41,35 +43,36 @@
         data = []
 
         for x in range(len(list_ts)):
             time_alert = float(list_ts[x])-float(
                 st.session_state['name_vid_sel'].partition('_')[0])
             alerts.append(int((time_alert)*st.session_state['fps']))
             data.append(list_data[x])
-
+    # checkbox to enable detections
     draw_detections = st.checkbox("Draw detections", value=True)
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
         # zone to display images
         stframe = st.empty()
     with column3:
-        # Alerts
+        # Create buttons for alerts
         st.subheader('Alerts :')
         num_buttons = len(alerts)
 
         button_values = {f'{i}': 0 for i in range(num_buttons)}
 
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 button_values = {label: 1 if label ==
                                  button_label else 0 for label in button_values}
 
         for button_label, button_value in button_values.items():
             if button_value == 1:
-                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, alerts[int(button_label)])
+                st.session_state["capture"].set(
+                    cv2.CAP_PROP_POS_FRAMES, alerts[int(button_label)])
                 st.session_state["resume"] = True
 
     # Buttons and zone of display
     col1, col2, col3, col4, col5, col6, col7 = st.columns(7, gap="small")
     with col1:
         container_2 = st.empty()
         pause = container_2.button('⏸')
@@ -106,38 +109,36 @@
                 st.session_state["frame"], caption='', width=500)
             time.sleep(0.05)
 
             if pause:
                 st.session_state["resume"] = True
                 break
             if plus:
-                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-1)
-                st.write(int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)))
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(
+                    st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-1)
                 st.session_state["resume"] = True
                 break
             if minus:
-                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-3)
-                st.write(int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-3)
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(
+                    st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-3)
                 st.session_state["resume"] = True
                 break
 
             # back to the first frame if the video is finished
             if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['capture'].get(cv2.CAP_PROP_FRAME_COUNT)):
-                st.write("fps : ",int(st.session_state['capture'].get(cv2.CAP_PROP_FRAME_COUNT)))
-                st.write("cap : ",int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)))
-
                 st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, 0)
                 st.session_state["resume"] = True
                 break
 
     if st.session_state["resume"]:
         container_2.empty()
         pause = container_2.button('▶')
         st.session_state["resume"] = False
 
+
 def main():
 
     video_path = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138.webm?sv=2021-10-04&st=2023-07-11T15%3A21%3A27Z&se=2023-07-26T15%3A21%3A00Z&sr=b&sp=r&sig=u6uuOUo9wvn5KJFNUnUR3axYtC815SUQBuDqNIC4L%2Bw%3D"
     down_json = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138_global.json?sv=2021-10-04&st=2023-07-11T15%3A22%3A03Z&se=2023-07-26T15%3A22%3A00Z&sr=b&sp=r&sig=qSHWvDUIOOT%2F%2Bff270JVX7ucSRn5Lylgw5%2Fh9iTa4BY%3D"
     if video_path is not None:
         display_video(video_path, down_json)
```

### Comparing `streamlitopencvplayer-1.3.5/test/test.py` & `streamlitopencvplayer-1.3.6/test/test.py`

 * *Files identical despite different names*

