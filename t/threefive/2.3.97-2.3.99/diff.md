# Comparing `tmp/threefive-2.3.97.tar.gz` & `tmp/threefive-2.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.3.97.tar", last modified: Thu Jun  8 10:08:53 2023, max compression
+gzip compressed data, was "threefive-2.3.99.tar", last modified: Mon Jul 17 06:08:54 2023, max compression
```

## Comparing `threefive-2.3.97.tar` & `threefive-2.3.99.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.97/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    13338 2023-06-08 10:08:53.534958 threefive-2.3.97/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    12767 2023-06-08 10:08:46.000000 threefive-2.3.97/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.530961 threefive-2.3.97/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.97/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-08 10:08:53.534958 threefive-2.3.97/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.97/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10691 2023-06-01 23:43:28.000000 threefive-2.3.97/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    18089 2023-06-08 10:05:54.000000 threefive-2.3.97/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-08 10:05:54.000000 threefive-2.3.97/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    13338 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-17 06:08:54.613906 threefive-2.3.99/
+-rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.99/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)    13790 2023-07-17 06:08:54.613906 threefive-2.3.99/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    13219 2023-07-17 06:04:01.000000 threefive-2.3.99/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-17 06:08:54.605905 threefive-2.3.99/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.99/bin/threefive
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-07-17 06:08:54.613906 threefive-2.3.99/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.99/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-17 06:08:54.613906 threefive-2.3.99/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/crc.py
+-rw-r--r--   0 a         (1000) a         (1000)    10691 2023-06-01 23:43:28.000000 threefive-2.3.99/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    13725 2023-07-17 06:08:43.000000 threefive-2.3.99/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)     2729 2023-06-15 07:20:38.000000 threefive-2.3.99/threefive/encode.py
+-rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    18089 2023-06-08 10:05:54.000000 threefive-2.3.99/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/stuff.py
+-rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.99/threefive/upids.py
+-rw-r--r--   0 a         (1000) a         (1000)       43 2023-07-17 06:08:43.000000 threefive-2.3.99/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-17 06:08:54.613906 threefive-2.3.99/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    13790 2023-07-17 06:08:54.000000 threefive-2.3.99/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      577 2023-07-17 06:08:54.000000 threefive-2.3.99/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-07-17 06:08:54.000000 threefive-2.3.99/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       24 2023-07-17 06:08:54.000000 threefive-2.3.99/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       10 2023-07-17 06:08:54.000000 threefive-2.3.99/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.3.97/LICENSE` & `threefive-2.3.99/LICENSE`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/PKG-INFO` & `threefive-2.3.99/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-Metadata-Version: 2.1
-Name: threefive
-Version: 2.3.97
-Summary: Pythonic SCTE35
-Home-page: https://github.com/futzu/threefive
-Author: Adrian and a Cast of Thousands.
-Author-email: spam@iodisco.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
-
-<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
-
- * __Removed__ The rogue file cmd.py.
-
-</details>
+ 🥇 threefive is the most advanced SCTE-35 decoder/encoder allowed by law.
+ ---
  
- <details><summary><b>Installation and Getting Started</b></summary>
+Latest Version is `2.3.97` 
+
+ <details><summary>Installation and Getting Started</summary>
 
 <details><summary>Requirements</summary>
 
 * threefive requires
   * [pypy3](https://pypy.org) or python 3.6+ (pypy3 runs threefive 2-3 times faster than python 3.10)
   * [new_reader](https://github.com/futzu/new_reader)
   *  __pyaes__
@@ -47,15 +28,15 @@
 '2.3.79'
 >>>
 ```
 * __Release__ versions are  __odd__.
 * __Unstable__ testing versions are __even__.
 </details>
 
- <details><summary><b>Parse SCTE-35 on the command line.</b> </summary>
+ <details><summary>Parse SCTE-35 on the command line.</summary>
  
 * `Parse base64`
 ```js
 threefive '/DAvAAAAAAAA///wFAVIAACPf+/+c2nALv4AUsz1AAAAAAAKAAhDVUVJAAABNWLbowo='
 ```
 * `Parse a hex value`
 ```js
@@ -72,15 +53,15 @@
 * `Parse multicast`
 ```lua
 threefive udp://@235.35.3.5:3535
 ```
 
 </details>
 
- <details><summary><b>Parse SCTE-35 programmatically with a few lines of code.</b></summary>
+ <details><summary>Parse SCTE-35 programmatically with a few lines of code.</summary>
 
    <details><summary>Mpegts Multicast in three lines of code.</summary>
 
 ```python3
 import threefive
 
 strm = threefive.Stream('udp://@239.35.0.35:1234')
@@ -95,14 +76,15 @@
 
 ```python3
 import threefive
 strm = threefive.Stream('https://iodisco.com/ch1/ready.ts')
 strm.decode()
 
 
+       
    </details>
 
  <details><summary>Base64 in five lines of code.</summary>
 
 ```python3
 >>> from threefive import Cue
 >>> stuff = '/DAvAAAAAAAA///wBQb+dGKQoAAZAhdDVUVJSAAAjn+fCAgAAAAALKChijUCAKnMZ1g='
@@ -454,14 +436,37 @@
                 Pid: 1054[0x41e]        Type: 0x6 PES Packets/Private Data
                 Pid: 1055[0x41f]        Type: 0x86 SCTE35 Data
 
 ```
 </details>
 
 
+<details><summary> Need to verify your splice points? </summary> 
+ 
+
+ 
+ 
+* Try [cue2vtt.py](https://github.com/futzu/scte35-threefive/blob/master/examples/stream/cue2vtt.py) in the examples.
+
+   * cue2vtt.py creates webvtt subtitles out of SCTE-35 Cue data
+ 
+* use it like this 
+
+ ```rebol
+ pypy3 cue2vtt.py video.ts | mplayer video.ts -sub -
+```
+
+
+ ![image](https://github.com/futzu/scte35-threefive/assets/52701496/5b8dbea3-1d39-48c4-8fbe-de03a53cc1dd)
+
+
+---
+
+</details> 
+
 <details><summary>Custom charsets for UPIDS aka upids.charset</summary>
 
 `Specify a charset for Upid data by setting threefive.upids.charset` [`issue #55`](https://github.com/futzu/scte35-threefive/issues/55)
 
 * default charset is ascii
 * python charsets info [Here](https://docs.python.org/3/library/codecs.html)
 * setting charset to None will return raw bytes.
@@ -488,27 +493,35 @@
 True
 >>> cue.descriptors[0].segmentation_upid
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
-### Powered by threefive
+
+
+ Powered by threefive
+---
 
   * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
- 
+  
+
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
+      * [amt-play ](https://github.com/vivoh-inc/amt-play) uses x9k3.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
+  
+  * [bpkio-cli](https://pypi.org/project/bpkio-cli/): A command line interface to the broadpeak.io APIs. 
 
-### other threefive stuff
+ threefive | more
+---
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
   * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.97/README.md` & `threefive-2.3.99/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,29 @@
-![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
+Metadata-Version: 2.1
+Name: threefive
+Version: 2.3.99
+Summary: Pythonic SCTE35
+Home-page: https://github.com/futzu/threefive
+Author: Adrian and a Cast of Thousands.
+Author-email: spam@iodisco.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
-
- * __Removed__ The rogue file cmd.py.
-
-</details>
+ 🥇 threefive is the most advanced SCTE-35 decoder/encoder allowed by law.
+ ---
  
- <details><summary><b>Installation and Getting Started</b></summary>
+Latest Version is `2.3.97` 
+
+ <details><summary>Installation and Getting Started</summary>
 
 <details><summary>Requirements</summary>
 
 * threefive requires
   * [pypy3](https://pypy.org) or python 3.6+ (pypy3 runs threefive 2-3 times faster than python 3.10)
   * [new_reader](https://github.com/futzu/new_reader)
   *  __pyaes__
@@ -31,15 +44,15 @@
 '2.3.79'
 >>>
 ```
 * __Release__ versions are  __odd__.
 * __Unstable__ testing versions are __even__.
 </details>
 
- <details><summary><b>Parse SCTE-35 on the command line.</b> </summary>
+ <details><summary>Parse SCTE-35 on the command line.</summary>
  
 * `Parse base64`
 ```js
 threefive '/DAvAAAAAAAA///wFAVIAACPf+/+c2nALv4AUsz1AAAAAAAKAAhDVUVJAAABNWLbowo='
 ```
 * `Parse a hex value`
 ```js
@@ -56,15 +69,15 @@
 * `Parse multicast`
 ```lua
 threefive udp://@235.35.3.5:3535
 ```
 
 </details>
 
- <details><summary><b>Parse SCTE-35 programmatically with a few lines of code.</b></summary>
+ <details><summary>Parse SCTE-35 programmatically with a few lines of code.</summary>
 
    <details><summary>Mpegts Multicast in three lines of code.</summary>
 
 ```python3
 import threefive
 
 strm = threefive.Stream('udp://@239.35.0.35:1234')
@@ -79,14 +92,15 @@
 
 ```python3
 import threefive
 strm = threefive.Stream('https://iodisco.com/ch1/ready.ts')
 strm.decode()
 
 
+       
    </details>
 
  <details><summary>Base64 in five lines of code.</summary>
 
 ```python3
 >>> from threefive import Cue
 >>> stuff = '/DAvAAAAAAAA///wBQb+dGKQoAAZAhdDVUVJSAAAjn+fCAgAAAAALKChijUCAKnMZ1g='
@@ -438,14 +452,37 @@
                 Pid: 1054[0x41e]        Type: 0x6 PES Packets/Private Data
                 Pid: 1055[0x41f]        Type: 0x86 SCTE35 Data
 
 ```
 </details>
 
 
+<details><summary> Need to verify your splice points? </summary> 
+ 
+
+ 
+ 
+* Try [cue2vtt.py](https://github.com/futzu/scte35-threefive/blob/master/examples/stream/cue2vtt.py) in the examples.
+
+   * cue2vtt.py creates webvtt subtitles out of SCTE-35 Cue data
+ 
+* use it like this 
+
+ ```rebol
+ pypy3 cue2vtt.py video.ts | mplayer video.ts -sub -
+```
+
+
+ ![image](https://github.com/futzu/scte35-threefive/assets/52701496/5b8dbea3-1d39-48c4-8fbe-de03a53cc1dd)
+
+
+---
+
+</details> 
+
 <details><summary>Custom charsets for UPIDS aka upids.charset</summary>
 
 `Specify a charset for Upid data by setting threefive.upids.charset` [`issue #55`](https://github.com/futzu/scte35-threefive/issues/55)
 
 * default charset is ascii
 * python charsets info [Here](https://docs.python.org/3/library/codecs.html)
 * setting charset to None will return raw bytes.
@@ -472,27 +509,35 @@
 True
 >>> cue.descriptors[0].segmentation_upid
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
-### Powered by threefive
+
+
+ Powered by threefive
+---
 
   * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
- 
+  
+
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
+      * [amt-play ](https://github.com/vivoh-inc/amt-play) uses x9k3.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
+  
+  * [bpkio-cli](https://pypi.org/project/bpkio-cli/): A command line interface to the broadpeak.io APIs. 
 
-### other threefive stuff
+ threefive | more
+---
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
   * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.97/bin/threefive` & `threefive-2.3.99/bin/threefive`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/setup.py` & `threefive-2.3.99/setup.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/__init__.py` & `threefive-2.3.99/threefive/__init__.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/base.py` & `threefive-2.3.99/threefive/base.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/bitn.py` & `threefive-2.3.99/threefive/bitn.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/commands.py` & `threefive-2.3.99/threefive/commands.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/crc.py` & `threefive-2.3.99/threefive/crc.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/cue.py` & `threefive-2.3.99/threefive/cue.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/decode.py` & `threefive-2.3.99/threefive/decode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/descriptors.py` & `threefive-2.3.99/threefive/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,22 +399,21 @@
 # map of known descriptors and associated classes
 descriptor_map = {
     0: AvailDescriptor,
     1: DtmfDescriptor,
     2: SegmentationDescriptor,
     3: TimeDescriptor,
     4: AudioDescriptor,
+    
 }
 
 
 def splice_descriptor(bites):
     """
-    splice_descriptor reads the
-    descriptor tag and decodes and
-    returns an instance self._descriptor_map[tag]
+    replaced splice_descriptor
     """
     tag = bites[0]
     if tag not in descriptor_map:
-        return False
+        return SpliceDescriptor(bites)
     spliced = descriptor_map[tag](bites)
     spliced.decode()
     return spliced
```

### Comparing `threefive-2.3.97/threefive/encode.py` & `threefive-2.3.99/threefive/encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     cue.command = ts
     cue.encode()
     return cue
 
 
 def mk_splice_insert(event_id, pts=None, duration=None, out=False):
     """
-    mk_cue returns a Cue with a Splice Insert.
+    mk_splice_insert returns a Cue with a Splice Insert.
 
     The args set the SpliceInsert vars.
 
     splice_event_id = event_id
 
     if pts is None (default):
         splice_immediate_flag      True
```

### Comparing `threefive-2.3.97/threefive/packetdata.py` & `threefive-2.3.99/threefive/packetdata.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/section.py` & `threefive-2.3.99/threefive/section.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/segment.py` & `threefive-2.3.99/threefive/segment.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/segmentation.py` & `threefive-2.3.99/threefive/segmentation.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/smoketest.py` & `threefive-2.3.99/threefive/smoketest.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/stream.py` & `threefive-2.3.99/threefive/stream.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive/upids.py` & `threefive-2.3.99/threefive/upids.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.97/threefive.egg-info/PKG-INFO` & `threefive-2.3.99/threefive.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.97
+Version: 2.3.99
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
-
-<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
-
- * __Removed__ The rogue file cmd.py.
-
-</details>
+ 🥇 threefive is the most advanced SCTE-35 decoder/encoder allowed by law.
+ ---
  
- <details><summary><b>Installation and Getting Started</b></summary>
+Latest Version is `2.3.97` 
+
+ <details><summary>Installation and Getting Started</summary>
 
 <details><summary>Requirements</summary>
 
 * threefive requires
   * [pypy3](https://pypy.org) or python 3.6+ (pypy3 runs threefive 2-3 times faster than python 3.10)
   * [new_reader](https://github.com/futzu/new_reader)
   *  __pyaes__
@@ -47,15 +44,15 @@
 '2.3.79'
 >>>
 ```
 * __Release__ versions are  __odd__.
 * __Unstable__ testing versions are __even__.
 </details>
 
- <details><summary><b>Parse SCTE-35 on the command line.</b> </summary>
+ <details><summary>Parse SCTE-35 on the command line.</summary>
  
 * `Parse base64`
 ```js
 threefive '/DAvAAAAAAAA///wFAVIAACPf+/+c2nALv4AUsz1AAAAAAAKAAhDVUVJAAABNWLbowo='
 ```
 * `Parse a hex value`
 ```js
@@ -72,15 +69,15 @@
 * `Parse multicast`
 ```lua
 threefive udp://@235.35.3.5:3535
 ```
 
 </details>
 
- <details><summary><b>Parse SCTE-35 programmatically with a few lines of code.</b></summary>
+ <details><summary>Parse SCTE-35 programmatically with a few lines of code.</summary>
 
    <details><summary>Mpegts Multicast in three lines of code.</summary>
 
 ```python3
 import threefive
 
 strm = threefive.Stream('udp://@239.35.0.35:1234')
@@ -95,14 +92,15 @@
 
 ```python3
 import threefive
 strm = threefive.Stream('https://iodisco.com/ch1/ready.ts')
 strm.decode()
 
 
+       
    </details>
 
  <details><summary>Base64 in five lines of code.</summary>
 
 ```python3
 >>> from threefive import Cue
 >>> stuff = '/DAvAAAAAAAA///wBQb+dGKQoAAZAhdDVUVJSAAAjn+fCAgAAAAALKChijUCAKnMZ1g='
@@ -454,14 +452,37 @@
                 Pid: 1054[0x41e]        Type: 0x6 PES Packets/Private Data
                 Pid: 1055[0x41f]        Type: 0x86 SCTE35 Data
 
 ```
 </details>
 
 
+<details><summary> Need to verify your splice points? </summary> 
+ 
+
+ 
+ 
+* Try [cue2vtt.py](https://github.com/futzu/scte35-threefive/blob/master/examples/stream/cue2vtt.py) in the examples.
+
+   * cue2vtt.py creates webvtt subtitles out of SCTE-35 Cue data
+ 
+* use it like this 
+
+ ```rebol
+ pypy3 cue2vtt.py video.ts | mplayer video.ts -sub -
+```
+
+
+ ![image](https://github.com/futzu/scte35-threefive/assets/52701496/5b8dbea3-1d39-48c4-8fbe-de03a53cc1dd)
+
+
+---
+
+</details> 
+
 <details><summary>Custom charsets for UPIDS aka upids.charset</summary>
 
 `Specify a charset for Upid data by setting threefive.upids.charset` [`issue #55`](https://github.com/futzu/scte35-threefive/issues/55)
 
 * default charset is ascii
 * python charsets info [Here](https://docs.python.org/3/library/codecs.html)
 * setting charset to None will return raw bytes.
@@ -488,27 +509,35 @@
 True
 >>> cue.descriptors[0].segmentation_upid
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
-### Powered by threefive
+
+
+ Powered by threefive
+---
 
   * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
- 
+  
+
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
+      * [amt-play ](https://github.com/vivoh-inc/amt-play) uses x9k3.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
+  
+  * [bpkio-cli](https://pypi.org/project/bpkio-cli/): A command line interface to the broadpeak.io APIs. 
 
-### other threefive stuff
+ threefive | more
+---
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
   * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.97/threefive.egg-info/SOURCES.txt` & `threefive-2.3.99/threefive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

