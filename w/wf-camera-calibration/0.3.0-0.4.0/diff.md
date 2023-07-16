# Comparing `tmp/wf-camera-calibration-0.3.0.tar.gz` & `tmp/wf-camera-calibration-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-camera-calibration-0.3.0.tar", last modified: Thu Dec 22 23:50:44 2022, max compression
+gzip compressed data, was "wf-camera-calibration-0.4.0.tar", last modified: Sun Jul 16 22:38:57 2023, max compression
```

## Comparing `wf-camera-calibration-0.3.0.tar` & `wf-camera-calibration-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-22 23:50:44.731696 wf-camera-calibration-0.3.0/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/LICENSE
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2022-12-22 23:50:44.731696 wf-camera-calibration-0.3.0/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      585 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/README.md
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        6 2022-12-22 23:49:54.000000 wf-camera-calibration-0.3.0/VERSION
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-22 23:50:44.731696 wf-camera-calibration-0.3.0/camera_calibration/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       70 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/camera_calibration/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2530 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/camera_calibration/analyze.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    36325 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/camera_calibration/colmap.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    19191 2022-12-22 13:51:39.000000 wf-camera-calibration-0.3.0/camera_calibration/visualize.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2022-12-22 23:50:44.731696 wf-camera-calibration-0.3.0/setup.cfg
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1626 2022-12-19 18:03:55.000000 wf-camera-calibration-0.3.0/setup.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-22 23:50:44.731696 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2022-12-22 23:50:44.000000 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      392 2022-12-22 23:50:44.000000 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2022-12-22 23:50:44.000000 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      110 2022-12-22 23:50:44.000000 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       19 2022-12-22 23:50:44.000000 wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      585 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/README.md
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        6 2023-07-16 22:38:13.000000 wf-camera-calibration-0.4.0/VERSION
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/camera_calibration/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       70 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/camera_calibration/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2530 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/camera_calibration/analyze.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    36335 2023-07-16 22:37:29.000000 wf-camera-calibration-0.4.0/camera_calibration/colmap.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    19191 2023-01-07 15:16:24.000000 wf-camera-calibration-0.4.0/camera_calibration/visualize.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1626 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      392 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      110 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       19 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/top_level.txt
```

### Comparing `wf-camera-calibration-0.3.0/LICENSE` & `wf-camera-calibration-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.3.0/PKG-INFO` & `wf-camera-calibration-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-camera-calibration
-Version: 0.3.0
+Version: 0.4.0
 Summary: Support for calculating intrinsic and extrinsic camera calibration parameters using COLMAP and other tools
 Home-page: https://github.com/WildflowerSchools/wf-camera-calibration
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `wf-camera-calibration-0.3.0/README.md` & `wf-camera-calibration-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.3.0/camera_calibration/analyze.py` & `wf-camera-calibration-0.4.0/camera_calibration/analyze.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.3.0/camera_calibration/colmap.py` & `wf-camera-calibration-0.4.0/camera_calibration/colmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 CALIBRATION_DATA_RE = r'(?P<colmap_image_id>[0-9]+) (?P<qw>[-0-9.]+) (?P<qx>[-0-9.]+) (?P<qy>[-0-9.]+) (?P<qz>[-0-9.]+) (?P<tx>[-0-9.]+) (?P<ty>[-0-9.]+) (?P<tz>[-0-9.]+) (?P<colmap_camera_id>[0-9]+) (?P<image_path>.+)'
 
 RECOGNIZED_IMAGE_EXTENSIONS = ['png', 'jpg', 'jpeg', 'gif']
 
 def prepare_colmap_inputs(
     calibration_directory=None,
     calibration_identifier=None,
+    environment_id=None,
+    environment_name=None,
     image_info_path=None,
     images_directory_path=None,
     ref_images_data_path=None,
     additional_images=None,
     chunk_size=100,
     client=None,
     uri=None,
     token_uri=None,
     audience=None,
     client_id=None,
     client_secret=None,
     local_image_directory='./images',
     image_filename_extension='png',
     local_video_directory='./videos',
-    video_filename_extension='mp4'
 ):
     """
     Prepares COLMAP input files based on data in local files and in Honeycomb.
 
     The script pulls calibration images from Honeycomb for each camera. To do
     so, it requires a CSV file which lists each camera along with its camera
     type (can be any string; used to group images by their intrinsic
@@ -135,26 +136,26 @@
     ref_images_lines = list()
     for index, camera in image_info_df.iterrows():
         camera_device_id = camera['device_id']
         image_timestamp = camera['image_timestamp']
         camera_type = camera['camera_type']
         image_metadata = video_io.fetch_images(
             image_timestamps=[image_timestamp],
+            environment_id=environment_id,
+            environment_name=environment_name,
             camera_device_ids=[camera_device_id],
-            chunk_size=chunk_size,
+            local_image_directory=local_image_directory,
+            image_filename_extension=image_filename_extension,
+            local_video_directory=local_video_directory,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
             client_secret=client_secret,
-            local_image_directory=local_image_directory,
-            image_filename_extension=image_filename_extension,
-            local_video_directory=local_video_directory,
-            video_filename_extension=video_filename_extension
         )
         if len(image_metadata) > 1:
             raise ValueError('More than one image returned for this camera and timestamp')
         image_info = image_metadata[0]
         source_path = image_info['image_local_path']
         # Copy image file
         output_directory = os.path.join(
```

### Comparing `wf-camera-calibration-0.3.0/camera_calibration/visualize.py` & `wf-camera-calibration-0.4.0/camera_calibration/visualize.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.3.0/setup.py` & `wf-camera-calibration-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.3.0/wf_camera_calibration.egg-info/PKG-INFO` & `wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-camera-calibration
-Version: 0.3.0
+Version: 0.4.0
 Summary: Support for calculating intrinsic and extrinsic camera calibration parameters using COLMAP and other tools
 Home-page: https://github.com/WildflowerSchools/wf-camera-calibration
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

