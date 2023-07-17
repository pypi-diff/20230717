# Comparing `tmp/fc2-live-dl-2.1.3.tar.gz` & `tmp/fc2-live-dl-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc2-live-dl-2.1.3.tar", last modified: Mon May 22 02:59:43 2023, max compression
+gzip compressed data, was "fc2-live-dl-2.2.0.tar", last modified: Mon Jul 17 16:50:02 2023, max compression
```

## Comparing `fc2-live-dl-2.1.3.tar` & `fc2-live-dl-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     1064 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/LICENSE
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/PKG-INFO
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     9890 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/README.md
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/fc2_live_dl/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    15362 2023-05-22 02:52:09.000000 fc2-live-dl-2.1.3/fc2_live_dl/FC2LiveDL.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     6125 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/__init__.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       58 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/__main__.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4160 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/autofc2.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10405 2023-04-04 06:42:28.000000 fc2-live-dl-2.1.3/fc2_live_dl/fc2.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     2751 2023-05-22 02:52:39.000000 fc2-live-dl-2.1.3/fc2_live_dl/ffmpeg.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     5448 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/hls.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4357 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/util.py
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/PKG-INFO
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      446 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/SOURCES.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)        1 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/dependency_links.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       84 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/entry_points.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       29 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/requires.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       12 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/top_level.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      104 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/pyproject.toml
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      947 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/setup.cfg
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-07-17 16:50:02.836269 fc2-live-dl-2.2.0/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     1064 2023-03-05 12:06:34.000000 fc2-live-dl-2.2.0/LICENSE
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    11417 2023-07-17 16:50:02.836269 fc2-live-dl-2.2.0/PKG-INFO
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10713 2023-07-17 16:28:49.000000 fc2-live-dl-2.2.0/README.md
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-07-17 16:50:02.836269 fc2-live-dl-2.2.0/fc2_live_dl/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    18426 2023-07-17 16:16:44.000000 fc2-live-dl-2.2.0/fc2_live_dl/FC2LiveDL.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     6102 2023-07-17 14:29:14.000000 fc2-live-dl-2.2.0/fc2_live_dl/__init__.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       58 2023-03-05 12:06:34.000000 fc2-live-dl-2.2.0/fc2_live_dl/__main__.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4951 2023-07-17 16:19:45.000000 fc2-live-dl-2.2.0/fc2_live_dl/autofc2.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10405 2023-04-04 06:42:28.000000 fc2-live-dl-2.2.0/fc2_live_dl/fc2.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     2751 2023-05-22 02:52:39.000000 fc2-live-dl-2.2.0/fc2_live_dl/ffmpeg.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     5448 2023-03-05 12:06:34.000000 fc2-live-dl-2.2.0/fc2_live_dl/hls.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4357 2023-03-05 12:06:34.000000 fc2-live-dl-2.2.0/fc2_live_dl/util.py
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-07-17 16:50:02.836269 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    11417 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/PKG-INFO
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      446 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)        1 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       84 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/entry_points.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       44 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/requires.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       12 2023-07-17 16:50:02.000000 fc2-live-dl-2.2.0/fc2_live_dl.egg-info/top_level.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      104 2023-03-05 12:06:34.000000 fc2-live-dl-2.2.0/pyproject.toml
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      965 2023-07-17 16:50:02.836269 fc2-live-dl-2.2.0/setup.cfg
```

### Comparing `fc2-live-dl-2.1.3/LICENSE` & `fc2-live-dl-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.3/PKG-INFO` & `fc2-live-dl-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc2-live-dl
-Version: 2.1.3
+Version: 2.2.0
 Summary: Download live streams from FC2
 Home-page: https://github.com/HoloArchivists/fc2-live-dl
 Author: Hizkia Felix
 Author-email: felix@hizkifw.me
 Project-URL: Bug Tracker, https://github.com/HoloArchivists/fc2-live-dl/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,29 +17,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fc2-live-dl
 
 > Tool to download FC2 live streams
 
-[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ 'PyPI')
+[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ "PyPI")
 
 ## Requirements
 
 - Python 3.8
 - ffmpeg
 
 ## Features
 
 - Wait for a stream to start and automatically start recording
 - Save comment/chat logs
 - Authenticate with cookies (Netscape format, same one used with youtube-dl)
 - Remux recordings to .mp4/.m4a after it's done
 - Continuously monitor multiple streams in parallel and automatically start
   downloading when any of them goes online
+- Get notifications when streams come online via
+  [Apprise](https://github.com/caronc/apprise)
 
 ## Installation
 
 ### Using pip
 
 To install the latest stable version:
 
@@ -167,14 +169,20 @@
     "wait_poll_interval": 5,
     "cookies_file": null,
     "remux": true,
     "keep_intermediates": false,
     "extract_audio": true,
     "trust_env_proxy": false
   },
+  "notifications": [
+    {
+      "url": "discord://{WebhookID}/{WebhookToken}",
+      "message": "%(channel_name)s is live!\nhttps://live.fc2.com/%(channel_id)s"
+    }
+  ],
   "channels": {
     "91544481": {
       "_en_name": "Necoma Karin",
       "quality": "sound",
       "write_thumbnail": true
     },
     "72364867": { "_en_name": "Uno Sakura" },
@@ -190,14 +198,27 @@
 properly. You can also override the parameters per-channel.
 
 Arbitrary parameters can be specified by prefixing them with `_`, and will be
 accessible in `outtmpl`. This is useful for specifying custom filenames just
 like in the example above. In the example I'm using `_en_name`, but you can use
 anything as long as it starts with `_`.
 
+For notifications, the URL follows the
+[Apprise syntax](https://github.com/caronc/apprise#supported-notifications). For
+example, if you want to use Discord webhooks, use the `discord://` like so:
+
+- Original URL: `https://discord.com/api/webhooks/12341234/abcdabcd`
+- Turns into: `discord://12341234/abcdabcd`
+
+You can find out more about the different types of notifiers and how to
+configure them on
+[Apprise's GitHub](https://github.com/caronc/apprise#supported-notifications).
+
+The `message` of the notifications follow the same syntax as `outtmpl`.
+
 **NOTE Windows users**: When specifying a file path (e.g. for cookies) in the
 json, double up your backslashes, for example:
 `"cookies_file": "C:\\Documents\\cookies.txt"`.
 
 Once configured, you can run the script:
 
 ```
```

### Comparing `fc2-live-dl-2.1.3/README.md` & `fc2-live-dl-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # fc2-live-dl
 
 > Tool to download FC2 live streams
 
-[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ 'PyPI')
+[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ "PyPI")
 
 ## Requirements
 
 - Python 3.8
 - ffmpeg
 
 ## Features
 
 - Wait for a stream to start and automatically start recording
 - Save comment/chat logs
 - Authenticate with cookies (Netscape format, same one used with youtube-dl)
 - Remux recordings to .mp4/.m4a after it's done
 - Continuously monitor multiple streams in parallel and automatically start
   downloading when any of them goes online
+- Get notifications when streams come online via
+  [Apprise](https://github.com/caronc/apprise)
 
 ## Installation
 
 ### Using pip
 
 To install the latest stable version:
 
@@ -148,14 +150,20 @@
     "wait_poll_interval": 5,
     "cookies_file": null,
     "remux": true,
     "keep_intermediates": false,
     "extract_audio": true,
     "trust_env_proxy": false
   },
+  "notifications": [
+    {
+      "url": "discord://{WebhookID}/{WebhookToken}",
+      "message": "%(channel_name)s is live!\nhttps://live.fc2.com/%(channel_id)s"
+    }
+  ],
   "channels": {
     "91544481": {
       "_en_name": "Necoma Karin",
       "quality": "sound",
       "write_thumbnail": true
     },
     "72364867": { "_en_name": "Uno Sakura" },
@@ -171,14 +179,27 @@
 properly. You can also override the parameters per-channel.
 
 Arbitrary parameters can be specified by prefixing them with `_`, and will be
 accessible in `outtmpl`. This is useful for specifying custom filenames just
 like in the example above. In the example I'm using `_en_name`, but you can use
 anything as long as it starts with `_`.
 
+For notifications, the URL follows the
+[Apprise syntax](https://github.com/caronc/apprise#supported-notifications). For
+example, if you want to use Discord webhooks, use the `discord://` like so:
+
+- Original URL: `https://discord.com/api/webhooks/12341234/abcdabcd`
+- Turns into: `discord://12341234/abcdabcd`
+
+You can find out more about the different types of notifiers and how to
+configure them on
+[Apprise's GitHub](https://github.com/caronc/apprise#supported-notifications).
+
+The `message` of the notifications follow the same syntax as `outtmpl`.
+
 **NOTE Windows users**: When specifying a file path (e.g. for cookies) in the
 json, double up your backslashes, for example:
 `"cookies_file": "C:\\Documents\\cookies.txt"`.
 
 Once configured, you can run the script:
 
 ```
```

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/FC2LiveDL.py` & `fc2-live-dl-2.2.0/fc2_live_dl/FC2LiveDL.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,43 @@
 import asyncio
 import http.cookies
 import json
 import os
 import pathlib
 import time
 from datetime import datetime
+from enum import Enum
 
 import aiohttp
 
 from .fc2 import FC2LiveStream, FC2WebSocket
 from .ffmpeg import FFMpeg
 from .hls import HLSDownloader
 from .util import Logger, sanitize_filename
 
 
+class CallbackEvent:
+    class Type(Enum):
+        WAITING_FOR_ONLINE = 1
+        STREAM_ONLINE = 2
+        WAITING_FOR_TARGET_QUALITY = 3
+        GOT_HLS_URL = 4
+        FRAGMENT_PROGRESS = 5
+        MUXING = 6
+
+    def __init__(self, instance, channel_id, type: Type, data=None):
+        self.instance = instance
+        self.channel_id = channel_id
+        self.type = type
+        self.data = data
+
+    def __repr__(self):
+        return f"CallbackEvent({self.channel_id}, {self.type}, {self.data})"
+
+
 class FC2LiveDL:
     # Constants
     STREAM_QUALITY = {
         "150Kbps": 10,
         "400Kbps": 20,
         "1.2Mbps": 30,
         "2Mbps": 40,
@@ -43,22 +63,22 @@
         "wait_for_quality_timeout": 15,
         "wait_poll_interval": 5,
         "cookies_file": None,
         "remux": True,
         "keep_intermediates": False,
         "extract_audio": False,
         "trust_env_proxy": False,
-        # Debug params
         "dump_websocket": False,
     }
 
-    def __init__(self, params={}):
+    def __init__(self, params={}, callback=None):
         self._logger = Logger("fc2")
         self._session = None
         self._background_tasks = []
+        self._callback = callback if callback is not None else lambda e: None
 
         self.params = json.loads(json.dumps(self.DEFAULT_PARAMS))
         self.params.update(params)
         # Validate outtmpl
         self._format_outtmpl()
 
         # Parse cookies
@@ -107,17 +127,32 @@
 
             self._logger.info("Fetching stream info")
 
             is_online = await live.is_online()
             if not is_online:
                 if not self.params["wait_for_live"]:
                     raise FC2LiveStream.NotOnlineException()
+                self._callback(
+                    CallbackEvent(
+                        self,
+                        channel_id,
+                        CallbackEvent.Type.WAITING_FOR_ONLINE,
+                    )
+                )
                 await live.wait_for_online(self.params["wait_poll_interval"])
 
             meta = await live.get_meta(refetch=False)
+            self._callback(
+                CallbackEvent(
+                    self,
+                    channel_id,
+                    CallbackEvent.Type.STREAM_ONLINE,
+                    meta,
+                )
+            )
 
             fname_info = self._prepare_file(meta, "info.json")
             fname_thumb = self._prepare_file(meta, "png")
             fname_stream = self._prepare_file(meta, "ts")
             fname_chat = self._prepare_file(meta, "fc2chat.json")
             fname_muxed = self._prepare_file(
                 meta, "m4a" if self.params["quality"] == "sound" else "mp4"
@@ -166,30 +201,55 @@
                             "Requested quality",
                             self._format_mode(mode),
                             "is not available, waiting ({}/{}s)".format(
                                 round(time.time() - started),
                                 self.params["wait_for_quality_timeout"],
                             ),
                         )
+                        self._callback(
+                            CallbackEvent(
+                                self,
+                                channel_id,
+                                CallbackEvent.Type.WAITING_FOR_TARGET_QUALITY,
+                                {
+                                    "requested": self._format_mode(mode),
+                                    "available": self._format_mode(got_mode),
+                                    "hls_info": hls_info,
+                                },
+                            )
+                        )
                         await asyncio.sleep(1)
 
                 if got_mode != mode:
                     self._logger.warn(
                         "Timeout reached, falling back to next best quality",
                         self._format_mode(got_mode),
                     )
 
+                self._callback(
+                    CallbackEvent(
+                        self,
+                        channel_id,
+                        CallbackEvent.Type.GOT_HLS_URL,
+                        {
+                            "requested": self._format_mode(mode),
+                            "available": self._format_mode(got_mode),
+                            "hls_url": hls_url,
+                        },
+                    )
+                )
+
                 self._logger.info("Received HLS info")
 
                 coros = []
 
                 coros.append(ws.wait_disconnection())
 
                 self._logger.info("Writing stream to", fname_stream)
-                coros.append(self._download_stream(hls_url, fname_stream))
+                coros.append(self._download_stream(channel_id, hls_url, fname_stream))
 
                 if self.params["write_chat"]:
                     self._logger.info("Writing chat to", fname_chat)
                     coros.append(self._download_chat(ws, fname_chat))
 
                 tasks = [asyncio.create_task(coro) for coro in coros]
 
@@ -224,33 +284,35 @@
 
         if (
             fname_stream is not None
             and self.params["remux"]
             and os.path.isfile(fname_stream)
         ):
             self._logger.info("Remuxing stream to", fname_muxed)
-            await self._remux_stream(fname_stream, fname_muxed)
+            await self._remux_stream(channel_id, fname_stream, fname_muxed)
             self._logger.debug("Finished remuxing stream", fname_muxed)
 
             if self.params["extract_audio"]:
                 self._logger.info("Extracting audio to", fname_audio)
-                await self._remux_stream(fname_stream, fname_audio, extra_flags=["-vn"])
+                await self._remux_stream(
+                    channel_id, fname_stream, fname_audio, extra_flags=["-vn"]
+                )
                 self._logger.debug("Finished remuxing stream", fname_muxed)
 
             if not self.params["keep_intermediates"] and os.path.isfile(fname_muxed):
                 self._logger.info("Removing intermediate files")
                 os.remove(fname_stream)
             else:
                 self._logger.debug("Not removing intermediates")
         else:
             self._logger.debug("Not remuxing stream")
 
         self._logger.info("Done")
 
-    async def _download_stream(self, hls_url, fname):
+    async def _download_stream(self, channel_id, hls_url, fname):
         def sizeof_fmt(num, suffix="B"):
             for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
                 if abs(num) < 1024.0:
                     return f"{num:3.1f}{unit}{suffix}"
                 num /= 1024.0
             return f"{num:.1f}Yi{suffix}"
 
@@ -268,20 +330,31 @@
                         self._logger.info(
                             "Downloaded",
                             n_frags,
                             "fragments,",
                             sizeof_fmt(total_size),
                             inline=True,
                         )
+                        self._callback(
+                            CallbackEvent(
+                                self,
+                                channel_id,
+                                CallbackEvent.Type.FRAGMENT_PROGRESS,
+                                {
+                                    "fragments_downloaded": n_frags,
+                                    "total_size": total_size,
+                                },
+                            )
+                        )
         except asyncio.CancelledError:
             self._logger.debug("_download_stream cancelled")
         except Exception as ex:
             self._logger.error(ex)
 
-    async def _remux_stream(self, ifname, ofname, *, extra_flags=[]):
+    async def _remux_stream(self, channel_id, ifname, ofname, *, extra_flags=[]):
         mux_flags = [
             "-y",
             "-hide_banner",
             "-loglevel",
             "fatal",
             "-stats",
             "-i",
@@ -291,14 +364,15 @@
             "copy",
             "-movflags",
             "faststart",
             ofname,
         ]
         async with FFMpeg(mux_flags) as mux:
             self._logger.info("Remuxing stream", inline=True)
+            self._callback(CallbackEvent(self, channel_id, CallbackEvent.Type.MUXING))
             while await mux.print_status():
                 pass
 
     async def _download_chat(self, ws, fname):
         with open(fname, "w") as f:
             while True:
                 comment = await ws.comments.get()
@@ -379,33 +453,44 @@
                     return fname
 
         fname = get_unique_name(meta, ext)
         fpath = pathlib.Path(fname)
         fpath.parent.mkdir(parents=True, exist_ok=True)
         return fname
 
-    def _format_outtmpl(self, meta=None, overrides={}):
+    @classmethod
+    def get_format_info(cls, *, meta=None, params={}, sanitize=False):
         finfo = {
             "channel_id": "",
             "channel_name": "",
             "date": datetime.now().strftime("%F"),
             "time": datetime.now().strftime("%H%M%S"),
             "title": "",
             "ext": "",
         }
 
+        sanitizer = sanitize_filename if sanitize else lambda x: x
+
         if meta is not None:
-            finfo["channel_id"] = sanitize_filename(meta["channel_data"]["channelid"])
-            finfo["channel_name"] = sanitize_filename(meta["profile_data"]["name"])
-            finfo["title"] = sanitize_filename(meta["channel_data"]["title"])
+            finfo["channel_id"] = sanitizer(meta["channel_data"]["channelid"])
+            finfo["channel_name"] = sanitizer(meta["profile_data"]["name"])
+            finfo["title"] = sanitizer(meta["channel_data"]["title"])
 
-        for key in self.params:
+        for key in params:
             if key.startswith("_"):
-                finfo[key] = self.params[key]
+                finfo[key] = params[key]
+
+        return finfo
 
+    def _format_outtmpl(self, meta=None, overrides={}):
+        finfo = FC2LiveDL.get_format_info(
+            meta=meta,
+            params=self.params,
+            sanitize=True,
+        )
         finfo.update(overrides)
 
         formatted = self.params["outtmpl"] % finfo
         if formatted.startswith("-"):
             formatted = "_" + formatted
 
         return formatted
```

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/__init__.py` & `fc2-live-dl-2.2.0/fc2_live_dl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         "wait_for_quality_timeout": args.wait_for_quality_timeout,
         "wait_poll_interval": args.poll_interval,
         "cookies_file": args.cookies,
         "remux": not args.no_remux,
         "keep_intermediates": args.keep_intermediates,
         "extract_audio": args.extract_audio,
         "trust_env_proxy": args.trust_env_proxy,
-        # Debug params
         "dump_websocket": args.dump_websocket,
     }
 
     logger = Logger("main")
 
     channel_id = None
     try:
```

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/fc2.py` & `fc2-live-dl-2.2.0/fc2_live_dl/fc2.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/ffmpeg.py` & `fc2-live-dl-2.2.0/fc2_live_dl/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/hls.py` & `fc2-live-dl-2.2.0/fc2_live_dl/hls.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl/util.py` & `fc2-live-dl-2.2.0/fc2_live_dl/util.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.3/fc2_live_dl.egg-info/PKG-INFO` & `fc2-live-dl-2.2.0/fc2_live_dl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc2-live-dl
-Version: 2.1.3
+Version: 2.2.0
 Summary: Download live streams from FC2
 Home-page: https://github.com/HoloArchivists/fc2-live-dl
 Author: Hizkia Felix
 Author-email: felix@hizkifw.me
 Project-URL: Bug Tracker, https://github.com/HoloArchivists/fc2-live-dl/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,29 +17,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fc2-live-dl
 
 > Tool to download FC2 live streams
 
-[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ 'PyPI')
+[![PyPI](https://img.shields.io/pypi/v/fc2-live-dl)](https://pypi.org/project/fc2-live-dl/ "PyPI")
 
 ## Requirements
 
 - Python 3.8
 - ffmpeg
 
 ## Features
 
 - Wait for a stream to start and automatically start recording
 - Save comment/chat logs
 - Authenticate with cookies (Netscape format, same one used with youtube-dl)
 - Remux recordings to .mp4/.m4a after it's done
 - Continuously monitor multiple streams in parallel and automatically start
   downloading when any of them goes online
+- Get notifications when streams come online via
+  [Apprise](https://github.com/caronc/apprise)
 
 ## Installation
 
 ### Using pip
 
 To install the latest stable version:
 
@@ -167,14 +169,20 @@
     "wait_poll_interval": 5,
     "cookies_file": null,
     "remux": true,
     "keep_intermediates": false,
     "extract_audio": true,
     "trust_env_proxy": false
   },
+  "notifications": [
+    {
+      "url": "discord://{WebhookID}/{WebhookToken}",
+      "message": "%(channel_name)s is live!\nhttps://live.fc2.com/%(channel_id)s"
+    }
+  ],
   "channels": {
     "91544481": {
       "_en_name": "Necoma Karin",
       "quality": "sound",
       "write_thumbnail": true
     },
     "72364867": { "_en_name": "Uno Sakura" },
@@ -190,14 +198,27 @@
 properly. You can also override the parameters per-channel.
 
 Arbitrary parameters can be specified by prefixing them with `_`, and will be
 accessible in `outtmpl`. This is useful for specifying custom filenames just
 like in the example above. In the example I'm using `_en_name`, but you can use
 anything as long as it starts with `_`.
 
+For notifications, the URL follows the
+[Apprise syntax](https://github.com/caronc/apprise#supported-notifications). For
+example, if you want to use Discord webhooks, use the `discord://` like so:
+
+- Original URL: `https://discord.com/api/webhooks/12341234/abcdabcd`
+- Turns into: `discord://12341234/abcdabcd`
+
+You can find out more about the different types of notifiers and how to
+configure them on
+[Apprise's GitHub](https://github.com/caronc/apprise#supported-notifications).
+
+The `message` of the notifications follow the same syntax as `outtmpl`.
+
 **NOTE Windows users**: When specifying a file path (e.g. for cookies) in the
 json, double up your backslashes, for example:
 `"cookies_file": "C:\\Documents\\cookies.txt"`.
 
 Once configured, you can run the script:
 
 ```
```

### Comparing `fc2-live-dl-2.1.3/setup.cfg` & `fc2-live-dl-2.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fc2-live-dl
-version = 2.1.3
+version = 2.2.0
 author = Hizkia Felix
 author_email = felix@hizkifw.me
 description = Download live streams from FC2
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HoloArchivists/fc2-live-dl
 project_urls = 
@@ -22,14 +22,15 @@
 package_dir = 
 	= .
 python_requires = >=3.8
 packages = find:
 install_requires = 
 	aiohttp >= 3.8.1
 	aiodns >= 3.0.0
+	apprise >= 1.4.5
 
 [options.entry_points]
 console_scripts = 
 	fc2-live-dl = fc2_live_dl:main
 	autofc2 = fc2_live_dl.autofc2:main
 
 [options.packages.find]
```

