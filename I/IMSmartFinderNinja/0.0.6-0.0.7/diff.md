# Comparing `tmp/IMSmartFinderNinja-0.0.6.tar.gz` & `tmp/IMSmartFinderNinja-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMSmartFinderNinja-0.0.6.tar", last modified: Mon Jul 17 09:27:30 2023, max compression
+gzip compressed data, was "IMSmartFinderNinja-0.0.7.tar", last modified: Mon Jul 17 09:41:46 2023, max compression
```

## Comparing `IMSmartFinderNinja-0.0.6.tar` & `IMSmartFinderNinja-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:27:30.783808 IMSmartFinderNinja-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      638 2023-07-17 09:27:30.784808 IMSmartFinderNinja-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      779 2023-07-17 09:27:30.787051 IMSmartFinderNinja-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 09:27:30.745771 IMSmartFinderNinja-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 09:27:30.770162 IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/
--rw-rw-rw-   0        0        0      638 2023-07-17 09:27:30.000000 IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-17 09:27:30.000000 IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:27:30.000000 IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 09:27:30.000000 IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 09:27:30.781800 IMSmartFinderNinja-0.0.6/src/Ninja/
--rw-rw-rw-   0        0        0    23171 2023-07-17 09:26:50.000000 IMSmartFinderNinja-0.0.6/src/Ninja/Ninja_Finder.py
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.6/src/Ninja/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:41:46.090513 IMSmartFinderNinja-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      638 2023-07-17 09:41:46.091515 IMSmartFinderNinja-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      779 2023-07-17 09:41:46.095081 IMSmartFinderNinja-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 09:41:46.053443 IMSmartFinderNinja-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 09:41:46.079010 IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-07-17 09:41:46.000000 IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-17 09:41:46.000000 IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:41:46.000000 IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 09:41:46.000000 IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:41:46.088513 IMSmartFinderNinja-0.0.7/src/Ninja/
+-rw-rw-rw-   0        0        0    23198 2023-07-17 09:41:22.000000 IMSmartFinderNinja-0.0.7/src/Ninja/Ninja_Finder.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.0.7/src/Ninja/__init__.py
```

### Comparing `IMSmartFinderNinja-0.0.6/PKG-INFO` & `IMSmartFinderNinja-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.6
+Version: 0.0.7
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.6/setup.cfg` & `IMSmartFinderNinja-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2049 4d53 6d61 7274 4669 6e64 6572   = IMSmartFinder
 00000020: 4e69 6e6a 610d 0a76 6572 7369 6f6e 203d  Ninja..version =
-00000030: 2030 2e30 2e36 0d0a 6175 7468 6f72 203d   0.0.6..author =
+00000030: 2030 2e30 2e37 0d0a 6175 7468 6f72 203d   0.0.7..author =
 00000040: 204d 6f68 616d 6564 2045 6c68 616a 6162   Mohamed Elhajab
 00000050: 646f 750d 0a61 7574 686f 725f 656d 6169  dou..author_emai
 00000060: 6c20 3d20 6d6f 6861 6d65 6465 6c73 6179  l = mohamedelsay
 00000070: 6564 6d6f 6861 6d6d 6564 2e32 3032 3040  edmohammed.2020@
 00000080: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000090: 6970 7469 6f6e 203d 2074 6869 7320 7665  iption = this ve
 000000a0: 7273 696f 6e20 6973 2066 6f72 2073 6d61  rsion is for sma
```

### Comparing `IMSmartFinderNinja-0.0.6/src/IMSmartFinderNinja.egg-info/PKG-INFO` & `IMSmartFinderNinja-0.0.7/src/IMSmartFinderNinja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.0.6
+Version: 0.0.7
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.0.6/src/Ninja/Ninja_Finder.py` & `IMSmartFinderNinja-0.0.7/src/Ninja/Ninja_Finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # import bisect
 
 # warnings.filterwarnings('ignore')
 import pandas as pd
 import re
 import warnings
 import math 
-
+from fuzzywuzzy import fuzz
 
 warnings.filterwarnings('ignore')
 
 class DataProcessor:
     @staticmethod
     def clean_column_values(data_frame, column):
         data_frame[column] = data_frame[column].str.strip().str.lower().fillna('Nan')
```

