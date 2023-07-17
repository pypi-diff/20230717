# Comparing `tmp/wyoming_piper-1.0.0.tar.gz` & `tmp/wyoming_piper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_piper-1.0.0.tar", last modified: Thu Jul 13 16:27:40 2023, max compression
+gzip compressed data, was "wyoming_piper-1.1.0.tar", last modified: Mon Jul 17 16:10:40 2023, max compression
```

## Comparing `wyoming_piper-1.0.0.tar` & `wyoming_piper-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       59 2023-07-13 15:51:03.000000 wyoming_piper-1.0.0/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-10 21:09:46.000000 wyoming_piper-1.0.0/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1378 2023-07-13 15:52:43.000000 wyoming_piper-1.0.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/wyoming_piper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-1.0.0/wyoming_piper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4663 2023-07-13 16:26:55.000000 wyoming_piper-1.0.0/wyoming_piper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-1.0.0/wyoming_piper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3866 2023-07-13 14:58:56.000000 wyoming_piper-1.0.0/wyoming_piper/download.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-1.0.0/wyoming_piper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4802 2023-07-13 16:05:48.000000 wyoming_piper-1.0.0/wyoming_piper/handler.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4280 2023-07-13 15:02:06.000000 wyoming_piper-1.0.0/wyoming_piper/process.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   116115 2023-07-13 15:29:35.000000 wyoming_piper-1.0.0/wyoming_piper/voices.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/wyoming_piper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      425 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       59 2023-07-13 15:51:03.000000 wyoming_piper-1.1.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-17 15:12:29.000000 wyoming_piper-1.1.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1392 2023-07-17 15:12:32.000000 wyoming_piper-1.1.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/wyoming_piper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-1.1.0/wyoming_piper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4773 2023-07-17 16:01:40.000000 wyoming_piper-1.1.0/wyoming_piper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-1.1.0/wyoming_piper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3866 2023-07-13 14:58:56.000000 wyoming_piper-1.1.0/wyoming_piper/download.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-1.1.0/wyoming_piper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4603 2023-07-17 15:31:35.000000 wyoming_piper-1.1.0/wyoming_piper/handler.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5707 2023-07-17 15:27:00.000000 wyoming_piper-1.1.0/wyoming_piper/process.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   116115 2023-07-13 15:29:35.000000 wyoming_piper-1.1.0/wyoming_piper/voices.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/wyoming_piper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      425 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/top_level.txt
```

### Comparing `wyoming_piper-1.0.0/PKG-INFO` & `wyoming_piper-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming_piper
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

### Comparing `wyoming_piper-1.0.0/setup.py` & `wyoming_piper-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
 data_files = [module_dir / "voices.json"]
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_piper",
-    version="1.0.0",
+    version="1.1.0",
     description="Wyoming Server for Piper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
-    package_data={"wyoming_piper": [str(p.relative_to(module_dir)) for p in data_files]},
+    package_data={
+        "wyoming_piper": [str(p.relative_to(module_dir)) for p in data_files]
+    },
     install_requires=requirements,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Text Processing :: Linguistic",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

### Comparing `wyoming_piper-1.0.0/wyoming_piper/__main__.py` & `wyoming_piper-1.1.0/wyoming_piper/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,43 +37,45 @@
     )
     parser.add_argument(
         "--download-dir",
         required=True,
         help="Directory to download voices into",
     )
     #
-    parser.add_argument("--speaker", type=int, help="Id of speaker for default voice")
+    parser.add_argument(
+        "--speaker", type=str, help="Name or id of speaker for default voice"
+    )
     parser.add_argument("--noise-scale", type=float, help="Generator noise")
     parser.add_argument("--length-scale", type=float, help="Phoneme length")
     parser.add_argument("--noise-w", type=float, help="Phoneme width noise")
     #
     parser.add_argument(
         "--auto-punctuation", default=".?!", help="Automatically add punctuation"
     )
     parser.add_argument("--samples-per-chunk", type=int, default=1024)
     parser.add_argument(
         "--max-piper-procs",
         type=int,
         default=1,
-        help="Maximum number of piper process to run simultaneously",
+        help="Maximum number of piper process to run simultaneously (default: 1)",
     )
     #
     parser.add_argument("--debug", action="store_true", help="Log DEBUG messages")
     args = parser.parse_args()
 
     logging.basicConfig(level=logging.DEBUG if args.debug else logging.INFO)
 
     # Load voice info
     voices_info = get_voices()
 
     # Resolve aliases for backwards compatibility with old voice names
     aliases_info: Dict[str, Any] = {}
     for voice_info in voices_info.values():
         for voice_alias in voice_info.get("aliases", []):
-            aliases_info[voice_alias] = voice_info
+            aliases_info[voice_alias] = {"_is_alias": True, **voice_info}
 
     voices_info.update(aliases_info)
 
     wyoming_info = Info(
         tts=[
             TtsProgram(
                 name="piper",
@@ -97,24 +99,25 @@
                         #     TtsVoiceSpeaker(name=speaker_name)
                         #     for speaker_name in voice_info["speaker_id_map"]
                         # ]
                         # if voice_info.get("speaker_id_map")
                         # else None,
                     )
                     for voice_name, voice_info in voices_info.items()
+                    if not voice_info.get("_is_alias", False)
                 ],
             )
         ],
     )
 
     process_manager = PiperProcessManager(args, voices_info)
 
     # Make sure default voice is loaded.
     # Other voices will be loaded on-demand.
-    await process_manager.get_process(args.voice)
+    await process_manager.get_process()
 
     # Start server
     server = AsyncServer.from_uri(args.uri)
 
     _LOGGER.info("Ready")
     await server.run(
         partial(
```

### Comparing `wyoming_piper-1.0.0/wyoming_piper/const.py` & `wyoming_piper-1.1.0/wyoming_piper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.0.0/wyoming_piper/download.py` & `wyoming_piper-1.1.0/wyoming_piper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.0.0/wyoming_piper/file_hash.py` & `wyoming_piper-1.1.0/wyoming_piper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.0.0/wyoming_piper/handler.py` & `wyoming_piper-1.1.0/wyoming_piper/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Event handler for clients of the server."""
 import argparse
 import json
 import logging
 import math
 import os
 import wave
-from typing import Optional
+from typing import Any, Dict, Optional
 
 from wyoming.audio import AudioChunk, AudioStart, AudioStop
 from wyoming.event import Event
 from wyoming.info import Describe, Info
 from wyoming.server import AsyncEventHandler
 from wyoming.tts import Synthesize
 
@@ -40,14 +40,16 @@
             return True
 
         if not Synthesize.is_type(event.type):
             _LOGGER.warning("Unexpected event: %s", event)
             return True
 
         synthesize = Synthesize.from_event(event)
+        _LOGGER.debug(synthesize)
+
         raw_text = synthesize.text
 
         # Join multiple lines
         text = " ".join(raw_text.strip().splitlines())
 
         if self.cli_args.auto_punctuation and text:
             # Add automatic punctuation (important for some voices)
@@ -70,32 +72,25 @@
 
             piper_proc = await self.process_manager.get_process(voice_name=voice_name)
 
             assert piper_proc.proc.stdin is not None
             assert piper_proc.proc.stdout is not None
 
             # JSON in, file path out
-            input_obj = {"text": text}
+            input_obj: Dict[str, Any] = {"text": text}
             if voice_speaker is not None:
-                speaker_id_map = piper_proc.config.get("speaker_id_map", {})
-                speaker_id = speaker_id_map.get(voice_speaker)
-                if speaker_id is None:
-                    try:
-                        # Try to interpret as an id
-                        speaker_id = int(voice_speaker)
-                    except ValueError:
-                        pass
-
+                speaker_id = piper_proc.get_speaker_id(voice_speaker)
                 if speaker_id is not None:
                     input_obj["speaker_id"] = speaker_id
                 else:
                     _LOGGER.warning(
                         "No speaker '%s' for voice '%s'", voice_speaker, voice_name
                     )
 
+            _LOGGER.debug("input: %s", input_obj)
             piper_proc.proc.stdin.write(
                 (json.dumps(input_obj, ensure_ascii=False) + "\n").encode()
             )
             await piper_proc.proc.stdin.drain()
 
             output_path = (await piper_proc.proc.stdout.readline()).decode().strip()
             _LOGGER.debug(output_path)
```

### Comparing `wyoming_piper-1.0.0/wyoming_piper/voices.json` & `wyoming_piper-1.1.0/wyoming_piper/voices.json`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.0.0/wyoming_piper.egg-info/PKG-INFO` & `wyoming_piper-1.1.0/wyoming_piper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming-piper
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

