# Comparing `tmp/rest_framework_simplejwt_byforde2-0.1.4.tar.gz` & `tmp/rest_framework_simplejwt_byforde2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-cuhq8lpe\rest_framework_simplejwt_byford", last modified: Mon Jul 17 08:15:12 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-ckv9cipv\rest_framework_simplejwt_byford", last modified: Mon Jul 17 08:27:26 2023, max compression
```

## Comparing `rest_framework_simplejwt_byforde2-0.1.4.tar` & `rest_framework_simplejwt_byforde2-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.339632 rest_framework_simplejwt_byforde2-0.1.4/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 rest_framework_simplejwt_byforde2-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      634 2023-07-17 08:15:12.339632 rest_framework_simplejwt_byforde2-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-17 07:14:11.000000 rest_framework_simplejwt_byforde2-0.1.4/README.md
--rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 rest_framework_simplejwt_byforde2-0.1.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.296061 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.326353 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/
--rw-rw-rw-   0        0        0      634 2023-07-17 08:15:12.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      892 2023-07-17 08:15:12.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:15:12.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 08:15:12.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.334162 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/
--rw-rw-rw-   0        0        0      168 2023-07-17 07:32:27.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      290 2023-07-17 07:32:08.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.335629 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:15:12.338634 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      379 2023-07-17 07:33:07.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/flushexpiredtokens.py
--rw-rw-rw-   0        0        0     1636 2023-07-17 07:31:58.000000 rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/models.py
--rw-rw-rw-   0        0        0      835 2023-07-17 08:15:12.342807 rest_framework_simplejwt_byforde2-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.679865 rest_framework_simplejwt_byforde2-0.1.5/
+-rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 rest_framework_simplejwt_byforde2-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-07-17 08:27:26.681872 rest_framework_simplejwt_byforde2-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-17 07:14:11.000000 rest_framework_simplejwt_byforde2-0.1.5/README.md
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 rest_framework_simplejwt_byforde2-0.1.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.632574 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.665550 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-07-17 08:27:26.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2023-07-17 08:27:26.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:27:26.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 08:27:26.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.673034 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/
+-rw-rw-rw-   0        0        0      168 2023-07-17 07:32:27.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      290 2023-07-17 07:32:08.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.675038 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:27:26.678362 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-07-17 07:33:07.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/flushexpiredtokens.py
+-rw-rw-rw-   0        0        0     1636 2023-07-17 07:31:58.000000 rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/models.py
+-rw-rw-rw-   0        0        0      835 2023-07-17 08:27:26.684869 rest_framework_simplejwt_byforde2-0.1.5/setup.cfg
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/PKG-INFO` & `rest_framework_simplejwt_byforde2-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest_framework_simplejwt_byforde2
-Version: 0.1.4
+Version: 0.1.5
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO` & `rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-simplejwt-byforde2
-Version: 0.1.4
+Version: 0.1.5
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt` & `rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/admin.py` & `rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/rest_framework_simplejwt_byforde2/token_blacklist/models.py` & `rest_framework_simplejwt_byforde2-0.1.5/rest_framework_simplejwt_byforde2/token_blacklist/models.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.4/setup.cfg` & `rest_framework_simplejwt_byforde2-0.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6573 745f 6672 616d 6577 6f72   = rest_framewor
 00000020: 6b5f 7369 6d70 6c65 6a77 745f 6279 666f  k_simplejwt_byfo
 00000030: 7264 6532 0d0a 7665 7273 696f 6e20 3d20  rde2..version = 
-00000040: 302e 312e 340d 0a61 7574 686f 7220 3d20  0.1.4..author = 
+00000040: 302e 312e 350d 0a61 7574 686f 7220 3d20  0.1.5..author = 
 00000050: 466f 7264 650d 0a61 7574 686f 725f 656d  Forde..author_em
 00000060: 6169 6c20 3d20 666f 722e 6465 7640 6f75  ail = for.dev@ou
 00000070: 746c 6f6f 6b2e 636f 6d0d 0a64 6573 6372  tlook.com..descr
 00000080: 6970 7469 6f6e 203d 2066 6978 6564 205f  iption = fixed _
 00000090: 6964 2066 6965 6c64 7320 746f 2077 6f72  id fields to wor
 000000a0: 6b20 7769 7468 2070 796d 6f6e 676f 2061  k with pymongo a
 000000b0: 6e64 2064 6a6f 6e67 6f2c 2065 7272 6f72  nd djongo, error
```

