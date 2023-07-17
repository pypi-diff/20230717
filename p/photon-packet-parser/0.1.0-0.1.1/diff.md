# Comparing `tmp/photon-packet-parser-0.1.0.tar.gz` & `tmp/photon-packet-parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photon-packet-parser-0.1.0.tar", last modified: Mon Jul 17 12:59:53 2023, max compression
+gzip compressed data, was "photon-packet-parser-0.1.1.tar", last modified: Mon Jul 17 13:09:48 2023, max compression
```

## Comparing `photon-packet-parser-0.1.0.tar` & `photon-packet-parser-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:59:53.523639 photon-packet-parser-0.1.0/
--rw-rw-rw-   0        0        0     1073 2023-07-17 12:56:56.000000 photon-packet-parser-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4186 2023-07-17 12:59:53.522641 photon-packet-parser-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3371 2023-07-17 12:51:11.000000 photon-packet-parser-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:59:53.501641 photon-packet-parser-0.1.0/photon_packet_parser/
--rw-rw-rw-   0        0        0       74 2023-07-17 12:28:50.000000 photon-packet-parser-0.1.0/photon_packet_parser/__init__.py
--rw-rw-rw-   0        0        0      122 2023-07-12 15:42:03.000000 photon-packet-parser-0.1.0/photon_packet_parser/byte_reader.py
--rw-rw-rw-   0        0        0      137 2023-07-01 10:02:55.000000 photon-packet-parser-0.1.0/photon_packet_parser/command_type.py
--rw-rw-rw-   0        0        0      472 2023-07-12 15:42:19.000000 photon-packet-parser-0.1.0/photon_packet_parser/crc_calculator.py
--rw-rw-rw-   0        0        0      123 2023-06-30 15:09:34.000000 photon-packet-parser-0.1.0/photon_packet_parser/event_data.py
--rw-rw-rw-   0        0        0      117 2023-07-01 10:03:15.000000 photon-packet-parser-0.1.0/photon_packet_parser/message_type.py
--rw-rw-rw-   0        0        0      670 2023-07-12 15:42:31.000000 photon-packet-parser-0.1.0/photon_packet_parser/number_serializer.py
--rw-rw-rw-   0        0        0      162 2023-06-30 16:07:54.000000 photon-packet-parser-0.1.0/photon_packet_parser/operation_request.py
--rw-rw-rw-   0        0        0      273 2023-06-30 16:08:38.000000 photon-packet-parser-0.1.0/photon_packet_parser/operation_response.py
--rw-rw-rw-   0        0        0     5790 2023-07-17 12:26:37.000000 photon-packet-parser-0.1.0/photon_packet_parser/photon_packet_parser.py
--rw-rw-rw-   0        0        0    12090 2023-07-17 12:27:03.000000 photon-packet-parser-0.1.0/photon_packet_parser/protocol16_deserializer.py
--rw-rw-rw-   0        0        0      451 2023-07-12 15:45:17.000000 photon-packet-parser-0.1.0/photon_packet_parser/protocol16_type.py
--rw-rw-rw-   0        0        0      239 2023-07-01 13:14:42.000000 photon-packet-parser-0.1.0/photon_packet_parser/segmented_package.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:59:53.521637 photon-packet-parser-0.1.0/photon_packet_parser.egg-info/
--rw-rw-rw-   0        0        0     4186 2023-07-17 12:59:53.000000 photon-packet-parser-0.1.0/photon_packet_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-17 12:59:53.000000 photon-packet-parser-0.1.0/photon_packet_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:59:53.000000 photon-packet-parser-0.1.0/photon_packet_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-17 12:59:53.000000 photon-packet-parser-0.1.0/photon_packet_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:59:53.523639 photon-packet-parser-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-07-17 12:30:05.000000 photon-packet-parser-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:09:48.140637 photon-packet-parser-0.1.1/
+-rw-rw-rw-   0        0        0     1073 2023-07-17 12:56:56.000000 photon-packet-parser-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4186 2023-07-17 13:09:48.140637 photon-packet-parser-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3371 2023-07-17 12:51:11.000000 photon-packet-parser-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:09:48.132637 photon-packet-parser-0.1.1/photon_packet_parser/
+-rw-rw-rw-   0        0        0       74 2023-07-17 12:28:50.000000 photon-packet-parser-0.1.1/photon_packet_parser/__init__.py
+-rw-rw-rw-   0        0        0      122 2023-07-12 15:42:03.000000 photon-packet-parser-0.1.1/photon_packet_parser/byte_reader.py
+-rw-rw-rw-   0        0        0      137 2023-07-01 10:02:55.000000 photon-packet-parser-0.1.1/photon_packet_parser/command_type.py
+-rw-rw-rw-   0        0        0      472 2023-07-12 15:42:19.000000 photon-packet-parser-0.1.1/photon_packet_parser/crc_calculator.py
+-rw-rw-rw-   0        0        0      123 2023-06-30 15:09:34.000000 photon-packet-parser-0.1.1/photon_packet_parser/event_data.py
+-rw-rw-rw-   0        0        0      117 2023-07-01 10:03:15.000000 photon-packet-parser-0.1.1/photon_packet_parser/message_type.py
+-rw-rw-rw-   0        0        0      670 2023-07-12 15:42:31.000000 photon-packet-parser-0.1.1/photon_packet_parser/number_serializer.py
+-rw-rw-rw-   0        0        0      162 2023-06-30 16:07:54.000000 photon-packet-parser-0.1.1/photon_packet_parser/operation_request.py
+-rw-rw-rw-   0        0        0      273 2023-06-30 16:08:38.000000 photon-packet-parser-0.1.1/photon_packet_parser/operation_response.py
+-rw-rw-rw-   0        0        0     5937 2023-07-17 13:06:00.000000 photon-packet-parser-0.1.1/photon_packet_parser/photon_packet_parser.py
+-rw-rw-rw-   0        0        0    12090 2023-07-17 12:27:03.000000 photon-packet-parser-0.1.1/photon_packet_parser/protocol16_deserializer.py
+-rw-rw-rw-   0        0        0      451 2023-07-12 15:45:17.000000 photon-packet-parser-0.1.1/photon_packet_parser/protocol16_type.py
+-rw-rw-rw-   0        0        0      239 2023-07-01 13:14:42.000000 photon-packet-parser-0.1.1/photon_packet_parser/segmented_package.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:09:48.139640 photon-packet-parser-0.1.1/photon_packet_parser.egg-info/
+-rw-rw-rw-   0        0        0     4186 2023-07-17 13:09:48.000000 photon-packet-parser-0.1.1/photon_packet_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-17 13:09:48.000000 photon-packet-parser-0.1.1/photon_packet_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:09:48.000000 photon-packet-parser-0.1.1/photon_packet_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 13:09:48.000000 photon-packet-parser-0.1.1/photon_packet_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:09:48.140637 photon-packet-parser-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-07-17 13:06:37.000000 photon-packet-parser-0.1.1/setup.py
```

### Comparing `photon-packet-parser-0.1.0/LICENSE` & `photon-packet-parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `photon-packet-parser-0.1.0/PKG-INFO` & `photon-packet-parser-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photon-packet-parser
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to parse Photon Protocol packets in Python
 Author: Santiago Carullo
 Author-email: santiago.carullo@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `photon-packet-parser-0.1.0/README.md` & `photon-packet-parser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `photon-packet-parser-0.1.0/photon_packet_parser/number_serializer.py` & `photon-packet-parser-0.1.1/photon_packet_parser/number_serializer.py`

 * *Files identical despite different names*

### Comparing `photon-packet-parser-0.1.0/photon_packet_parser/photon_packet_parser.py` & `photon-packet-parser-0.1.1/photon_packet_parser/photon_packet_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
-from message_type import MessageType
-from command_type import CommandType
-from segmented_package import SegmentedPackage
-from protocol16_deserializer import Protocol16Deserializer
-from byte_reader import ByteReader
-from crc_calculator import CrcCalculator
-from number_serializer import NumberSerializer
+from photon_packet_parser.message_type import MessageType
+from photon_packet_parser.command_type import CommandType
+from photon_packet_parser.segmented_package import SegmentedPackage
+from photon_packet_parser.protocol16_deserializer import Protocol16Deserializer
+from photon_packet_parser.byte_reader import ByteReader
+from photon_packet_parser.crc_calculator import CrcCalculator
+from photon_packet_parser.number_serializer import NumberSerializer
 
 COMMAND_HEADER_LENGTH = 12
 PHOTON_HEADER_LENGTH = 12
 
 class PhotonPacketParser:
     def __init__(self, on_event, on_request, on_response):
         self._pending_segments = {}
```

### Comparing `photon-packet-parser-0.1.0/photon_packet_parser/protocol16_deserializer.py` & `photon-packet-parser-0.1.1/photon_packet_parser/protocol16_deserializer.py`

 * *Files identical despite different names*

### Comparing `photon-packet-parser-0.1.0/photon_packet_parser.egg-info/PKG-INFO` & `photon-packet-parser-0.1.1/photon_packet_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photon-packet-parser
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to parse Photon Protocol packets in Python
 Author: Santiago Carullo
 Author-email: santiago.carullo@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `photon-packet-parser-0.1.0/photon_packet_parser.egg-info/SOURCES.txt` & `photon-packet-parser-0.1.1/photon_packet_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `photon-packet-parser-0.1.0/setup.py` & `photon-packet-parser-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="photon-packet-parser",
-    version="0.1.0",
+    version="0.1.1",
     description="A package to parse Photon Protocol packets in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Santiago Carullo",
     author_email="santiago.carullo@gmail.com",
     license="MIT",
     classifiers=[
```

