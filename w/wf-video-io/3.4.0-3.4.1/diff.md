# Comparing `tmp/wf_video_io-3.4.0.tar.gz` & `tmp/wf_video_io-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.4.0.tar", max compression
+gzip compressed data, was "wf_video_io-3.4.1.tar", max compression
```

## Comparing `wf_video_io-3.4.0.tar` & `wf_video_io-3.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.4.0/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.4.0/README.md
--rw-r--r--   0        0        0     1181 2023-06-29 21:08:51.791466 wf_video_io-3.4.0/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.4.0/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.4.0/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    18738 2023-06-29 21:12:27.242562 wf_video_io-3.4.0/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-06-29 21:08:51.793888 wf_video_io-3.4.0/video_io/client/errors.py
--rw-r--r--   0        0        0     3412 2023-06-29 21:08:51.794977 wf_video_io-3.4.0/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.4.0/video_io/config.py
--rwxr-xr-x   0        0        0    49247 2023-06-29 21:14:15.999435 wf_video_io-3.4.0/video_io/core.py
--rw-r--r--   0        0        0       41 2023-06-29 21:08:51.797796 wf_video_io-3.4.0/video_io/errors.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.4.0/video_io/log_retry.py
--rw-r--r--   0        0        0    11076 2023-06-29 21:14:05.674928 wf_video_io-3.4.0/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.4.0/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.4.0/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.4.1/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.4.1/README.md
+-rw-r--r--   0        0        0     1181 2023-06-30 14:20:35.240825 wf_video_io-3.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0       50 2023-06-30 14:20:35.233610 wf_video_io-3.4.1/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.4.1/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    18738 2023-06-29 21:12:27.242562 wf_video_io-3.4.1/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-06-29 21:08:51.793888 wf_video_io-3.4.1/video_io/client/errors.py
+-rw-r--r--   0        0        0     3412 2023-06-29 21:08:51.794977 wf_video_io-3.4.1/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.4.1/video_io/config.py
+-rwxr-xr-x   0        0        0    49247 2023-06-29 21:14:15.999435 wf_video_io-3.4.1/video_io/core.py
+-rw-r--r--   0        0        0       41 2023-06-29 21:08:51.797796 wf_video_io-3.4.1/video_io/errors.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.4.1/video_io/log_retry.py
+-rw-r--r--   0        0        0    11210 2023-06-30 20:46:41.555236 wf_video_io-3.4.1/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.4.1/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.4.1/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.4.1/PKG-INFO
```

### Comparing `wf_video_io-3.4.0/LICENSE` & `wf_video_io-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/pyproject.toml` & `wf_video_io-3.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "wf-video-io"
 #dynamic = ["version"]
-version = "3.4.0"
+version = "3.4.1"
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.4.0"
+version = "3.4.1"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.4.0/video_io/client/core.py` & `wf_video_io-3.4.1/video_io/client/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/video_io/client/utils.py` & `wf_video_io-3.4.1/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/video_io/config.py` & `wf_video_io-3.4.1/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/video_io/core.py` & `wf_video_io-3.4.1/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/video_io/utils.py` & `wf_video_io-3.4.1/video_io/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,16 @@
                             format="concat",
                             safe=0,
                             r=video_snippet_fps,
                         ).output(
                             f"file:{video_output_path}",
                             c="copy",
                             r=video_snippet_fps,
-                            vsync=0,
+                            fps_mode=0,
+                            video_track_timescale=video_snippet_fps,
                         ).overwrite_output().global_args(
                             "-hide_banner", "-loglevel", "warning"
                         ).run()
                     except Exception as e:
                         logger.error(e)
                         raise e
 
@@ -182,18 +183,21 @@
     should_overwrite_input = input_path == output_path
     ffmpeg_output_path = output_path
     try:
         if should_overwrite_input:
             tmp_file = tempfile.NamedTemporaryFile(suffix=".mp4")
             ffmpeg_output_path = tmp_file.name
 
-        ffmpeg.input(input_path).output(
+        ffmpeg.input(
+            input_path,
+            r=fps,
+        ).output(
             ffmpeg_output_path,
             r=fps,
-            vf=f"trim=start_frame={int(start_trim * video_reader.fps())}:end_frame={int(end_trim * video_reader.fps())}",
+            vf=f"trim=start_frame={int(start_trim * video_reader.fps())}:end_frame={int(end_trim * video_reader.fps())},setpts=PTS-STARTPTS",
         ).overwrite_output().global_args("-hide_banner", "-loglevel", "warning").run()
 
         if should_overwrite_input:
             shutil.copy(ffmpeg_output_path, input_path)
     except ffmpeg._run.Error as e:
         logging.error(f"Failed trimming video {input_path}")
         logging.error(e)
```

### Comparing `wf_video_io-3.4.0/video_io/video_reader.py` & `wf_video_io-3.4.1/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.0/setup.py` & `wf_video_io-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.4.0',
+    'version': '3.4.1',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.4.0/PKG-INFO` & `wf_video_io-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.4.0
+Version: 3.4.1
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

