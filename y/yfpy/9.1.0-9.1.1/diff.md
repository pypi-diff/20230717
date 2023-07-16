# Comparing `tmp/yfpy-9.1.0.tar.gz` & `tmp/yfpy-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfpy-9.1.0.tar", last modified: Fri Oct 14 00:05:43 2022, max compression
+gzip compressed data, was "yfpy-9.1.1.tar", last modified: Sun Jul 16 04:01:07 2023, max compression
```

## Comparing `yfpy-9.1.0.tar` & `yfpy-9.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.409993 yfpy-9.1.0/
--rw-r--r--   0 wrenjr     (501) staff       (20)    35149 2021-12-25 14:15:46.000000 yfpy-9.1.0/LICENSE
--rw-r--r--   0 wrenjr     (501) staff       (20)      584 2022-05-05 05:12:04.000000 yfpy-9.1.0/MANIFEST.in
--rw-r--r--   0 wrenjr     (501) staff       (20)    11566 2022-10-14 00:05:43.410089 yfpy-9.1.0/PKG-INFO
--rw-r--r--   0 wrenjr     (501) staff       (20)    10470 2022-05-14 20:31:47.000000 yfpy-9.1.0/README.md
--rw-r--r--   0 wrenjr     (501) staff       (20)      132 2022-10-13 23:59:35.000000 yfpy-9.1.0/requirements.txt
--rw-r--r--   0 wrenjr     (501) staff       (20)      508 2022-10-14 00:05:43.410544 yfpy-9.1.0/setup.cfg
--rw-r--r--   0 wrenjr     (501) staff       (20)     2681 2022-05-12 18:37:29.000000 yfpy-9.1.0/setup.py
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.406424 yfpy-9.1.0/test/
--rw-r--r--   0 wrenjr     (501) staff       (20)        0 2022-05-11 16:56:02.000000 yfpy-9.1.0/test/__init__.py
--rw-r--r--   0 wrenjr     (501) staff       (20)      399 2022-07-20 03:10:45.000000 yfpy-9.1.0/test/conftest.py
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.408069 yfpy-9.1.0/test/integration/
--rw-r--r--   0 wrenjr     (501) staff       (20)      122 2022-05-05 05:12:04.000000 yfpy-9.1.0/test/integration/EXAMPLE.env
--rw-r--r--   0 wrenjr     (501) staff       (20)      130 2022-05-05 05:12:04.000000 yfpy-9.1.0/test/integration/EXAMPLE.private.json
--rw-r--r--   0 wrenjr     (501) staff       (20)      149 2022-05-11 21:54:15.000000 yfpy-9.1.0/test/integration/__init__.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     5457 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/conftest.py
--rw-r--r--   0 wrenjr     (501) staff       (20)    10653 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/test_api_game_data.py
--rw-r--r--   0 wrenjr     (501) staff       (20)    10813 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/test_api_league_data.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     7395 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/test_api_player_data.py
--rw-r--r--   0 wrenjr     (501) staff       (20)    13566 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/test_api_team_data.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     4161 2022-10-13 23:59:35.000000 yfpy-9.1.0/test/integration/test_api_user_data.py
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.408419 yfpy-9.1.0/test/unit/
--rw-r--r--   0 wrenjr     (501) staff       (20)      142 2022-05-11 21:54:15.000000 yfpy-9.1.0/test/unit/__init__.py
--rw-r--r--   0 wrenjr     (501) staff       (20)      161 2022-05-11 21:59:02.000000 yfpy-9.1.0/test/unit/conftest.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     3289 2022-05-12 18:17:51.000000 yfpy-9.1.0/test/unit/test_utils.py
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.409338 yfpy-9.1.0/yfpy/
--rw-r--r--   0 wrenjr     (501) staff       (20)      629 2021-12-25 14:15:46.000000 yfpy-9.1.0/yfpy/__init__.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     9549 2022-10-13 23:59:40.000000 yfpy-9.1.0/yfpy/data.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     1288 2022-05-05 05:12:04.000000 yfpy-9.1.0/yfpy/exceptions.py
--rw-r--r--   0 wrenjr     (501) staff       (20)     1043 2022-10-13 23:59:35.000000 yfpy-9.1.0/yfpy/logger.py
--rw-r--r--   0 wrenjr     (501) staff       (20)    72101 2022-10-13 23:59:40.000000 yfpy-9.1.0/yfpy/models.py
--rw-r--r--   0 wrenjr     (501) staff       (20)   117434 2022-10-13 23:59:35.000000 yfpy-9.1.0/yfpy/query.py
--rw-r--r--   0 wrenjr     (501) staff       (20)    12796 2022-10-13 23:59:40.000000 yfpy-9.1.0/yfpy/utils.py
-drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2022-10-14 00:05:43.409897 yfpy-9.1.0/yfpy.egg-info/
--rw-r--r--   0 wrenjr     (501) staff       (20)    11566 2022-10-14 00:05:43.000000 yfpy-9.1.0/yfpy.egg-info/PKG-INFO
--rw-r--r--   0 wrenjr     (501) staff       (20)      737 2022-10-14 00:05:43.000000 yfpy-9.1.0/yfpy.egg-info/SOURCES.txt
--rw-r--r--   0 wrenjr     (501) staff       (20)        1 2022-10-14 00:05:43.000000 yfpy-9.1.0/yfpy.egg-info/dependency_links.txt
--rw-r--r--   0 wrenjr     (501) staff       (20)      132 2022-10-14 00:05:43.000000 yfpy-9.1.0/yfpy.egg-info/requires.txt
--rw-r--r--   0 wrenjr     (501) staff       (20)       10 2022-10-14 00:05:43.000000 yfpy-9.1.0/yfpy.egg-info/top_level.txt
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.744591 yfpy-9.1.1/
+-rw-r--r--   0 wrenjr     (501) staff       (20)    35149 2021-12-25 14:15:46.000000 yfpy-9.1.1/LICENSE
+-rw-r--r--   0 wrenjr     (501) staff       (20)      584 2022-05-05 05:12:04.000000 yfpy-9.1.1/MANIFEST.in
+-rw-r--r--   0 wrenjr     (501) staff       (20)    11566 2023-07-16 04:01:07.744680 yfpy-9.1.1/PKG-INFO
+-rw-r--r--   0 wrenjr     (501) staff       (20)    10470 2022-05-14 20:31:47.000000 yfpy-9.1.1/README.md
+-rw-r--r--   0 wrenjr     (501) staff       (20)      131 2023-07-16 03:40:22.000000 yfpy-9.1.1/requirements.txt
+-rw-r--r--   0 wrenjr     (501) staff       (20)      508 2023-07-16 04:01:07.745018 yfpy-9.1.1/setup.cfg
+-rw-r--r--   0 wrenjr     (501) staff       (20)     2681 2022-05-12 18:37:29.000000 yfpy-9.1.1/setup.py
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.740969 yfpy-9.1.1/test/
+-rw-r--r--   0 wrenjr     (501) staff       (20)        0 2022-05-11 16:56:02.000000 yfpy-9.1.1/test/__init__.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)      399 2022-07-20 03:10:45.000000 yfpy-9.1.1/test/conftest.py
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.742346 yfpy-9.1.1/test/integration/
+-rw-r--r--   0 wrenjr     (501) staff       (20)      122 2022-05-05 05:12:04.000000 yfpy-9.1.1/test/integration/EXAMPLE.env
+-rw-r--r--   0 wrenjr     (501) staff       (20)      130 2022-05-05 05:12:04.000000 yfpy-9.1.1/test/integration/EXAMPLE.private.json
+-rw-r--r--   0 wrenjr     (501) staff       (20)      149 2022-05-11 21:54:15.000000 yfpy-9.1.1/test/integration/__init__.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     5457 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/conftest.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)    10653 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/test_api_game_data.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)    10813 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/test_api_league_data.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     7395 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/test_api_player_data.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)    13566 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/test_api_team_data.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     4161 2022-10-13 23:59:35.000000 yfpy-9.1.1/test/integration/test_api_user_data.py
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.742785 yfpy-9.1.1/test/unit/
+-rw-r--r--   0 wrenjr     (501) staff       (20)      142 2022-05-11 21:54:15.000000 yfpy-9.1.1/test/unit/__init__.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)      161 2022-05-11 21:59:02.000000 yfpy-9.1.1/test/unit/conftest.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     3289 2022-05-12 18:17:51.000000 yfpy-9.1.1/test/unit/test_utils.py
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.743982 yfpy-9.1.1/yfpy/
+-rw-r--r--   0 wrenjr     (501) staff       (20)      629 2021-12-25 14:15:46.000000 yfpy-9.1.1/yfpy/__init__.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     9549 2022-10-14 00:15:30.000000 yfpy-9.1.1/yfpy/data.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     1288 2022-05-05 05:12:04.000000 yfpy-9.1.1/yfpy/exceptions.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)     1043 2022-10-13 23:59:35.000000 yfpy-9.1.1/yfpy/logger.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)    72101 2023-07-16 03:39:39.000000 yfpy-9.1.1/yfpy/models.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)   117434 2022-10-18 20:10:43.000000 yfpy-9.1.1/yfpy/query.py
+-rw-r--r--   0 wrenjr     (501) staff       (20)    12796 2022-10-14 00:15:30.000000 yfpy-9.1.1/yfpy/utils.py
+drwxr-xr-x   0 wrenjr     (501) staff       (20)        0 2023-07-16 04:01:07.744493 yfpy-9.1.1/yfpy.egg-info/
+-rw-r--r--   0 wrenjr     (501) staff       (20)    11566 2023-07-16 04:01:07.000000 yfpy-9.1.1/yfpy.egg-info/PKG-INFO
+-rw-r--r--   0 wrenjr     (501) staff       (20)      737 2023-07-16 04:01:07.000000 yfpy-9.1.1/yfpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wrenjr     (501) staff       (20)        1 2023-07-16 04:01:07.000000 yfpy-9.1.1/yfpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wrenjr     (501) staff       (20)      131 2023-07-16 04:01:07.000000 yfpy-9.1.1/yfpy.egg-info/requires.txt
+-rw-r--r--   0 wrenjr     (501) staff       (20)       10 2023-07-16 04:01:07.000000 yfpy-9.1.1/yfpy.egg-info/top_level.txt
```

### Comparing `yfpy-9.1.0/LICENSE` & `yfpy-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/MANIFEST.in` & `yfpy-9.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/PKG-INFO` & `yfpy-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yfpy
-Version: 9.1.0
+Version: 9.1.1
 Summary: Python API wrapper for the Yahoo Fantasy Sports public API.
 Home-page: https://github.com/uberfastman/yfpy
 Author: Wren J. R.
 Author-email: uberfastman@uberfastman.dev
 License: UNKNOWN
-Download-URL: https://github.com/uberfastman/yfpy/archive/v9.1.0.tar.gz
+Download-URL: https://github.com/uberfastman/yfpy/archive/v9.1.1.tar.gz
 Keywords: yahoo fantasy sports api wrapper nfl football nhl hockey mlb baseball nba basketball
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yfpy-9.1.0/README.md` & `yfpy-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/setup.py` & `yfpy-9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/conftest.py` & `yfpy-9.1.1/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/test_api_game_data.py` & `yfpy-9.1.1/test/integration/test_api_game_data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/test_api_league_data.py` & `yfpy-9.1.1/test/integration/test_api_league_data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/test_api_player_data.py` & `yfpy-9.1.1/test/integration/test_api_player_data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/test_api_team_data.py` & `yfpy-9.1.1/test/integration/test_api_team_data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/integration/test_api_user_data.py` & `yfpy-9.1.1/test/integration/test_api_user_data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/test/unit/test_utils.py` & `yfpy-9.1.1/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/__init__.py` & `yfpy-9.1.1/yfpy/__init__.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/data.py` & `yfpy-9.1.1/yfpy/data.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/exceptions.py` & `yfpy-9.1.1/yfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/logger.py` & `yfpy-9.1.1/yfpy/logger.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/models.py` & `yfpy-9.1.1/yfpy/models.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/query.py` & `yfpy-9.1.1/yfpy/query.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy/utils.py` & `yfpy-9.1.1/yfpy/utils.py`

 * *Files identical despite different names*

### Comparing `yfpy-9.1.0/yfpy.egg-info/PKG-INFO` & `yfpy-9.1.1/yfpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yfpy
-Version: 9.1.0
+Version: 9.1.1
 Summary: Python API wrapper for the Yahoo Fantasy Sports public API.
 Home-page: https://github.com/uberfastman/yfpy
 Author: Wren J. R.
 Author-email: uberfastman@uberfastman.dev
 License: UNKNOWN
-Download-URL: https://github.com/uberfastman/yfpy/archive/v9.1.0.tar.gz
+Download-URL: https://github.com/uberfastman/yfpy/archive/v9.1.1.tar.gz
 Keywords: yahoo fantasy sports api wrapper nfl football nhl hockey mlb baseball nba basketball
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yfpy-9.1.0/yfpy.egg-info/SOURCES.txt` & `yfpy-9.1.1/yfpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

