# Comparing `tmp/pypx-3.8.0.tar.gz` & `tmp/pypx-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypx-3.8.0.tar", last modified: Wed May 11 15:43:10 2022, max compression
+gzip compressed data, was "pypx-3.8.2.tar", last modified: Fri May 13 18:05:05 2022, max compression
```

## Comparing `pypx-3.8.0.tar` & `pypx-3.8.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2022-05-11 15:43:10.515679 pypx-3.8.0/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       18 2017-10-09 16:46:38.000000 pypx-3.8.0/MANIFEST.in
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    13105 2022-05-11 15:43:10.519012 pypx-3.8.0/PKG-INFO
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    12885 2022-05-11 15:41:17.000000 pypx-3.8.0/README.rst
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2022-05-11 15:43:10.492346 pypx-3.8.0/bin/
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    11003 2021-12-07 22:45:56.000000 pypx-3.8.0/bin/pfstorage
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    11307 2021-10-26 01:19:07.000000 pypx-3.8.0/bin/px-do
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     7510 2021-06-04 16:20:30.000000 pypx-3.8.0/bin/px-echo
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    21695 2021-12-09 17:52:50.000000 pypx-3.8.0/bin/px-find
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     6403 2021-06-04 16:20:55.000000 pypx-3.8.0/bin/px-listen
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     8670 2021-06-04 16:21:06.000000 pypx-3.8.0/bin/px-move
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    11909 2022-05-06 14:24:38.000000 pypx-3.8.0/bin/px-push
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    11817 2022-05-11 15:41:49.000000 pypx-3.8.0/bin/px-register
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     9601 2022-05-06 14:24:38.000000 pypx-3.8.0/bin/px-repack
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    12281 2022-05-06 21:24:50.000000 pypx-3.8.0/bin/px-report
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     5795 2021-12-07 16:12:48.000000 pypx-3.8.0/bin/px-smdb
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     7840 2021-08-22 17:40:34.000000 pypx-3.8.0/bin/px-status
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2022-05-11 15:43:10.515679 pypx-3.8.0/pypx/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      821 2021-05-20 19:30:21.000000 pypx-3.8.0/pypx/__init__.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     6841 2021-04-23 15:30:03.000000 pypx-3.8.0/pypx/base.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    21009 2021-12-09 17:52:27.000000 pypx-3.8.0/pypx/do.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1190 2020-01-17 21:19:11.000000 pypx-3.8.0/pypx/echo.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    17600 2021-10-26 01:19:07.000000 pypx-3.8.0/pypx/find.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    18727 2021-06-03 00:54:40.000000 pypx-3.8.0/pypx/listen.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     2019 2021-06-04 18:02:38.000000 pypx-3.8.0/pypx/move.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)    28452 2021-12-07 22:43:54.000000 pypx-3.8.0/pypx/pfstorage.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    11593 2022-05-06 16:16:40.000000 pypx-3.8.0/pypx/push.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    21285 2022-05-11 14:55:35.000000 pypx-3.8.0/pypx/register.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    39059 2022-05-06 16:20:19.000000 pypx-3.8.0/pypx/repack.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    39212 2022-05-06 21:23:36.000000 pypx-3.8.0/pypx/report.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    73769 2021-12-07 16:59:28.000000 pypx-3.8.0/pypx/smdb.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3094 2021-08-20 18:37:59.000000 pypx-3.8.0/pypx/status.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1626 2017-10-09 16:46:38.000000 pypx-3.8.0/pypx/utils.py
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2022-05-11 15:43:10.515679 pypx-3.8.0/pypx.egg-info/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    13105 2022-05-11 15:43:10.000000 pypx-3.8.0/pypx.egg-info/PKG-INFO
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      590 2022-05-11 15:43:10.000000 pypx-3.8.0/pypx.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2022-05-11 15:43:10.000000 pypx-3.8.0/pypx.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2021-06-04 16:41:29.000000 pypx-3.8.0/pypx.egg-info/not-zip-safe
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      117 2022-05-11 15:43:10.000000 pypx-3.8.0/pypx.egg-info/requires.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        5 2022-05-11 15:43:10.000000 pypx-3.8.0/pypx.egg-info/top_level.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       65 2022-05-11 15:43:10.519012 pypx-3.8.0/setup.cfg
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1592 2022-05-11 15:41:27.000000 pypx-3.8.0/setup.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1143 2021-06-23 20:14:15.000000 pypx-3.8.0/storescp.sh
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-05-13 18:05:05.265588 pypx-3.8.2/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       18 2022-05-05 17:57:25.000000 pypx-3.8.2/MANIFEST.in
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    13105 2022-05-13 18:05:05.265588 pypx-3.8.2/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    12885 2022-05-13 18:03:18.000000 pypx-3.8.2/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-05-13 18:05:05.262254 pypx-3.8.2/bin/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    11003 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/pfstorage
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    11307 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-do
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     7510 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-echo
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    21695 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-find
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     6403 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-listen
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     8670 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-move
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    11909 2022-05-05 22:46:49.000000 pypx-3.8.2/bin/px-push
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    11817 2022-05-12 19:59:30.000000 pypx-3.8.2/bin/px-register
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     9601 2022-05-05 21:38:44.000000 pypx-3.8.2/bin/px-repack
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    12281 2022-05-10 18:19:42.000000 pypx-3.8.2/bin/px-report
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     5795 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-smdb
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     7840 2022-05-05 17:57:25.000000 pypx-3.8.2/bin/px-status
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-05-13 18:05:05.265588 pypx-3.8.2/pypx/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      821 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6841 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/base.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    21195 2022-05-13 18:02:34.000000 pypx-3.8.2/pypx/do.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1190 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/echo.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    17600 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/find.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    18727 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/listen.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2019 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/move.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    28452 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/pfstorage.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11593 2022-05-10 18:19:42.000000 pypx-3.8.2/pypx/push.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    21285 2022-05-13 18:02:52.000000 pypx-3.8.2/pypx/register.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    39059 2022-05-10 18:19:42.000000 pypx-3.8.2/pypx/repack.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    39212 2022-05-10 18:19:42.000000 pypx-3.8.2/pypx/report.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    73769 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/smdb.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3094 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/status.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1626 2022-05-05 17:57:25.000000 pypx-3.8.2/pypx/utils.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-05-13 18:05:05.265588 pypx-3.8.2/pypx.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    13105 2022-05-13 18:05:05.000000 pypx-3.8.2/pypx.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      590 2022-05-13 18:05:05.000000 pypx-3.8.2/pypx.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-05-13 18:05:05.000000 pypx-3.8.2/pypx.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-05-05 17:59:36.000000 pypx-3.8.2/pypx.egg-info/not-zip-safe
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      117 2022-05-13 18:05:05.000000 pypx-3.8.2/pypx.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        5 2022-05-13 18:05:05.000000 pypx-3.8.2/pypx.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       65 2022-05-13 18:05:05.265588 pypx-3.8.2/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1592 2022-05-13 18:03:10.000000 pypx-3.8.2/setup.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     1143 2022-05-05 17:57:25.000000 pypx-3.8.2/storescp.sh
```

### Comparing `pypx-3.8.0/PKG-INFO` & `pypx-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypx
-Version: 3.8.0
+Version: 3.8.2
 Summary: PACS/ChRIS core tools and utils
 Home-page: http://github.com/fnndsc/pypx
 Author: FNNDSC Developers
 Author-email: dev@babymri.com
 License: MIT
 Platform: UNKNOWN
 
 ####################################
-pypx - 3.8.0
+pypx - 3.8.2
 ####################################
 
 .. image:: https://badge.fury.io/py/pypx.svg
     :target: https://badge.fury.io/py/pypx
 
 .. image:: https://travis-ci.org/FNNDSC/pypx.svg?branch=master
     :target: https://travis-ci.org/FNNDSC/pypx
```

### Comparing `pypx-3.8.0/README.rst` & `pypx-3.8.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################
-pypx - 3.8.0
+pypx - 3.8.2
 ####################################
 
 .. image:: https://badge.fury.io/py/pypx.svg
     :target: https://badge.fury.io/py/pypx
 
 .. image:: https://travis-ci.org/FNNDSC/pypx.svg?branch=master
     :target: https://travis-ci.org/FNNDSC/pypx
```

### Comparing `pypx-3.8.0/bin/pfstorage` & `pypx-3.8.2/bin/pfstorage`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-do` & `pypx-3.8.2/bin/px-do`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-echo` & `pypx-3.8.2/bin/px-echo`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-find` & `pypx-3.8.2/bin/px-find`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-listen` & `pypx-3.8.2/bin/px-listen`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-move` & `pypx-3.8.2/bin/px-move`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-push` & `pypx-3.8.2/bin/px-push`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-register` & `pypx-3.8.2/bin/px-register`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-repack` & `pypx-3.8.2/bin/px-repack`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-report` & `pypx-3.8.2/bin/px-report`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-smdb` & `pypx-3.8.2/bin/px-smdb`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/bin/px-status` & `pypx-3.8.2/bin/px-status`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/__init__.py` & `pypx-3.8.2/pypx/__init__.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/base.py` & `pypx-3.8.2/pypx/base.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/do.py` & `pypx-3.8.2/pypx/do.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,29 +416,32 @@
             str_line                : str   = presenter.seriesRegister_print(
                 studyIndex  = studyIndex,
                 seriesIndex = seriesIndex,
                 fileCounts  = db.series_receivedAndRequested(str_seriesInstanceUID)
             )
 
             if self.arg['withFeedBack']: self.log(str_line)
-
             d_then                  : dict  = {}
             d_seriesDir             : dict  = db.imageDirs_getOnSeriesInstanceUID(str_seriesInstanceUID)
             registerParser                  = registerParser_setup("Register Parser")
             d_registerArgs                  = pushParser_JSONinterpret(registerParser, d_registerArgsCLI)
             d_registerArgs.str_xcrdir       = d_seriesDir[str_seriesInstanceUID]
             d_then      = pypx.register(
                             d_registerArgs,
                         )
             try:
                 str_msg     = next(gen_dict_extract('msg', d_then))
             except:
                 str_msg     = ""
             if len(str_msg):
-                self.log(json.dumps(json.loads(str_msg), indent = 4), comms = 'error')
+                try:
+                    self.log(json.dumps(json.loads(str_msg), indent = 4), comms = 'error')
+                except:
+                    self.log(json.dumps(d_seriesDir, indent = 4), comms = 'error')
+                    self.log(str_msg, comms = 'error')
             return d_then
 
         def gen_dict_extract(key, var):
             if hasattr(var,'items'):
                 for k, v in var.items():
                     if k == key:
                         yield v
```

### Comparing `pypx-3.8.0/pypx/echo.py` & `pypx-3.8.2/pypx/echo.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/find.py` & `pypx-3.8.2/pypx/find.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/listen.py` & `pypx-3.8.2/pypx/listen.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/move.py` & `pypx-3.8.2/pypx/move.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/pfstorage.py` & `pypx-3.8.2/pypx/pfstorage.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/push.py` & `pypx-3.8.2/pypx/push.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/register.py` & `pypx-3.8.2/pypx/register.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/repack.py` & `pypx-3.8.2/pypx/repack.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/report.py` & `pypx-3.8.2/pypx/report.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/smdb.py` & `pypx-3.8.2/pypx/smdb.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/status.py` & `pypx-3.8.2/pypx/status.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx/utils.py` & `pypx-3.8.2/pypx/utils.py`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/pypx.egg-info/PKG-INFO` & `pypx-3.8.2/pypx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypx
-Version: 3.8.0
+Version: 3.8.2
 Summary: PACS/ChRIS core tools and utils
 Home-page: http://github.com/fnndsc/pypx
 Author: FNNDSC Developers
 Author-email: dev@babymri.com
 License: MIT
 Platform: UNKNOWN
 
 ####################################
-pypx - 3.8.0
+pypx - 3.8.2
 ####################################
 
 .. image:: https://badge.fury.io/py/pypx.svg
     :target: https://badge.fury.io/py/pypx
 
 .. image:: https://travis-ci.org/FNNDSC/pypx.svg?branch=master
     :target: https://travis-ci.org/FNNDSC/pypx
```

### Comparing `pypx-3.8.0/pypx.egg-info/SOURCES.txt` & `pypx-3.8.2/pypx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypx-3.8.0/setup.py` & `pypx-3.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
         name                =   'pypx',
-        version             =   '3.8.0',
+        version             =   '3.8.2',
         description         =   'PACS/ChRIS core tools and utils',
         long_description    =   readme(),
         url                 =   'http://github.com/fnndsc/pypx',
         author              =   'FNNDSC Developers',
         author_email        =   'dev@babymri.com',
         license             =   'MIT',
         packages            =   ['pypx'],
```

### Comparing `pypx-3.8.0/storescp.sh` & `pypx-3.8.2/storescp.sh`

 * *Files identical despite different names*

