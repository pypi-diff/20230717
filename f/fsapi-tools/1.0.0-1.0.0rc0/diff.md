# Comparing `tmp/fsapi-tools-1.0.0.tar.gz` & `tmp/fsapi-tools-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsapi-tools-1.0.0.tar", last modified: Mon Jul 17 09:57:52 2023, max compression
+gzip compressed data, was "fsapi-tools-1.0.0rc0.tar", last modified: Mon Jul 17 09:52:49 2023, max compression
```

## Comparing `fsapi-tools-1.0.0.tar` & `fsapi-tools-1.0.0rc0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:52.849978 fsapi-tools-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-07-16 17:34:26.000000 fsapi-tools-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10819 2023-07-17 09:57:52.851588 fsapi-tools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10015 2023-07-17 09:57:26.000000 fsapi-tools-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:51.998496 fsapi-tools-1.0.0/fsapi/
--rw-rw-rw-   0        0        0     1308 2023-07-17 09:56:44.000000 fsapi-tools-1.0.0/fsapi/__init__.py
--rw-rw-rw-   0        0        0     1202 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:52.148788 fsapi-tools-1.0.0/fsapi/ecmascript/
--rw-rw-rw-   0        0        0     2169 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/ecmascript/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/ecmascript/__main__.py
--rw-rw-rw-   0        0        0     3180 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/ecmascript/cli.py
--rw-rw-rw-   0        0        0     4611 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/ecmascript/esbin.py
--rw-rw-rw-   0        0        0     9035 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/ecmascript/opcode.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:52.443458 fsapi-tools-1.0.0/fsapi/isu/
--rw-rw-rw-   0        0        0     2820 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/__init__.py
--rw-rw-rw-   0        0        0     1187 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/__main__.py
--rw-rw-rw-   0        0        0     9012 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/cli.py
--rw-rw-rw-   0        0        0    12597 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/format.py
--rw-rw-rw-   0        0        0     6965 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/product.py
--rw-rw-rw-   0        0        0    11934 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/update.py
--rw-rw-rw-   0        0        0     4126 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/isu/util.py
--rw-rw-rw-   0        0        0     2619 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:52.683753 fsapi-tools-1.0.0/fsapi/netremote/
--rw-rw-rw-   0        0        0     5190 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netremote/__init__.py
--rw-rw-rw-   0        0        0     9939 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netremote/basenode.py
--rw-rw-rw-   0        0        0    11710 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netremote/cli.py
--rw-rw-rw-   0        0        0   162959 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netremote/nodes.py
--rw-rw-rw-   0        0        0     8638 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0/fsapi/netremote/radiohttp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:57:52.830177 fsapi-tools-1.0.0/fsapi_tools.egg-info/
--rw-rw-rw-   0        0        0    10819 2023-07-17 09:57:51.000000 fsapi-tools-1.0.0/fsapi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-07-17 09:57:51.000000 fsapi-tools-1.0.0/fsapi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:57:51.000000 fsapi-tools-1.0.0/fsapi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-07-17 09:57:51.000000 fsapi-tools-1.0.0/fsapi_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 09:57:51.000000 fsapi-tools-1.0.0/fsapi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      970 2023-07-17 09:56:44.000000 fsapi-tools-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 09:57:52.882667 fsapi-tools-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:49.023280 fsapi-tools-1.0.0rc0/
+-rw-rw-rw-   0        0        0     1090 2023-07-16 17:34:26.000000 fsapi-tools-1.0.0rc0/LICENSE
+-rw-rw-rw-   0        0        0    10789 2023-07-17 09:52:49.032733 fsapi-tools-1.0.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     9982 2023-07-17 09:33:01.000000 fsapi-tools-1.0.0rc0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.060670 fsapi-tools-1.0.0rc0/fsapi/
+-rw-rw-rw-   0        0        0     1311 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/__init__.py
+-rw-rw-rw-   0        0        0     1202 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.208990 fsapi-tools-1.0.0rc0/fsapi/ecmascript/
+-rw-rw-rw-   0        0        0     2169 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/__main__.py
+-rw-rw-rw-   0        0        0     3180 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/cli.py
+-rw-rw-rw-   0        0        0     4611 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/esbin.py
+-rw-rw-rw-   0        0        0     9035 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/opcode.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.483648 fsapi-tools-1.0.0rc0/fsapi/isu/
+-rw-rw-rw-   0        0        0     2820 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/__init__.py
+-rw-rw-rw-   0        0        0     1187 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/__main__.py
+-rw-rw-rw-   0        0        0     9012 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/cli.py
+-rw-rw-rw-   0        0        0    12597 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/format.py
+-rw-rw-rw-   0        0        0     6965 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/product.py
+-rw-rw-rw-   0        0        0    11934 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/update.py
+-rw-rw-rw-   0        0        0     4126 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/util.py
+-rw-rw-rw-   0        0        0     2619 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.802739 fsapi-tools-1.0.0rc0/fsapi/netremote/
+-rw-rw-rw-   0        0        0     5190 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/__init__.py
+-rw-rw-rw-   0        0        0     9939 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/basenode.py
+-rw-rw-rw-   0        0        0    11710 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/cli.py
+-rw-rw-rw-   0        0        0   162959 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/nodes.py
+-rw-rw-rw-   0        0        0     8638 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/radiohttp.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.936612 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/
+-rw-rw-rw-   0        0        0    10789 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      973 2023-07-17 09:09:49.000000 fsapi-tools-1.0.0rc0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:52:49.134566 fsapi-tools-1.0.0rc0/setup.cfg
```

### Comparing `fsapi-tools-1.0.0/LICENSE` & `fsapi-tools-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/PKG-INFO` & `fsapi-tools-1.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsapi-tools
-Version: 1.0.0
+Version: 1.0.0rc0
 Summary: Frontier Smart Firmware Tools and FSAPI Implementation.
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/frontier-smart-api
 Project-URL: API-Docs, https://matrixeditor.github.io/frontier-smart-api/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
 <div align="center">
 
-![Company logo would be displayed here.](docs/graphics/company_logo.png)
+![logo](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
```

### Comparing `fsapi-tools-1.0.0/README.md` & `fsapi-tools-1.0.0rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div id="top"></div>
 <div align="center">
 
-![Company logo would be displayed here.](docs/graphics/company_logo.png)
+![logo](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
```

### Comparing `fsapi-tools-1.0.0/fsapi/__init__.py` & `fsapi-tools-1.0.0rc0/fsapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 """
 A python implementation of the FSAPI with all possible nodes. To run this
 module type:
 
 >>> python3 -m fsapi --help
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.0-rc"
 __author__ = 'MatrixEditor'
```

### Comparing `fsapi-tools-1.0.0/fsapi/__main__.py` & `fsapi-tools-1.0.0rc0/fsapi/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/ecmascript/__init__.py` & `fsapi-tools-1.0.0rc0/fsapi/ecmascript/__init__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/ecmascript/__main__.py` & `fsapi-tools-1.0.0rc0/fsapi/ecmascript/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/ecmascript/cli.py` & `fsapi-tools-1.0.0rc0/fsapi/ecmascript/cli.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/ecmascript/esbin.py` & `fsapi-tools-1.0.0rc0/fsapi/ecmascript/esbin.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/ecmascript/opcode.py` & `fsapi-tools-1.0.0rc0/fsapi/ecmascript/opcode.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/__init__.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/__init__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/__main__.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/cli.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/cli.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/format.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/format.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/product.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/product.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/update.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/update.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/isu/util.py` & `fsapi-tools-1.0.0rc0/fsapi/isu/util.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netconfig.py` & `fsapi-tools-1.0.0rc0/fsapi/netconfig.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netremote/__init__.py` & `fsapi-tools-1.0.0rc0/fsapi/netremote/__init__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netremote/basenode.py` & `fsapi-tools-1.0.0rc0/fsapi/netremote/basenode.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netremote/cli.py` & `fsapi-tools-1.0.0rc0/fsapi/netremote/cli.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netremote/nodes.py` & `fsapi-tools-1.0.0rc0/fsapi/netremote/nodes.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi/netremote/radiohttp.py` & `fsapi-tools-1.0.0rc0/fsapi/netremote/radiohttp.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/fsapi_tools.egg-info/PKG-INFO` & `fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsapi-tools
-Version: 1.0.0
+Version: 1.0.0rc0
 Summary: Frontier Smart Firmware Tools and FSAPI Implementation.
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/frontier-smart-api
 Project-URL: API-Docs, https://matrixeditor.github.io/frontier-smart-api/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
 <div align="center">
 
-![Company logo would be displayed here.](docs/graphics/company_logo.png)
+![logo](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
```

### Comparing `fsapi-tools-1.0.0/fsapi_tools.egg-info/SOURCES.txt` & `fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0/pyproject.toml` & `fsapi-tools-1.0.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2266 7361 7069 2d74 6f6f 6c73 220d  = "fsapi-tools".
 00000020: 0a76 6572 7369 6f6e 203d 2022 312e 302e  .version = "1.0.
-00000030: 3022 0d0a 6465 7363 7269 7074 696f 6e3d  0"..description=
-00000040: 2246 726f 6e74 6965 7220 536d 6172 7420  "Frontier Smart 
-00000050: 4669 726d 7761 7265 2054 6f6f 6c73 2061  Firmware Tools a
-00000060: 6e64 2046 5341 5049 2049 6d70 6c65 6d65  nd FSAPI Impleme
-00000070: 6e74 6174 696f 6e2e 220d 0a61 7574 686f  ntation."..autho
-00000080: 7273 203d 205b 0d0a 2020 7b20 6e61 6d65  rs = [..  { name
-00000090: 3d22 4d61 7472 6978 4564 6974 6f72 222c  ="MatrixEditor",
-000000a0: 2065 6d61 696c 3d22 6e6f 7440 7375 7070   email="not@supp
-000000b0: 6f72 7465 642e 636f 6d22 207d 2c0d 0a5d  orted.com" },..]
-000000c0: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-000000d0: 4d45 2e6d 6422 0d0a 636c 6173 7369 6669  ME.md"..classifi
-000000e0: 6572 7320 3d20 5b0d 0a20 2020 2027 4465  ers = [..    'De
-000000f0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000100: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-00000110: 6f6e 2f53 7461 626c 6527 2c0d 0a20 2020  on/Stable',..   
-00000120: 2027 496e 7465 6e64 6564 2041 7564 6965   'Intended Audie
-00000130: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00000140: 6573 6561 7263 6827 2c0d 0a20 2020 2027  esearch',..    '
-00000150: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000160: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000170: 6963 656e 7365 272c 0d0a 2020 2020 2750  icense',..    'P
-00000180: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000190: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001a0: 2033 2e36 272c 0d0a 2020 2020 2750 726f   3.6',..    'Pro
-000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001d0: 2e37 272c 0d0a 2020 2020 2750 726f 6772  .7',..    'Progr
-000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000200: 272c 0d0a 2020 2020 2750 726f 6772 616d  ',..    'Program
-00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000220: 2050 7974 686f 6e20 3a3a 2033 2e39 272c   Python :: 3.9',
-00000230: 0d0a 2020 2020 2750 726f 6772 616d 6d69  ..    'Programmi
-00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000250: 7974 686f 6e20 3a3a 2033 2e31 3027 2c0d  ython :: 3.10',.
-00000260: 0a20 205d 0d0a 0d0a 5b70 726f 6a65 6374  .  ]....[project
-00000270: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
-00000280: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
-00000290: 7468 7562 2e63 6f6d 2f4d 6174 7269 7845  thub.com/MatrixE
-000002a0: 6469 746f 722f 6672 6f6e 7469 6572 2d73  ditor/frontier-s
-000002b0: 6d61 7274 2d61 7069 220d 0a22 4150 492d  mart-api".."API-
-000002c0: 446f 6373 2220 3d20 2268 7474 7073 3a2f  Docs" = "https:/
-000002d0: 2f6d 6174 7269 7865 6469 746f 722e 6769  /matrixeditor.gi
-000002e0: 7468 7562 2e69 6f2f 6672 6f6e 7469 6572  thub.io/frontier
-000002f0: 2d73 6d61 7274 2d61 7069 2f22 0d0a 0d0a  -smart-api/"....
-00000300: 5b70 726f 6a65 6374 2e73 6372 6970 7473  [project.scripts
-00000310: 5d0d 0a69 7375 746f 6f6c 203d 2022 6673  ]..isutool = "fs
-00000320: 6170 692e 6973 752e 636c 693a 6d61 696e  api.isu.cli:main
-00000330: 220d 0a66 7361 7069 2d78 6472 203d 2022  "..fsapi-xdr = "
-00000340: 6673 6170 692e 6563 6d61 7363 7269 7074  fsapi.ecmascript
-00000350: 2e63 6c69 3a6d 6169 6e22 0d0a 6673 6170  .cli:main"..fsap
-00000360: 692d 6e65 7420 3d20 2266 7361 7069 2e6e  i-net = "fsapi.n
-00000370: 6574 7265 6d6f 7465 2e63 6c69 3a6d 6169  etremote.cli:mai
-00000380: 6e22 0d0a 0d0a 5b74 6f6f 6c2e 7365 7475  n"....[tool.setu
-00000390: 7074 6f6f 6c73 2e70 6163 6b61 6765 732e  ptools.packages.
-000003a0: 6669 6e64 5d0d 0a77 6865 7265 203d 205b  find]..where = [
-000003b0: 222e 225d 0d0a 696e 636c 7564 6520 3d20  "."]..include = 
-000003c0: 5b22 6673 6170 692a 225d                 ["fsapi*"]
+00000030: 302d 7263 220d 0a64 6573 6372 6970 7469  0-rc"..descripti
+00000040: 6f6e 3d22 4672 6f6e 7469 6572 2053 6d61  on="Frontier Sma
+00000050: 7274 2046 6972 6d77 6172 6520 546f 6f6c  rt Firmware Tool
+00000060: 7320 616e 6420 4653 4150 4920 496d 706c  s and FSAPI Impl
+00000070: 656d 656e 7461 7469 6f6e 2e22 0d0a 6175  ementation."..au
+00000080: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
+00000090: 616d 653d 224d 6174 7269 7845 6469 746f  ame="MatrixEdito
+000000a0: 7222 2c20 656d 6169 6c3d 226e 6f74 4073  r", email="not@s
+000000b0: 7570 706f 7274 6564 2e63 6f6d 2220 7d2c  upported.com" },
+000000c0: 0d0a 5d0d 0a72 6561 646d 6520 3d20 2252  ..]..readme = "R
+000000d0: 4541 444d 452e 6d64 220d 0a63 6c61 7373  EADME.md"..class
+000000e0: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
+000000f0: 2744 6576 656c 6f70 6d65 6e74 2053 7461  'Development Sta
+00000100: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000110: 6374 696f 6e2f 5374 6162 6c65 272c 0d0a  ction/Stable',..
+00000120: 2020 2020 2749 6e74 656e 6465 6420 4175      'Intended Au
+00000130: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+00000140: 652f 5265 7365 6172 6368 272c 0d0a 2020  e/Research',..  
+00000150: 2020 274c 6963 656e 7365 203a 3a20 4f53    'License :: OS
+00000160: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000170: 5420 4c69 6365 6e73 6527 2c0d 0a20 2020  T License',..   
+00000180: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
+00000190: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001a0: 203a 3a20 332e 3627 2c0d 0a20 2020 2027   :: 3.6',..    '
+000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001d0: 3a20 332e 3727 2c0d 0a20 2020 2027 5072  : 3.7',..    'Pr
+000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000200: 332e 3827 2c0d 0a20 2020 2027 5072 6f67  3.8',..    'Prog
+00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000230: 3927 2c0d 0a20 2020 2027 5072 6f67 7261  9',..    'Progra
+00000240: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000250: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000260: 272c 0d0a 2020 5d0d 0a0d 0a5b 7072 6f6a  ',..  ]....[proj
+00000270: 6563 742e 7572 6c73 5d0d 0a22 486f 6d65  ect.urls].."Home
+00000280: 7061 6765 2220 3d20 2268 7474 7073 3a2f  page" = "https:/
+00000290: 2f67 6974 6875 622e 636f 6d2f 4d61 7472  /github.com/Matr
+000002a0: 6978 4564 6974 6f72 2f66 726f 6e74 6965  ixEditor/frontie
+000002b0: 722d 736d 6172 742d 6170 6922 0d0a 2241  r-smart-api".."A
+000002c0: 5049 2d44 6f63 7322 203d 2022 6874 7470  PI-Docs" = "http
+000002d0: 733a 2f2f 6d61 7472 6978 6564 6974 6f72  s://matrixeditor
+000002e0: 2e67 6974 6875 622e 696f 2f66 726f 6e74  .github.io/front
+000002f0: 6965 722d 736d 6172 742d 6170 692f 220d  ier-smart-api/".
+00000300: 0a0d 0a5b 7072 6f6a 6563 742e 7363 7269  ...[project.scri
+00000310: 7074 735d 0d0a 6973 7574 6f6f 6c20 3d20  pts]..isutool = 
+00000320: 2266 7361 7069 2e69 7375 2e63 6c69 3a6d  "fsapi.isu.cli:m
+00000330: 6169 6e22 0d0a 6673 6170 692d 7864 7220  ain"..fsapi-xdr 
+00000340: 3d20 2266 7361 7069 2e65 636d 6173 6372  = "fsapi.ecmascr
+00000350: 6970 742e 636c 693a 6d61 696e 220d 0a66  ipt.cli:main"..f
+00000360: 7361 7069 2d6e 6574 203d 2022 6673 6170  sapi-net = "fsap
+00000370: 692e 6e65 7472 656d 6f74 652e 636c 693a  i.netremote.cli:
+00000380: 6d61 696e 220d 0a0d 0a5b 746f 6f6c 2e73  main"....[tool.s
+00000390: 6574 7570 746f 6f6c 732e 7061 636b 6167  etuptools.packag
+000003a0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000003b0: 3d20 5b22 2e22 5d0d 0a69 6e63 6c75 6465  = ["."]..include
+000003c0: 203d 205b 2266 7361 7069 2a22 5d          = ["fsapi*"]
```

