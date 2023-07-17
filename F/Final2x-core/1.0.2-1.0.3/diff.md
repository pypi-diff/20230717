# Comparing `tmp/Final2x-core-1.0.2.tar.gz` & `tmp/Final2x-core-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Final2x-core-1.0.2.tar", last modified: Wed Jul 12 20:10:52 2023, max compression
+gzip compressed data, was "Final2x-core-1.0.3.tar", last modified: Mon Jul 17 02:23:42 2023, max compression
```

## Comparing `Final2x-core-1.0.2.tar` & `Final2x-core-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/Final2x_core/Final2x-core-pip.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/SRFactory/
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALCUGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALESRGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRBaseClass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRMD.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/WAIFU2X.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRFactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/SRncnn/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/SRMDncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/SRqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/getConfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/progressLog.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-12 20:10:51.000000 Final2x-core-1.0.2/Final2x_core/src/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/Final2x_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-12 20:10:52.000000 Final2x-core-1.0.2/Final2x_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-07-12 20:10:28.000000 Final2x-core-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 20:10:52.484762 Final2x-core-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-12 20:10:29.000000 Final2x-core-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/Final2x_core/Final2x-core-pip.md
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/SRFactory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALCUGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALESRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRMD.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/WAIFU2X.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/SRncnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALCUGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALESRGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/SRMDncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/getConfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/progressLog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-17 02:23:23.000000 Final2x-core-1.0.3/setup.py
```

### Comparing `Final2x-core-1.0.2/Final2x_core/__main__.py` & `Final2x-core-1.0.3/Final2x_core/__main__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/config.yaml` & `Final2x-core-1.0.3/Final2x_core/config.yaml`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALCUGAN.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALCUGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/REALESRGAN.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALESRGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRBaseClass.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRBaseClass.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRFactory.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRFactory.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/SRMD.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRMD.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/WAIFU2X.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/WAIFU2X.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRFactory/__init__.py` & `Final2x-core-1.0.3/Final2x_core/src/SRFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALCUGANncnn.py` & `Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALCUGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRncnn/REALESRGANncnn.py` & `Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALESRGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRncnn/SRMDncnn.py` & `Final2x-core-1.0.3/Final2x_core/src/SRncnn/SRMDncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRncnn/WAIFU2Xncnn.py` & `Final2x-core-1.0.3/Final2x_core/src/SRncnn/WAIFU2Xncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/SRqueue.py` & `Final2x-core-1.0.3/Final2x_core/src/SRqueue.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/utils/getConfig.py` & `Final2x-core-1.0.3/Final2x_core/src/utils/getConfig.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core/src/utils/progressLog.py` & `Final2x-core-1.0.3/Final2x_core/src/utils/progressLog.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/Final2x_core.egg-info/PKG-INFO` & `Final2x-core-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,453 +1,475 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 4669 6e61  : 2.1.Name: Fina
-00000020: 6c32 782d 636f 7265 0a56 6572 7369 6f6e  l2x-core.Version
-00000030: 3a20 312e 302e 320a 5375 6d6d 6172 793a  : 1.0.2.Summary:
-00000040: 2055 4e4b 4e4f 574e 0a48 6f6d 652d 7061   UNKNOWN.Home-pa
-00000050: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000060: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
-00000070: 4669 6e61 6c32 782d 636f 7265 0a41 7574  Final2x-core.Aut
-00000080: 686f 723a 2054 6f68 7275 736b 790a 4c69  hor: Tohrusky.Li
-00000090: 6365 6e73 653a 2055 4e4b 4e4f 574e 0a50  cense: UNKNOWN.P
-000000a0: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
-000000b0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-000000c0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-000000d0: 3a3a 2033 202d 2041 6c70 6861 0a43 6c61  :: 3 - Alpha.Cla
-000000e0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000000f0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000100: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-00000110: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000120: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000130: 4253 4420 4c69 6365 6e73 650a 436c 6173  BSD License.Clas
-00000140: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000160: 5079 7468 6f6e 203a 3a20 332e 360a 436c  Python :: 3.6.Cl
-00000170: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000180: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000190: 3a20 5079 7468 6f6e 203a 3a20 332e 370a  : Python :: 3.7.
-000001a0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000001b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001d0: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
-000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000200: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
-00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000230: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-00000240: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000260: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
-00000270: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
-00000280: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000290: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000002a0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-000002b0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-000002c0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000002d0: 223e 0a0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
-000002e0: 7470 733a 2f2f 7332 2e6c 6f6c 692e 6e65  tps://s2.loli.ne
-000002f0: 742f 3230 3233 2f30 362f 3139 2f35 3437  t/2023/06/19/547
-00000300: 7152 6563 4864 6e4a 4962 4b75 2e70 6e67  qRecHdnJIbKu.png
-00000310: 2220 6865 6967 6874 3d22 3132 3822 3e0a  " height="128">.
-00000320: 0a3c 2f70 3e0a 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
-00000330: 3d22 6365 6e74 6572 223e 2046 696e 616c  ="center"> Final
-00000340: 3278 2d63 6f72 6520 3c2f 6831 3e0a 0a21  2x-core </h1>..!
-00000350: 5b4d 6163 4f53 2078 3634 5d28 6874 7470  [MacOS x64](http
-00000360: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000370: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
-00000380: 2d4d 6163 4f53 2532 3078 3634 2d62 6c75  -MacOS%20x64-blu
-00000390: 653f 6c6f 676f 3d41 7070 6c65 2673 7479  e?logo=Apple&sty
-000003a0: 6c65 3d66 6c61 742d 7371 7561 7265 290a  le=flat-square).
-000003b0: 215b 4d61 634f 5320 6172 6d36 345d 2868  ![MacOS arm64](h
-000003c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000003d0: 6473 2e69 6f2f 6261 6467 652f 5375 7070  ds.io/badge/Supp
-000003e0: 6f72 742d 4d61 634f 5325 3230 6172 6d36  ort-MacOS%20arm6
-000003f0: 342d 626c 7565 3f6c 6f67 6f3d 4170 706c  4-blue?logo=Appl
-00000400: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-00000410: 6172 6529 0a21 5b57 696e 646f 7773 2078  are).![Windows x
-00000420: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000430: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000440: 2f53 7570 706f 7274 2d57 696e 646f 7773  /Support-Windows
-00000450: 2532 3078 3634 2d62 6c75 653f 6c6f 676f  %20x64-blue?logo
-00000460: 3d57 696e 646f 7773 2673 7479 6c65 3d66  =Windows&style=f
-00000470: 6c61 742d 7371 7561 7265 290a 215b 5769  lat-square).![Wi
-00000480: 6e64 6f77 7320 6172 6d36 345d 2868 7474  ndows arm64](htt
-00000490: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000004a0: 2e69 6f2f 6261 6467 652f 5375 7070 6f72  .io/badge/Suppor
-000004b0: 742d 5769 6e64 6f77 7325 3230 6172 6d36  t-Windows%20arm6
-000004c0: 342d 626c 7565 3f6c 6f67 6f3d 5769 6e64  4-blue?logo=Wind
-000004d0: 6f77 7326 7374 796c 653d 666c 6174 2d73  ows&style=flat-s
-000004e0: 7175 6172 6529 0a21 5b4c 696e 7578 2078  quare).![Linux x
-000004f0: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000500: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000510: 2f53 7570 706f 7274 2d4c 696e 7578 2532  /Support-Linux%2
-00000520: 3078 3634 2d62 6c75 653f 6c6f 676f 3d4c  0x64-blue?logo=L
-00000530: 696e 7578 2673 7479 6c65 3d66 6c61 742d  inux&style=flat-
-00000540: 7371 7561 7265 290a 5b21 5b63 6f64 6563  square).[![codec
-00000550: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
-00000560: 636f 762e 696f 2f67 682f 546f 6872 7573  cov.io/gh/Tohrus
-00000570: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-00000580: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
-00000590: 682f 6261 6467 652e 7376 673f 746f 6b65  h/badge.svg?toke
-000005a0: 6e3d 4232 544e 4b59 4e34 4f34 295d 2868  n=B2TNKYN4O4)](h
-000005b0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000005c0: 6f2f 6768 2f54 6f68 7275 736b 792f 4669  o/gh/Tohrusky/Fi
-000005d0: 6e61 6c32 782d 636f 7265 290a 5b21 5b43  nal2x-core).[![C
-000005e0: 492d 7465 7374 5d28 6874 7470 733a 2f2f  I-test](https://
-000005f0: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-00000600: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-00000610: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000620: 7773 2f43 492d 7465 7374 2e79 6d6c 2f62  ws/CI-test.yml/b
-00000630: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00000640: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00000650: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
-00000660: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
-00000670: 666c 6f77 732f 4349 2d74 6573 742e 796d  flows/CI-test.ym
-00000680: 6c29 0a5b 215b 4349 2d62 7569 6c64 5d28  l).[![CI-build](
-00000690: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006a0: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
-000006b0: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
-000006c0: 2f77 6f72 6b66 6c6f 7773 2f43 492d 6275  /workflows/CI-bu
-000006d0: 696c 642e 796d 6c2f 6261 6467 652e 7376  ild.yml/badge.sv
-000006e0: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-000006f0: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
-00000700: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
-00000710: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f43  ions/workflows/C
-00000720: 492d 6275 696c 642e 796d 6c29 0a5b 215b  I-build.yml).[![
-00000730: 5265 6c65 6173 655d 2868 7474 7073 3a2f  Release](https:/
-00000740: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
-00000750: 7573 6b79 2f46 696e 616c 3278 2d63 6f72  usky/Final2x-cor
-00000760: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-00000770: 6f77 732f 5265 6c65 6173 652e 796d 6c2f  ows/Release.yml/
-00000780: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00000790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000007a0: 6f68 7275 736b 792f 4669 6e61 6c32 782d  ohrusky/Final2x-
-000007b0: 636f 7265 2f61 6374 696f 6e73 2f77 6f72  core/actions/wor
-000007c0: 6b66 6c6f 7773 2f52 656c 6561 7365 2e79  kflows/Release.y
-000007d0: 6d6c 290a 5b21 5b50 4950 2d74 6573 745d  ml).[![PIP-test]
-000007e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007f0: 636f 6d2f 546f 6872 7573 6b79 2f46 696e  com/Tohrusky/Fin
-00000800: 616c 3278 2d63 6f72 652f 6163 7469 6f6e  al2x-core/action
-00000810: 732f 776f 726b 666c 6f77 732f 5049 502d  s/workflows/PIP-
-00000820: 7465 7374 2e79 6d6c 2f62 6164 6765 2e73  test.yml/badge.s
-00000830: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000840: 6875 622e 636f 6d2f 546f 6872 7573 6b79  hub.com/Tohrusky
-00000850: 2f46 696e 616c 3278 2d63 6f72 652f 6163  /Final2x-core/ac
-00000860: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000870: 5049 502d 7465 7374 2e79 6d6c 290a 5b21  PIP-test.yml).[!
-00000880: 5b52 656c 6561 7365 2d70 7970 695d 2868  [Release-pypi](h
-00000890: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000008a0: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-000008b0: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
-000008c0: 776f 726b 666c 6f77 732f 5265 6c65 6173  workflows/Releas
-000008d0: 652d 7079 7069 2e79 6d6c 2f62 6164 6765  e-pypi.yml/badge
-000008e0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-000008f0: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
-00000900: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-00000910: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000920: 732f 5265 6c65 6173 652d 7079 7069 2e79  s/Release-pypi.y
-00000930: 6d6c 290a 5b21 5b50 7950 4920 7665 7273  ml).[![PyPI vers
-00000940: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
-00000950: 6765 2e66 7572 792e 696f 2f70 792f 4669  ge.fury.io/py/Fi
-00000960: 6e61 6c32 782d 636f 7265 2e73 7667 295d  nal2x-core.svg)]
-00000970: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000980: 7572 792e 696f 2f70 792f 4669 6e61 6c32  ury.io/py/Final2
-00000990: 782d 636f 7265 290a 215b 4769 7448 7562  x-core).![GitHub
-000009a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000009b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000009c0: 6c69 6365 6e73 652f 546f 6872 7573 6b79  license/Tohrusky
-000009d0: 2f46 696e 616c 3278 2d63 6f72 6529 0a0a  /Final2x-core)..
-000009e0: 4669 6e61 6c32 782d 636f 7265 2069 7320  Final2x-core is 
-000009f0: 6120 6372 6f73 732d 706c 6174 666f 726d  a cross-platform
-00000a00: 2069 6d61 6765 2073 7570 6572 2d72 6573   image super-res
-00000a10: 6f6c 7574 696f 6e20 434c 4920 746f 6f6c  olution CLI tool
-00000a20: 2066 6f72 205b 4669 6e61 6c32 785d 2868   for [Final2x](h
-00000a30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a40: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-00000a50: 3278 292e 2049 6620 796f 7520 6861 7665  2x). If you have
-00000a60: 2061 6e79 2071 7565 7374 696f 6e73 2c20   any questions, 
-00000a70: 706c 6561 7365 2072 6169 7365 2061 6e20  please raise an 
-00000a80: 6973 7375 6520 5b69 6e20 7468 6973 2072  issue [in this r
-00000a90: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-00000aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00000ab0: 6872 7573 6b79 2f46 696e 616c 3278 292e  hrusky/Final2x).
-00000ac0: 0a0a 2320 496e 7374 616c 6c0a 0a44 6f77  ..# Install..Dow
-00000ad0: 6e6c 6f61 6420 696e 205b 5265 6c65 6173  nload in [Releas
-00000ae0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000af0: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
-00000b00: 696e 616c 3278 2d63 6f72 652f 7265 6c65  inal2x-core/rele
-00000b10: 6173 6573 2920 6f72 2075 7365 2070 6970  ases) or use pip
-00000b20: 2028 7079 7468 6f6e 203e 3d20 332e 362c   (python >= 3.6,
-00000b30: 203e 3d33 2e39 2066 6f72 204d 6163 4f53   >=3.9 for MacOS
-00000b40: 0a61 726d 3634 290a 0a60 6060 7368 656c  .arm64)..```shel
-00000b50: 6c0a 7069 7020 696e 7374 616c 6c20 4669  l.pip install Fi
-00000b60: 6e61 6c32 782d 636f 7265 0a60 6060 0a0a  nal2x-core.```..
-00000b70: 2320 5573 650a 0a60 6060 7368 656c 6c0a  # Use..```shell.
-00000b80: 7573 6167 653a 2046 696e 616c 3278 2d63  usage: Final2x-c
-00000b90: 6f72 6520 5b2d 685d 205b 2d62 2042 4153  ore [-h] [-b BAS
-00000ba0: 4536 345d 205b 2d6a 204a 534f 4e5d 205b  E64] [-j JSON] [
-00000bb0: 2d79 2059 414d 4c5d 205b 2d6f 5d0a 0a77  -y YAML] [-o]..w
-00000bc0: 6865 6e20 7061 7261 2069 7320 6e6f 7420  hen para is not 
-00000bd0: 7370 6563 6966 6965 642c 2074 6865 2063  specified, the c
-00000be0: 6f6e 6669 672e 7961 6d6c 2066 696c 6520  onfig.yaml file 
-00000bf0: 696e 2074 6865 2064 6972 6563 746f 7279  in the directory
-00000c00: 2077 696c 6c20 6265 2072 6561 6420 6175   will be read au
-00000c10: 746f 6d61 7469 6361 6c6c 790a 0a6f 7074  tomatically..opt
-00000c20: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
-00000c30: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
-00000c40: 2020 2020 2020 2020 2073 686f 7720 7468           show th
-00000c50: 6973 2068 656c 7020 6d65 7373 6167 6520  is help message 
-00000c60: 616e 6420 6578 6974 0a20 202d 6220 4241  and exit.  -b BA
-00000c70: 5345 3634 2c20 2d2d 4241 5345 3634 2042  SE64, --BASE64 B
-00000c80: 4153 4536 340a 2020 2020 2020 2020 2020  ASE64.          
-00000c90: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00000ca0: 7365 3634 2073 7472 696e 6720 666f 7220  se64 string for 
-00000cb0: 636f 6e66 6967 206a 736f 6e0a 2020 2d6a  config json.  -j
-00000cc0: 204a 534f 4e2c 202d 2d4a 534f 4e20 4a53   JSON, --JSON JS
-00000cd0: 4f4e 2020 4a53 4f4e 2073 7472 696e 6720  ON  JSON string 
-00000ce0: 666f 7220 636f 6e66 6967 0a20 202d 7920  for config.  -y 
-00000cf0: 5941 4d4c 2c20 2d2d 5941 4d4c 2059 414d  YAML, --YAML YAM
-00000d00: 4c20 2079 616d 6c20 636f 6e66 6967 2066  L  yaml config f
-00000d10: 696c 6520 7061 7468 0a20 202d 6c2c 202d  ile path.  -l, -
-00000d20: 2d4c 4f47 2020 2020 2020 2020 2020 2020  -LOG            
-00000d30: 2073 6176 6520 6c6f 670a 2020 2d6f 2c20   save log.  -o, 
-00000d40: 2d2d 4f50 2020 2020 2020 2020 2020 2020  --OP            
-00000d50: 2020 6368 6563 6b20 696e 7374 616c 6c0a    check install.
-00000d60: 6060 600a 0a23 2043 6f6e 6669 670a 0a50  ```..# Config..P
-00000d70: 6173 7320 7468 6520 636f 6e66 6967 206a  ass the config j
-00000d80: 736f 6e20 7374 7269 6e67 2074 6f20 7468  son string to th
-00000d90: 6520 7072 6f67 7261 6d20 7468 726f 7567  e program throug
-00000da0: 6820 7468 6520 602d 6a60 2070 6172 616d  h the `-j` param
-00000db0: 6574 6572 2e0a 0a2a 2a50 4c45 4153 4520  eter...**PLEASE 
-00000dc0: 4e4f 5445 3a20 7468 6520 636f 6e66 6967  NOTE: the config
-00000dd0: 2069 7320 4a53 4f4e 2c20 7265 6d6f 7665   is JSON, remove
-00000de0: 2074 6865 202f 2f20 636f 6d6d 656e 7473   the // comments
-00000df0: 2062 6566 6f72 6520 7573 652e 2a2a 0a0a   before use.**..
-00000e00: 6060 606a 736f 6e0a 7b0a 2020 2267 7075  ```json.{.  "gpu
-00000e10: 6964 223a 2030 2c0a 2020 2f2f 2047 5055  id": 0,.  // GPU
-00000e20: 2069 642c 203e 3d20 2d31 2028 2d31 2066   id, >= -1 (-1 f
-00000e30: 6f72 2043 5055 2c20 6d61 7920 6e6f 7420  or CPU, may not 
-00000e40: 776f 726b 2066 6f72 2073 6f6d 6520 6d6f  work for some mo
-00000e50: 6465 6c73 2e29 0a20 2022 696e 7075 7470  dels.).  "inputp
-00000e60: 6174 6822 3a20 5b0a 2020 2020 2f2f 2049  ath": [.    // I
-00000e70: 6e70 7574 2069 6d61 6765 2070 6174 6873  nput image paths
-00000e80: 2c20 7368 6f75 6c64 2062 6520 6120 6c69  , should be a li
-00000e90: 7374 2e0a 2020 2020 2270 6174 682f 746f  st..    "path/to
-00000ea0: 2f69 6d67 312e 6a70 6722 2c0a 2020 2020  /img1.jpg",.    
-00000eb0: 2270 6174 682f 746f 2f69 6d67 322e 706e  "path/to/img2.pn
-00000ec0: 6722 0a20 205d 2c0a 2020 226d 6f64 656c  g".  ],.  "model
-00000ed0: 223a 2022 5265 616c 4355 4741 4e2d 7072  ": "RealCUGAN-pr
-00000ee0: 6f22 2c0a 2020 2f2f 206d 6f64 656c 206e  o",.  // model n
-00000ef0: 616d 650a 2020 226d 6f64 656c 7363 616c  ame.  "modelscal
-00000f00: 6522 3a20 322c 0a20 202f 2f20 6d6f 6465  e": 2,.  // mode
-00000f10: 6c20 7570 7363 616c 6520 6661 6374 6f72  l upscale factor
-00000f20: 0a20 2022 6d6f 6465 6c6e 6f69 7365 223a  .  "modelnoise":
-00000f30: 202d 312c 0a20 202f 2f20 4445 4e4f 4953   -1,.  // DENOIS
-00000f40: 4520 6c65 7665 6c0a 2020 226f 7574 7075  E level.  "outpu
-00000f50: 7470 6174 6822 3a20 2270 6174 682f 746f  tpath": "path/to
-00000f60: 2f6f 7574 7075 7422 2c0a 2020 2f2f 206f  /output",.  // o
-00000f70: 7574 7075 7420 7061 7468 0a20 2022 7461  utput path.  "ta
-00000f80: 7267 6574 7363 616c 6522 3a20 322e 302c  rgetscale": 2.0,
-00000f90: 0a20 202f 2f20 5461 7267 6574 2075 7073  .  // Target ups
-00000fa0: 6361 6c65 2066 6163 746f 722c 2075 7073  cale factor, ups
-00000fb0: 6361 6c65 206d 756c 7469 706c 6520 7469  cale multiple ti
-00000fc0: 6d65 7320 746f 2061 6368 6965 7665 2074  mes to achieve t
-00000fd0: 6865 2074 6172 6765 7420 7570 7363 616c  he target upscal
-00000fe0: 6520 6661 6374 6f72 2e0a 2020 2f2f 2049  e factor..  // I
-00000ff0: 6620 6e6f 7420 696e 7661 6c69 642c 2075  f not invalid, u
-00001000: 7365 206d 6f64 656c 7363 616c 652e 0a20  se modelscale.. 
-00001010: 2022 7474 6122 3a20 6661 6c73 650a 2020   "tta": false.  
-00001020: 2f2f 2054 6573 7420 5469 6d65 2041 7567  // Test Time Aug
-00001030: 6d65 6e74 6174 696f 6e2c 2064 6566 6175  mentation, defau
-00001040: 6c74 2066 616c 7365 0a7d 0a60 6060 0a0a  lt false.}.```..
-00001050: 2a2a 5355 5050 4f52 5445 4420 4d4f 4445  **SUPPORTED MODE
-00001060: 4c20 4c49 5354 3a2a 2a0a 0a60 6060 7961  L LIST:**..```ya
-00001070: 6d6c 0a2d 2052 6561 6c43 5547 414e 2d73  ml.- RealCUGAN-s
-00001080: 653a 0a20 2020 202d 206d 6f64 656c 3a20  e:.    - model: 
-00001090: 2252 6561 6c43 5547 414e 2d73 6522 0a20  "RealCUGAN-se". 
-000010a0: 2020 202d 2073 6361 6c65 3a20 320a 2020     - scale: 2.  
-000010b0: 2020 2020 2020 2020 2020 2020 202d 206e               - n
-000010c0: 6f69 7365 3a20 2d31 2c20 302c 2031 2c20  oise: -1, 0, 1, 
-000010d0: 322c 2033 0a20 2020 202d 2073 6361 6c65  2, 3.    - scale
-000010e0: 3a20 332c 2034 0a20 2020 2020 2020 2020  : 3, 4.         
-000010f0: 2020 2020 2020 2d20 6e6f 6973 653a 202d        - noise: -
-00001100: 312c 2030 2c20 330a 0a2d 2052 6561 6c43  1, 0, 3..- RealC
-00001110: 5547 414e 2d70 726f 3a0a 2020 2020 2d20  UGAN-pro:.    - 
-00001120: 6d6f 6465 6c3a 2022 5265 616c 4355 4741  model: "RealCUGA
-00001130: 4e2d 7072 6f22 0a20 2020 202d 2073 6361  N-pro".    - sca
-00001140: 6c65 3a20 322c 2033 0a20 2020 202d 206e  le: 2, 3.    - n
-00001150: 6f69 7365 3a20 2d31 2c20 302c 2033 0a0a  oise: -1, 0, 3..
-00001160: 2d20 5265 616c 4553 5247 414e 2d61 6e69  - RealESRGAN-ani
-00001170: 6d65 7669 6465 6f76 333a 0a20 2020 202d  mevideov3:.    -
-00001180: 2067 7075 6964 3a20 3e3d 2030 0a20 2020   gpuid: >= 0.   
-00001190: 202d 206d 6f64 656c 3a20 2252 6561 6c45   - model: "RealE
-000011a0: 5352 4741 4e2d 616e 696d 6576 6964 656f  SRGAN-animevideo
-000011b0: 7633 220a 2020 2020 2d20 7363 616c 653a  v3".    - scale:
-000011c0: 2032 2c20 332c 2034 0a0a 2d20 5265 616c   2, 3, 4..- Real
-000011d0: 4553 5247 414e 3a0a 2020 2020 2d20 6770  ESRGAN:.    - gp
-000011e0: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-000011f0: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00001200: 414e 220a 2020 2020 2d20 7363 616c 653a  AN".    - scale:
-00001210: 2034 0a0a 2d20 5265 616c 4553 5247 414e   4..- RealESRGAN
-00001220: 2d61 6e69 6d65 3a0a 2020 2020 2d20 6770  -anime:.    - gp
-00001230: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-00001240: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00001250: 414e 2d61 6e69 6d65 220a 2020 2020 2d20  AN-anime".    - 
-00001260: 7363 616c 653a 2034 0a0a 2d20 5761 6966  scale: 4..- Waif
-00001270: 7532 782d 6375 6e65 743a 0a20 2020 202d  u2x-cunet:.    -
-00001280: 206d 6f64 656c 3a20 2257 6169 6675 3278   model: "Waifu2x
-00001290: 2d63 756e 6574 220a 2020 2020 2d20 7363  -cunet".    - sc
-000012a0: 616c 653a 2031 0a20 2020 2020 2020 2020  ale: 1.         
-000012b0: 2020 2020 2020 2d20 6e6f 6973 653a 2030        - noise: 0
-000012c0: 2c20 312c 2032 2c20 330a 2020 2020 2d20  , 1, 2, 3.    - 
-000012d0: 7363 616c 653a 2032 0a20 2020 2020 2020  scale: 2.       
-000012e0: 2020 2020 2020 2020 2d20 6e6f 6973 653a          - noise:
-000012f0: 202d 312c 2030 2c20 312c 2032 2c20 330a   -1, 0, 1, 2, 3.
-00001300: 0a2d 2057 6169 6675 3278 2d75 7063 6f6e  .- Waifu2x-upcon
-00001310: 765f 375f 616e 696d 655f 7374 796c 655f  v_7_anime_style_
-00001320: 6172 745f 7267 623a 0a20 2020 202d 206d  art_rgb:.    - m
-00001330: 6f64 656c 3a20 2257 6169 6675 3278 2d75  odel: "Waifu2x-u
-00001340: 7063 6f6e 765f 375f 616e 696d 655f 7374  pconv_7_anime_st
-00001350: 796c 655f 6172 745f 7267 6222 0a20 2020  yle_art_rgb".   
-00001360: 202d 2073 6361 6c65 3a20 320a 2020 2020   - scale: 2.    
-00001370: 2d20 6e6f 6973 653a 202d 312c 2030 2c20  - noise: -1, 0, 
-00001380: 312c 2032 2c20 330a 0a2d 2057 6169 6675  1, 2, 3..- Waifu
-00001390: 3278 2d75 7063 6f6e 765f 375f 7068 6f74  2x-upconv_7_phot
-000013a0: 6f3a 0a20 2020 202d 206d 6f64 656c 3a20  o:.    - model: 
-000013b0: 2257 6169 6675 3278 2d75 7063 6f6e 765f  "Waifu2x-upconv_
-000013c0: 375f 7068 6f74 6f22 0a20 2020 202d 2073  7_photo".    - s
-000013d0: 6361 6c65 3a20 320a 2020 2020 2d20 6e6f  cale: 2.    - no
-000013e0: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-000013f0: 2c20 330a 0a2d 2053 524d 443a 0a20 2020  , 3..- SRMD:.   
-00001400: 202d 2067 7075 6964 3a20 3e3d 2030 0a20   - gpuid: >= 0. 
-00001410: 2020 202d 206d 6f64 656c 3a20 2253 524d     - model: "SRM
-00001420: 4422 0a20 2020 202d 2073 6361 6c65 3a20  D".    - scale: 
-00001430: 322c 2033 2c20 340a 2020 2020 2d20 6e6f  2, 3, 4.    - no
-00001440: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-00001450: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-00001460: 2038 2c20 392c 2031 300a 6060 600a 0a23   8, 9, 10.```..#
-00001470: 2042 7569 6c64 0a0a 5b47 6974 6875 6220   Build..[Github 
-00001480: 4163 7469 6f6e 5d28 6874 7470 733a 2f2f  Action](https://
-00001490: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-000014a0: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-000014b0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000014c0: 7773 2f43 492d 6275 696c 642e 796d 6c29  ws/CI-build.yml)
-000014d0: 0a0a 2a54 6865 2070 726f 6a65 6374 206a  ..*The project j
-000014e0: 7573 7420 6f6e 6c79 2062 6565 6e20 7465  ust only been te
-000014f0: 7374 6564 2069 6e20 5562 756e 7475 2031  sted in Ubuntu 1
-00001500: 382b 2061 6e64 2044 6562 6961 6e20 392b  8+ and Debian 9+
-00001510: 2065 6e76 6972 6f6e 6d65 6e74 7320 6f6e   environments on
-00001520: 204c 696e 7578 2c20 736f 2069 6620 7468   Linux, so if th
-00001530: 6520 7072 6f6a 6563 7420 646f 6573 206e  e project does n
-00001540: 6f74 2077 6f72 6b20 6f6e 0a79 6f75 7220  ot work on.your 
-00001550: 7379 7374 656d 2c20 706c 6561 7365 2074  system, please t
-00001560: 7279 2062 7569 6c64 696e 6720 6974 2e2a  ry building it.*
-00001570: 0a0a 2320 5265 6665 7265 6e63 650a 0a54  ..# Reference..T
-00001580: 6865 2066 6f6c 6c6f 7769 6e67 2072 6566  he following ref
-00001590: 6572 656e 6365 7320 7765 7265 2075 7365  erences were use
-000015a0: 6420 696e 2074 6865 2064 6576 656c 6f70  d in the develop
-000015b0: 6d65 6e74 206f 6620 7468 6973 2070 726f  ment of this pro
-000015c0: 6a65 6374 3a0a 0a2d 205b 6e63 6e6e 5d28  ject:..- [ncnn](
-000015d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000015e0: 6f6d 2f54 656e 6365 6e74 2f6e 636e 6e29  om/Tencent/ncnn)
-000015f0: 202d 206e 636e 6e20 6973 2061 2068 6967   - ncnn is a hig
-00001600: 682d 7065 7266 6f72 6d61 6e63 6520 6e65  h-performance ne
-00001610: 7572 616c 206e 6574 776f 726b 2069 6e66  ural network inf
-00001620: 6572 656e 6365 2066 7261 6d65 776f 726b  erence framework
-00001630: 2064 6576 656c 6f70 6564 2062 790a 2020   developed by.  
-00001640: 5465 6e63 656e 7420 4149 204c 6162 2e0a  Tencent AI Lab..
-00001650: 2d20 5b6e 6968 7569 2f72 6561 6c63 7567  - [nihui/realcug
-00001660: 616e 2d6e 636e 6e2d 7675 6c6b 616e 5d28  an-ncnn-vulkan](
-00001670: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001680: 6f6d 2f6e 6968 7569 2f72 6561 6c63 7567  om/nihui/realcug
-00001690: 616e 2d6e 636e 6e2d 7675 6c6b 616e 2920  an-ncnn-vulkan) 
-000016a0: 2d20 5468 6973 2070 726f 6a65 6374 2070  - This project p
-000016b0: 726f 7669 6465 6420 7468 6520 636f 7265  rovided the core
-000016c0: 0a20 2069 6d70 6c65 6d65 6e74 6174 696f  .  implementatio
-000016d0: 6e20 6f66 2074 6865 2052 6561 6c2d 4355  n of the Real-CU
-000016e0: 4741 4e20 616c 676f 7269 7468 6d20 7573  GAN algorithm us
-000016f0: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
-00001700: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
-00001710: 732e 0a2d 205b 7869 6e6e 7461 6f2f 5265  s..- [xinntao/Re
-00001720: 616c 2d45 5352 4741 4e2d 6e63 6e6e 2d76  al-ESRGAN-ncnn-v
-00001730: 756c 6b61 6e5d 2868 7474 7073 3a2f 2f67  ulkan](https://g
-00001740: 6974 6875 622e 636f 6d2f 7869 6e6e 7461  ithub.com/xinnta
-00001750: 6f2f 5265 616c 2d45 5352 4741 4e2d 6e63  o/Real-ESRGAN-nc
-00001760: 6e6e 2d76 756c 6b61 6e29 202d 2054 6869  nn-vulkan) - Thi
-00001770: 7320 7072 6f6a 6563 7420 7072 6f76 6964  s project provid
-00001780: 6564 2074 6865 2063 6f72 650a 2020 696d  ed the core.  im
-00001790: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-000017a0: 7468 6520 5265 616c 2d45 5352 4741 4e20  the Real-ESRGAN 
-000017b0: 616c 676f 7269 7468 6d20 7573 696e 6720  algorithm using 
-000017c0: 7468 6520 6e63 6e6e 2061 6e64 2056 756c  the ncnn and Vul
-000017d0: 6b61 6e0a 2020 6c69 6272 6172 6965 732e  kan.  libraries.
-000017e0: 0a2d 205b 6e69 6875 692f 7761 6966 7532  .- [nihui/waifu2
-000017f0: 782d 6e63 6e6e 2d76 756c 6b61 6e5d 2868  x-ncnn-vulkan](h
-00001800: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001810: 6d2f 6e69 6875 692f 7761 6966 7532 782d  m/nihui/waifu2x-
-00001820: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
-00001830: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
-00001840: 6964 6564 2074 6865 2063 6f72 650a 2020  ided the core.  
-00001850: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00001860: 6620 7468 6520 5761 6966 7532 7820 616c  f the Waifu2x al
-00001870: 676f 7269 7468 6d20 7573 696e 6720 7468  gorithm using th
-00001880: 6520 6e63 6e6e 2061 6e64 2056 756c 6b61  e ncnn and Vulka
-00001890: 6e20 6c69 6272 6172 6965 732e 0a2d 205b  n libraries..- [
-000018a0: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
-000018b0: 7675 6c6b 616e 5d28 6874 7470 733a 2f2f  vulkan](https://
-000018c0: 6769 7468 7562 2e63 6f6d 2f6e 6968 7569  github.com/nihui
-000018d0: 2f73 726d 642d 6e63 6e6e 2d76 756c 6b61  /srmd-ncnn-vulka
-000018e0: 6e29 202d 2054 6869 7320 7072 6f6a 6563  n) - This projec
-000018f0: 7420 7072 6f76 6964 6564 2074 6865 2063  t provided the c
-00001900: 6f72 6520 696d 706c 656d 656e 7461 7469  ore implementati
-00001910: 6f6e 206f 660a 2020 7468 6520 5352 4d44  on of.  the SRMD
-00001920: 2061 6c67 6f72 6974 686d 2075 7369 6e67   algorithm using
-00001930: 2074 6865 206e 636e 6e20 616e 6420 5675   the ncnn and Vu
-00001940: 6c6b 616e 206c 6962 7261 7269 6573 2e0a  lkan libraries..
-00001950: 2d20 5b72 6561 6c63 7567 616e 2d6e 636e  - [realcugan-ncn
-00001960: 6e2d 7079 5d28 6874 7470 733a 2f2f 6769  n-py](https://gi
-00001970: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
-00001980: 792f 7265 616c 6375 6761 6e2d 6e63 6e6e  y/realcugan-ncnn
-00001990: 2d70 7929 202d 2054 6869 7320 7072 6f6a  -py) - This proj
-000019a0: 6563 7420 7072 6f76 6964 6564 2074 6865  ect provided the
-000019b0: 2050 7974 686f 6e20 4269 6e64 696e 6720   Python Binding 
-000019c0: 666f 720a 2020 7265 616c 6375 6761 6e2d  for.  realcugan-
-000019d0: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
-000019e0: 2050 7942 696e 6431 310a 2d20 5b72 6561   PyBind11.- [rea
-000019f0: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 795d  lesrgan-ncnn-py]
-00001a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001a10: 636f 6d2f 546f 6872 7573 6b79 2f72 6561  com/Tohrusky/rea
-00001a20: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 7929  lesrgan-ncnn-py)
-00001a30: 202d 2054 6869 7320 7072 6f6a 6563 7420   - This project 
-00001a40: 7072 6f76 6964 6564 2074 6865 2050 7974  provided the Pyt
-00001a50: 686f 6e20 4269 6e64 696e 6720 666f 720a  hon Binding for.
-00001a60: 2020 7265 616c 6573 7267 616e 2d6e 636e    realesrgan-ncn
-00001a70: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
-00001a80: 4269 6e64 3131 0a2d 205b 7761 6966 7532  Bind11.- [waifu2
-00001a90: 782d 6e63 6e6e 2d70 795d 2868 7474 7073  x-ncnn-py](https
-00001aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00001ab0: 6872 7573 6b79 2f77 6169 6675 3278 2d6e  hrusky/waifu2x-n
-00001ac0: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
-00001ad0: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
-00001ae0: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
-00001af0: 6e67 2066 6f72 0a20 2077 6169 6675 3278  ng for.  waifu2x
-00001b00: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
-00001b10: 6820 5079 4269 6e64 3131 0a2d 205b 7372  h PyBind11.- [sr
-00001b20: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
-00001b30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00001b40: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
-00001b50: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
-00001b60: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
-00001b70: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
-00001b80: 2066 6f72 0a20 2073 726d 642d 6e63 6e6e   for.  srmd-ncnn
-00001b90: 2d76 756c 6b61 6e0a 2020 7769 7468 2050  -vulkan.  with P
-00001ba0: 7942 696e 6431 310a 0a23 204c 6963 656e  yBind11..# Licen
-00001bb0: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00001bc0: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00001bd0: 6572 2074 6865 2042 5344 2033 2d43 6c61  er the BSD 3-Cla
-00001be0: 7573 6520 2d20 7365 650a 7468 6520 5b4c  use - see.the [L
-00001bf0: 4943 454e 5345 2066 696c 655d 2868 7474  ICENSE file](htt
-00001c00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001c10: 546f 6872 7573 6b79 2f46 696e 616c 3278  Tohrusky/Final2x
-00001c20: 2d63 6f72 652f 626c 6f62 2f6d 6169 6e2f  -core/blob/main/
-00001c30: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
-00001c40: 6169 6c73 2e0a 0a0a                      ails....
+00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000010: 2f73 6f63 6961 6c69 6679 2e67 6974 2e63  /socialify.git.c
+00000020: 692f 546f 6872 7573 6b79 2f46 696e 616c  i/Tohrusky/Final
+00000030: 3278 2d63 6f72 652f 696d 6167 653f 6465  2x-core/image?de
+00000040: 7363 7269 7074 696f 6e3d 3126 666f 726b  scription=1&fork
+00000050: 733d 3126 6973 7375 6573 3d31 266c 616e  s=1&issues=1&lan
+00000060: 6775 6167 653d 3126 6c6f 676f 3d68 7474  guage=1&logo=htt
+00000070: 7073 2533 4125 3246 2532 4672 6177 2e67  ps%3A%2F%2Fraw.g
+00000080: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000090: 2e63 6f6d 2532 4654 6f68 7275 736b 7925  .com%2FTohrusky%
+000000a0: 3246 546f 6872 7573 6b79 2532 466d 6169  2FTohrusky%2Fmai
+000000b0: 6e25 3246 6963 6f6e 2532 466c 6f67 6f2e  n%2Ficon%2Flogo.
+000000c0: 706e 6726 6e61 6d65 3d31 2670 6174 7465  png&name=1&patte
+000000d0: 726e 3d43 6972 6375 6974 2532 3042 6f61  rn=Circuit%20Boa
+000000e0: 7264 2670 756c 6c73 3d31 2673 7461 7267  rd&pulls=1&starg
+000000f0: 617a 6572 733d 3126 7468 656d 653d 4c69  azers=1&theme=Li
+00000100: 6768 7422 3e0a 2020 3c70 6963 7475 7265  ght">.  <picture
+00000110: 3e0a 2020 2020 3c73 6f75 7263 6520 6d65  >.    <source me
+00000120: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
+00000130: 6c6f 722d 7363 6865 6d65 3a20 6461 726b  lor-scheme: dark
+00000140: 2922 2073 7263 7365 743d 2268 7474 7073  )" srcset="https
+00000150: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+00000160: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+00000170: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+00000180: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+00000190: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+000001a0: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+000001b0: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+000001c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000001d0: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+000001e0: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+000001f0: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+00000200: 6f2d 6461 726b 2e70 6e67 266e 616d 653d  o-dark.png&name=
+00000210: 3126 7061 7474 6572 6e3d 4369 7263 7569  1&pattern=Circui
+00000220: 7425 3230 426f 6172 6426 7075 6c6c 733d  t%20Board&pulls=
+00000230: 3126 7374 6172 6761 7a65 7273 3d31 2674  1&stargazers=1&t
+00000240: 6865 6d65 3d44 6172 6b22 202f 3e0a 2020  heme=Dark" />.  
+00000250: 2020 3c73 6f75 7263 6520 6d65 6469 613d    <source media=
+00000260: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
+00000270: 7363 6865 6d65 3a20 6c69 6768 7429 2220  scheme: light)" 
+00000280: 7372 6373 6574 3d22 6874 7470 733a 2f2f  srcset="https://
+00000290: 736f 6369 616c 6966 792e 6769 742e 6369  socialify.git.ci
+000002a0: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+000002b0: 782d 636f 7265 2f69 6d61 6765 3f64 6573  x-core/image?des
+000002c0: 6372 6970 7469 6f6e 3d31 2666 6f72 6b73  cription=1&forks
+000002d0: 3d31 2669 7373 7565 733d 3126 6c61 6e67  =1&issues=1&lang
+000002e0: 7561 6765 3d31 266c 6f67 6f3d 6874 7470  uage=1&logo=http
+000002f0: 7325 3341 2532 4625 3246 7261 772e 6769  s%3A%2F%2Fraw.gi
+00000300: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000310: 636f 6d25 3246 546f 6872 7573 6b79 2532  com%2FTohrusky%2
+00000320: 4654 6f68 7275 736b 7925 3246 6d61 696e  FTohrusky%2Fmain
+00000330: 2532 4669 636f 6e25 3246 6c6f 676f 2e70  %2Ficon%2Flogo.p
+00000340: 6e67 266e 616d 653d 3126 7061 7474 6572  ng&name=1&patter
+00000350: 6e3d 4369 7263 7569 7425 3230 426f 6172  n=Circuit%20Boar
+00000360: 6426 7075 6c6c 733d 3126 7374 6172 6761  d&pulls=1&starga
+00000370: 7a65 7273 3d31 2674 6865 6d65 3d4c 6967  zers=1&theme=Lig
+00000380: 6874 2220 2f3e 0a20 2020 203c 696d 6720  ht" />.    <img 
+00000390: 616c 743d 2253 6f63 6961 6c69 6679 2049  alt="Socialify I
+000003a0: 6d61 6765 2220 7372 633d 2268 7474 7073  mage" src="https
+000003b0: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+000003c0: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+000003d0: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+000003e0: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+000003f0: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+00000400: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+00000410: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+00000420: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000430: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+00000440: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+00000450: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+00000460: 6f2e 706e 6726 6e61 6d65 3d31 2670 6174  o.png&name=1&pat
+00000470: 7465 726e 3d43 6972 6375 6974 2532 3042  tern=Circuit%20B
+00000480: 6f61 7264 2670 756c 6c73 3d31 2673 7461  oard&pulls=1&sta
+00000490: 7267 617a 6572 733d 3126 7468 656d 653d  rgazers=1&theme=
+000004a0: 4c69 6768 7422 202f 3e0a 2020 3c2f 7069  Light" />.  </pi
+000004b0: 6374 7572 653e 0a3c 2f61 3e0a 0a0a 215b  cture>.</a>...![
+000004c0: 4d61 634f 5320 7836 345d 2868 7474 7073  MacOS x64](https
+000004d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004e0: 6f2f 6261 6467 652f 5375 7070 6f72 742d  o/badge/Support-
+000004f0: 4d61 634f 5325 3230 7836 342d 626c 7565  MacOS%20x64-blue
+00000500: 3f6c 6f67 6f3d 4170 706c 6526 7374 796c  ?logo=Apple&styl
+00000510: 653d 666c 6174 2d73 7175 6172 6529 0a21  e=flat-square).!
+00000520: 5b4d 6163 4f53 2061 726d 3634 5d28 6874  [MacOS arm64](ht
+00000530: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000540: 732e 696f 2f62 6164 6765 2f53 7570 706f  s.io/badge/Suppo
+00000550: 7274 2d4d 6163 4f53 2532 3061 726d 3634  rt-MacOS%20arm64
+00000560: 2d62 6c75 653f 6c6f 676f 3d41 7070 6c65  -blue?logo=Apple
+00000570: 2673 7479 6c65 3d66 6c61 742d 7371 7561  &style=flat-squa
+00000580: 7265 290a 215b 5769 6e64 6f77 7320 7836  re).![Windows x6
+00000590: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+000005a0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000005b0: 5375 7070 6f72 742d 5769 6e64 6f77 7325  Support-Windows%
+000005c0: 3230 7836 342d 626c 7565 3f6c 6f67 6f3d  20x64-blue?logo=
+000005d0: 5769 6e64 6f77 7326 7374 796c 653d 666c  Windows&style=fl
+000005e0: 6174 2d73 7175 6172 6529 0a21 5b57 696e  at-square).![Win
+000005f0: 646f 7773 2061 726d 3634 5d28 6874 7470  dows arm64](http
+00000600: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000610: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
+00000620: 2d57 696e 646f 7773 2532 3061 726d 3634  -Windows%20arm64
+00000630: 2d62 6c75 653f 6c6f 676f 3d57 696e 646f  -blue?logo=Windo
+00000640: 7773 2673 7479 6c65 3d66 6c61 742d 7371  ws&style=flat-sq
+00000650: 7561 7265 290a 215b 4c69 6e75 7820 7836  uare).![Linux x6
+00000660: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+00000670: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000680: 5375 7070 6f72 742d 4c69 6e75 7825 3230  Support-Linux%20
+00000690: 7836 342d 626c 7565 3f6c 6f67 6f3d 4c69  x64-blue?logo=Li
+000006a0: 6e75 7826 7374 796c 653d 666c 6174 2d73  nux&style=flat-s
+000006b0: 7175 6172 6529 0a5b 215b 636f 6465 636f  quare).[![codeco
+000006c0: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+000006d0: 6f76 2e69 6f2f 6768 2f54 6f68 7275 736b  ov.io/gh/Tohrusk
+000006e0: 792f 4669 6e61 6c32 782d 636f 7265 2f62  y/Final2x-core/b
+000006f0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+00000700: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000710: 3d42 3254 4e4b 594e 344f 3429 5d28 6874  =B2TNKYN4O4)](ht
+00000720: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000730: 2f67 682f 546f 6872 7573 6b79 2f46 696e  /gh/Tohrusky/Fin
+00000740: 616c 3278 2d63 6f72 6529 0a5b 215b 4349  al2x-core).[![CI
+00000750: 2d74 6573 745d 2868 7474 7073 3a2f 2f67  -test](https://g
+00000760: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+00000770: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+00000780: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000790: 732f 4349 2d74 6573 742e 796d 6c2f 6261  s/CI-test.yml/ba
+000007a0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+000007b0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+000007c0: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+000007d0: 7265 2f61 6374 696f 6e73 2f77 6f72 6b66  re/actions/workf
+000007e0: 6c6f 7773 2f43 492d 7465 7374 2e79 6d6c  lows/CI-test.yml
+000007f0: 290a 5b21 5b43 492d 6275 696c 645d 2868  ).[![CI-build](h
+00000800: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000810: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
+00000820: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
+00000830: 776f 726b 666c 6f77 732f 4349 2d62 7569  workflows/CI-bui
+00000840: 6c64 2e79 6d6c 2f62 6164 6765 2e73 7667  ld.yml/badge.svg
+00000850: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000860: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
+00000870: 696e 616c 3278 2d63 6f72 652f 6163 7469  inal2x-core/acti
+00000880: 6f6e 732f 776f 726b 666c 6f77 732f 4349  ons/workflows/CI
+00000890: 2d62 7569 6c64 2e79 6d6c 290a 5b21 5b52  -build.yml).[![R
+000008a0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+000008b0: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
+000008c0: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
+000008d0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000008e0: 7773 2f52 656c 6561 7365 2e79 6d6c 2f62  ws/Release.yml/b
+000008f0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000900: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00000910: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
+00000920: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
+00000930: 666c 6f77 732f 5265 6c65 6173 652e 796d  flows/Release.ym
+00000940: 6c29 0a5b 215b 5049 502d 7465 7374 5d28  l).[![PIP-test](
+00000950: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000960: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
+00000970: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
+00000980: 2f77 6f72 6b66 6c6f 7773 2f50 4950 2d74  /workflows/PIP-t
+00000990: 6573 742e 796d 6c2f 6261 6467 652e 7376  est.yml/badge.sv
+000009a0: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+000009b0: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
+000009c0: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
+000009d0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f50  ions/workflows/P
+000009e0: 4950 2d74 6573 742e 796d 6c29 0a5b 215b  IP-test.yml).[![
+000009f0: 5265 6c65 6173 652d 7079 7069 5d28 6874  Release-pypi](ht
+00000a00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a10: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000a20: 782d 636f 7265 2f61 6374 696f 6e73 2f77  x-core/actions/w
+00000a30: 6f72 6b66 6c6f 7773 2f52 656c 6561 7365  orkflows/Release
+00000a40: 2d70 7970 692e 796d 6c2f 6261 6467 652e  -pypi.yml/badge.
+00000a50: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000a60: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
+00000a70: 792f 4669 6e61 6c32 782d 636f 7265 2f61  y/Final2x-core/a
+00000a80: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000a90: 2f52 656c 6561 7365 2d70 7970 692e 796d  /Release-pypi.ym
+00000aa0: 6c29 0a5b 215b 5079 5049 2076 6572 7369  l).[![PyPI versi
+00000ab0: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000ac0: 652e 6675 7279 2e69 6f2f 7079 2f46 696e  e.fury.io/py/Fin
+00000ad0: 616c 3278 2d63 6f72 652e 7376 6729 5d28  al2x-core.svg)](
+00000ae0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000af0: 7279 2e69 6f2f 7079 2f46 696e 616c 3278  ry.io/py/Final2x
+00000b00: 2d63 6f72 6529 0a21 5b47 6974 4875 625d  -core).![GitHub]
+00000b10: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000b20: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000b30: 6963 656e 7365 2f54 6f68 7275 736b 792f  icense/Tohrusky/
+00000b40: 4669 6e61 6c32 782d 636f 7265 290a 0a46  Final2x-core)..F
+00000b50: 696e 616c 3278 2d63 6f72 6520 6973 2061  inal2x-core is a
+00000b60: 2063 726f 7373 2d70 6c61 7466 6f72 6d20   cross-platform 
+00000b70: 696d 6167 6520 7375 7065 722d 7265 736f  image super-reso
+00000b80: 6c75 7469 6f6e 2043 4c49 2074 6f6f 6c20  lution CLI tool 
+00000b90: 666f 7220 5b46 696e 616c 3278 5d28 6874  for [Final2x](ht
+00000ba0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000bb0: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000bc0: 7829 2e20 4966 2079 6f75 2068 6176 6520  x). If you have 
+00000bd0: 616e 7920 7175 6573 7469 6f6e 732c 2070  any questions, p
+00000be0: 6c65 6173 6520 7261 6973 6520 616e 2069  lease raise an i
+00000bf0: 7373 7565 205b 696e 2074 6869 7320 7265  ssue [in this re
+00000c00: 706f 7369 746f 7279 5d28 6874 7470 733a  pository](https:
+00000c10: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00000c20: 7275 736b 792f 4669 6e61 6c32 7829 2e0a  rusky/Final2x)..
+00000c30: 0a23 2049 6e73 7461 6c6c 0a0a 446f 776e  .# Install..Down
+00000c40: 6c6f 6164 2069 6e20 5b52 656c 6561 7365  load in [Release
+00000c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000c60: 2e63 6f6d 2f54 6f68 7275 736b 792f 4669  .com/Tohrusky/Fi
+00000c70: 6e61 6c32 782d 636f 7265 2f72 656c 6561  nal2x-core/relea
+00000c80: 7365 7329 206f 7220 7573 6520 7069 7020  ses) or use pip 
+00000c90: 2870 7974 686f 6e20 3e3d 2033 2e36 2c20  (python >= 3.6, 
+00000ca0: 3e3d 332e 3920 666f 7220 4d61 634f 530a  >=3.9 for MacOS.
+00000cb0: 6172 6d36 3429 0a0a 6060 6073 6865 6c6c  arm64)..```shell
+00000cc0: 0a70 6970 2069 6e73 7461 6c6c 2046 696e  .pip install Fin
+00000cd0: 616c 3278 2d63 6f72 650a 6060 600a 0a23  al2x-core.```..#
+00000ce0: 2055 7365 0a0a 6060 6073 6865 6c6c 0a75   Use..```shell.u
+00000cf0: 7361 6765 3a20 4669 6e61 6c32 782d 636f  sage: Final2x-co
+00000d00: 7265 205b 2d68 5d20 5b2d 6220 4241 5345  re [-h] [-b BASE
+00000d10: 3634 5d20 5b2d 6a20 4a53 4f4e 5d20 5b2d  64] [-j JSON] [-
+00000d20: 7920 5941 4d4c 5d20 5b2d 6f5d 0a0a 7768  y YAML] [-o]..wh
+00000d30: 656e 2070 6172 6120 6973 206e 6f74 2073  en para is not s
+00000d40: 7065 6369 6669 6564 2c20 7468 6520 636f  pecified, the co
+00000d50: 6e66 6967 2e79 616d 6c20 6669 6c65 2069  nfig.yaml file i
+00000d60: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
+00000d70: 7769 6c6c 2062 6520 7265 6164 2061 7574  will be read aut
+00000d80: 6f6d 6174 6963 616c 6c79 0a0a 6f70 7469  omatically..opti
+00000d90: 6f6e 616c 2061 7267 756d 656e 7473 3a0a  onal arguments:.
+00000da0: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+00000db0: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
+00000dc0: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
+00000dd0: 6e64 2065 7869 740a 2020 2d62 2042 4153  nd exit.  -b BAS
+00000de0: 4536 342c 202d 2d42 4153 4536 3420 4241  E64, --BASE64 BA
+00000df0: 5345 3634 0a20 2020 2020 2020 2020 2020  SE64.           
+00000e00: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+00000e10: 6536 3420 7374 7269 6e67 2066 6f72 2063  e64 string for c
+00000e20: 6f6e 6669 6720 6a73 6f6e 0a20 202d 6a20  onfig json.  -j 
+00000e30: 4a53 4f4e 2c20 2d2d 4a53 4f4e 204a 534f  JSON, --JSON JSO
+00000e40: 4e20 204a 534f 4e20 7374 7269 6e67 2066  N  JSON string f
+00000e50: 6f72 2063 6f6e 6669 670a 2020 2d79 2059  or config.  -y Y
+00000e60: 414d 4c2c 202d 2d59 414d 4c20 5941 4d4c  AML, --YAML YAML
+00000e70: 2020 7961 6d6c 2063 6f6e 6669 6720 6669    yaml config fi
+00000e80: 6c65 2070 6174 680a 2020 2d6c 2c20 2d2d  le path.  -l, --
+00000e90: 4c4f 4720 2020 2020 2020 2020 2020 2020  LOG             
+00000ea0: 7361 7665 206c 6f67 0a20 202d 6f2c 202d  save log.  -o, -
+00000eb0: 2d4f 5020 2020 2020 2020 2020 2020 2020  -OP             
+00000ec0: 2063 6865 636b 2069 6e73 7461 6c6c 0a60   check install.`
+00000ed0: 6060 0a0a 2320 436f 6e66 6967 0a0a 5061  ``..# Config..Pa
+00000ee0: 7373 2074 6865 2063 6f6e 6669 6720 6a73  ss the config js
+00000ef0: 6f6e 2073 7472 696e 6720 746f 2074 6865  on string to the
+00000f00: 2070 726f 6772 616d 2074 6872 6f75 6768   program through
+00000f10: 2074 6865 2060 2d6a 6020 7061 7261 6d65   the `-j` parame
+00000f20: 7465 722e 0a0a 2a2a 504c 4541 5345 204e  ter...**PLEASE N
+00000f30: 4f54 453a 2074 6865 2063 6f6e 6669 6720  OTE: the config 
+00000f40: 6973 204a 534f 4e2c 2072 656d 6f76 6520  is JSON, remove 
+00000f50: 7468 6520 2f2f 2063 6f6d 6d65 6e74 7320  the // comments 
+00000f60: 6265 666f 7265 2075 7365 2e2a 2a0a 0a60  before use.**..`
+00000f70: 6060 6a73 6f6e 0a7b 0a20 2022 6770 7569  ``json.{.  "gpui
+00000f80: 6422 3a20 302c 0a20 202f 2f20 4750 5520  d": 0,.  // GPU 
+00000f90: 6964 2c20 3e3d 202d 3120 282d 3120 666f  id, >= -1 (-1 fo
+00000fa0: 7220 4350 552c 206d 6179 206e 6f74 2077  r CPU, may not w
+00000fb0: 6f72 6b20 666f 7220 736f 6d65 206d 6f64  ork for some mod
+00000fc0: 656c 732e 290a 2020 2269 6e70 7574 7061  els.).  "inputpa
+00000fd0: 7468 223a 205b 0a20 2020 202f 2f20 496e  th": [.    // In
+00000fe0: 7075 7420 696d 6167 6520 7061 7468 732c  put image paths,
+00000ff0: 2073 686f 756c 6420 6265 2061 206c 6973   should be a lis
+00001000: 742e 0a20 2020 2022 7061 7468 2f74 6f2f  t..    "path/to/
+00001010: 696d 6731 2e6a 7067 222c 0a20 2020 2022  img1.jpg",.    "
+00001020: 7061 7468 2f74 6f2f 696d 6732 2e70 6e67  path/to/img2.png
+00001030: 220a 2020 5d2c 0a20 2022 6d6f 6465 6c22  ".  ],.  "model"
+00001040: 3a20 2252 6561 6c43 5547 414e 2d70 726f  : "RealCUGAN-pro
+00001050: 222c 0a20 202f 2f20 6d6f 6465 6c20 6e61  ",.  // model na
+00001060: 6d65 0a20 2022 6d6f 6465 6c73 6361 6c65  me.  "modelscale
+00001070: 223a 2032 2c0a 2020 2f2f 206d 6f64 656c  ": 2,.  // model
+00001080: 2075 7073 6361 6c65 2066 6163 746f 720a   upscale factor.
+00001090: 2020 226d 6f64 656c 6e6f 6973 6522 3a20    "modelnoise": 
+000010a0: 2d31 2c0a 2020 2f2f 2044 454e 4f49 5345  -1,.  // DENOISE
+000010b0: 206c 6576 656c 0a20 2022 6f75 7470 7574   level.  "output
+000010c0: 7061 7468 223a 2022 7061 7468 2f74 6f2f  path": "path/to/
+000010d0: 6f75 7470 7574 222c 0a20 202f 2f20 6f75  output",.  // ou
+000010e0: 7470 7574 2070 6174 680a 2020 2274 6172  tput path.  "tar
+000010f0: 6765 7473 6361 6c65 223a 2032 2e30 2c0a  getscale": 2.0,.
+00001100: 2020 2f2f 2054 6172 6765 7420 7570 7363    // Target upsc
+00001110: 616c 6520 6661 6374 6f72 2c20 7570 7363  ale factor, upsc
+00001120: 616c 6520 6d75 6c74 6970 6c65 2074 696d  ale multiple tim
+00001130: 6573 2074 6f20 6163 6869 6576 6520 7468  es to achieve th
+00001140: 6520 7461 7267 6574 2075 7073 6361 6c65  e target upscale
+00001150: 2066 6163 746f 722e 0a20 202f 2f20 4966   factor..  // If
+00001160: 206e 6f74 2069 6e76 616c 6964 2c20 7573   not invalid, us
+00001170: 6520 6d6f 6465 6c73 6361 6c65 2e0a 2020  e modelscale..  
+00001180: 2274 7461 223a 2066 616c 7365 0a20 202f  "tta": false.  /
+00001190: 2f20 5465 7374 2054 696d 6520 4175 676d  / Test Time Augm
+000011a0: 656e 7461 7469 6f6e 2c20 6465 6661 756c  entation, defaul
+000011b0: 7420 6661 6c73 650a 7d0a 6060 600a 0a2a  t false.}.```..*
+000011c0: 2a53 5550 504f 5254 4544 204d 4f44 454c  *SUPPORTED MODEL
+000011d0: 204c 4953 543a 2a2a 0a0a 6060 6079 616d   LIST:**..```yam
+000011e0: 6c0a 2d20 5265 616c 4355 4741 4e2d 7365  l.- RealCUGAN-se
+000011f0: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+00001200: 5265 616c 4355 4741 4e2d 7365 220a 2020  RealCUGAN-se".  
+00001210: 2020 2d20 7363 616c 653a 2032 0a20 2020    - scale: 2.   
+00001220: 2020 2020 2020 2020 2020 2020 2d20 6e6f              - no
+00001230: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
+00001240: 2c20 330a 2020 2020 2d20 7363 616c 653a  , 3.    - scale:
+00001250: 2033 2c20 340a 2020 2020 2020 2020 2020   3, 4.          
+00001260: 2020 2020 202d 206e 6f69 7365 3a20 2d31       - noise: -1
+00001270: 2c20 302c 2033 0a0a 2d20 5265 616c 4355  , 0, 3..- RealCU
+00001280: 4741 4e2d 7072 6f3a 0a20 2020 202d 206d  GAN-pro:.    - m
+00001290: 6f64 656c 3a20 2252 6561 6c43 5547 414e  odel: "RealCUGAN
+000012a0: 2d70 726f 220a 2020 2020 2d20 7363 616c  -pro".    - scal
+000012b0: 653a 2032 2c20 330a 2020 2020 2d20 6e6f  e: 2, 3.    - no
+000012c0: 6973 653a 202d 312c 2030 2c20 330a 0a2d  ise: -1, 0, 3..-
+000012d0: 2052 6561 6c45 5352 4741 4e2d 616e 696d   RealESRGAN-anim
+000012e0: 6576 6964 656f 7633 3a0a 2020 2020 2d20  evideov3:.    - 
+000012f0: 6770 7569 643a 203e 3d20 300a 2020 2020  gpuid: >= 0.    
+00001300: 2d20 6d6f 6465 6c3a 2022 5265 616c 4553  - model: "RealES
+00001310: 5247 414e 2d61 6e69 6d65 7669 6465 6f76  RGAN-animevideov
+00001320: 3322 0a20 2020 202d 2073 6361 6c65 3a20  3".    - scale: 
+00001330: 322c 2033 2c20 340a 0a2d 2052 6561 6c45  2, 3, 4..- RealE
+00001340: 5352 4741 4e3a 0a20 2020 202d 2067 7075  SRGAN:.    - gpu
+00001350: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+00001360: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+00001370: 4e22 0a20 2020 202d 2073 6361 6c65 3a20  N".    - scale: 
+00001380: 340a 0a2d 2052 6561 6c45 5352 4741 4e2d  4..- RealESRGAN-
+00001390: 616e 696d 653a 0a20 2020 202d 2067 7075  anime:.    - gpu
+000013a0: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+000013b0: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+000013c0: 4e2d 616e 696d 6522 0a20 2020 202d 2073  N-anime".    - s
+000013d0: 6361 6c65 3a20 340a 0a2d 2057 6169 6675  cale: 4..- Waifu
+000013e0: 3278 2d63 756e 6574 3a0a 2020 2020 2d20  2x-cunet:.    - 
+000013f0: 6d6f 6465 6c3a 2022 5761 6966 7532 782d  model: "Waifu2x-
+00001400: 6375 6e65 7422 0a20 2020 202d 2073 6361  cunet".    - sca
+00001410: 6c65 3a20 310a 2020 2020 2020 2020 2020  le: 1.          
+00001420: 2020 2020 202d 206e 6f69 7365 3a20 302c       - noise: 0,
+00001430: 2031 2c20 322c 2033 0a20 2020 202d 2073   1, 2, 3.    - s
+00001440: 6361 6c65 3a20 320a 2020 2020 2020 2020  cale: 2.        
+00001450: 2020 2020 2020 202d 206e 6f69 7365 3a20         - noise: 
+00001460: 2d31 2c20 302c 2031 2c20 322c 2033 0a0a  -1, 0, 1, 2, 3..
+00001470: 2d20 5761 6966 7532 782d 7570 636f 6e76  - Waifu2x-upconv
+00001480: 5f37 5f61 6e69 6d65 5f73 7479 6c65 5f61  _7_anime_style_a
+00001490: 7274 5f72 6762 3a0a 2020 2020 2d20 6d6f  rt_rgb:.    - mo
+000014a0: 6465 6c3a 2022 5761 6966 7532 782d 7570  del: "Waifu2x-up
+000014b0: 636f 6e76 5f37 5f61 6e69 6d65 5f73 7479  conv_7_anime_sty
+000014c0: 6c65 5f61 7274 5f72 6762 220a 2020 2020  le_art_rgb".    
+000014d0: 2d20 7363 616c 653a 2032 0a20 2020 202d  - scale: 2.    -
+000014e0: 206e 6f69 7365 3a20 2d31 2c20 302c 2031   noise: -1, 0, 1
+000014f0: 2c20 322c 2033 0a0a 2d20 5761 6966 7532  , 2, 3..- Waifu2
+00001500: 782d 7570 636f 6e76 5f37 5f70 686f 746f  x-upconv_7_photo
+00001510: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+00001520: 5761 6966 7532 782d 7570 636f 6e76 5f37  Waifu2x-upconv_7
+00001530: 5f70 686f 746f 220a 2020 2020 2d20 7363  _photo".    - sc
+00001540: 616c 653a 2032 0a20 2020 202d 206e 6f69  ale: 2.    - noi
+00001550: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+00001560: 2033 0a0a 2d20 5352 4d44 3a0a 2020 2020   3..- SRMD:.    
+00001570: 2d20 6770 7569 643a 203e 3d20 300a 2020  - gpuid: >= 0.  
+00001580: 2020 2d20 6d6f 6465 6c3a 2022 5352 4d44    - model: "SRMD
+00001590: 220a 2020 2020 2d20 7363 616c 653a 2032  ".    - scale: 2
+000015a0: 2c20 332c 2034 0a20 2020 202d 206e 6f69  , 3, 4.    - noi
+000015b0: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+000015c0: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+000015d0: 382c 2039 2c20 3130 0a60 6060 0a0a 2320  8, 9, 10.```..# 
+000015e0: 4275 696c 640a 0a5b 4769 7468 7562 2041  Build..[Github A
+000015f0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f67  ction](https://g
+00001600: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+00001610: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+00001620: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00001630: 732f 4349 2d62 7569 6c64 2e79 6d6c 290a  s/CI-build.yml).
+00001640: 0a2a 5468 6520 7072 6f6a 6563 7420 6a75  .*The project ju
+00001650: 7374 206f 6e6c 7920 6265 656e 2074 6573  st only been tes
+00001660: 7465 6420 696e 2055 6275 6e74 7520 3138  ted in Ubuntu 18
+00001670: 2b20 616e 6420 4465 6269 616e 2039 2b20  + and Debian 9+ 
+00001680: 656e 7669 726f 6e6d 656e 7473 206f 6e20  environments on 
+00001690: 4c69 6e75 782c 2073 6f20 6966 2074 6865  Linux, so if the
+000016a0: 2070 726f 6a65 6374 2064 6f65 7320 6e6f   project does no
+000016b0: 7420 776f 726b 206f 6e0a 796f 7572 2073  t work on.your s
+000016c0: 7973 7465 6d2c 2070 6c65 6173 6520 7472  ystem, please tr
+000016d0: 7920 6275 696c 6469 6e67 2069 742e 2a0a  y building it.*.
+000016e0: 0a23 2052 6566 6572 656e 6365 0a0a 5468  .# Reference..Th
+000016f0: 6520 666f 6c6c 6f77 696e 6720 7265 6665  e following refe
+00001700: 7265 6e63 6573 2077 6572 6520 7573 6564  rences were used
+00001710: 2069 6e20 7468 6520 6465 7665 6c6f 706d   in the developm
+00001720: 656e 7420 6f66 2074 6869 7320 7072 6f6a  ent of this proj
+00001730: 6563 743a 0a0a 2d20 5b6e 636e 6e5d 2868  ect:..- [ncnn](h
+00001740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001750: 6d2f 5465 6e63 656e 742f 6e63 6e6e 2920  m/Tencent/ncnn) 
+00001760: 2d20 6e63 6e6e 2069 7320 6120 6869 6768  - ncnn is a high
+00001770: 2d70 6572 666f 726d 616e 6365 206e 6575  -performance neu
+00001780: 7261 6c20 6e65 7477 6f72 6b20 696e 6665  ral network infe
+00001790: 7265 6e63 6520 6672 616d 6577 6f72 6b20  rence framework 
+000017a0: 6465 7665 6c6f 7065 6420 6279 2054 656e  developed by Ten
+000017b0: 6365 6e74 2041 4920 4c61 622e 0a2d 205b  cent AI Lab..- [
+000017c0: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+000017d0: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+000017e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000017f0: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+00001800: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
+00001810: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
+00001820: 6964 6564 2074 6865 2063 6f72 6520 696d  ided the core im
+00001830: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001840: 7468 6520 5265 616c 2d43 5547 414e 2061  the Real-CUGAN a
+00001850: 6c67 6f72 6974 686d 2075 7369 6e67 2074  lgorithm using t
+00001860: 6865 206e 636e 6e20 616e 6420 5675 6c6b  he ncnn and Vulk
+00001870: 616e 206c 6962 7261 7269 6573 2e0a 2d20  an libraries..- 
+00001880: 5b78 696e 6e74 616f 2f52 6561 6c2d 4553  [xinntao/Real-ES
+00001890: 5247 414e 2d6e 636e 6e2d 7675 6c6b 616e  RGAN-ncnn-vulkan
+000018a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000018b0: 2e63 6f6d 2f78 696e 6e74 616f 2f52 6561  .com/xinntao/Rea
+000018c0: 6c2d 4553 5247 414e 2d6e 636e 6e2d 7675  l-ESRGAN-ncnn-vu
+000018d0: 6c6b 616e 2920 2d20 5468 6973 2070 726f  lkan) - This pro
+000018e0: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+000018f0: 6520 636f 7265 2069 6d70 6c65 6d65 6e74  e core implement
+00001900: 6174 696f 6e20 6f66 2074 6865 2052 6561  ation of the Rea
+00001910: 6c2d 4553 5247 414e 2061 6c67 6f72 6974  l-ESRGAN algorit
+00001920: 686d 2075 7369 6e67 2074 6865 206e 636e  hm using the ncn
+00001930: 6e20 616e 6420 5675 6c6b 616e 206c 6962  n and Vulkan lib
+00001940: 7261 7269 6573 2e0a 2d20 5b6e 6968 7569  raries..- [nihui
+00001950: 2f77 6169 6675 3278 2d6e 636e 6e2d 7675  /waifu2x-ncnn-vu
+00001960: 6c6b 616e 5d28 6874 7470 733a 2f2f 6769  lkan](https://gi
+00001970: 7468 7562 2e63 6f6d 2f6e 6968 7569 2f77  thub.com/nihui/w
+00001980: 6169 6675 3278 2d6e 636e 6e2d 7675 6c6b  aifu2x-ncnn-vulk
+00001990: 616e 2920 2d20 5468 6973 2070 726f 6a65  an) - This proje
+000019a0: 6374 2070 726f 7669 6465 6420 7468 6520  ct provided the 
+000019b0: 636f 7265 2069 6d70 6c65 6d65 6e74 6174  core implementat
+000019c0: 696f 6e20 6f66 2074 6865 2057 6169 6675  ion of the Waifu
+000019d0: 3278 2061 6c67 6f72 6974 686d 2075 7369  2x algorithm usi
+000019e0: 6e67 2074 6865 206e 636e 6e20 616e 6420  ng the ncnn and 
+000019f0: 5675 6c6b 616e 206c 6962 7261 7269 6573  Vulkan libraries
+00001a00: 2e0a 2d20 5b6e 6968 7569 2f73 726d 642d  ..- [nihui/srmd-
+00001a10: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+00001a20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001a30: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
+00001a40: 7675 6c6b 616e 2920 2d20 5468 6973 2070  vulkan) - This p
+00001a50: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001a60: 7468 6520 636f 7265 2069 6d70 6c65 6d65  the core impleme
+00001a70: 6e74 6174 696f 6e20 6f66 2074 6865 2053  ntation of the S
+00001a80: 524d 4420 616c 676f 7269 7468 6d20 7573  RMD algorithm us
+00001a90: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
+00001aa0: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
+00001ab0: 732e 0a2d 205b 7265 616c 6375 6761 6e2d  s..- [realcugan-
+00001ac0: 6e63 6e6e 2d70 795d 2868 7474 7073 3a2f  ncnn-py](https:/
+00001ad0: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
+00001ae0: 7573 6b79 2f72 6561 6c63 7567 616e 2d6e  usky/realcugan-n
+00001af0: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
+00001b00: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001b10: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
+00001b20: 6e67 2066 6f72 2072 6561 6c63 7567 616e  ng for realcugan
+00001b30: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
+00001b40: 6820 5079 4269 6e64 3131 2e0a 2d20 5b72  h PyBind11..- [r
+00001b50: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001b60: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00001b70: 622e 636f 6d2f 546f 6872 7573 6b79 2f72  b.com/Tohrusky/r
+00001b80: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001b90: 7929 202d 2054 6869 7320 7072 6f6a 6563  y) - This projec
+00001ba0: 7420 7072 6f76 6964 6564 2074 6865 2050  t provided the P
+00001bb0: 7974 686f 6e20 4269 6e64 696e 6720 666f  ython Binding fo
+00001bc0: 7220 7265 616c 6573 7267 616e 2d6e 636e  r realesrgan-ncn
+00001bd0: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
+00001be0: 4269 6e64 3131 2e0a 2d20 5b77 6169 6675  Bind11..- [waifu
+00001bf0: 3278 2d6e 636e 6e2d 7079 5d28 6874 7470  2x-ncnn-py](http
+00001c00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001c10: 6f68 7275 736b 792f 7761 6966 7532 782d  ohrusky/waifu2x-
+00001c20: 6e63 6e6e 2d70 7929 202d 2054 6869 7320  ncnn-py) - This 
+00001c30: 7072 6f6a 6563 7420 7072 6f76 6964 6564  project provided
+00001c40: 2074 6865 2050 7974 686f 6e20 4269 6e64   the Python Bind
+00001c50: 696e 6720 666f 7220 7761 6966 7532 782d  ing for waifu2x-
+00001c60: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
+00001c70: 2050 7942 696e 6431 312e 0a2d 205b 7372   PyBind11..- [sr
+00001c80: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
+00001c90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001ca0: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
+00001cb0: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
+00001cc0: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+00001cd0: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
+00001ce0: 2066 6f72 2073 726d 642d 6e63 6e6e 2d76   for srmd-ncnn-v
+00001cf0: 756c 6b61 6e20 7769 7468 2050 7942 696e  ulkan with PyBin
+00001d00: 6431 312e 0a0a 2320 4c69 6365 6e73 650a  d11...# License.
+00001d10: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001d20: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001d30: 7468 6520 4253 4420 332d 436c 6175 7365  the BSD 3-Clause
+00001d40: 202d 2073 6565 0a74 6865 205b 4c49 4345   - see.the [LICE
+00001d50: 4e53 4520 6669 6c65 5d28 6874 7470 733a  NSE file](https:
+00001d60: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00001d70: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+00001d80: 7265 2f62 6c6f 622f 6d61 696e 2f4c 4943  re/blob/main/LIC
+00001d90: 454e 5345 2920 666f 7220 6465 7461 696c  ENSE) for detail
+00001da0: 732e 0a                                  s..
```

### Comparing `Final2x-core-1.0.2/Final2x_core.egg-info/SOURCES.txt` & `Final2x-core-1.0.3/Final2x_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/LICENSE` & `Final2x-core-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.2/PKG-INFO` & `Final2x-core-1.0.3/Final2x_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4669 6e61  : 2.1.Name: Fina
 00000020: 6c32 782d 636f 7265 0a56 6572 7369 6f6e  l2x-core.Version
-00000030: 3a20 312e 302e 320a 5375 6d6d 6172 793a  : 1.0.2.Summary:
+00000030: 3a20 312e 302e 330a 5375 6d6d 6172 793a  : 1.0.3.Summary:
 00000040: 2055 4e4b 4e4f 574e 0a48 6f6d 652d 7061   UNKNOWN.Home-pa
 00000050: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000060: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
 00000070: 4669 6e61 6c32 782d 636f 7265 0a41 7574  Final2x-core.Aut
 00000080: 686f 723a 2054 6f68 7275 736b 790a 4c69  hor: Tohrusky.Li
 00000090: 6365 6e73 653a 2055 4e4b 4e4f 574e 0a50  cense: UNKNOWN.P
 000000a0: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
@@ -38,416 +38,482 @@
 00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 00000260: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
 00000270: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
 00000280: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000290: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 000002a0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
 000002b0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-000002c0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000002d0: 223e 0a0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
-000002e0: 7470 733a 2f2f 7332 2e6c 6f6c 692e 6e65  tps://s2.loli.ne
-000002f0: 742f 3230 3233 2f30 362f 3139 2f35 3437  t/2023/06/19/547
-00000300: 7152 6563 4864 6e4a 4962 4b75 2e70 6e67  qRecHdnJIbKu.png
-00000310: 2220 6865 6967 6874 3d22 3132 3822 3e0a  " height="128">.
-00000320: 0a3c 2f70 3e0a 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
-00000330: 3d22 6365 6e74 6572 223e 2046 696e 616c  ="center"> Final
-00000340: 3278 2d63 6f72 6520 3c2f 6831 3e0a 0a21  2x-core </h1>..!
-00000350: 5b4d 6163 4f53 2078 3634 5d28 6874 7470  [MacOS x64](http
-00000360: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000370: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
-00000380: 2d4d 6163 4f53 2532 3078 3634 2d62 6c75  -MacOS%20x64-blu
-00000390: 653f 6c6f 676f 3d41 7070 6c65 2673 7479  e?logo=Apple&sty
-000003a0: 6c65 3d66 6c61 742d 7371 7561 7265 290a  le=flat-square).
-000003b0: 215b 4d61 634f 5320 6172 6d36 345d 2868  ![MacOS arm64](h
-000003c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000003d0: 6473 2e69 6f2f 6261 6467 652f 5375 7070  ds.io/badge/Supp
-000003e0: 6f72 742d 4d61 634f 5325 3230 6172 6d36  ort-MacOS%20arm6
-000003f0: 342d 626c 7565 3f6c 6f67 6f3d 4170 706c  4-blue?logo=Appl
-00000400: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-00000410: 6172 6529 0a21 5b57 696e 646f 7773 2078  are).![Windows x
-00000420: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000430: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000440: 2f53 7570 706f 7274 2d57 696e 646f 7773  /Support-Windows
-00000450: 2532 3078 3634 2d62 6c75 653f 6c6f 676f  %20x64-blue?logo
-00000460: 3d57 696e 646f 7773 2673 7479 6c65 3d66  =Windows&style=f
-00000470: 6c61 742d 7371 7561 7265 290a 215b 5769  lat-square).![Wi
-00000480: 6e64 6f77 7320 6172 6d36 345d 2868 7474  ndows arm64](htt
-00000490: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000004a0: 2e69 6f2f 6261 6467 652f 5375 7070 6f72  .io/badge/Suppor
-000004b0: 742d 5769 6e64 6f77 7325 3230 6172 6d36  t-Windows%20arm6
-000004c0: 342d 626c 7565 3f6c 6f67 6f3d 5769 6e64  4-blue?logo=Wind
-000004d0: 6f77 7326 7374 796c 653d 666c 6174 2d73  ows&style=flat-s
-000004e0: 7175 6172 6529 0a21 5b4c 696e 7578 2078  quare).![Linux x
-000004f0: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000500: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000510: 2f53 7570 706f 7274 2d4c 696e 7578 2532  /Support-Linux%2
-00000520: 3078 3634 2d62 6c75 653f 6c6f 676f 3d4c  0x64-blue?logo=L
-00000530: 696e 7578 2673 7479 6c65 3d66 6c61 742d  inux&style=flat-
-00000540: 7371 7561 7265 290a 5b21 5b63 6f64 6563  square).[![codec
-00000550: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
-00000560: 636f 762e 696f 2f67 682f 546f 6872 7573  cov.io/gh/Tohrus
-00000570: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-00000580: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
-00000590: 682f 6261 6467 652e 7376 673f 746f 6b65  h/badge.svg?toke
-000005a0: 6e3d 4232 544e 4b59 4e34 4f34 295d 2868  n=B2TNKYN4O4)](h
-000005b0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000005c0: 6f2f 6768 2f54 6f68 7275 736b 792f 4669  o/gh/Tohrusky/Fi
-000005d0: 6e61 6c32 782d 636f 7265 290a 5b21 5b43  nal2x-core).[![C
-000005e0: 492d 7465 7374 5d28 6874 7470 733a 2f2f  I-test](https://
-000005f0: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-00000600: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-00000610: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000620: 7773 2f43 492d 7465 7374 2e79 6d6c 2f62  ws/CI-test.yml/b
-00000630: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00000640: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00000650: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
-00000660: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
-00000670: 666c 6f77 732f 4349 2d74 6573 742e 796d  flows/CI-test.ym
-00000680: 6c29 0a5b 215b 4349 2d62 7569 6c64 5d28  l).[![CI-build](
-00000690: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006a0: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
-000006b0: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
-000006c0: 2f77 6f72 6b66 6c6f 7773 2f43 492d 6275  /workflows/CI-bu
-000006d0: 696c 642e 796d 6c2f 6261 6467 652e 7376  ild.yml/badge.sv
-000006e0: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-000006f0: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
-00000700: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
-00000710: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f43  ions/workflows/C
-00000720: 492d 6275 696c 642e 796d 6c29 0a5b 215b  I-build.yml).[![
-00000730: 5265 6c65 6173 655d 2868 7474 7073 3a2f  Release](https:/
-00000740: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
-00000750: 7573 6b79 2f46 696e 616c 3278 2d63 6f72  usky/Final2x-cor
-00000760: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-00000770: 6f77 732f 5265 6c65 6173 652e 796d 6c2f  ows/Release.yml/
-00000780: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00000790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000007a0: 6f68 7275 736b 792f 4669 6e61 6c32 782d  ohrusky/Final2x-
-000007b0: 636f 7265 2f61 6374 696f 6e73 2f77 6f72  core/actions/wor
-000007c0: 6b66 6c6f 7773 2f52 656c 6561 7365 2e79  kflows/Release.y
-000007d0: 6d6c 290a 5b21 5b50 4950 2d74 6573 745d  ml).[![PIP-test]
-000007e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007f0: 636f 6d2f 546f 6872 7573 6b79 2f46 696e  com/Tohrusky/Fin
-00000800: 616c 3278 2d63 6f72 652f 6163 7469 6f6e  al2x-core/action
-00000810: 732f 776f 726b 666c 6f77 732f 5049 502d  s/workflows/PIP-
-00000820: 7465 7374 2e79 6d6c 2f62 6164 6765 2e73  test.yml/badge.s
-00000830: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000840: 6875 622e 636f 6d2f 546f 6872 7573 6b79  hub.com/Tohrusky
-00000850: 2f46 696e 616c 3278 2d63 6f72 652f 6163  /Final2x-core/ac
-00000860: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000870: 5049 502d 7465 7374 2e79 6d6c 290a 5b21  PIP-test.yml).[!
-00000880: 5b52 656c 6561 7365 2d70 7970 695d 2868  [Release-pypi](h
-00000890: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000008a0: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-000008b0: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
-000008c0: 776f 726b 666c 6f77 732f 5265 6c65 6173  workflows/Releas
-000008d0: 652d 7079 7069 2e79 6d6c 2f62 6164 6765  e-pypi.yml/badge
-000008e0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-000008f0: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
-00000900: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-00000910: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000920: 732f 5265 6c65 6173 652d 7079 7069 2e79  s/Release-pypi.y
-00000930: 6d6c 290a 5b21 5b50 7950 4920 7665 7273  ml).[![PyPI vers
-00000940: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
-00000950: 6765 2e66 7572 792e 696f 2f70 792f 4669  ge.fury.io/py/Fi
-00000960: 6e61 6c32 782d 636f 7265 2e73 7667 295d  nal2x-core.svg)]
-00000970: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000980: 7572 792e 696f 2f70 792f 4669 6e61 6c32  ury.io/py/Final2
-00000990: 782d 636f 7265 290a 215b 4769 7448 7562  x-core).![GitHub
-000009a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000009b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000009c0: 6c69 6365 6e73 652f 546f 6872 7573 6b79  license/Tohrusky
-000009d0: 2f46 696e 616c 3278 2d63 6f72 6529 0a0a  /Final2x-core)..
-000009e0: 4669 6e61 6c32 782d 636f 7265 2069 7320  Final2x-core is 
-000009f0: 6120 6372 6f73 732d 706c 6174 666f 726d  a cross-platform
-00000a00: 2069 6d61 6765 2073 7570 6572 2d72 6573   image super-res
-00000a10: 6f6c 7574 696f 6e20 434c 4920 746f 6f6c  olution CLI tool
-00000a20: 2066 6f72 205b 4669 6e61 6c32 785d 2868   for [Final2x](h
-00000a30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a40: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-00000a50: 3278 292e 2049 6620 796f 7520 6861 7665  2x). If you have
-00000a60: 2061 6e79 2071 7565 7374 696f 6e73 2c20   any questions, 
-00000a70: 706c 6561 7365 2072 6169 7365 2061 6e20  please raise an 
-00000a80: 6973 7375 6520 5b69 6e20 7468 6973 2072  issue [in this r
-00000a90: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-00000aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00000ab0: 6872 7573 6b79 2f46 696e 616c 3278 292e  hrusky/Final2x).
-00000ac0: 0a0a 2320 496e 7374 616c 6c0a 0a44 6f77  ..# Install..Dow
-00000ad0: 6e6c 6f61 6420 696e 205b 5265 6c65 6173  nload in [Releas
-00000ae0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000af0: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
-00000b00: 696e 616c 3278 2d63 6f72 652f 7265 6c65  inal2x-core/rele
-00000b10: 6173 6573 2920 6f72 2075 7365 2070 6970  ases) or use pip
-00000b20: 2028 7079 7468 6f6e 203e 3d20 332e 362c   (python >= 3.6,
-00000b30: 203e 3d33 2e39 2066 6f72 204d 6163 4f53   >=3.9 for MacOS
-00000b40: 0a61 726d 3634 290a 0a60 6060 7368 656c  .arm64)..```shel
-00000b50: 6c0a 7069 7020 696e 7374 616c 6c20 4669  l.pip install Fi
-00000b60: 6e61 6c32 782d 636f 7265 0a60 6060 0a0a  nal2x-core.```..
-00000b70: 2320 5573 650a 0a60 6060 7368 656c 6c0a  # Use..```shell.
-00000b80: 7573 6167 653a 2046 696e 616c 3278 2d63  usage: Final2x-c
-00000b90: 6f72 6520 5b2d 685d 205b 2d62 2042 4153  ore [-h] [-b BAS
-00000ba0: 4536 345d 205b 2d6a 204a 534f 4e5d 205b  E64] [-j JSON] [
-00000bb0: 2d79 2059 414d 4c5d 205b 2d6f 5d0a 0a77  -y YAML] [-o]..w
-00000bc0: 6865 6e20 7061 7261 2069 7320 6e6f 7420  hen para is not 
-00000bd0: 7370 6563 6966 6965 642c 2074 6865 2063  specified, the c
-00000be0: 6f6e 6669 672e 7961 6d6c 2066 696c 6520  onfig.yaml file 
-00000bf0: 696e 2074 6865 2064 6972 6563 746f 7279  in the directory
-00000c00: 2077 696c 6c20 6265 2072 6561 6420 6175   will be read au
-00000c10: 746f 6d61 7469 6361 6c6c 790a 0a6f 7074  tomatically..opt
-00000c20: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
-00000c30: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
-00000c40: 2020 2020 2020 2020 2073 686f 7720 7468           show th
-00000c50: 6973 2068 656c 7020 6d65 7373 6167 6520  is help message 
-00000c60: 616e 6420 6578 6974 0a20 202d 6220 4241  and exit.  -b BA
-00000c70: 5345 3634 2c20 2d2d 4241 5345 3634 2042  SE64, --BASE64 B
-00000c80: 4153 4536 340a 2020 2020 2020 2020 2020  ASE64.          
-00000c90: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00000ca0: 7365 3634 2073 7472 696e 6720 666f 7220  se64 string for 
-00000cb0: 636f 6e66 6967 206a 736f 6e0a 2020 2d6a  config json.  -j
-00000cc0: 204a 534f 4e2c 202d 2d4a 534f 4e20 4a53   JSON, --JSON JS
-00000cd0: 4f4e 2020 4a53 4f4e 2073 7472 696e 6720  ON  JSON string 
-00000ce0: 666f 7220 636f 6e66 6967 0a20 202d 7920  for config.  -y 
-00000cf0: 5941 4d4c 2c20 2d2d 5941 4d4c 2059 414d  YAML, --YAML YAM
-00000d00: 4c20 2079 616d 6c20 636f 6e66 6967 2066  L  yaml config f
-00000d10: 696c 6520 7061 7468 0a20 202d 6c2c 202d  ile path.  -l, -
-00000d20: 2d4c 4f47 2020 2020 2020 2020 2020 2020  -LOG            
-00000d30: 2073 6176 6520 6c6f 670a 2020 2d6f 2c20   save log.  -o, 
-00000d40: 2d2d 4f50 2020 2020 2020 2020 2020 2020  --OP            
-00000d50: 2020 6368 6563 6b20 696e 7374 616c 6c0a    check install.
-00000d60: 6060 600a 0a23 2043 6f6e 6669 670a 0a50  ```..# Config..P
-00000d70: 6173 7320 7468 6520 636f 6e66 6967 206a  ass the config j
-00000d80: 736f 6e20 7374 7269 6e67 2074 6f20 7468  son string to th
-00000d90: 6520 7072 6f67 7261 6d20 7468 726f 7567  e program throug
-00000da0: 6820 7468 6520 602d 6a60 2070 6172 616d  h the `-j` param
-00000db0: 6574 6572 2e0a 0a2a 2a50 4c45 4153 4520  eter...**PLEASE 
-00000dc0: 4e4f 5445 3a20 7468 6520 636f 6e66 6967  NOTE: the config
-00000dd0: 2069 7320 4a53 4f4e 2c20 7265 6d6f 7665   is JSON, remove
-00000de0: 2074 6865 202f 2f20 636f 6d6d 656e 7473   the // comments
-00000df0: 2062 6566 6f72 6520 7573 652e 2a2a 0a0a   before use.**..
-00000e00: 6060 606a 736f 6e0a 7b0a 2020 2267 7075  ```json.{.  "gpu
-00000e10: 6964 223a 2030 2c0a 2020 2f2f 2047 5055  id": 0,.  // GPU
-00000e20: 2069 642c 203e 3d20 2d31 2028 2d31 2066   id, >= -1 (-1 f
-00000e30: 6f72 2043 5055 2c20 6d61 7920 6e6f 7420  or CPU, may not 
-00000e40: 776f 726b 2066 6f72 2073 6f6d 6520 6d6f  work for some mo
-00000e50: 6465 6c73 2e29 0a20 2022 696e 7075 7470  dels.).  "inputp
-00000e60: 6174 6822 3a20 5b0a 2020 2020 2f2f 2049  ath": [.    // I
-00000e70: 6e70 7574 2069 6d61 6765 2070 6174 6873  nput image paths
-00000e80: 2c20 7368 6f75 6c64 2062 6520 6120 6c69  , should be a li
-00000e90: 7374 2e0a 2020 2020 2270 6174 682f 746f  st..    "path/to
-00000ea0: 2f69 6d67 312e 6a70 6722 2c0a 2020 2020  /img1.jpg",.    
-00000eb0: 2270 6174 682f 746f 2f69 6d67 322e 706e  "path/to/img2.pn
-00000ec0: 6722 0a20 205d 2c0a 2020 226d 6f64 656c  g".  ],.  "model
-00000ed0: 223a 2022 5265 616c 4355 4741 4e2d 7072  ": "RealCUGAN-pr
-00000ee0: 6f22 2c0a 2020 2f2f 206d 6f64 656c 206e  o",.  // model n
-00000ef0: 616d 650a 2020 226d 6f64 656c 7363 616c  ame.  "modelscal
-00000f00: 6522 3a20 322c 0a20 202f 2f20 6d6f 6465  e": 2,.  // mode
-00000f10: 6c20 7570 7363 616c 6520 6661 6374 6f72  l upscale factor
-00000f20: 0a20 2022 6d6f 6465 6c6e 6f69 7365 223a  .  "modelnoise":
-00000f30: 202d 312c 0a20 202f 2f20 4445 4e4f 4953   -1,.  // DENOIS
-00000f40: 4520 6c65 7665 6c0a 2020 226f 7574 7075  E level.  "outpu
-00000f50: 7470 6174 6822 3a20 2270 6174 682f 746f  tpath": "path/to
-00000f60: 2f6f 7574 7075 7422 2c0a 2020 2f2f 206f  /output",.  // o
-00000f70: 7574 7075 7420 7061 7468 0a20 2022 7461  utput path.  "ta
-00000f80: 7267 6574 7363 616c 6522 3a20 322e 302c  rgetscale": 2.0,
-00000f90: 0a20 202f 2f20 5461 7267 6574 2075 7073  .  // Target ups
-00000fa0: 6361 6c65 2066 6163 746f 722c 2075 7073  cale factor, ups
-00000fb0: 6361 6c65 206d 756c 7469 706c 6520 7469  cale multiple ti
-00000fc0: 6d65 7320 746f 2061 6368 6965 7665 2074  mes to achieve t
-00000fd0: 6865 2074 6172 6765 7420 7570 7363 616c  he target upscal
-00000fe0: 6520 6661 6374 6f72 2e0a 2020 2f2f 2049  e factor..  // I
-00000ff0: 6620 6e6f 7420 696e 7661 6c69 642c 2075  f not invalid, u
-00001000: 7365 206d 6f64 656c 7363 616c 652e 0a20  se modelscale.. 
-00001010: 2022 7474 6122 3a20 6661 6c73 650a 2020   "tta": false.  
-00001020: 2f2f 2054 6573 7420 5469 6d65 2041 7567  // Test Time Aug
-00001030: 6d65 6e74 6174 696f 6e2c 2064 6566 6175  mentation, defau
-00001040: 6c74 2066 616c 7365 0a7d 0a60 6060 0a0a  lt false.}.```..
-00001050: 2a2a 5355 5050 4f52 5445 4420 4d4f 4445  **SUPPORTED MODE
-00001060: 4c20 4c49 5354 3a2a 2a0a 0a60 6060 7961  L LIST:**..```ya
-00001070: 6d6c 0a2d 2052 6561 6c43 5547 414e 2d73  ml.- RealCUGAN-s
-00001080: 653a 0a20 2020 202d 206d 6f64 656c 3a20  e:.    - model: 
-00001090: 2252 6561 6c43 5547 414e 2d73 6522 0a20  "RealCUGAN-se". 
-000010a0: 2020 202d 2073 6361 6c65 3a20 320a 2020     - scale: 2.  
-000010b0: 2020 2020 2020 2020 2020 2020 202d 206e               - n
-000010c0: 6f69 7365 3a20 2d31 2c20 302c 2031 2c20  oise: -1, 0, 1, 
-000010d0: 322c 2033 0a20 2020 202d 2073 6361 6c65  2, 3.    - scale
-000010e0: 3a20 332c 2034 0a20 2020 2020 2020 2020  : 3, 4.         
-000010f0: 2020 2020 2020 2d20 6e6f 6973 653a 202d        - noise: -
-00001100: 312c 2030 2c20 330a 0a2d 2052 6561 6c43  1, 0, 3..- RealC
-00001110: 5547 414e 2d70 726f 3a0a 2020 2020 2d20  UGAN-pro:.    - 
-00001120: 6d6f 6465 6c3a 2022 5265 616c 4355 4741  model: "RealCUGA
-00001130: 4e2d 7072 6f22 0a20 2020 202d 2073 6361  N-pro".    - sca
-00001140: 6c65 3a20 322c 2033 0a20 2020 202d 206e  le: 2, 3.    - n
-00001150: 6f69 7365 3a20 2d31 2c20 302c 2033 0a0a  oise: -1, 0, 3..
-00001160: 2d20 5265 616c 4553 5247 414e 2d61 6e69  - RealESRGAN-ani
-00001170: 6d65 7669 6465 6f76 333a 0a20 2020 202d  mevideov3:.    -
-00001180: 2067 7075 6964 3a20 3e3d 2030 0a20 2020   gpuid: >= 0.   
-00001190: 202d 206d 6f64 656c 3a20 2252 6561 6c45   - model: "RealE
-000011a0: 5352 4741 4e2d 616e 696d 6576 6964 656f  SRGAN-animevideo
-000011b0: 7633 220a 2020 2020 2d20 7363 616c 653a  v3".    - scale:
-000011c0: 2032 2c20 332c 2034 0a0a 2d20 5265 616c   2, 3, 4..- Real
-000011d0: 4553 5247 414e 3a0a 2020 2020 2d20 6770  ESRGAN:.    - gp
-000011e0: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-000011f0: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00001200: 414e 220a 2020 2020 2d20 7363 616c 653a  AN".    - scale:
-00001210: 2034 0a0a 2d20 5265 616c 4553 5247 414e   4..- RealESRGAN
-00001220: 2d61 6e69 6d65 3a0a 2020 2020 2d20 6770  -anime:.    - gp
-00001230: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-00001240: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00001250: 414e 2d61 6e69 6d65 220a 2020 2020 2d20  AN-anime".    - 
-00001260: 7363 616c 653a 2034 0a0a 2d20 5761 6966  scale: 4..- Waif
-00001270: 7532 782d 6375 6e65 743a 0a20 2020 202d  u2x-cunet:.    -
-00001280: 206d 6f64 656c 3a20 2257 6169 6675 3278   model: "Waifu2x
-00001290: 2d63 756e 6574 220a 2020 2020 2d20 7363  -cunet".    - sc
-000012a0: 616c 653a 2031 0a20 2020 2020 2020 2020  ale: 1.         
-000012b0: 2020 2020 2020 2d20 6e6f 6973 653a 2030        - noise: 0
-000012c0: 2c20 312c 2032 2c20 330a 2020 2020 2d20  , 1, 2, 3.    - 
-000012d0: 7363 616c 653a 2032 0a20 2020 2020 2020  scale: 2.       
-000012e0: 2020 2020 2020 2020 2d20 6e6f 6973 653a          - noise:
-000012f0: 202d 312c 2030 2c20 312c 2032 2c20 330a   -1, 0, 1, 2, 3.
-00001300: 0a2d 2057 6169 6675 3278 2d75 7063 6f6e  .- Waifu2x-upcon
-00001310: 765f 375f 616e 696d 655f 7374 796c 655f  v_7_anime_style_
-00001320: 6172 745f 7267 623a 0a20 2020 202d 206d  art_rgb:.    - m
-00001330: 6f64 656c 3a20 2257 6169 6675 3278 2d75  odel: "Waifu2x-u
-00001340: 7063 6f6e 765f 375f 616e 696d 655f 7374  pconv_7_anime_st
-00001350: 796c 655f 6172 745f 7267 6222 0a20 2020  yle_art_rgb".   
-00001360: 202d 2073 6361 6c65 3a20 320a 2020 2020   - scale: 2.    
-00001370: 2d20 6e6f 6973 653a 202d 312c 2030 2c20  - noise: -1, 0, 
-00001380: 312c 2032 2c20 330a 0a2d 2057 6169 6675  1, 2, 3..- Waifu
-00001390: 3278 2d75 7063 6f6e 765f 375f 7068 6f74  2x-upconv_7_phot
-000013a0: 6f3a 0a20 2020 202d 206d 6f64 656c 3a20  o:.    - model: 
-000013b0: 2257 6169 6675 3278 2d75 7063 6f6e 765f  "Waifu2x-upconv_
-000013c0: 375f 7068 6f74 6f22 0a20 2020 202d 2073  7_photo".    - s
-000013d0: 6361 6c65 3a20 320a 2020 2020 2d20 6e6f  cale: 2.    - no
-000013e0: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-000013f0: 2c20 330a 0a2d 2053 524d 443a 0a20 2020  , 3..- SRMD:.   
-00001400: 202d 2067 7075 6964 3a20 3e3d 2030 0a20   - gpuid: >= 0. 
-00001410: 2020 202d 206d 6f64 656c 3a20 2253 524d     - model: "SRM
-00001420: 4422 0a20 2020 202d 2073 6361 6c65 3a20  D".    - scale: 
-00001430: 322c 2033 2c20 340a 2020 2020 2d20 6e6f  2, 3, 4.    - no
-00001440: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-00001450: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-00001460: 2038 2c20 392c 2031 300a 6060 600a 0a23   8, 9, 10.```..#
-00001470: 2042 7569 6c64 0a0a 5b47 6974 6875 6220   Build..[Github 
-00001480: 4163 7469 6f6e 5d28 6874 7470 733a 2f2f  Action](https://
-00001490: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-000014a0: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-000014b0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000014c0: 7773 2f43 492d 6275 696c 642e 796d 6c29  ws/CI-build.yml)
-000014d0: 0a0a 2a54 6865 2070 726f 6a65 6374 206a  ..*The project j
-000014e0: 7573 7420 6f6e 6c79 2062 6565 6e20 7465  ust only been te
-000014f0: 7374 6564 2069 6e20 5562 756e 7475 2031  sted in Ubuntu 1
-00001500: 382b 2061 6e64 2044 6562 6961 6e20 392b  8+ and Debian 9+
-00001510: 2065 6e76 6972 6f6e 6d65 6e74 7320 6f6e   environments on
-00001520: 204c 696e 7578 2c20 736f 2069 6620 7468   Linux, so if th
-00001530: 6520 7072 6f6a 6563 7420 646f 6573 206e  e project does n
-00001540: 6f74 2077 6f72 6b20 6f6e 0a79 6f75 7220  ot work on.your 
-00001550: 7379 7374 656d 2c20 706c 6561 7365 2074  system, please t
-00001560: 7279 2062 7569 6c64 696e 6720 6974 2e2a  ry building it.*
-00001570: 0a0a 2320 5265 6665 7265 6e63 650a 0a54  ..# Reference..T
-00001580: 6865 2066 6f6c 6c6f 7769 6e67 2072 6566  he following ref
-00001590: 6572 656e 6365 7320 7765 7265 2075 7365  erences were use
-000015a0: 6420 696e 2074 6865 2064 6576 656c 6f70  d in the develop
-000015b0: 6d65 6e74 206f 6620 7468 6973 2070 726f  ment of this pro
-000015c0: 6a65 6374 3a0a 0a2d 205b 6e63 6e6e 5d28  ject:..- [ncnn](
-000015d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000015e0: 6f6d 2f54 656e 6365 6e74 2f6e 636e 6e29  om/Tencent/ncnn)
-000015f0: 202d 206e 636e 6e20 6973 2061 2068 6967   - ncnn is a hig
-00001600: 682d 7065 7266 6f72 6d61 6e63 6520 6e65  h-performance ne
-00001610: 7572 616c 206e 6574 776f 726b 2069 6e66  ural network inf
-00001620: 6572 656e 6365 2066 7261 6d65 776f 726b  erence framework
-00001630: 2064 6576 656c 6f70 6564 2062 790a 2020   developed by.  
-00001640: 5465 6e63 656e 7420 4149 204c 6162 2e0a  Tencent AI Lab..
-00001650: 2d20 5b6e 6968 7569 2f72 6561 6c63 7567  - [nihui/realcug
-00001660: 616e 2d6e 636e 6e2d 7675 6c6b 616e 5d28  an-ncnn-vulkan](
-00001670: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001680: 6f6d 2f6e 6968 7569 2f72 6561 6c63 7567  om/nihui/realcug
-00001690: 616e 2d6e 636e 6e2d 7675 6c6b 616e 2920  an-ncnn-vulkan) 
-000016a0: 2d20 5468 6973 2070 726f 6a65 6374 2070  - This project p
-000016b0: 726f 7669 6465 6420 7468 6520 636f 7265  rovided the core
-000016c0: 0a20 2069 6d70 6c65 6d65 6e74 6174 696f  .  implementatio
-000016d0: 6e20 6f66 2074 6865 2052 6561 6c2d 4355  n of the Real-CU
-000016e0: 4741 4e20 616c 676f 7269 7468 6d20 7573  GAN algorithm us
-000016f0: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
-00001700: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
-00001710: 732e 0a2d 205b 7869 6e6e 7461 6f2f 5265  s..- [xinntao/Re
-00001720: 616c 2d45 5352 4741 4e2d 6e63 6e6e 2d76  al-ESRGAN-ncnn-v
-00001730: 756c 6b61 6e5d 2868 7474 7073 3a2f 2f67  ulkan](https://g
-00001740: 6974 6875 622e 636f 6d2f 7869 6e6e 7461  ithub.com/xinnta
-00001750: 6f2f 5265 616c 2d45 5352 4741 4e2d 6e63  o/Real-ESRGAN-nc
-00001760: 6e6e 2d76 756c 6b61 6e29 202d 2054 6869  nn-vulkan) - Thi
-00001770: 7320 7072 6f6a 6563 7420 7072 6f76 6964  s project provid
-00001780: 6564 2074 6865 2063 6f72 650a 2020 696d  ed the core.  im
-00001790: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-000017a0: 7468 6520 5265 616c 2d45 5352 4741 4e20  the Real-ESRGAN 
-000017b0: 616c 676f 7269 7468 6d20 7573 696e 6720  algorithm using 
-000017c0: 7468 6520 6e63 6e6e 2061 6e64 2056 756c  the ncnn and Vul
-000017d0: 6b61 6e0a 2020 6c69 6272 6172 6965 732e  kan.  libraries.
-000017e0: 0a2d 205b 6e69 6875 692f 7761 6966 7532  .- [nihui/waifu2
-000017f0: 782d 6e63 6e6e 2d76 756c 6b61 6e5d 2868  x-ncnn-vulkan](h
-00001800: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001810: 6d2f 6e69 6875 692f 7761 6966 7532 782d  m/nihui/waifu2x-
-00001820: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
-00001830: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
-00001840: 6964 6564 2074 6865 2063 6f72 650a 2020  ided the core.  
-00001850: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00001860: 6620 7468 6520 5761 6966 7532 7820 616c  f the Waifu2x al
-00001870: 676f 7269 7468 6d20 7573 696e 6720 7468  gorithm using th
-00001880: 6520 6e63 6e6e 2061 6e64 2056 756c 6b61  e ncnn and Vulka
-00001890: 6e20 6c69 6272 6172 6965 732e 0a2d 205b  n libraries..- [
-000018a0: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
-000018b0: 7675 6c6b 616e 5d28 6874 7470 733a 2f2f  vulkan](https://
-000018c0: 6769 7468 7562 2e63 6f6d 2f6e 6968 7569  github.com/nihui
-000018d0: 2f73 726d 642d 6e63 6e6e 2d76 756c 6b61  /srmd-ncnn-vulka
-000018e0: 6e29 202d 2054 6869 7320 7072 6f6a 6563  n) - This projec
-000018f0: 7420 7072 6f76 6964 6564 2074 6865 2063  t provided the c
-00001900: 6f72 6520 696d 706c 656d 656e 7461 7469  ore implementati
-00001910: 6f6e 206f 660a 2020 7468 6520 5352 4d44  on of.  the SRMD
-00001920: 2061 6c67 6f72 6974 686d 2075 7369 6e67   algorithm using
-00001930: 2074 6865 206e 636e 6e20 616e 6420 5675   the ncnn and Vu
-00001940: 6c6b 616e 206c 6962 7261 7269 6573 2e0a  lkan libraries..
-00001950: 2d20 5b72 6561 6c63 7567 616e 2d6e 636e  - [realcugan-ncn
-00001960: 6e2d 7079 5d28 6874 7470 733a 2f2f 6769  n-py](https://gi
-00001970: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
-00001980: 792f 7265 616c 6375 6761 6e2d 6e63 6e6e  y/realcugan-ncnn
-00001990: 2d70 7929 202d 2054 6869 7320 7072 6f6a  -py) - This proj
-000019a0: 6563 7420 7072 6f76 6964 6564 2074 6865  ect provided the
-000019b0: 2050 7974 686f 6e20 4269 6e64 696e 6720   Python Binding 
-000019c0: 666f 720a 2020 7265 616c 6375 6761 6e2d  for.  realcugan-
-000019d0: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
-000019e0: 2050 7942 696e 6431 310a 2d20 5b72 6561   PyBind11.- [rea
-000019f0: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 795d  lesrgan-ncnn-py]
-00001a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001a10: 636f 6d2f 546f 6872 7573 6b79 2f72 6561  com/Tohrusky/rea
-00001a20: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 7929  lesrgan-ncnn-py)
-00001a30: 202d 2054 6869 7320 7072 6f6a 6563 7420   - This project 
-00001a40: 7072 6f76 6964 6564 2074 6865 2050 7974  provided the Pyt
-00001a50: 686f 6e20 4269 6e64 696e 6720 666f 720a  hon Binding for.
-00001a60: 2020 7265 616c 6573 7267 616e 2d6e 636e    realesrgan-ncn
-00001a70: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
-00001a80: 4269 6e64 3131 0a2d 205b 7761 6966 7532  Bind11.- [waifu2
-00001a90: 782d 6e63 6e6e 2d70 795d 2868 7474 7073  x-ncnn-py](https
-00001aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00001ab0: 6872 7573 6b79 2f77 6169 6675 3278 2d6e  hrusky/waifu2x-n
-00001ac0: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
-00001ad0: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
-00001ae0: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
-00001af0: 6e67 2066 6f72 0a20 2077 6169 6675 3278  ng for.  waifu2x
-00001b00: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
-00001b10: 6820 5079 4269 6e64 3131 0a2d 205b 7372  h PyBind11.- [sr
-00001b20: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
-00001b30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00001b40: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
-00001b50: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
-00001b60: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
-00001b70: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
-00001b80: 2066 6f72 0a20 2073 726d 642d 6e63 6e6e   for.  srmd-ncnn
-00001b90: 2d76 756c 6b61 6e0a 2020 7769 7468 2050  -vulkan.  with P
-00001ba0: 7942 696e 6431 310a 0a23 204c 6963 656e  yBind11..# Licen
-00001bb0: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00001bc0: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00001bd0: 6572 2074 6865 2042 5344 2033 2d43 6c61  er the BSD 3-Cla
-00001be0: 7573 6520 2d20 7365 650a 7468 6520 5b4c  use - see.the [L
-00001bf0: 4943 454e 5345 2066 696c 655d 2868 7474  ICENSE file](htt
-00001c00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001c10: 546f 6872 7573 6b79 2f46 696e 616c 3278  Tohrusky/Final2x
-00001c20: 2d63 6f72 652f 626c 6f62 2f6d 6169 6e2f  -core/blob/main/
-00001c30: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
-00001c40: 6169 6c73 2e0a 0a0a                      ails....
+000002c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002d0: 2f73 6f63 6961 6c69 6679 2e67 6974 2e63  /socialify.git.c
+000002e0: 692f 546f 6872 7573 6b79 2f46 696e 616c  i/Tohrusky/Final
+000002f0: 3278 2d63 6f72 652f 696d 6167 653f 6465  2x-core/image?de
+00000300: 7363 7269 7074 696f 6e3d 3126 666f 726b  scription=1&fork
+00000310: 733d 3126 6973 7375 6573 3d31 266c 616e  s=1&issues=1&lan
+00000320: 6775 6167 653d 3126 6c6f 676f 3d68 7474  guage=1&logo=htt
+00000330: 7073 2533 4125 3246 2532 4672 6177 2e67  ps%3A%2F%2Fraw.g
+00000340: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000350: 2e63 6f6d 2532 4654 6f68 7275 736b 7925  .com%2FTohrusky%
+00000360: 3246 546f 6872 7573 6b79 2532 466d 6169  2FTohrusky%2Fmai
+00000370: 6e25 3246 6963 6f6e 2532 466c 6f67 6f2e  n%2Ficon%2Flogo.
+00000380: 706e 6726 6e61 6d65 3d31 2670 6174 7465  png&name=1&patte
+00000390: 726e 3d43 6972 6375 6974 2532 3042 6f61  rn=Circuit%20Boa
+000003a0: 7264 2670 756c 6c73 3d31 2673 7461 7267  rd&pulls=1&starg
+000003b0: 617a 6572 733d 3126 7468 656d 653d 4c69  azers=1&theme=Li
+000003c0: 6768 7422 3e0a 2020 3c70 6963 7475 7265  ght">.  <picture
+000003d0: 3e0a 2020 2020 3c73 6f75 7263 6520 6d65  >.    <source me
+000003e0: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
+000003f0: 6c6f 722d 7363 6865 6d65 3a20 6461 726b  lor-scheme: dark
+00000400: 2922 2073 7263 7365 743d 2268 7474 7073  )" srcset="https
+00000410: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+00000420: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+00000430: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+00000440: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+00000450: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+00000460: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+00000470: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+00000480: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000490: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+000004a0: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+000004b0: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+000004c0: 6f2d 6461 726b 2e70 6e67 266e 616d 653d  o-dark.png&name=
+000004d0: 3126 7061 7474 6572 6e3d 4369 7263 7569  1&pattern=Circui
+000004e0: 7425 3230 426f 6172 6426 7075 6c6c 733d  t%20Board&pulls=
+000004f0: 3126 7374 6172 6761 7a65 7273 3d31 2674  1&stargazers=1&t
+00000500: 6865 6d65 3d44 6172 6b22 202f 3e0a 2020  heme=Dark" />.  
+00000510: 2020 3c73 6f75 7263 6520 6d65 6469 613d    <source media=
+00000520: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
+00000530: 7363 6865 6d65 3a20 6c69 6768 7429 2220  scheme: light)" 
+00000540: 7372 6373 6574 3d22 6874 7470 733a 2f2f  srcset="https://
+00000550: 736f 6369 616c 6966 792e 6769 742e 6369  socialify.git.ci
+00000560: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000570: 782d 636f 7265 2f69 6d61 6765 3f64 6573  x-core/image?des
+00000580: 6372 6970 7469 6f6e 3d31 2666 6f72 6b73  cription=1&forks
+00000590: 3d31 2669 7373 7565 733d 3126 6c61 6e67  =1&issues=1&lang
+000005a0: 7561 6765 3d31 266c 6f67 6f3d 6874 7470  uage=1&logo=http
+000005b0: 7325 3341 2532 4625 3246 7261 772e 6769  s%3A%2F%2Fraw.gi
+000005c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000005d0: 636f 6d25 3246 546f 6872 7573 6b79 2532  com%2FTohrusky%2
+000005e0: 4654 6f68 7275 736b 7925 3246 6d61 696e  FTohrusky%2Fmain
+000005f0: 2532 4669 636f 6e25 3246 6c6f 676f 2e70  %2Ficon%2Flogo.p
+00000600: 6e67 266e 616d 653d 3126 7061 7474 6572  ng&name=1&patter
+00000610: 6e3d 4369 7263 7569 7425 3230 426f 6172  n=Circuit%20Boar
+00000620: 6426 7075 6c6c 733d 3126 7374 6172 6761  d&pulls=1&starga
+00000630: 7a65 7273 3d31 2674 6865 6d65 3d4c 6967  zers=1&theme=Lig
+00000640: 6874 2220 2f3e 0a20 2020 203c 696d 6720  ht" />.    <img 
+00000650: 616c 743d 2253 6f63 6961 6c69 6679 2049  alt="Socialify I
+00000660: 6d61 6765 2220 7372 633d 2268 7474 7073  mage" src="https
+00000670: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+00000680: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+00000690: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+000006a0: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+000006b0: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+000006c0: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+000006d0: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+000006e0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000006f0: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+00000700: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+00000710: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+00000720: 6f2e 706e 6726 6e61 6d65 3d31 2670 6174  o.png&name=1&pat
+00000730: 7465 726e 3d43 6972 6375 6974 2532 3042  tern=Circuit%20B
+00000740: 6f61 7264 2670 756c 6c73 3d31 2673 7461  oard&pulls=1&sta
+00000750: 7267 617a 6572 733d 3126 7468 656d 653d  rgazers=1&theme=
+00000760: 4c69 6768 7422 202f 3e0a 2020 3c2f 7069  Light" />.  </pi
+00000770: 6374 7572 653e 0a3c 2f61 3e0a 0a0a 215b  cture>.</a>...![
+00000780: 4d61 634f 5320 7836 345d 2868 7474 7073  MacOS x64](https
+00000790: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000007a0: 6f2f 6261 6467 652f 5375 7070 6f72 742d  o/badge/Support-
+000007b0: 4d61 634f 5325 3230 7836 342d 626c 7565  MacOS%20x64-blue
+000007c0: 3f6c 6f67 6f3d 4170 706c 6526 7374 796c  ?logo=Apple&styl
+000007d0: 653d 666c 6174 2d73 7175 6172 6529 0a21  e=flat-square).!
+000007e0: 5b4d 6163 4f53 2061 726d 3634 5d28 6874  [MacOS arm64](ht
+000007f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000800: 732e 696f 2f62 6164 6765 2f53 7570 706f  s.io/badge/Suppo
+00000810: 7274 2d4d 6163 4f53 2532 3061 726d 3634  rt-MacOS%20arm64
+00000820: 2d62 6c75 653f 6c6f 676f 3d41 7070 6c65  -blue?logo=Apple
+00000830: 2673 7479 6c65 3d66 6c61 742d 7371 7561  &style=flat-squa
+00000840: 7265 290a 215b 5769 6e64 6f77 7320 7836  re).![Windows x6
+00000850: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+00000860: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000870: 5375 7070 6f72 742d 5769 6e64 6f77 7325  Support-Windows%
+00000880: 3230 7836 342d 626c 7565 3f6c 6f67 6f3d  20x64-blue?logo=
+00000890: 5769 6e64 6f77 7326 7374 796c 653d 666c  Windows&style=fl
+000008a0: 6174 2d73 7175 6172 6529 0a21 5b57 696e  at-square).![Win
+000008b0: 646f 7773 2061 726d 3634 5d28 6874 7470  dows arm64](http
+000008c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000008d0: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
+000008e0: 2d57 696e 646f 7773 2532 3061 726d 3634  -Windows%20arm64
+000008f0: 2d62 6c75 653f 6c6f 676f 3d57 696e 646f  -blue?logo=Windo
+00000900: 7773 2673 7479 6c65 3d66 6c61 742d 7371  ws&style=flat-sq
+00000910: 7561 7265 290a 215b 4c69 6e75 7820 7836  uare).![Linux x6
+00000920: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+00000930: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000940: 5375 7070 6f72 742d 4c69 6e75 7825 3230  Support-Linux%20
+00000950: 7836 342d 626c 7565 3f6c 6f67 6f3d 4c69  x64-blue?logo=Li
+00000960: 6e75 7826 7374 796c 653d 666c 6174 2d73  nux&style=flat-s
+00000970: 7175 6172 6529 0a5b 215b 636f 6465 636f  quare).[![codeco
+00000980: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000990: 6f76 2e69 6f2f 6768 2f54 6f68 7275 736b  ov.io/gh/Tohrusk
+000009a0: 792f 4669 6e61 6c32 782d 636f 7265 2f62  y/Final2x-core/b
+000009b0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+000009c0: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+000009d0: 3d42 3254 4e4b 594e 344f 3429 5d28 6874  =B2TNKYN4O4)](ht
+000009e0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000009f0: 2f67 682f 546f 6872 7573 6b79 2f46 696e  /gh/Tohrusky/Fin
+00000a00: 616c 3278 2d63 6f72 6529 0a5b 215b 4349  al2x-core).[![CI
+00000a10: 2d74 6573 745d 2868 7474 7073 3a2f 2f67  -test](https://g
+00000a20: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+00000a30: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+00000a40: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000a50: 732f 4349 2d74 6573 742e 796d 6c2f 6261  s/CI-test.yml/ba
+00000a60: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000a70: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00000a80: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+00000a90: 7265 2f61 6374 696f 6e73 2f77 6f72 6b66  re/actions/workf
+00000aa0: 6c6f 7773 2f43 492d 7465 7374 2e79 6d6c  lows/CI-test.yml
+00000ab0: 290a 5b21 5b43 492d 6275 696c 645d 2868  ).[![CI-build](h
+00000ac0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ad0: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
+00000ae0: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
+00000af0: 776f 726b 666c 6f77 732f 4349 2d62 7569  workflows/CI-bui
+00000b00: 6c64 2e79 6d6c 2f62 6164 6765 2e73 7667  ld.yml/badge.svg
+00000b10: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000b20: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
+00000b30: 696e 616c 3278 2d63 6f72 652f 6163 7469  inal2x-core/acti
+00000b40: 6f6e 732f 776f 726b 666c 6f77 732f 4349  ons/workflows/CI
+00000b50: 2d62 7569 6c64 2e79 6d6c 290a 5b21 5b52  -build.yml).[![R
+00000b60: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00000b70: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
+00000b80: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
+00000b90: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000ba0: 7773 2f52 656c 6561 7365 2e79 6d6c 2f62  ws/Release.yml/b
+00000bb0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000bc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00000bd0: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
+00000be0: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
+00000bf0: 666c 6f77 732f 5265 6c65 6173 652e 796d  flows/Release.ym
+00000c00: 6c29 0a5b 215b 5049 502d 7465 7374 5d28  l).[![PIP-test](
+00000c10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000c20: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
+00000c30: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
+00000c40: 2f77 6f72 6b66 6c6f 7773 2f50 4950 2d74  /workflows/PIP-t
+00000c50: 6573 742e 796d 6c2f 6261 6467 652e 7376  est.yml/badge.sv
+00000c60: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000c70: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
+00000c80: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
+00000c90: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f50  ions/workflows/P
+00000ca0: 4950 2d74 6573 742e 796d 6c29 0a5b 215b  IP-test.yml).[![
+00000cb0: 5265 6c65 6173 652d 7079 7069 5d28 6874  Release-pypi](ht
+00000cc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000cd0: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000ce0: 782d 636f 7265 2f61 6374 696f 6e73 2f77  x-core/actions/w
+00000cf0: 6f72 6b66 6c6f 7773 2f52 656c 6561 7365  orkflows/Release
+00000d00: 2d70 7970 692e 796d 6c2f 6261 6467 652e  -pypi.yml/badge.
+00000d10: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000d20: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
+00000d30: 792f 4669 6e61 6c32 782d 636f 7265 2f61  y/Final2x-core/a
+00000d40: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000d50: 2f52 656c 6561 7365 2d70 7970 692e 796d  /Release-pypi.ym
+00000d60: 6c29 0a5b 215b 5079 5049 2076 6572 7369  l).[![PyPI versi
+00000d70: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000d80: 652e 6675 7279 2e69 6f2f 7079 2f46 696e  e.fury.io/py/Fin
+00000d90: 616c 3278 2d63 6f72 652e 7376 6729 5d28  al2x-core.svg)](
+00000da0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000db0: 7279 2e69 6f2f 7079 2f46 696e 616c 3278  ry.io/py/Final2x
+00000dc0: 2d63 6f72 6529 0a21 5b47 6974 4875 625d  -core).![GitHub]
+00000dd0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000de0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000df0: 6963 656e 7365 2f54 6f68 7275 736b 792f  icense/Tohrusky/
+00000e00: 4669 6e61 6c32 782d 636f 7265 290a 0a46  Final2x-core)..F
+00000e10: 696e 616c 3278 2d63 6f72 6520 6973 2061  inal2x-core is a
+00000e20: 2063 726f 7373 2d70 6c61 7466 6f72 6d20   cross-platform 
+00000e30: 696d 6167 6520 7375 7065 722d 7265 736f  image super-reso
+00000e40: 6c75 7469 6f6e 2043 4c49 2074 6f6f 6c20  lution CLI tool 
+00000e50: 666f 7220 5b46 696e 616c 3278 5d28 6874  for [Final2x](ht
+00000e60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e70: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000e80: 7829 2e20 4966 2079 6f75 2068 6176 6520  x). If you have 
+00000e90: 616e 7920 7175 6573 7469 6f6e 732c 2070  any questions, p
+00000ea0: 6c65 6173 6520 7261 6973 6520 616e 2069  lease raise an i
+00000eb0: 7373 7565 205b 696e 2074 6869 7320 7265  ssue [in this re
+00000ec0: 706f 7369 746f 7279 5d28 6874 7470 733a  pository](https:
+00000ed0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00000ee0: 7275 736b 792f 4669 6e61 6c32 7829 2e0a  rusky/Final2x)..
+00000ef0: 0a23 2049 6e73 7461 6c6c 0a0a 446f 776e  .# Install..Down
+00000f00: 6c6f 6164 2069 6e20 5b52 656c 6561 7365  load in [Release
+00000f10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000f20: 2e63 6f6d 2f54 6f68 7275 736b 792f 4669  .com/Tohrusky/Fi
+00000f30: 6e61 6c32 782d 636f 7265 2f72 656c 6561  nal2x-core/relea
+00000f40: 7365 7329 206f 7220 7573 6520 7069 7020  ses) or use pip 
+00000f50: 2870 7974 686f 6e20 3e3d 2033 2e36 2c20  (python >= 3.6, 
+00000f60: 3e3d 332e 3920 666f 7220 4d61 634f 530a  >=3.9 for MacOS.
+00000f70: 6172 6d36 3429 0a0a 6060 6073 6865 6c6c  arm64)..```shell
+00000f80: 0a70 6970 2069 6e73 7461 6c6c 2046 696e  .pip install Fin
+00000f90: 616c 3278 2d63 6f72 650a 6060 600a 0a23  al2x-core.```..#
+00000fa0: 2055 7365 0a0a 6060 6073 6865 6c6c 0a75   Use..```shell.u
+00000fb0: 7361 6765 3a20 4669 6e61 6c32 782d 636f  sage: Final2x-co
+00000fc0: 7265 205b 2d68 5d20 5b2d 6220 4241 5345  re [-h] [-b BASE
+00000fd0: 3634 5d20 5b2d 6a20 4a53 4f4e 5d20 5b2d  64] [-j JSON] [-
+00000fe0: 7920 5941 4d4c 5d20 5b2d 6f5d 0a0a 7768  y YAML] [-o]..wh
+00000ff0: 656e 2070 6172 6120 6973 206e 6f74 2073  en para is not s
+00001000: 7065 6369 6669 6564 2c20 7468 6520 636f  pecified, the co
+00001010: 6e66 6967 2e79 616d 6c20 6669 6c65 2069  nfig.yaml file i
+00001020: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
+00001030: 7769 6c6c 2062 6520 7265 6164 2061 7574  will be read aut
+00001040: 6f6d 6174 6963 616c 6c79 0a0a 6f70 7469  omatically..opti
+00001050: 6f6e 616c 2061 7267 756d 656e 7473 3a0a  onal arguments:.
+00001060: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+00001070: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
+00001080: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
+00001090: 6e64 2065 7869 740a 2020 2d62 2042 4153  nd exit.  -b BAS
+000010a0: 4536 342c 202d 2d42 4153 4536 3420 4241  E64, --BASE64 BA
+000010b0: 5345 3634 0a20 2020 2020 2020 2020 2020  SE64.           
+000010c0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+000010d0: 6536 3420 7374 7269 6e67 2066 6f72 2063  e64 string for c
+000010e0: 6f6e 6669 6720 6a73 6f6e 0a20 202d 6a20  onfig json.  -j 
+000010f0: 4a53 4f4e 2c20 2d2d 4a53 4f4e 204a 534f  JSON, --JSON JSO
+00001100: 4e20 204a 534f 4e20 7374 7269 6e67 2066  N  JSON string f
+00001110: 6f72 2063 6f6e 6669 670a 2020 2d79 2059  or config.  -y Y
+00001120: 414d 4c2c 202d 2d59 414d 4c20 5941 4d4c  AML, --YAML YAML
+00001130: 2020 7961 6d6c 2063 6f6e 6669 6720 6669    yaml config fi
+00001140: 6c65 2070 6174 680a 2020 2d6c 2c20 2d2d  le path.  -l, --
+00001150: 4c4f 4720 2020 2020 2020 2020 2020 2020  LOG             
+00001160: 7361 7665 206c 6f67 0a20 202d 6f2c 202d  save log.  -o, -
+00001170: 2d4f 5020 2020 2020 2020 2020 2020 2020  -OP             
+00001180: 2063 6865 636b 2069 6e73 7461 6c6c 0a60   check install.`
+00001190: 6060 0a0a 2320 436f 6e66 6967 0a0a 5061  ``..# Config..Pa
+000011a0: 7373 2074 6865 2063 6f6e 6669 6720 6a73  ss the config js
+000011b0: 6f6e 2073 7472 696e 6720 746f 2074 6865  on string to the
+000011c0: 2070 726f 6772 616d 2074 6872 6f75 6768   program through
+000011d0: 2074 6865 2060 2d6a 6020 7061 7261 6d65   the `-j` parame
+000011e0: 7465 722e 0a0a 2a2a 504c 4541 5345 204e  ter...**PLEASE N
+000011f0: 4f54 453a 2074 6865 2063 6f6e 6669 6720  OTE: the config 
+00001200: 6973 204a 534f 4e2c 2072 656d 6f76 6520  is JSON, remove 
+00001210: 7468 6520 2f2f 2063 6f6d 6d65 6e74 7320  the // comments 
+00001220: 6265 666f 7265 2075 7365 2e2a 2a0a 0a60  before use.**..`
+00001230: 6060 6a73 6f6e 0a7b 0a20 2022 6770 7569  ``json.{.  "gpui
+00001240: 6422 3a20 302c 0a20 202f 2f20 4750 5520  d": 0,.  // GPU 
+00001250: 6964 2c20 3e3d 202d 3120 282d 3120 666f  id, >= -1 (-1 fo
+00001260: 7220 4350 552c 206d 6179 206e 6f74 2077  r CPU, may not w
+00001270: 6f72 6b20 666f 7220 736f 6d65 206d 6f64  ork for some mod
+00001280: 656c 732e 290a 2020 2269 6e70 7574 7061  els.).  "inputpa
+00001290: 7468 223a 205b 0a20 2020 202f 2f20 496e  th": [.    // In
+000012a0: 7075 7420 696d 6167 6520 7061 7468 732c  put image paths,
+000012b0: 2073 686f 756c 6420 6265 2061 206c 6973   should be a lis
+000012c0: 742e 0a20 2020 2022 7061 7468 2f74 6f2f  t..    "path/to/
+000012d0: 696d 6731 2e6a 7067 222c 0a20 2020 2022  img1.jpg",.    "
+000012e0: 7061 7468 2f74 6f2f 696d 6732 2e70 6e67  path/to/img2.png
+000012f0: 220a 2020 5d2c 0a20 2022 6d6f 6465 6c22  ".  ],.  "model"
+00001300: 3a20 2252 6561 6c43 5547 414e 2d70 726f  : "RealCUGAN-pro
+00001310: 222c 0a20 202f 2f20 6d6f 6465 6c20 6e61  ",.  // model na
+00001320: 6d65 0a20 2022 6d6f 6465 6c73 6361 6c65  me.  "modelscale
+00001330: 223a 2032 2c0a 2020 2f2f 206d 6f64 656c  ": 2,.  // model
+00001340: 2075 7073 6361 6c65 2066 6163 746f 720a   upscale factor.
+00001350: 2020 226d 6f64 656c 6e6f 6973 6522 3a20    "modelnoise": 
+00001360: 2d31 2c0a 2020 2f2f 2044 454e 4f49 5345  -1,.  // DENOISE
+00001370: 206c 6576 656c 0a20 2022 6f75 7470 7574   level.  "output
+00001380: 7061 7468 223a 2022 7061 7468 2f74 6f2f  path": "path/to/
+00001390: 6f75 7470 7574 222c 0a20 202f 2f20 6f75  output",.  // ou
+000013a0: 7470 7574 2070 6174 680a 2020 2274 6172  tput path.  "tar
+000013b0: 6765 7473 6361 6c65 223a 2032 2e30 2c0a  getscale": 2.0,.
+000013c0: 2020 2f2f 2054 6172 6765 7420 7570 7363    // Target upsc
+000013d0: 616c 6520 6661 6374 6f72 2c20 7570 7363  ale factor, upsc
+000013e0: 616c 6520 6d75 6c74 6970 6c65 2074 696d  ale multiple tim
+000013f0: 6573 2074 6f20 6163 6869 6576 6520 7468  es to achieve th
+00001400: 6520 7461 7267 6574 2075 7073 6361 6c65  e target upscale
+00001410: 2066 6163 746f 722e 0a20 202f 2f20 4966   factor..  // If
+00001420: 206e 6f74 2069 6e76 616c 6964 2c20 7573   not invalid, us
+00001430: 6520 6d6f 6465 6c73 6361 6c65 2e0a 2020  e modelscale..  
+00001440: 2274 7461 223a 2066 616c 7365 0a20 202f  "tta": false.  /
+00001450: 2f20 5465 7374 2054 696d 6520 4175 676d  / Test Time Augm
+00001460: 656e 7461 7469 6f6e 2c20 6465 6661 756c  entation, defaul
+00001470: 7420 6661 6c73 650a 7d0a 6060 600a 0a2a  t false.}.```..*
+00001480: 2a53 5550 504f 5254 4544 204d 4f44 454c  *SUPPORTED MODEL
+00001490: 204c 4953 543a 2a2a 0a0a 6060 6079 616d   LIST:**..```yam
+000014a0: 6c0a 2d20 5265 616c 4355 4741 4e2d 7365  l.- RealCUGAN-se
+000014b0: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+000014c0: 5265 616c 4355 4741 4e2d 7365 220a 2020  RealCUGAN-se".  
+000014d0: 2020 2d20 7363 616c 653a 2032 0a20 2020    - scale: 2.   
+000014e0: 2020 2020 2020 2020 2020 2020 2d20 6e6f              - no
+000014f0: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
+00001500: 2c20 330a 2020 2020 2d20 7363 616c 653a  , 3.    - scale:
+00001510: 2033 2c20 340a 2020 2020 2020 2020 2020   3, 4.          
+00001520: 2020 2020 202d 206e 6f69 7365 3a20 2d31       - noise: -1
+00001530: 2c20 302c 2033 0a0a 2d20 5265 616c 4355  , 0, 3..- RealCU
+00001540: 4741 4e2d 7072 6f3a 0a20 2020 202d 206d  GAN-pro:.    - m
+00001550: 6f64 656c 3a20 2252 6561 6c43 5547 414e  odel: "RealCUGAN
+00001560: 2d70 726f 220a 2020 2020 2d20 7363 616c  -pro".    - scal
+00001570: 653a 2032 2c20 330a 2020 2020 2d20 6e6f  e: 2, 3.    - no
+00001580: 6973 653a 202d 312c 2030 2c20 330a 0a2d  ise: -1, 0, 3..-
+00001590: 2052 6561 6c45 5352 4741 4e2d 616e 696d   RealESRGAN-anim
+000015a0: 6576 6964 656f 7633 3a0a 2020 2020 2d20  evideov3:.    - 
+000015b0: 6770 7569 643a 203e 3d20 300a 2020 2020  gpuid: >= 0.    
+000015c0: 2d20 6d6f 6465 6c3a 2022 5265 616c 4553  - model: "RealES
+000015d0: 5247 414e 2d61 6e69 6d65 7669 6465 6f76  RGAN-animevideov
+000015e0: 3322 0a20 2020 202d 2073 6361 6c65 3a20  3".    - scale: 
+000015f0: 322c 2033 2c20 340a 0a2d 2052 6561 6c45  2, 3, 4..- RealE
+00001600: 5352 4741 4e3a 0a20 2020 202d 2067 7075  SRGAN:.    - gpu
+00001610: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+00001620: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+00001630: 4e22 0a20 2020 202d 2073 6361 6c65 3a20  N".    - scale: 
+00001640: 340a 0a2d 2052 6561 6c45 5352 4741 4e2d  4..- RealESRGAN-
+00001650: 616e 696d 653a 0a20 2020 202d 2067 7075  anime:.    - gpu
+00001660: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+00001670: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+00001680: 4e2d 616e 696d 6522 0a20 2020 202d 2073  N-anime".    - s
+00001690: 6361 6c65 3a20 340a 0a2d 2057 6169 6675  cale: 4..- Waifu
+000016a0: 3278 2d63 756e 6574 3a0a 2020 2020 2d20  2x-cunet:.    - 
+000016b0: 6d6f 6465 6c3a 2022 5761 6966 7532 782d  model: "Waifu2x-
+000016c0: 6375 6e65 7422 0a20 2020 202d 2073 6361  cunet".    - sca
+000016d0: 6c65 3a20 310a 2020 2020 2020 2020 2020  le: 1.          
+000016e0: 2020 2020 202d 206e 6f69 7365 3a20 302c       - noise: 0,
+000016f0: 2031 2c20 322c 2033 0a20 2020 202d 2073   1, 2, 3.    - s
+00001700: 6361 6c65 3a20 320a 2020 2020 2020 2020  cale: 2.        
+00001710: 2020 2020 2020 202d 206e 6f69 7365 3a20         - noise: 
+00001720: 2d31 2c20 302c 2031 2c20 322c 2033 0a0a  -1, 0, 1, 2, 3..
+00001730: 2d20 5761 6966 7532 782d 7570 636f 6e76  - Waifu2x-upconv
+00001740: 5f37 5f61 6e69 6d65 5f73 7479 6c65 5f61  _7_anime_style_a
+00001750: 7274 5f72 6762 3a0a 2020 2020 2d20 6d6f  rt_rgb:.    - mo
+00001760: 6465 6c3a 2022 5761 6966 7532 782d 7570  del: "Waifu2x-up
+00001770: 636f 6e76 5f37 5f61 6e69 6d65 5f73 7479  conv_7_anime_sty
+00001780: 6c65 5f61 7274 5f72 6762 220a 2020 2020  le_art_rgb".    
+00001790: 2d20 7363 616c 653a 2032 0a20 2020 202d  - scale: 2.    -
+000017a0: 206e 6f69 7365 3a20 2d31 2c20 302c 2031   noise: -1, 0, 1
+000017b0: 2c20 322c 2033 0a0a 2d20 5761 6966 7532  , 2, 3..- Waifu2
+000017c0: 782d 7570 636f 6e76 5f37 5f70 686f 746f  x-upconv_7_photo
+000017d0: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+000017e0: 5761 6966 7532 782d 7570 636f 6e76 5f37  Waifu2x-upconv_7
+000017f0: 5f70 686f 746f 220a 2020 2020 2d20 7363  _photo".    - sc
+00001800: 616c 653a 2032 0a20 2020 202d 206e 6f69  ale: 2.    - noi
+00001810: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+00001820: 2033 0a0a 2d20 5352 4d44 3a0a 2020 2020   3..- SRMD:.    
+00001830: 2d20 6770 7569 643a 203e 3d20 300a 2020  - gpuid: >= 0.  
+00001840: 2020 2d20 6d6f 6465 6c3a 2022 5352 4d44    - model: "SRMD
+00001850: 220a 2020 2020 2d20 7363 616c 653a 2032  ".    - scale: 2
+00001860: 2c20 332c 2034 0a20 2020 202d 206e 6f69  , 3, 4.    - noi
+00001870: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+00001880: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+00001890: 382c 2039 2c20 3130 0a60 6060 0a0a 2320  8, 9, 10.```..# 
+000018a0: 4275 696c 640a 0a5b 4769 7468 7562 2041  Build..[Github A
+000018b0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f67  ction](https://g
+000018c0: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+000018d0: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+000018e0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000018f0: 732f 4349 2d62 7569 6c64 2e79 6d6c 290a  s/CI-build.yml).
+00001900: 0a2a 5468 6520 7072 6f6a 6563 7420 6a75  .*The project ju
+00001910: 7374 206f 6e6c 7920 6265 656e 2074 6573  st only been tes
+00001920: 7465 6420 696e 2055 6275 6e74 7520 3138  ted in Ubuntu 18
+00001930: 2b20 616e 6420 4465 6269 616e 2039 2b20  + and Debian 9+ 
+00001940: 656e 7669 726f 6e6d 656e 7473 206f 6e20  environments on 
+00001950: 4c69 6e75 782c 2073 6f20 6966 2074 6865  Linux, so if the
+00001960: 2070 726f 6a65 6374 2064 6f65 7320 6e6f   project does no
+00001970: 7420 776f 726b 206f 6e0a 796f 7572 2073  t work on.your s
+00001980: 7973 7465 6d2c 2070 6c65 6173 6520 7472  ystem, please tr
+00001990: 7920 6275 696c 6469 6e67 2069 742e 2a0a  y building it.*.
+000019a0: 0a23 2052 6566 6572 656e 6365 0a0a 5468  .# Reference..Th
+000019b0: 6520 666f 6c6c 6f77 696e 6720 7265 6665  e following refe
+000019c0: 7265 6e63 6573 2077 6572 6520 7573 6564  rences were used
+000019d0: 2069 6e20 7468 6520 6465 7665 6c6f 706d   in the developm
+000019e0: 656e 7420 6f66 2074 6869 7320 7072 6f6a  ent of this proj
+000019f0: 6563 743a 0a0a 2d20 5b6e 636e 6e5d 2868  ect:..- [ncnn](h
+00001a00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a10: 6d2f 5465 6e63 656e 742f 6e63 6e6e 2920  m/Tencent/ncnn) 
+00001a20: 2d20 6e63 6e6e 2069 7320 6120 6869 6768  - ncnn is a high
+00001a30: 2d70 6572 666f 726d 616e 6365 206e 6575  -performance neu
+00001a40: 7261 6c20 6e65 7477 6f72 6b20 696e 6665  ral network infe
+00001a50: 7265 6e63 6520 6672 616d 6577 6f72 6b20  rence framework 
+00001a60: 6465 7665 6c6f 7065 6420 6279 2054 656e  developed by Ten
+00001a70: 6365 6e74 2041 4920 4c61 622e 0a2d 205b  cent AI Lab..- [
+00001a80: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+00001a90: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+00001aa0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001ab0: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+00001ac0: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
+00001ad0: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
+00001ae0: 6964 6564 2074 6865 2063 6f72 6520 696d  ided the core im
+00001af0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001b00: 7468 6520 5265 616c 2d43 5547 414e 2061  the Real-CUGAN a
+00001b10: 6c67 6f72 6974 686d 2075 7369 6e67 2074  lgorithm using t
+00001b20: 6865 206e 636e 6e20 616e 6420 5675 6c6b  he ncnn and Vulk
+00001b30: 616e 206c 6962 7261 7269 6573 2e0a 2d20  an libraries..- 
+00001b40: 5b78 696e 6e74 616f 2f52 6561 6c2d 4553  [xinntao/Real-ES
+00001b50: 5247 414e 2d6e 636e 6e2d 7675 6c6b 616e  RGAN-ncnn-vulkan
+00001b60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001b70: 2e63 6f6d 2f78 696e 6e74 616f 2f52 6561  .com/xinntao/Rea
+00001b80: 6c2d 4553 5247 414e 2d6e 636e 6e2d 7675  l-ESRGAN-ncnn-vu
+00001b90: 6c6b 616e 2920 2d20 5468 6973 2070 726f  lkan) - This pro
+00001ba0: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+00001bb0: 6520 636f 7265 2069 6d70 6c65 6d65 6e74  e core implement
+00001bc0: 6174 696f 6e20 6f66 2074 6865 2052 6561  ation of the Rea
+00001bd0: 6c2d 4553 5247 414e 2061 6c67 6f72 6974  l-ESRGAN algorit
+00001be0: 686d 2075 7369 6e67 2074 6865 206e 636e  hm using the ncn
+00001bf0: 6e20 616e 6420 5675 6c6b 616e 206c 6962  n and Vulkan lib
+00001c00: 7261 7269 6573 2e0a 2d20 5b6e 6968 7569  raries..- [nihui
+00001c10: 2f77 6169 6675 3278 2d6e 636e 6e2d 7675  /waifu2x-ncnn-vu
+00001c20: 6c6b 616e 5d28 6874 7470 733a 2f2f 6769  lkan](https://gi
+00001c30: 7468 7562 2e63 6f6d 2f6e 6968 7569 2f77  thub.com/nihui/w
+00001c40: 6169 6675 3278 2d6e 636e 6e2d 7675 6c6b  aifu2x-ncnn-vulk
+00001c50: 616e 2920 2d20 5468 6973 2070 726f 6a65  an) - This proje
+00001c60: 6374 2070 726f 7669 6465 6420 7468 6520  ct provided the 
+00001c70: 636f 7265 2069 6d70 6c65 6d65 6e74 6174  core implementat
+00001c80: 696f 6e20 6f66 2074 6865 2057 6169 6675  ion of the Waifu
+00001c90: 3278 2061 6c67 6f72 6974 686d 2075 7369  2x algorithm usi
+00001ca0: 6e67 2074 6865 206e 636e 6e20 616e 6420  ng the ncnn and 
+00001cb0: 5675 6c6b 616e 206c 6962 7261 7269 6573  Vulkan libraries
+00001cc0: 2e0a 2d20 5b6e 6968 7569 2f73 726d 642d  ..- [nihui/srmd-
+00001cd0: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+00001ce0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001cf0: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
+00001d00: 7675 6c6b 616e 2920 2d20 5468 6973 2070  vulkan) - This p
+00001d10: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001d20: 7468 6520 636f 7265 2069 6d70 6c65 6d65  the core impleme
+00001d30: 6e74 6174 696f 6e20 6f66 2074 6865 2053  ntation of the S
+00001d40: 524d 4420 616c 676f 7269 7468 6d20 7573  RMD algorithm us
+00001d50: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
+00001d60: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
+00001d70: 732e 0a2d 205b 7265 616c 6375 6761 6e2d  s..- [realcugan-
+00001d80: 6e63 6e6e 2d70 795d 2868 7474 7073 3a2f  ncnn-py](https:/
+00001d90: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
+00001da0: 7573 6b79 2f72 6561 6c63 7567 616e 2d6e  usky/realcugan-n
+00001db0: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
+00001dc0: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001dd0: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
+00001de0: 6e67 2066 6f72 2072 6561 6c63 7567 616e  ng for realcugan
+00001df0: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
+00001e00: 6820 5079 4269 6e64 3131 2e0a 2d20 5b72  h PyBind11..- [r
+00001e10: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001e20: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00001e30: 622e 636f 6d2f 546f 6872 7573 6b79 2f72  b.com/Tohrusky/r
+00001e40: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001e50: 7929 202d 2054 6869 7320 7072 6f6a 6563  y) - This projec
+00001e60: 7420 7072 6f76 6964 6564 2074 6865 2050  t provided the P
+00001e70: 7974 686f 6e20 4269 6e64 696e 6720 666f  ython Binding fo
+00001e80: 7220 7265 616c 6573 7267 616e 2d6e 636e  r realesrgan-ncn
+00001e90: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
+00001ea0: 4269 6e64 3131 2e0a 2d20 5b77 6169 6675  Bind11..- [waifu
+00001eb0: 3278 2d6e 636e 6e2d 7079 5d28 6874 7470  2x-ncnn-py](http
+00001ec0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001ed0: 6f68 7275 736b 792f 7761 6966 7532 782d  ohrusky/waifu2x-
+00001ee0: 6e63 6e6e 2d70 7929 202d 2054 6869 7320  ncnn-py) - This 
+00001ef0: 7072 6f6a 6563 7420 7072 6f76 6964 6564  project provided
+00001f00: 2074 6865 2050 7974 686f 6e20 4269 6e64   the Python Bind
+00001f10: 696e 6720 666f 7220 7761 6966 7532 782d  ing for waifu2x-
+00001f20: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
+00001f30: 2050 7942 696e 6431 312e 0a2d 205b 7372   PyBind11..- [sr
+00001f40: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
+00001f50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001f60: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
+00001f70: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
+00001f80: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+00001f90: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
+00001fa0: 2066 6f72 2073 726d 642d 6e63 6e6e 2d76   for srmd-ncnn-v
+00001fb0: 756c 6b61 6e20 7769 7468 2050 7942 696e  ulkan with PyBin
+00001fc0: 6431 312e 0a0a 2320 4c69 6365 6e73 650a  d11...# License.
+00001fd0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001fe0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001ff0: 7468 6520 4253 4420 332d 436c 6175 7365  the BSD 3-Clause
+00002000: 202d 2073 6565 0a74 6865 205b 4c49 4345   - see.the [LICE
+00002010: 4e53 4520 6669 6c65 5d28 6874 7470 733a  NSE file](https:
+00002020: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00002030: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+00002040: 7265 2f62 6c6f 622f 6d61 696e 2f4c 4943  re/blob/main/LIC
+00002050: 454e 5345 2920 666f 7220 6465 7461 696c  ENSE) for detail
+00002060: 732e 0a0a 0a                             s....
```

### Comparing `Final2x-core-1.0.2/README.md` & `Final2x-core-1.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,409 +1,519 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
-00000020: 7470 733a 2f2f 7332 2e6c 6f6c 692e 6e65  tps://s2.loli.ne
-00000030: 742f 3230 3233 2f30 362f 3139 2f35 3437  t/2023/06/19/547
-00000040: 7152 6563 4864 6e4a 4962 4b75 2e70 6e67  qRecHdnJIbKu.png
-00000050: 2220 6865 6967 6874 3d22 3132 3822 3e0a  " height="128">.
-00000060: 0a3c 2f70 3e0a 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
-00000070: 3d22 6365 6e74 6572 223e 2046 696e 616c  ="center"> Final
-00000080: 3278 2d63 6f72 6520 3c2f 6831 3e0a 0a21  2x-core </h1>..!
-00000090: 5b4d 6163 4f53 2078 3634 5d28 6874 7470  [MacOS x64](http
-000000a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000000b0: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
-000000c0: 2d4d 6163 4f53 2532 3078 3634 2d62 6c75  -MacOS%20x64-blu
-000000d0: 653f 6c6f 676f 3d41 7070 6c65 2673 7479  e?logo=Apple&sty
-000000e0: 6c65 3d66 6c61 742d 7371 7561 7265 290a  le=flat-square).
-000000f0: 215b 4d61 634f 5320 6172 6d36 345d 2868  ![MacOS arm64](h
-00000100: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000110: 6473 2e69 6f2f 6261 6467 652f 5375 7070  ds.io/badge/Supp
-00000120: 6f72 742d 4d61 634f 5325 3230 6172 6d36  ort-MacOS%20arm6
-00000130: 342d 626c 7565 3f6c 6f67 6f3d 4170 706c  4-blue?logo=Appl
-00000140: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-00000150: 6172 6529 0a21 5b57 696e 646f 7773 2078  are).![Windows x
-00000160: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000170: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000180: 2f53 7570 706f 7274 2d57 696e 646f 7773  /Support-Windows
-00000190: 2532 3078 3634 2d62 6c75 653f 6c6f 676f  %20x64-blue?logo
-000001a0: 3d57 696e 646f 7773 2673 7479 6c65 3d66  =Windows&style=f
-000001b0: 6c61 742d 7371 7561 7265 290a 215b 5769  lat-square).![Wi
-000001c0: 6e64 6f77 7320 6172 6d36 345d 2868 7474  ndows arm64](htt
-000001d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000001e0: 2e69 6f2f 6261 6467 652f 5375 7070 6f72  .io/badge/Suppor
-000001f0: 742d 5769 6e64 6f77 7325 3230 6172 6d36  t-Windows%20arm6
-00000200: 342d 626c 7565 3f6c 6f67 6f3d 5769 6e64  4-blue?logo=Wind
-00000210: 6f77 7326 7374 796c 653d 666c 6174 2d73  ows&style=flat-s
-00000220: 7175 6172 6529 0a21 5b4c 696e 7578 2078  quare).![Linux x
-00000230: 3634 5d28 6874 7470 733a 2f2f 696d 672e  64](https://img.
-00000240: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000250: 2f53 7570 706f 7274 2d4c 696e 7578 2532  /Support-Linux%2
-00000260: 3078 3634 2d62 6c75 653f 6c6f 676f 3d4c  0x64-blue?logo=L
-00000270: 696e 7578 2673 7479 6c65 3d66 6c61 742d  inux&style=flat-
-00000280: 7371 7561 7265 290a 5b21 5b63 6f64 6563  square).[![codec
-00000290: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
-000002a0: 636f 762e 696f 2f67 682f 546f 6872 7573  cov.io/gh/Tohrus
-000002b0: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-000002c0: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
-000002d0: 682f 6261 6467 652e 7376 673f 746f 6b65  h/badge.svg?toke
-000002e0: 6e3d 4232 544e 4b59 4e34 4f34 295d 2868  n=B2TNKYN4O4)](h
-000002f0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-00000300: 6f2f 6768 2f54 6f68 7275 736b 792f 4669  o/gh/Tohrusky/Fi
-00000310: 6e61 6c32 782d 636f 7265 290a 5b21 5b43  nal2x-core).[![C
-00000320: 492d 7465 7374 5d28 6874 7470 733a 2f2f  I-test](https://
-00000330: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-00000340: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-00000350: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000360: 7773 2f43 492d 7465 7374 2e79 6d6c 2f62  ws/CI-test.yml/b
-00000370: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00000380: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-00000390: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
-000003a0: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
-000003b0: 666c 6f77 732f 4349 2d74 6573 742e 796d  flows/CI-test.ym
-000003c0: 6c29 0a5b 215b 4349 2d62 7569 6c64 5d28  l).[![CI-build](
-000003d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003e0: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
-000003f0: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
-00000400: 2f77 6f72 6b66 6c6f 7773 2f43 492d 6275  /workflows/CI-bu
-00000410: 696c 642e 796d 6c2f 6261 6467 652e 7376  ild.yml/badge.sv
-00000420: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00000430: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
-00000440: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
-00000450: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f43  ions/workflows/C
-00000460: 492d 6275 696c 642e 796d 6c29 0a5b 215b  I-build.yml).[![
-00000470: 5265 6c65 6173 655d 2868 7474 7073 3a2f  Release](https:/
-00000480: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
-00000490: 7573 6b79 2f46 696e 616c 3278 2d63 6f72  usky/Final2x-cor
-000004a0: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-000004b0: 6f77 732f 5265 6c65 6173 652e 796d 6c2f  ows/Release.yml/
-000004c0: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-000004d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000004e0: 6f68 7275 736b 792f 4669 6e61 6c32 782d  ohrusky/Final2x-
-000004f0: 636f 7265 2f61 6374 696f 6e73 2f77 6f72  core/actions/wor
-00000500: 6b66 6c6f 7773 2f52 656c 6561 7365 2e79  kflows/Release.y
-00000510: 6d6c 290a 5b21 5b50 4950 2d74 6573 745d  ml).[![PIP-test]
-00000520: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000530: 636f 6d2f 546f 6872 7573 6b79 2f46 696e  com/Tohrusky/Fin
-00000540: 616c 3278 2d63 6f72 652f 6163 7469 6f6e  al2x-core/action
-00000550: 732f 776f 726b 666c 6f77 732f 5049 502d  s/workflows/PIP-
-00000560: 7465 7374 2e79 6d6c 2f62 6164 6765 2e73  test.yml/badge.s
-00000570: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000580: 6875 622e 636f 6d2f 546f 6872 7573 6b79  hub.com/Tohrusky
-00000590: 2f46 696e 616c 3278 2d63 6f72 652f 6163  /Final2x-core/ac
-000005a0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000005b0: 5049 502d 7465 7374 2e79 6d6c 290a 5b21  PIP-test.yml).[!
-000005c0: 5b52 656c 6561 7365 2d70 7970 695d 2868  [Release-pypi](h
-000005d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005e0: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-000005f0: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
-00000600: 776f 726b 666c 6f77 732f 5265 6c65 6173  workflows/Releas
-00000610: 652d 7079 7069 2e79 6d6c 2f62 6164 6765  e-pypi.yml/badge
-00000620: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000630: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
-00000640: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
-00000650: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000660: 732f 5265 6c65 6173 652d 7079 7069 2e79  s/Release-pypi.y
-00000670: 6d6c 290a 5b21 5b50 7950 4920 7665 7273  ml).[![PyPI vers
-00000680: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
-00000690: 6765 2e66 7572 792e 696f 2f70 792f 4669  ge.fury.io/py/Fi
-000006a0: 6e61 6c32 782d 636f 7265 2e73 7667 295d  nal2x-core.svg)]
-000006b0: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-000006c0: 7572 792e 696f 2f70 792f 4669 6e61 6c32  ury.io/py/Final2
-000006d0: 782d 636f 7265 290a 215b 4769 7448 7562  x-core).![GitHub
-000006e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000006f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000700: 6c69 6365 6e73 652f 546f 6872 7573 6b79  license/Tohrusky
-00000710: 2f46 696e 616c 3278 2d63 6f72 6529 0a0a  /Final2x-core)..
-00000720: 4669 6e61 6c32 782d 636f 7265 2069 7320  Final2x-core is 
-00000730: 6120 6372 6f73 732d 706c 6174 666f 726d  a cross-platform
-00000740: 2069 6d61 6765 2073 7570 6572 2d72 6573   image super-res
-00000750: 6f6c 7574 696f 6e20 434c 4920 746f 6f6c  olution CLI tool
-00000760: 2066 6f72 205b 4669 6e61 6c32 785d 2868   for [Final2x](h
-00000770: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000780: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
-00000790: 3278 292e 2049 6620 796f 7520 6861 7665  2x). If you have
-000007a0: 2061 6e79 2071 7565 7374 696f 6e73 2c20   any questions, 
-000007b0: 706c 6561 7365 2072 6169 7365 2061 6e20  please raise an 
-000007c0: 6973 7375 6520 5b69 6e20 7468 6973 2072  issue [in this r
-000007d0: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-000007f0: 6872 7573 6b79 2f46 696e 616c 3278 292e  hrusky/Final2x).
-00000800: 0a0a 2320 496e 7374 616c 6c0a 0a44 6f77  ..# Install..Dow
-00000810: 6e6c 6f61 6420 696e 205b 5265 6c65 6173  nload in [Releas
-00000820: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000830: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
-00000840: 696e 616c 3278 2d63 6f72 652f 7265 6c65  inal2x-core/rele
-00000850: 6173 6573 2920 6f72 2075 7365 2070 6970  ases) or use pip
-00000860: 2028 7079 7468 6f6e 203e 3d20 332e 362c   (python >= 3.6,
-00000870: 203e 3d33 2e39 2066 6f72 204d 6163 4f53   >=3.9 for MacOS
-00000880: 0a61 726d 3634 290a 0a60 6060 7368 656c  .arm64)..```shel
-00000890: 6c0a 7069 7020 696e 7374 616c 6c20 4669  l.pip install Fi
-000008a0: 6e61 6c32 782d 636f 7265 0a60 6060 0a0a  nal2x-core.```..
-000008b0: 2320 5573 650a 0a60 6060 7368 656c 6c0a  # Use..```shell.
-000008c0: 7573 6167 653a 2046 696e 616c 3278 2d63  usage: Final2x-c
-000008d0: 6f72 6520 5b2d 685d 205b 2d62 2042 4153  ore [-h] [-b BAS
-000008e0: 4536 345d 205b 2d6a 204a 534f 4e5d 205b  E64] [-j JSON] [
-000008f0: 2d79 2059 414d 4c5d 205b 2d6f 5d0a 0a77  -y YAML] [-o]..w
-00000900: 6865 6e20 7061 7261 2069 7320 6e6f 7420  hen para is not 
-00000910: 7370 6563 6966 6965 642c 2074 6865 2063  specified, the c
-00000920: 6f6e 6669 672e 7961 6d6c 2066 696c 6520  onfig.yaml file 
-00000930: 696e 2074 6865 2064 6972 6563 746f 7279  in the directory
-00000940: 2077 696c 6c20 6265 2072 6561 6420 6175   will be read au
-00000950: 746f 6d61 7469 6361 6c6c 790a 0a6f 7074  tomatically..opt
-00000960: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
-00000970: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
-00000980: 2020 2020 2020 2020 2073 686f 7720 7468           show th
-00000990: 6973 2068 656c 7020 6d65 7373 6167 6520  is help message 
-000009a0: 616e 6420 6578 6974 0a20 202d 6220 4241  and exit.  -b BA
-000009b0: 5345 3634 2c20 2d2d 4241 5345 3634 2042  SE64, --BASE64 B
-000009c0: 4153 4536 340a 2020 2020 2020 2020 2020  ASE64.          
-000009d0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-000009e0: 7365 3634 2073 7472 696e 6720 666f 7220  se64 string for 
-000009f0: 636f 6e66 6967 206a 736f 6e0a 2020 2d6a  config json.  -j
-00000a00: 204a 534f 4e2c 202d 2d4a 534f 4e20 4a53   JSON, --JSON JS
-00000a10: 4f4e 2020 4a53 4f4e 2073 7472 696e 6720  ON  JSON string 
-00000a20: 666f 7220 636f 6e66 6967 0a20 202d 7920  for config.  -y 
-00000a30: 5941 4d4c 2c20 2d2d 5941 4d4c 2059 414d  YAML, --YAML YAM
-00000a40: 4c20 2079 616d 6c20 636f 6e66 6967 2066  L  yaml config f
-00000a50: 696c 6520 7061 7468 0a20 202d 6c2c 202d  ile path.  -l, -
-00000a60: 2d4c 4f47 2020 2020 2020 2020 2020 2020  -LOG            
-00000a70: 2073 6176 6520 6c6f 670a 2020 2d6f 2c20   save log.  -o, 
-00000a80: 2d2d 4f50 2020 2020 2020 2020 2020 2020  --OP            
-00000a90: 2020 6368 6563 6b20 696e 7374 616c 6c0a    check install.
-00000aa0: 6060 600a 0a23 2043 6f6e 6669 670a 0a50  ```..# Config..P
-00000ab0: 6173 7320 7468 6520 636f 6e66 6967 206a  ass the config j
-00000ac0: 736f 6e20 7374 7269 6e67 2074 6f20 7468  son string to th
-00000ad0: 6520 7072 6f67 7261 6d20 7468 726f 7567  e program throug
-00000ae0: 6820 7468 6520 602d 6a60 2070 6172 616d  h the `-j` param
-00000af0: 6574 6572 2e0a 0a2a 2a50 4c45 4153 4520  eter...**PLEASE 
-00000b00: 4e4f 5445 3a20 7468 6520 636f 6e66 6967  NOTE: the config
-00000b10: 2069 7320 4a53 4f4e 2c20 7265 6d6f 7665   is JSON, remove
-00000b20: 2074 6865 202f 2f20 636f 6d6d 656e 7473   the // comments
-00000b30: 2062 6566 6f72 6520 7573 652e 2a2a 0a0a   before use.**..
-00000b40: 6060 606a 736f 6e0a 7b0a 2020 2267 7075  ```json.{.  "gpu
-00000b50: 6964 223a 2030 2c0a 2020 2f2f 2047 5055  id": 0,.  // GPU
-00000b60: 2069 642c 203e 3d20 2d31 2028 2d31 2066   id, >= -1 (-1 f
-00000b70: 6f72 2043 5055 2c20 6d61 7920 6e6f 7420  or CPU, may not 
-00000b80: 776f 726b 2066 6f72 2073 6f6d 6520 6d6f  work for some mo
-00000b90: 6465 6c73 2e29 0a20 2022 696e 7075 7470  dels.).  "inputp
-00000ba0: 6174 6822 3a20 5b0a 2020 2020 2f2f 2049  ath": [.    // I
-00000bb0: 6e70 7574 2069 6d61 6765 2070 6174 6873  nput image paths
-00000bc0: 2c20 7368 6f75 6c64 2062 6520 6120 6c69  , should be a li
-00000bd0: 7374 2e0a 2020 2020 2270 6174 682f 746f  st..    "path/to
-00000be0: 2f69 6d67 312e 6a70 6722 2c0a 2020 2020  /img1.jpg",.    
-00000bf0: 2270 6174 682f 746f 2f69 6d67 322e 706e  "path/to/img2.pn
-00000c00: 6722 0a20 205d 2c0a 2020 226d 6f64 656c  g".  ],.  "model
-00000c10: 223a 2022 5265 616c 4355 4741 4e2d 7072  ": "RealCUGAN-pr
-00000c20: 6f22 2c0a 2020 2f2f 206d 6f64 656c 206e  o",.  // model n
-00000c30: 616d 650a 2020 226d 6f64 656c 7363 616c  ame.  "modelscal
-00000c40: 6522 3a20 322c 0a20 202f 2f20 6d6f 6465  e": 2,.  // mode
-00000c50: 6c20 7570 7363 616c 6520 6661 6374 6f72  l upscale factor
-00000c60: 0a20 2022 6d6f 6465 6c6e 6f69 7365 223a  .  "modelnoise":
-00000c70: 202d 312c 0a20 202f 2f20 4445 4e4f 4953   -1,.  // DENOIS
-00000c80: 4520 6c65 7665 6c0a 2020 226f 7574 7075  E level.  "outpu
-00000c90: 7470 6174 6822 3a20 2270 6174 682f 746f  tpath": "path/to
-00000ca0: 2f6f 7574 7075 7422 2c0a 2020 2f2f 206f  /output",.  // o
-00000cb0: 7574 7075 7420 7061 7468 0a20 2022 7461  utput path.  "ta
-00000cc0: 7267 6574 7363 616c 6522 3a20 322e 302c  rgetscale": 2.0,
-00000cd0: 0a20 202f 2f20 5461 7267 6574 2075 7073  .  // Target ups
-00000ce0: 6361 6c65 2066 6163 746f 722c 2075 7073  cale factor, ups
-00000cf0: 6361 6c65 206d 756c 7469 706c 6520 7469  cale multiple ti
-00000d00: 6d65 7320 746f 2061 6368 6965 7665 2074  mes to achieve t
-00000d10: 6865 2074 6172 6765 7420 7570 7363 616c  he target upscal
-00000d20: 6520 6661 6374 6f72 2e0a 2020 2f2f 2049  e factor..  // I
-00000d30: 6620 6e6f 7420 696e 7661 6c69 642c 2075  f not invalid, u
-00000d40: 7365 206d 6f64 656c 7363 616c 652e 0a20  se modelscale.. 
-00000d50: 2022 7474 6122 3a20 6661 6c73 650a 2020   "tta": false.  
-00000d60: 2f2f 2054 6573 7420 5469 6d65 2041 7567  // Test Time Aug
-00000d70: 6d65 6e74 6174 696f 6e2c 2064 6566 6175  mentation, defau
-00000d80: 6c74 2066 616c 7365 0a7d 0a60 6060 0a0a  lt false.}.```..
-00000d90: 2a2a 5355 5050 4f52 5445 4420 4d4f 4445  **SUPPORTED MODE
-00000da0: 4c20 4c49 5354 3a2a 2a0a 0a60 6060 7961  L LIST:**..```ya
-00000db0: 6d6c 0a2d 2052 6561 6c43 5547 414e 2d73  ml.- RealCUGAN-s
-00000dc0: 653a 0a20 2020 202d 206d 6f64 656c 3a20  e:.    - model: 
-00000dd0: 2252 6561 6c43 5547 414e 2d73 6522 0a20  "RealCUGAN-se". 
-00000de0: 2020 202d 2073 6361 6c65 3a20 320a 2020     - scale: 2.  
-00000df0: 2020 2020 2020 2020 2020 2020 202d 206e               - n
-00000e00: 6f69 7365 3a20 2d31 2c20 302c 2031 2c20  oise: -1, 0, 1, 
-00000e10: 322c 2033 0a20 2020 202d 2073 6361 6c65  2, 3.    - scale
-00000e20: 3a20 332c 2034 0a20 2020 2020 2020 2020  : 3, 4.         
-00000e30: 2020 2020 2020 2d20 6e6f 6973 653a 202d        - noise: -
-00000e40: 312c 2030 2c20 330a 0a2d 2052 6561 6c43  1, 0, 3..- RealC
-00000e50: 5547 414e 2d70 726f 3a0a 2020 2020 2d20  UGAN-pro:.    - 
-00000e60: 6d6f 6465 6c3a 2022 5265 616c 4355 4741  model: "RealCUGA
-00000e70: 4e2d 7072 6f22 0a20 2020 202d 2073 6361  N-pro".    - sca
-00000e80: 6c65 3a20 322c 2033 0a20 2020 202d 206e  le: 2, 3.    - n
-00000e90: 6f69 7365 3a20 2d31 2c20 302c 2033 0a0a  oise: -1, 0, 3..
-00000ea0: 2d20 5265 616c 4553 5247 414e 2d61 6e69  - RealESRGAN-ani
-00000eb0: 6d65 7669 6465 6f76 333a 0a20 2020 202d  mevideov3:.    -
-00000ec0: 2067 7075 6964 3a20 3e3d 2030 0a20 2020   gpuid: >= 0.   
-00000ed0: 202d 206d 6f64 656c 3a20 2252 6561 6c45   - model: "RealE
-00000ee0: 5352 4741 4e2d 616e 696d 6576 6964 656f  SRGAN-animevideo
-00000ef0: 7633 220a 2020 2020 2d20 7363 616c 653a  v3".    - scale:
-00000f00: 2032 2c20 332c 2034 0a0a 2d20 5265 616c   2, 3, 4..- Real
-00000f10: 4553 5247 414e 3a0a 2020 2020 2d20 6770  ESRGAN:.    - gp
-00000f20: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-00000f30: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00000f40: 414e 220a 2020 2020 2d20 7363 616c 653a  AN".    - scale:
-00000f50: 2034 0a0a 2d20 5265 616c 4553 5247 414e   4..- RealESRGAN
-00000f60: 2d61 6e69 6d65 3a0a 2020 2020 2d20 6770  -anime:.    - gp
-00000f70: 7569 643a 203e 3d20 300a 2020 2020 2d20  uid: >= 0.    - 
-00000f80: 6d6f 6465 6c3a 2022 5265 616c 4553 5247  model: "RealESRG
-00000f90: 414e 2d61 6e69 6d65 220a 2020 2020 2d20  AN-anime".    - 
-00000fa0: 7363 616c 653a 2034 0a0a 2d20 5761 6966  scale: 4..- Waif
-00000fb0: 7532 782d 6375 6e65 743a 0a20 2020 202d  u2x-cunet:.    -
-00000fc0: 206d 6f64 656c 3a20 2257 6169 6675 3278   model: "Waifu2x
-00000fd0: 2d63 756e 6574 220a 2020 2020 2d20 7363  -cunet".    - sc
-00000fe0: 616c 653a 2031 0a20 2020 2020 2020 2020  ale: 1.         
-00000ff0: 2020 2020 2020 2d20 6e6f 6973 653a 2030        - noise: 0
-00001000: 2c20 312c 2032 2c20 330a 2020 2020 2d20  , 1, 2, 3.    - 
-00001010: 7363 616c 653a 2032 0a20 2020 2020 2020  scale: 2.       
-00001020: 2020 2020 2020 2020 2d20 6e6f 6973 653a          - noise:
-00001030: 202d 312c 2030 2c20 312c 2032 2c20 330a   -1, 0, 1, 2, 3.
-00001040: 0a2d 2057 6169 6675 3278 2d75 7063 6f6e  .- Waifu2x-upcon
-00001050: 765f 375f 616e 696d 655f 7374 796c 655f  v_7_anime_style_
-00001060: 6172 745f 7267 623a 0a20 2020 202d 206d  art_rgb:.    - m
-00001070: 6f64 656c 3a20 2257 6169 6675 3278 2d75  odel: "Waifu2x-u
-00001080: 7063 6f6e 765f 375f 616e 696d 655f 7374  pconv_7_anime_st
-00001090: 796c 655f 6172 745f 7267 6222 0a20 2020  yle_art_rgb".   
-000010a0: 202d 2073 6361 6c65 3a20 320a 2020 2020   - scale: 2.    
-000010b0: 2d20 6e6f 6973 653a 202d 312c 2030 2c20  - noise: -1, 0, 
-000010c0: 312c 2032 2c20 330a 0a2d 2057 6169 6675  1, 2, 3..- Waifu
-000010d0: 3278 2d75 7063 6f6e 765f 375f 7068 6f74  2x-upconv_7_phot
-000010e0: 6f3a 0a20 2020 202d 206d 6f64 656c 3a20  o:.    - model: 
-000010f0: 2257 6169 6675 3278 2d75 7063 6f6e 765f  "Waifu2x-upconv_
-00001100: 375f 7068 6f74 6f22 0a20 2020 202d 2073  7_photo".    - s
-00001110: 6361 6c65 3a20 320a 2020 2020 2d20 6e6f  cale: 2.    - no
-00001120: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-00001130: 2c20 330a 0a2d 2053 524d 443a 0a20 2020  , 3..- SRMD:.   
-00001140: 202d 2067 7075 6964 3a20 3e3d 2030 0a20   - gpuid: >= 0. 
-00001150: 2020 202d 206d 6f64 656c 3a20 2253 524d     - model: "SRM
-00001160: 4422 0a20 2020 202d 2073 6361 6c65 3a20  D".    - scale: 
-00001170: 322c 2033 2c20 340a 2020 2020 2d20 6e6f  2, 3, 4.    - no
-00001180: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
-00001190: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-000011a0: 2038 2c20 392c 2031 300a 6060 600a 0a23   8, 9, 10.```..#
-000011b0: 2042 7569 6c64 0a0a 5b47 6974 6875 6220   Build..[Github 
-000011c0: 4163 7469 6f6e 5d28 6874 7470 733a 2f2f  Action](https://
-000011d0: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
-000011e0: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
-000011f0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00001200: 7773 2f43 492d 6275 696c 642e 796d 6c29  ws/CI-build.yml)
-00001210: 0a0a 2a54 6865 2070 726f 6a65 6374 206a  ..*The project j
-00001220: 7573 7420 6f6e 6c79 2062 6565 6e20 7465  ust only been te
-00001230: 7374 6564 2069 6e20 5562 756e 7475 2031  sted in Ubuntu 1
-00001240: 382b 2061 6e64 2044 6562 6961 6e20 392b  8+ and Debian 9+
-00001250: 2065 6e76 6972 6f6e 6d65 6e74 7320 6f6e   environments on
-00001260: 204c 696e 7578 2c20 736f 2069 6620 7468   Linux, so if th
-00001270: 6520 7072 6f6a 6563 7420 646f 6573 206e  e project does n
-00001280: 6f74 2077 6f72 6b20 6f6e 0a79 6f75 7220  ot work on.your 
-00001290: 7379 7374 656d 2c20 706c 6561 7365 2074  system, please t
-000012a0: 7279 2062 7569 6c64 696e 6720 6974 2e2a  ry building it.*
-000012b0: 0a0a 2320 5265 6665 7265 6e63 650a 0a54  ..# Reference..T
-000012c0: 6865 2066 6f6c 6c6f 7769 6e67 2072 6566  he following ref
-000012d0: 6572 656e 6365 7320 7765 7265 2075 7365  erences were use
-000012e0: 6420 696e 2074 6865 2064 6576 656c 6f70  d in the develop
-000012f0: 6d65 6e74 206f 6620 7468 6973 2070 726f  ment of this pro
-00001300: 6a65 6374 3a0a 0a2d 205b 6e63 6e6e 5d28  ject:..- [ncnn](
-00001310: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001320: 6f6d 2f54 656e 6365 6e74 2f6e 636e 6e29  om/Tencent/ncnn)
-00001330: 202d 206e 636e 6e20 6973 2061 2068 6967   - ncnn is a hig
-00001340: 682d 7065 7266 6f72 6d61 6e63 6520 6e65  h-performance ne
-00001350: 7572 616c 206e 6574 776f 726b 2069 6e66  ural network inf
-00001360: 6572 656e 6365 2066 7261 6d65 776f 726b  erence framework
-00001370: 2064 6576 656c 6f70 6564 2062 790a 2020   developed by.  
-00001380: 5465 6e63 656e 7420 4149 204c 6162 2e0a  Tencent AI Lab..
-00001390: 2d20 5b6e 6968 7569 2f72 6561 6c63 7567  - [nihui/realcug
-000013a0: 616e 2d6e 636e 6e2d 7675 6c6b 616e 5d28  an-ncnn-vulkan](
-000013b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000013c0: 6f6d 2f6e 6968 7569 2f72 6561 6c63 7567  om/nihui/realcug
-000013d0: 616e 2d6e 636e 6e2d 7675 6c6b 616e 2920  an-ncnn-vulkan) 
-000013e0: 2d20 5468 6973 2070 726f 6a65 6374 2070  - This project p
-000013f0: 726f 7669 6465 6420 7468 6520 636f 7265  rovided the core
-00001400: 0a20 2069 6d70 6c65 6d65 6e74 6174 696f  .  implementatio
-00001410: 6e20 6f66 2074 6865 2052 6561 6c2d 4355  n of the Real-CU
-00001420: 4741 4e20 616c 676f 7269 7468 6d20 7573  GAN algorithm us
-00001430: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
-00001440: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
-00001450: 732e 0a2d 205b 7869 6e6e 7461 6f2f 5265  s..- [xinntao/Re
-00001460: 616c 2d45 5352 4741 4e2d 6e63 6e6e 2d76  al-ESRGAN-ncnn-v
-00001470: 756c 6b61 6e5d 2868 7474 7073 3a2f 2f67  ulkan](https://g
-00001480: 6974 6875 622e 636f 6d2f 7869 6e6e 7461  ithub.com/xinnta
-00001490: 6f2f 5265 616c 2d45 5352 4741 4e2d 6e63  o/Real-ESRGAN-nc
-000014a0: 6e6e 2d76 756c 6b61 6e29 202d 2054 6869  nn-vulkan) - Thi
-000014b0: 7320 7072 6f6a 6563 7420 7072 6f76 6964  s project provid
-000014c0: 6564 2074 6865 2063 6f72 650a 2020 696d  ed the core.  im
-000014d0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-000014e0: 7468 6520 5265 616c 2d45 5352 4741 4e20  the Real-ESRGAN 
-000014f0: 616c 676f 7269 7468 6d20 7573 696e 6720  algorithm using 
-00001500: 7468 6520 6e63 6e6e 2061 6e64 2056 756c  the ncnn and Vul
-00001510: 6b61 6e0a 2020 6c69 6272 6172 6965 732e  kan.  libraries.
-00001520: 0a2d 205b 6e69 6875 692f 7761 6966 7532  .- [nihui/waifu2
-00001530: 782d 6e63 6e6e 2d76 756c 6b61 6e5d 2868  x-ncnn-vulkan](h
-00001540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001550: 6d2f 6e69 6875 692f 7761 6966 7532 782d  m/nihui/waifu2x-
-00001560: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
-00001570: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
-00001580: 6964 6564 2074 6865 2063 6f72 650a 2020  ided the core.  
-00001590: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-000015a0: 6620 7468 6520 5761 6966 7532 7820 616c  f the Waifu2x al
-000015b0: 676f 7269 7468 6d20 7573 696e 6720 7468  gorithm using th
-000015c0: 6520 6e63 6e6e 2061 6e64 2056 756c 6b61  e ncnn and Vulka
-000015d0: 6e20 6c69 6272 6172 6965 732e 0a2d 205b  n libraries..- [
-000015e0: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
-000015f0: 7675 6c6b 616e 5d28 6874 7470 733a 2f2f  vulkan](https://
-00001600: 6769 7468 7562 2e63 6f6d 2f6e 6968 7569  github.com/nihui
-00001610: 2f73 726d 642d 6e63 6e6e 2d76 756c 6b61  /srmd-ncnn-vulka
-00001620: 6e29 202d 2054 6869 7320 7072 6f6a 6563  n) - This projec
-00001630: 7420 7072 6f76 6964 6564 2074 6865 2063  t provided the c
-00001640: 6f72 6520 696d 706c 656d 656e 7461 7469  ore implementati
-00001650: 6f6e 206f 660a 2020 7468 6520 5352 4d44  on of.  the SRMD
-00001660: 2061 6c67 6f72 6974 686d 2075 7369 6e67   algorithm using
-00001670: 2074 6865 206e 636e 6e20 616e 6420 5675   the ncnn and Vu
-00001680: 6c6b 616e 206c 6962 7261 7269 6573 2e0a  lkan libraries..
-00001690: 2d20 5b72 6561 6c63 7567 616e 2d6e 636e  - [realcugan-ncn
-000016a0: 6e2d 7079 5d28 6874 7470 733a 2f2f 6769  n-py](https://gi
-000016b0: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
-000016c0: 792f 7265 616c 6375 6761 6e2d 6e63 6e6e  y/realcugan-ncnn
-000016d0: 2d70 7929 202d 2054 6869 7320 7072 6f6a  -py) - This proj
-000016e0: 6563 7420 7072 6f76 6964 6564 2074 6865  ect provided the
-000016f0: 2050 7974 686f 6e20 4269 6e64 696e 6720   Python Binding 
-00001700: 666f 720a 2020 7265 616c 6375 6761 6e2d  for.  realcugan-
-00001710: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
-00001720: 2050 7942 696e 6431 310a 2d20 5b72 6561   PyBind11.- [rea
-00001730: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 795d  lesrgan-ncnn-py]
-00001740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001750: 636f 6d2f 546f 6872 7573 6b79 2f72 6561  com/Tohrusky/rea
-00001760: 6c65 7372 6761 6e2d 6e63 6e6e 2d70 7929  lesrgan-ncnn-py)
-00001770: 202d 2054 6869 7320 7072 6f6a 6563 7420   - This project 
-00001780: 7072 6f76 6964 6564 2074 6865 2050 7974  provided the Pyt
-00001790: 686f 6e20 4269 6e64 696e 6720 666f 720a  hon Binding for.
-000017a0: 2020 7265 616c 6573 7267 616e 2d6e 636e    realesrgan-ncn
-000017b0: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
-000017c0: 4269 6e64 3131 0a2d 205b 7761 6966 7532  Bind11.- [waifu2
-000017d0: 782d 6e63 6e6e 2d70 795d 2868 7474 7073  x-ncnn-py](https
-000017e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
-000017f0: 6872 7573 6b79 2f77 6169 6675 3278 2d6e  hrusky/waifu2x-n
-00001800: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
-00001810: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
-00001820: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
-00001830: 6e67 2066 6f72 0a20 2077 6169 6675 3278  ng for.  waifu2x
-00001840: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
-00001850: 6820 5079 4269 6e64 3131 0a2d 205b 7372  h PyBind11.- [sr
-00001860: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
-00001870: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00001880: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
-00001890: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
-000018a0: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
-000018b0: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
-000018c0: 2066 6f72 0a20 2073 726d 642d 6e63 6e6e   for.  srmd-ncnn
-000018d0: 2d76 756c 6b61 6e0a 2020 7769 7468 2050  -vulkan.  with P
-000018e0: 7942 696e 6431 310a 0a23 204c 6963 656e  yBind11..# Licen
-000018f0: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00001900: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00001910: 6572 2074 6865 2042 5344 2033 2d43 6c61  er the BSD 3-Cla
-00001920: 7573 6520 2d20 7365 650a 7468 6520 5b4c  use - see.the [L
-00001930: 4943 454e 5345 2066 696c 655d 2868 7474  ICENSE file](htt
-00001940: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001950: 546f 6872 7573 6b79 2f46 696e 616c 3278  Tohrusky/Final2x
-00001960: 2d63 6f72 652f 626c 6f62 2f6d 6169 6e2f  -core/blob/main/
-00001970: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
-00001980: 6169 6c73 2e0a                           ails..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 4669 6e61  : 2.1.Name: Fina
+00000020: 6c32 782d 636f 7265 0a56 6572 7369 6f6e  l2x-core.Version
+00000030: 3a20 312e 302e 330a 5375 6d6d 6172 793a  : 1.0.3.Summary:
+00000040: 2055 4e4b 4e4f 574e 0a48 6f6d 652d 7061   UNKNOWN.Home-pa
+00000050: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+00000060: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
+00000070: 4669 6e61 6c32 782d 636f 7265 0a41 7574  Final2x-core.Aut
+00000080: 686f 723a 2054 6f68 7275 736b 790a 4c69  hor: Tohrusky.Li
+00000090: 6365 6e73 653a 2055 4e4b 4e4f 574e 0a50  cense: UNKNOWN.P
+000000a0: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
+000000b0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
+000000c0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+000000d0: 3a3a 2033 202d 2041 6c70 6861 0a43 6c61  :: 3 - Alpha.Cla
+000000e0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+000000f0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000100: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
+00000110: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+00000120: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000130: 4253 4420 4c69 6365 6e73 650a 436c 6173  BSD License.Clas
+00000140: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000160: 5079 7468 6f6e 203a 3a20 332e 360a 436c  Python :: 3.6.Cl
+00000170: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000180: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000190: 3a20 5079 7468 6f6e 203a 3a20 332e 370a  : Python :: 3.7.
+000001a0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001d0: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
+000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000200: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000230: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+00000240: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000260: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
+00000270: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
+00000280: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000290: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000002a0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+000002b0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+000002c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002d0: 2f73 6f63 6961 6c69 6679 2e67 6974 2e63  /socialify.git.c
+000002e0: 692f 546f 6872 7573 6b79 2f46 696e 616c  i/Tohrusky/Final
+000002f0: 3278 2d63 6f72 652f 696d 6167 653f 6465  2x-core/image?de
+00000300: 7363 7269 7074 696f 6e3d 3126 666f 726b  scription=1&fork
+00000310: 733d 3126 6973 7375 6573 3d31 266c 616e  s=1&issues=1&lan
+00000320: 6775 6167 653d 3126 6c6f 676f 3d68 7474  guage=1&logo=htt
+00000330: 7073 2533 4125 3246 2532 4672 6177 2e67  ps%3A%2F%2Fraw.g
+00000340: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000350: 2e63 6f6d 2532 4654 6f68 7275 736b 7925  .com%2FTohrusky%
+00000360: 3246 546f 6872 7573 6b79 2532 466d 6169  2FTohrusky%2Fmai
+00000370: 6e25 3246 6963 6f6e 2532 466c 6f67 6f2e  n%2Ficon%2Flogo.
+00000380: 706e 6726 6e61 6d65 3d31 2670 6174 7465  png&name=1&patte
+00000390: 726e 3d43 6972 6375 6974 2532 3042 6f61  rn=Circuit%20Boa
+000003a0: 7264 2670 756c 6c73 3d31 2673 7461 7267  rd&pulls=1&starg
+000003b0: 617a 6572 733d 3126 7468 656d 653d 4c69  azers=1&theme=Li
+000003c0: 6768 7422 3e0a 2020 3c70 6963 7475 7265  ght">.  <picture
+000003d0: 3e0a 2020 2020 3c73 6f75 7263 6520 6d65  >.    <source me
+000003e0: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
+000003f0: 6c6f 722d 7363 6865 6d65 3a20 6461 726b  lor-scheme: dark
+00000400: 2922 2073 7263 7365 743d 2268 7474 7073  )" srcset="https
+00000410: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+00000420: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+00000430: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+00000440: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+00000450: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+00000460: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+00000470: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+00000480: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000490: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+000004a0: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+000004b0: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+000004c0: 6f2d 6461 726b 2e70 6e67 266e 616d 653d  o-dark.png&name=
+000004d0: 3126 7061 7474 6572 6e3d 4369 7263 7569  1&pattern=Circui
+000004e0: 7425 3230 426f 6172 6426 7075 6c6c 733d  t%20Board&pulls=
+000004f0: 3126 7374 6172 6761 7a65 7273 3d31 2674  1&stargazers=1&t
+00000500: 6865 6d65 3d44 6172 6b22 202f 3e0a 2020  heme=Dark" />.  
+00000510: 2020 3c73 6f75 7263 6520 6d65 6469 613d    <source media=
+00000520: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
+00000530: 7363 6865 6d65 3a20 6c69 6768 7429 2220  scheme: light)" 
+00000540: 7372 6373 6574 3d22 6874 7470 733a 2f2f  srcset="https://
+00000550: 736f 6369 616c 6966 792e 6769 742e 6369  socialify.git.ci
+00000560: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000570: 782d 636f 7265 2f69 6d61 6765 3f64 6573  x-core/image?des
+00000580: 6372 6970 7469 6f6e 3d31 2666 6f72 6b73  cription=1&forks
+00000590: 3d31 2669 7373 7565 733d 3126 6c61 6e67  =1&issues=1&lang
+000005a0: 7561 6765 3d31 266c 6f67 6f3d 6874 7470  uage=1&logo=http
+000005b0: 7325 3341 2532 4625 3246 7261 772e 6769  s%3A%2F%2Fraw.gi
+000005c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000005d0: 636f 6d25 3246 546f 6872 7573 6b79 2532  com%2FTohrusky%2
+000005e0: 4654 6f68 7275 736b 7925 3246 6d61 696e  FTohrusky%2Fmain
+000005f0: 2532 4669 636f 6e25 3246 6c6f 676f 2e70  %2Ficon%2Flogo.p
+00000600: 6e67 266e 616d 653d 3126 7061 7474 6572  ng&name=1&patter
+00000610: 6e3d 4369 7263 7569 7425 3230 426f 6172  n=Circuit%20Boar
+00000620: 6426 7075 6c6c 733d 3126 7374 6172 6761  d&pulls=1&starga
+00000630: 7a65 7273 3d31 2674 6865 6d65 3d4c 6967  zers=1&theme=Lig
+00000640: 6874 2220 2f3e 0a20 2020 203c 696d 6720  ht" />.    <img 
+00000650: 616c 743d 2253 6f63 6961 6c69 6679 2049  alt="Socialify I
+00000660: 6d61 6765 2220 7372 633d 2268 7474 7073  mage" src="https
+00000670: 3a2f 2f73 6f63 6961 6c69 6679 2e67 6974  ://socialify.git
+00000680: 2e63 692f 546f 6872 7573 6b79 2f46 696e  .ci/Tohrusky/Fin
+00000690: 616c 3278 2d63 6f72 652f 696d 6167 653f  al2x-core/image?
+000006a0: 6465 7363 7269 7074 696f 6e3d 3126 666f  description=1&fo
+000006b0: 726b 733d 3126 6973 7375 6573 3d31 266c  rks=1&issues=1&l
+000006c0: 616e 6775 6167 653d 3126 6c6f 676f 3d68  anguage=1&logo=h
+000006d0: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
+000006e0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000006f0: 6e74 2e63 6f6d 2532 4654 6f68 7275 736b  nt.com%2FTohrusk
+00000700: 7925 3246 546f 6872 7573 6b79 2532 466d  y%2FTohrusky%2Fm
+00000710: 6169 6e25 3246 6963 6f6e 2532 466c 6f67  ain%2Ficon%2Flog
+00000720: 6f2e 706e 6726 6e61 6d65 3d31 2670 6174  o.png&name=1&pat
+00000730: 7465 726e 3d43 6972 6375 6974 2532 3042  tern=Circuit%20B
+00000740: 6f61 7264 2670 756c 6c73 3d31 2673 7461  oard&pulls=1&sta
+00000750: 7267 617a 6572 733d 3126 7468 656d 653d  rgazers=1&theme=
+00000760: 4c69 6768 7422 202f 3e0a 2020 3c2f 7069  Light" />.  </pi
+00000770: 6374 7572 653e 0a3c 2f61 3e0a 0a0a 215b  cture>.</a>...![
+00000780: 4d61 634f 5320 7836 345d 2868 7474 7073  MacOS x64](https
+00000790: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000007a0: 6f2f 6261 6467 652f 5375 7070 6f72 742d  o/badge/Support-
+000007b0: 4d61 634f 5325 3230 7836 342d 626c 7565  MacOS%20x64-blue
+000007c0: 3f6c 6f67 6f3d 4170 706c 6526 7374 796c  ?logo=Apple&styl
+000007d0: 653d 666c 6174 2d73 7175 6172 6529 0a21  e=flat-square).!
+000007e0: 5b4d 6163 4f53 2061 726d 3634 5d28 6874  [MacOS arm64](ht
+000007f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000800: 732e 696f 2f62 6164 6765 2f53 7570 706f  s.io/badge/Suppo
+00000810: 7274 2d4d 6163 4f53 2532 3061 726d 3634  rt-MacOS%20arm64
+00000820: 2d62 6c75 653f 6c6f 676f 3d41 7070 6c65  -blue?logo=Apple
+00000830: 2673 7479 6c65 3d66 6c61 742d 7371 7561  &style=flat-squa
+00000840: 7265 290a 215b 5769 6e64 6f77 7320 7836  re).![Windows x6
+00000850: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+00000860: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000870: 5375 7070 6f72 742d 5769 6e64 6f77 7325  Support-Windows%
+00000880: 3230 7836 342d 626c 7565 3f6c 6f67 6f3d  20x64-blue?logo=
+00000890: 5769 6e64 6f77 7326 7374 796c 653d 666c  Windows&style=fl
+000008a0: 6174 2d73 7175 6172 6529 0a21 5b57 696e  at-square).![Win
+000008b0: 646f 7773 2061 726d 3634 5d28 6874 7470  dows arm64](http
+000008c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000008d0: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
+000008e0: 2d57 696e 646f 7773 2532 3061 726d 3634  -Windows%20arm64
+000008f0: 2d62 6c75 653f 6c6f 676f 3d57 696e 646f  -blue?logo=Windo
+00000900: 7773 2673 7479 6c65 3d66 6c61 742d 7371  ws&style=flat-sq
+00000910: 7561 7265 290a 215b 4c69 6e75 7820 7836  uare).![Linux x6
+00000920: 345d 2868 7474 7073 3a2f 2f69 6d67 2e73  4](https://img.s
+00000930: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000940: 5375 7070 6f72 742d 4c69 6e75 7825 3230  Support-Linux%20
+00000950: 7836 342d 626c 7565 3f6c 6f67 6f3d 4c69  x64-blue?logo=Li
+00000960: 6e75 7826 7374 796c 653d 666c 6174 2d73  nux&style=flat-s
+00000970: 7175 6172 6529 0a5b 215b 636f 6465 636f  quare).[![codeco
+00000980: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000990: 6f76 2e69 6f2f 6768 2f54 6f68 7275 736b  ov.io/gh/Tohrusk
+000009a0: 792f 4669 6e61 6c32 782d 636f 7265 2f62  y/Final2x-core/b
+000009b0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+000009c0: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+000009d0: 3d42 3254 4e4b 594e 344f 3429 5d28 6874  =B2TNKYN4O4)](ht
+000009e0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000009f0: 2f67 682f 546f 6872 7573 6b79 2f46 696e  /gh/Tohrusky/Fin
+00000a00: 616c 3278 2d63 6f72 6529 0a5b 215b 4349  al2x-core).[![CI
+00000a10: 2d74 6573 745d 2868 7474 7073 3a2f 2f67  -test](https://g
+00000a20: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+00000a30: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+00000a40: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000a50: 732f 4349 2d74 6573 742e 796d 6c2f 6261  s/CI-test.yml/ba
+00000a60: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000a70: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00000a80: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+00000a90: 7265 2f61 6374 696f 6e73 2f77 6f72 6b66  re/actions/workf
+00000aa0: 6c6f 7773 2f43 492d 7465 7374 2e79 6d6c  lows/CI-test.yml
+00000ab0: 290a 5b21 5b43 492d 6275 696c 645d 2868  ).[![CI-build](h
+00000ac0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ad0: 6d2f 546f 6872 7573 6b79 2f46 696e 616c  m/Tohrusky/Final
+00000ae0: 3278 2d63 6f72 652f 6163 7469 6f6e 732f  2x-core/actions/
+00000af0: 776f 726b 666c 6f77 732f 4349 2d62 7569  workflows/CI-bui
+00000b00: 6c64 2e79 6d6c 2f62 6164 6765 2e73 7667  ld.yml/badge.svg
+00000b10: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000b20: 622e 636f 6d2f 546f 6872 7573 6b79 2f46  b.com/Tohrusky/F
+00000b30: 696e 616c 3278 2d63 6f72 652f 6163 7469  inal2x-core/acti
+00000b40: 6f6e 732f 776f 726b 666c 6f77 732f 4349  ons/workflows/CI
+00000b50: 2d62 7569 6c64 2e79 6d6c 290a 5b21 5b52  -build.yml).[![R
+00000b60: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00000b70: 6769 7468 7562 2e63 6f6d 2f54 6f68 7275  github.com/Tohru
+00000b80: 736b 792f 4669 6e61 6c32 782d 636f 7265  sky/Final2x-core
+00000b90: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000ba0: 7773 2f52 656c 6561 7365 2e79 6d6c 2f62  ws/Release.yml/b
+00000bb0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000bc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 546f  ://github.com/To
+00000bd0: 6872 7573 6b79 2f46 696e 616c 3278 2d63  hrusky/Final2x-c
+00000be0: 6f72 652f 6163 7469 6f6e 732f 776f 726b  ore/actions/work
+00000bf0: 666c 6f77 732f 5265 6c65 6173 652e 796d  flows/Release.ym
+00000c00: 6c29 0a5b 215b 5049 502d 7465 7374 5d28  l).[![PIP-test](
+00000c10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000c20: 6f6d 2f54 6f68 7275 736b 792f 4669 6e61  om/Tohrusky/Fina
+00000c30: 6c32 782d 636f 7265 2f61 6374 696f 6e73  l2x-core/actions
+00000c40: 2f77 6f72 6b66 6c6f 7773 2f50 4950 2d74  /workflows/PIP-t
+00000c50: 6573 742e 796d 6c2f 6261 6467 652e 7376  est.yml/badge.sv
+00000c60: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000c70: 7562 2e63 6f6d 2f54 6f68 7275 736b 792f  ub.com/Tohrusky/
+00000c80: 4669 6e61 6c32 782d 636f 7265 2f61 6374  Final2x-core/act
+00000c90: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f50  ions/workflows/P
+00000ca0: 4950 2d74 6573 742e 796d 6c29 0a5b 215b  IP-test.yml).[![
+00000cb0: 5265 6c65 6173 652d 7079 7069 5d28 6874  Release-pypi](ht
+00000cc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000cd0: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000ce0: 782d 636f 7265 2f61 6374 696f 6e73 2f77  x-core/actions/w
+00000cf0: 6f72 6b66 6c6f 7773 2f52 656c 6561 7365  orkflows/Release
+00000d00: 2d70 7970 692e 796d 6c2f 6261 6467 652e  -pypi.yml/badge.
+00000d10: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000d20: 7468 7562 2e63 6f6d 2f54 6f68 7275 736b  thub.com/Tohrusk
+00000d30: 792f 4669 6e61 6c32 782d 636f 7265 2f61  y/Final2x-core/a
+00000d40: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000d50: 2f52 656c 6561 7365 2d70 7970 692e 796d  /Release-pypi.ym
+00000d60: 6c29 0a5b 215b 5079 5049 2076 6572 7369  l).[![PyPI versi
+00000d70: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000d80: 652e 6675 7279 2e69 6f2f 7079 2f46 696e  e.fury.io/py/Fin
+00000d90: 616c 3278 2d63 6f72 652e 7376 6729 5d28  al2x-core.svg)](
+00000da0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000db0: 7279 2e69 6f2f 7079 2f46 696e 616c 3278  ry.io/py/Final2x
+00000dc0: 2d63 6f72 6529 0a21 5b47 6974 4875 625d  -core).![GitHub]
+00000dd0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000de0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000df0: 6963 656e 7365 2f54 6f68 7275 736b 792f  icense/Tohrusky/
+00000e00: 4669 6e61 6c32 782d 636f 7265 290a 0a46  Final2x-core)..F
+00000e10: 696e 616c 3278 2d63 6f72 6520 6973 2061  inal2x-core is a
+00000e20: 2063 726f 7373 2d70 6c61 7466 6f72 6d20   cross-platform 
+00000e30: 696d 6167 6520 7375 7065 722d 7265 736f  image super-reso
+00000e40: 6c75 7469 6f6e 2043 4c49 2074 6f6f 6c20  lution CLI tool 
+00000e50: 666f 7220 5b46 696e 616c 3278 5d28 6874  for [Final2x](ht
+00000e60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e70: 2f54 6f68 7275 736b 792f 4669 6e61 6c32  /Tohrusky/Final2
+00000e80: 7829 2e20 4966 2079 6f75 2068 6176 6520  x). If you have 
+00000e90: 616e 7920 7175 6573 7469 6f6e 732c 2070  any questions, p
+00000ea0: 6c65 6173 6520 7261 6973 6520 616e 2069  lease raise an i
+00000eb0: 7373 7565 205b 696e 2074 6869 7320 7265  ssue [in this re
+00000ec0: 706f 7369 746f 7279 5d28 6874 7470 733a  pository](https:
+00000ed0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00000ee0: 7275 736b 792f 4669 6e61 6c32 7829 2e0a  rusky/Final2x)..
+00000ef0: 0a23 2049 6e73 7461 6c6c 0a0a 446f 776e  .# Install..Down
+00000f00: 6c6f 6164 2069 6e20 5b52 656c 6561 7365  load in [Release
+00000f10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000f20: 2e63 6f6d 2f54 6f68 7275 736b 792f 4669  .com/Tohrusky/Fi
+00000f30: 6e61 6c32 782d 636f 7265 2f72 656c 6561  nal2x-core/relea
+00000f40: 7365 7329 206f 7220 7573 6520 7069 7020  ses) or use pip 
+00000f50: 2870 7974 686f 6e20 3e3d 2033 2e36 2c20  (python >= 3.6, 
+00000f60: 3e3d 332e 3920 666f 7220 4d61 634f 530a  >=3.9 for MacOS.
+00000f70: 6172 6d36 3429 0a0a 6060 6073 6865 6c6c  arm64)..```shell
+00000f80: 0a70 6970 2069 6e73 7461 6c6c 2046 696e  .pip install Fin
+00000f90: 616c 3278 2d63 6f72 650a 6060 600a 0a23  al2x-core.```..#
+00000fa0: 2055 7365 0a0a 6060 6073 6865 6c6c 0a75   Use..```shell.u
+00000fb0: 7361 6765 3a20 4669 6e61 6c32 782d 636f  sage: Final2x-co
+00000fc0: 7265 205b 2d68 5d20 5b2d 6220 4241 5345  re [-h] [-b BASE
+00000fd0: 3634 5d20 5b2d 6a20 4a53 4f4e 5d20 5b2d  64] [-j JSON] [-
+00000fe0: 7920 5941 4d4c 5d20 5b2d 6f5d 0a0a 7768  y YAML] [-o]..wh
+00000ff0: 656e 2070 6172 6120 6973 206e 6f74 2073  en para is not s
+00001000: 7065 6369 6669 6564 2c20 7468 6520 636f  pecified, the co
+00001010: 6e66 6967 2e79 616d 6c20 6669 6c65 2069  nfig.yaml file i
+00001020: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
+00001030: 7769 6c6c 2062 6520 7265 6164 2061 7574  will be read aut
+00001040: 6f6d 6174 6963 616c 6c79 0a0a 6f70 7469  omatically..opti
+00001050: 6f6e 616c 2061 7267 756d 656e 7473 3a0a  onal arguments:.
+00001060: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+00001070: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
+00001080: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
+00001090: 6e64 2065 7869 740a 2020 2d62 2042 4153  nd exit.  -b BAS
+000010a0: 4536 342c 202d 2d42 4153 4536 3420 4241  E64, --BASE64 BA
+000010b0: 5345 3634 0a20 2020 2020 2020 2020 2020  SE64.           
+000010c0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+000010d0: 6536 3420 7374 7269 6e67 2066 6f72 2063  e64 string for c
+000010e0: 6f6e 6669 6720 6a73 6f6e 0a20 202d 6a20  onfig json.  -j 
+000010f0: 4a53 4f4e 2c20 2d2d 4a53 4f4e 204a 534f  JSON, --JSON JSO
+00001100: 4e20 204a 534f 4e20 7374 7269 6e67 2066  N  JSON string f
+00001110: 6f72 2063 6f6e 6669 670a 2020 2d79 2059  or config.  -y Y
+00001120: 414d 4c2c 202d 2d59 414d 4c20 5941 4d4c  AML, --YAML YAML
+00001130: 2020 7961 6d6c 2063 6f6e 6669 6720 6669    yaml config fi
+00001140: 6c65 2070 6174 680a 2020 2d6c 2c20 2d2d  le path.  -l, --
+00001150: 4c4f 4720 2020 2020 2020 2020 2020 2020  LOG             
+00001160: 7361 7665 206c 6f67 0a20 202d 6f2c 202d  save log.  -o, -
+00001170: 2d4f 5020 2020 2020 2020 2020 2020 2020  -OP             
+00001180: 2063 6865 636b 2069 6e73 7461 6c6c 0a60   check install.`
+00001190: 6060 0a0a 2320 436f 6e66 6967 0a0a 5061  ``..# Config..Pa
+000011a0: 7373 2074 6865 2063 6f6e 6669 6720 6a73  ss the config js
+000011b0: 6f6e 2073 7472 696e 6720 746f 2074 6865  on string to the
+000011c0: 2070 726f 6772 616d 2074 6872 6f75 6768   program through
+000011d0: 2074 6865 2060 2d6a 6020 7061 7261 6d65   the `-j` parame
+000011e0: 7465 722e 0a0a 2a2a 504c 4541 5345 204e  ter...**PLEASE N
+000011f0: 4f54 453a 2074 6865 2063 6f6e 6669 6720  OTE: the config 
+00001200: 6973 204a 534f 4e2c 2072 656d 6f76 6520  is JSON, remove 
+00001210: 7468 6520 2f2f 2063 6f6d 6d65 6e74 7320  the // comments 
+00001220: 6265 666f 7265 2075 7365 2e2a 2a0a 0a60  before use.**..`
+00001230: 6060 6a73 6f6e 0a7b 0a20 2022 6770 7569  ``json.{.  "gpui
+00001240: 6422 3a20 302c 0a20 202f 2f20 4750 5520  d": 0,.  // GPU 
+00001250: 6964 2c20 3e3d 202d 3120 282d 3120 666f  id, >= -1 (-1 fo
+00001260: 7220 4350 552c 206d 6179 206e 6f74 2077  r CPU, may not w
+00001270: 6f72 6b20 666f 7220 736f 6d65 206d 6f64  ork for some mod
+00001280: 656c 732e 290a 2020 2269 6e70 7574 7061  els.).  "inputpa
+00001290: 7468 223a 205b 0a20 2020 202f 2f20 496e  th": [.    // In
+000012a0: 7075 7420 696d 6167 6520 7061 7468 732c  put image paths,
+000012b0: 2073 686f 756c 6420 6265 2061 206c 6973   should be a lis
+000012c0: 742e 0a20 2020 2022 7061 7468 2f74 6f2f  t..    "path/to/
+000012d0: 696d 6731 2e6a 7067 222c 0a20 2020 2022  img1.jpg",.    "
+000012e0: 7061 7468 2f74 6f2f 696d 6732 2e70 6e67  path/to/img2.png
+000012f0: 220a 2020 5d2c 0a20 2022 6d6f 6465 6c22  ".  ],.  "model"
+00001300: 3a20 2252 6561 6c43 5547 414e 2d70 726f  : "RealCUGAN-pro
+00001310: 222c 0a20 202f 2f20 6d6f 6465 6c20 6e61  ",.  // model na
+00001320: 6d65 0a20 2022 6d6f 6465 6c73 6361 6c65  me.  "modelscale
+00001330: 223a 2032 2c0a 2020 2f2f 206d 6f64 656c  ": 2,.  // model
+00001340: 2075 7073 6361 6c65 2066 6163 746f 720a   upscale factor.
+00001350: 2020 226d 6f64 656c 6e6f 6973 6522 3a20    "modelnoise": 
+00001360: 2d31 2c0a 2020 2f2f 2044 454e 4f49 5345  -1,.  // DENOISE
+00001370: 206c 6576 656c 0a20 2022 6f75 7470 7574   level.  "output
+00001380: 7061 7468 223a 2022 7061 7468 2f74 6f2f  path": "path/to/
+00001390: 6f75 7470 7574 222c 0a20 202f 2f20 6f75  output",.  // ou
+000013a0: 7470 7574 2070 6174 680a 2020 2274 6172  tput path.  "tar
+000013b0: 6765 7473 6361 6c65 223a 2032 2e30 2c0a  getscale": 2.0,.
+000013c0: 2020 2f2f 2054 6172 6765 7420 7570 7363    // Target upsc
+000013d0: 616c 6520 6661 6374 6f72 2c20 7570 7363  ale factor, upsc
+000013e0: 616c 6520 6d75 6c74 6970 6c65 2074 696d  ale multiple tim
+000013f0: 6573 2074 6f20 6163 6869 6576 6520 7468  es to achieve th
+00001400: 6520 7461 7267 6574 2075 7073 6361 6c65  e target upscale
+00001410: 2066 6163 746f 722e 0a20 202f 2f20 4966   factor..  // If
+00001420: 206e 6f74 2069 6e76 616c 6964 2c20 7573   not invalid, us
+00001430: 6520 6d6f 6465 6c73 6361 6c65 2e0a 2020  e modelscale..  
+00001440: 2274 7461 223a 2066 616c 7365 0a20 202f  "tta": false.  /
+00001450: 2f20 5465 7374 2054 696d 6520 4175 676d  / Test Time Augm
+00001460: 656e 7461 7469 6f6e 2c20 6465 6661 756c  entation, defaul
+00001470: 7420 6661 6c73 650a 7d0a 6060 600a 0a2a  t false.}.```..*
+00001480: 2a53 5550 504f 5254 4544 204d 4f44 454c  *SUPPORTED MODEL
+00001490: 204c 4953 543a 2a2a 0a0a 6060 6079 616d   LIST:**..```yam
+000014a0: 6c0a 2d20 5265 616c 4355 4741 4e2d 7365  l.- RealCUGAN-se
+000014b0: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+000014c0: 5265 616c 4355 4741 4e2d 7365 220a 2020  RealCUGAN-se".  
+000014d0: 2020 2d20 7363 616c 653a 2032 0a20 2020    - scale: 2.   
+000014e0: 2020 2020 2020 2020 2020 2020 2d20 6e6f              - no
+000014f0: 6973 653a 202d 312c 2030 2c20 312c 2032  ise: -1, 0, 1, 2
+00001500: 2c20 330a 2020 2020 2d20 7363 616c 653a  , 3.    - scale:
+00001510: 2033 2c20 340a 2020 2020 2020 2020 2020   3, 4.          
+00001520: 2020 2020 202d 206e 6f69 7365 3a20 2d31       - noise: -1
+00001530: 2c20 302c 2033 0a0a 2d20 5265 616c 4355  , 0, 3..- RealCU
+00001540: 4741 4e2d 7072 6f3a 0a20 2020 202d 206d  GAN-pro:.    - m
+00001550: 6f64 656c 3a20 2252 6561 6c43 5547 414e  odel: "RealCUGAN
+00001560: 2d70 726f 220a 2020 2020 2d20 7363 616c  -pro".    - scal
+00001570: 653a 2032 2c20 330a 2020 2020 2d20 6e6f  e: 2, 3.    - no
+00001580: 6973 653a 202d 312c 2030 2c20 330a 0a2d  ise: -1, 0, 3..-
+00001590: 2052 6561 6c45 5352 4741 4e2d 616e 696d   RealESRGAN-anim
+000015a0: 6576 6964 656f 7633 3a0a 2020 2020 2d20  evideov3:.    - 
+000015b0: 6770 7569 643a 203e 3d20 300a 2020 2020  gpuid: >= 0.    
+000015c0: 2d20 6d6f 6465 6c3a 2022 5265 616c 4553  - model: "RealES
+000015d0: 5247 414e 2d61 6e69 6d65 7669 6465 6f76  RGAN-animevideov
+000015e0: 3322 0a20 2020 202d 2073 6361 6c65 3a20  3".    - scale: 
+000015f0: 322c 2033 2c20 340a 0a2d 2052 6561 6c45  2, 3, 4..- RealE
+00001600: 5352 4741 4e3a 0a20 2020 202d 2067 7075  SRGAN:.    - gpu
+00001610: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+00001620: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+00001630: 4e22 0a20 2020 202d 2073 6361 6c65 3a20  N".    - scale: 
+00001640: 340a 0a2d 2052 6561 6c45 5352 4741 4e2d  4..- RealESRGAN-
+00001650: 616e 696d 653a 0a20 2020 202d 2067 7075  anime:.    - gpu
+00001660: 6964 3a20 3e3d 2030 0a20 2020 202d 206d  id: >= 0.    - m
+00001670: 6f64 656c 3a20 2252 6561 6c45 5352 4741  odel: "RealESRGA
+00001680: 4e2d 616e 696d 6522 0a20 2020 202d 2073  N-anime".    - s
+00001690: 6361 6c65 3a20 340a 0a2d 2057 6169 6675  cale: 4..- Waifu
+000016a0: 3278 2d63 756e 6574 3a0a 2020 2020 2d20  2x-cunet:.    - 
+000016b0: 6d6f 6465 6c3a 2022 5761 6966 7532 782d  model: "Waifu2x-
+000016c0: 6375 6e65 7422 0a20 2020 202d 2073 6361  cunet".    - sca
+000016d0: 6c65 3a20 310a 2020 2020 2020 2020 2020  le: 1.          
+000016e0: 2020 2020 202d 206e 6f69 7365 3a20 302c       - noise: 0,
+000016f0: 2031 2c20 322c 2033 0a20 2020 202d 2073   1, 2, 3.    - s
+00001700: 6361 6c65 3a20 320a 2020 2020 2020 2020  cale: 2.        
+00001710: 2020 2020 2020 202d 206e 6f69 7365 3a20         - noise: 
+00001720: 2d31 2c20 302c 2031 2c20 322c 2033 0a0a  -1, 0, 1, 2, 3..
+00001730: 2d20 5761 6966 7532 782d 7570 636f 6e76  - Waifu2x-upconv
+00001740: 5f37 5f61 6e69 6d65 5f73 7479 6c65 5f61  _7_anime_style_a
+00001750: 7274 5f72 6762 3a0a 2020 2020 2d20 6d6f  rt_rgb:.    - mo
+00001760: 6465 6c3a 2022 5761 6966 7532 782d 7570  del: "Waifu2x-up
+00001770: 636f 6e76 5f37 5f61 6e69 6d65 5f73 7479  conv_7_anime_sty
+00001780: 6c65 5f61 7274 5f72 6762 220a 2020 2020  le_art_rgb".    
+00001790: 2d20 7363 616c 653a 2032 0a20 2020 202d  - scale: 2.    -
+000017a0: 206e 6f69 7365 3a20 2d31 2c20 302c 2031   noise: -1, 0, 1
+000017b0: 2c20 322c 2033 0a0a 2d20 5761 6966 7532  , 2, 3..- Waifu2
+000017c0: 782d 7570 636f 6e76 5f37 5f70 686f 746f  x-upconv_7_photo
+000017d0: 3a0a 2020 2020 2d20 6d6f 6465 6c3a 2022  :.    - model: "
+000017e0: 5761 6966 7532 782d 7570 636f 6e76 5f37  Waifu2x-upconv_7
+000017f0: 5f70 686f 746f 220a 2020 2020 2d20 7363  _photo".    - sc
+00001800: 616c 653a 2032 0a20 2020 202d 206e 6f69  ale: 2.    - noi
+00001810: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+00001820: 2033 0a0a 2d20 5352 4d44 3a0a 2020 2020   3..- SRMD:.    
+00001830: 2d20 6770 7569 643a 203e 3d20 300a 2020  - gpuid: >= 0.  
+00001840: 2020 2d20 6d6f 6465 6c3a 2022 5352 4d44    - model: "SRMD
+00001850: 220a 2020 2020 2d20 7363 616c 653a 2032  ".    - scale: 2
+00001860: 2c20 332c 2034 0a20 2020 202d 206e 6f69  , 3, 4.    - noi
+00001870: 7365 3a20 2d31 2c20 302c 2031 2c20 322c  se: -1, 0, 1, 2,
+00001880: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+00001890: 382c 2039 2c20 3130 0a60 6060 0a0a 2320  8, 9, 10.```..# 
+000018a0: 4275 696c 640a 0a5b 4769 7468 7562 2041  Build..[Github A
+000018b0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f67  ction](https://g
+000018c0: 6974 6875 622e 636f 6d2f 546f 6872 7573  ithub.com/Tohrus
+000018d0: 6b79 2f46 696e 616c 3278 2d63 6f72 652f  ky/Final2x-core/
+000018e0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000018f0: 732f 4349 2d62 7569 6c64 2e79 6d6c 290a  s/CI-build.yml).
+00001900: 0a2a 5468 6520 7072 6f6a 6563 7420 6a75  .*The project ju
+00001910: 7374 206f 6e6c 7920 6265 656e 2074 6573  st only been tes
+00001920: 7465 6420 696e 2055 6275 6e74 7520 3138  ted in Ubuntu 18
+00001930: 2b20 616e 6420 4465 6269 616e 2039 2b20  + and Debian 9+ 
+00001940: 656e 7669 726f 6e6d 656e 7473 206f 6e20  environments on 
+00001950: 4c69 6e75 782c 2073 6f20 6966 2074 6865  Linux, so if the
+00001960: 2070 726f 6a65 6374 2064 6f65 7320 6e6f   project does no
+00001970: 7420 776f 726b 206f 6e0a 796f 7572 2073  t work on.your s
+00001980: 7973 7465 6d2c 2070 6c65 6173 6520 7472  ystem, please tr
+00001990: 7920 6275 696c 6469 6e67 2069 742e 2a0a  y building it.*.
+000019a0: 0a23 2052 6566 6572 656e 6365 0a0a 5468  .# Reference..Th
+000019b0: 6520 666f 6c6c 6f77 696e 6720 7265 6665  e following refe
+000019c0: 7265 6e63 6573 2077 6572 6520 7573 6564  rences were used
+000019d0: 2069 6e20 7468 6520 6465 7665 6c6f 706d   in the developm
+000019e0: 656e 7420 6f66 2074 6869 7320 7072 6f6a  ent of this proj
+000019f0: 6563 743a 0a0a 2d20 5b6e 636e 6e5d 2868  ect:..- [ncnn](h
+00001a00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a10: 6d2f 5465 6e63 656e 742f 6e63 6e6e 2920  m/Tencent/ncnn) 
+00001a20: 2d20 6e63 6e6e 2069 7320 6120 6869 6768  - ncnn is a high
+00001a30: 2d70 6572 666f 726d 616e 6365 206e 6575  -performance neu
+00001a40: 7261 6c20 6e65 7477 6f72 6b20 696e 6665  ral network infe
+00001a50: 7265 6e63 6520 6672 616d 6577 6f72 6b20  rence framework 
+00001a60: 6465 7665 6c6f 7065 6420 6279 2054 656e  developed by Ten
+00001a70: 6365 6e74 2041 4920 4c61 622e 0a2d 205b  cent AI Lab..- [
+00001a80: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+00001a90: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+00001aa0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001ab0: 6e69 6875 692f 7265 616c 6375 6761 6e2d  nihui/realcugan-
+00001ac0: 6e63 6e6e 2d76 756c 6b61 6e29 202d 2054  ncnn-vulkan) - T
+00001ad0: 6869 7320 7072 6f6a 6563 7420 7072 6f76  his project prov
+00001ae0: 6964 6564 2074 6865 2063 6f72 6520 696d  ided the core im
+00001af0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001b00: 7468 6520 5265 616c 2d43 5547 414e 2061  the Real-CUGAN a
+00001b10: 6c67 6f72 6974 686d 2075 7369 6e67 2074  lgorithm using t
+00001b20: 6865 206e 636e 6e20 616e 6420 5675 6c6b  he ncnn and Vulk
+00001b30: 616e 206c 6962 7261 7269 6573 2e0a 2d20  an libraries..- 
+00001b40: 5b78 696e 6e74 616f 2f52 6561 6c2d 4553  [xinntao/Real-ES
+00001b50: 5247 414e 2d6e 636e 6e2d 7675 6c6b 616e  RGAN-ncnn-vulkan
+00001b60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001b70: 2e63 6f6d 2f78 696e 6e74 616f 2f52 6561  .com/xinntao/Rea
+00001b80: 6c2d 4553 5247 414e 2d6e 636e 6e2d 7675  l-ESRGAN-ncnn-vu
+00001b90: 6c6b 616e 2920 2d20 5468 6973 2070 726f  lkan) - This pro
+00001ba0: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+00001bb0: 6520 636f 7265 2069 6d70 6c65 6d65 6e74  e core implement
+00001bc0: 6174 696f 6e20 6f66 2074 6865 2052 6561  ation of the Rea
+00001bd0: 6c2d 4553 5247 414e 2061 6c67 6f72 6974  l-ESRGAN algorit
+00001be0: 686d 2075 7369 6e67 2074 6865 206e 636e  hm using the ncn
+00001bf0: 6e20 616e 6420 5675 6c6b 616e 206c 6962  n and Vulkan lib
+00001c00: 7261 7269 6573 2e0a 2d20 5b6e 6968 7569  raries..- [nihui
+00001c10: 2f77 6169 6675 3278 2d6e 636e 6e2d 7675  /waifu2x-ncnn-vu
+00001c20: 6c6b 616e 5d28 6874 7470 733a 2f2f 6769  lkan](https://gi
+00001c30: 7468 7562 2e63 6f6d 2f6e 6968 7569 2f77  thub.com/nihui/w
+00001c40: 6169 6675 3278 2d6e 636e 6e2d 7675 6c6b  aifu2x-ncnn-vulk
+00001c50: 616e 2920 2d20 5468 6973 2070 726f 6a65  an) - This proje
+00001c60: 6374 2070 726f 7669 6465 6420 7468 6520  ct provided the 
+00001c70: 636f 7265 2069 6d70 6c65 6d65 6e74 6174  core implementat
+00001c80: 696f 6e20 6f66 2074 6865 2057 6169 6675  ion of the Waifu
+00001c90: 3278 2061 6c67 6f72 6974 686d 2075 7369  2x algorithm usi
+00001ca0: 6e67 2074 6865 206e 636e 6e20 616e 6420  ng the ncnn and 
+00001cb0: 5675 6c6b 616e 206c 6962 7261 7269 6573  Vulkan libraries
+00001cc0: 2e0a 2d20 5b6e 6968 7569 2f73 726d 642d  ..- [nihui/srmd-
+00001cd0: 6e63 6e6e 2d76 756c 6b61 6e5d 2868 7474  ncnn-vulkan](htt
+00001ce0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001cf0: 6e69 6875 692f 7372 6d64 2d6e 636e 6e2d  nihui/srmd-ncnn-
+00001d00: 7675 6c6b 616e 2920 2d20 5468 6973 2070  vulkan) - This p
+00001d10: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001d20: 7468 6520 636f 7265 2069 6d70 6c65 6d65  the core impleme
+00001d30: 6e74 6174 696f 6e20 6f66 2074 6865 2053  ntation of the S
+00001d40: 524d 4420 616c 676f 7269 7468 6d20 7573  RMD algorithm us
+00001d50: 696e 6720 7468 6520 6e63 6e6e 2061 6e64  ing the ncnn and
+00001d60: 2056 756c 6b61 6e20 6c69 6272 6172 6965   Vulkan librarie
+00001d70: 732e 0a2d 205b 7265 616c 6375 6761 6e2d  s..- [realcugan-
+00001d80: 6e63 6e6e 2d70 795d 2868 7474 7073 3a2f  ncnn-py](https:/
+00001d90: 2f67 6974 6875 622e 636f 6d2f 546f 6872  /github.com/Tohr
+00001da0: 7573 6b79 2f72 6561 6c63 7567 616e 2d6e  usky/realcugan-n
+00001db0: 636e 6e2d 7079 2920 2d20 5468 6973 2070  cnn-py) - This p
+00001dc0: 726f 6a65 6374 2070 726f 7669 6465 6420  roject provided 
+00001dd0: 7468 6520 5079 7468 6f6e 2042 696e 6469  the Python Bindi
+00001de0: 6e67 2066 6f72 2072 6561 6c63 7567 616e  ng for realcugan
+00001df0: 2d6e 636e 6e2d 7675 6c6b 616e 2077 6974  -ncnn-vulkan wit
+00001e00: 6820 5079 4269 6e64 3131 2e0a 2d20 5b72  h PyBind11..- [r
+00001e10: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001e20: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00001e30: 622e 636f 6d2f 546f 6872 7573 6b79 2f72  b.com/Tohrusky/r
+00001e40: 6561 6c65 7372 6761 6e2d 6e63 6e6e 2d70  ealesrgan-ncnn-p
+00001e50: 7929 202d 2054 6869 7320 7072 6f6a 6563  y) - This projec
+00001e60: 7420 7072 6f76 6964 6564 2074 6865 2050  t provided the P
+00001e70: 7974 686f 6e20 4269 6e64 696e 6720 666f  ython Binding fo
+00001e80: 7220 7265 616c 6573 7267 616e 2d6e 636e  r realesrgan-ncn
+00001e90: 6e2d 7675 6c6b 616e 2077 6974 6820 5079  n-vulkan with Py
+00001ea0: 4269 6e64 3131 2e0a 2d20 5b77 6169 6675  Bind11..- [waifu
+00001eb0: 3278 2d6e 636e 6e2d 7079 5d28 6874 7470  2x-ncnn-py](http
+00001ec0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001ed0: 6f68 7275 736b 792f 7761 6966 7532 782d  ohrusky/waifu2x-
+00001ee0: 6e63 6e6e 2d70 7929 202d 2054 6869 7320  ncnn-py) - This 
+00001ef0: 7072 6f6a 6563 7420 7072 6f76 6964 6564  project provided
+00001f00: 2074 6865 2050 7974 686f 6e20 4269 6e64   the Python Bind
+00001f10: 696e 6720 666f 7220 7761 6966 7532 782d  ing for waifu2x-
+00001f20: 6e63 6e6e 2d76 756c 6b61 6e20 7769 7468  ncnn-vulkan with
+00001f30: 2050 7942 696e 6431 312e 0a2d 205b 7372   PyBind11..- [sr
+00001f40: 6d64 2d6e 636e 6e2d 7079 5d28 6874 7470  md-ncnn-py](http
+00001f50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00001f60: 6f68 7275 736b 792f 7372 6d64 2d6e 636e  ohrusky/srmd-ncn
+00001f70: 6e2d 7079 2920 2d20 5468 6973 2070 726f  n-py) - This pro
+00001f80: 6a65 6374 2070 726f 7669 6465 6420 7468  ject provided th
+00001f90: 6520 5079 7468 6f6e 2042 696e 6469 6e67  e Python Binding
+00001fa0: 2066 6f72 2073 726d 642d 6e63 6e6e 2d76   for srmd-ncnn-v
+00001fb0: 756c 6b61 6e20 7769 7468 2050 7942 696e  ulkan with PyBin
+00001fc0: 6431 312e 0a0a 2320 4c69 6365 6e73 650a  d11...# License.
+00001fd0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001fe0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001ff0: 7468 6520 4253 4420 332d 436c 6175 7365  the BSD 3-Clause
+00002000: 202d 2073 6565 0a74 6865 205b 4c49 4345   - see.the [LICE
+00002010: 4e53 4520 6669 6c65 5d28 6874 7470 733a  NSE file](https:
+00002020: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f68  //github.com/Toh
+00002030: 7275 736b 792f 4669 6e61 6c32 782d 636f  rusky/Final2x-co
+00002040: 7265 2f62 6c6f 622f 6d61 696e 2f4c 4943  re/blob/main/LIC
+00002050: 454e 5345 2920 666f 7220 6465 7461 696c  ENSE) for detail
+00002060: 732e 0a0a 0a                             s....
```

### Comparing `Final2x-core-1.0.2/setup.py` & `Final2x-core-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-_version: str = "1.0.2"
+_version: str = "1.0.3"
 
 
 def My_find_packages(*tops):
     packages = []
     for d in tops:
         for root, dirs, files in os.walk(d, followlinks=True):
             packages.append(root)
```

