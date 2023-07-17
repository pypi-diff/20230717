# Comparing `tmp/atbu-pkg-0.0.8.tar.gz` & `tmp/atbu-pkg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atbu-pkg-0.0.8.tar", last modified: Wed Jun  1 20:42:04 2022, max compression
+gzip compressed data, was "atbu-pkg-0.0.9.tar", last modified: Wed Jun  1 20:44:31 2022, max compression
```

## Comparing `atbu-pkg-0.0.8.tar` & `atbu-pkg-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:04.032085 atbu-pkg-0.0.8/
--rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1133 2022-06-01 20:42:04.030084 atbu-pkg-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0   265683 2022-06-01 20:38:39.000000 atbu-pkg-0.0.8/README.rst
--rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-01 20:42:04.032085 atbu-pkg-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2588 2022-06-01 20:40:38.000000 atbu-pkg-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.909103 atbu-pkg-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.930091 atbu-pkg-0.0.8/src/atbu/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.953083 atbu-pkg-0.0.8/src/atbu/backup/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/backup/__init__.py
--rw-rw-rw-   0        0        0    12123 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/backup_cmdline.py
--rw-rw-rw-   0        0        0   130275 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/backup_core.py
--rw-rw-rw-   0        0        0    24377 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/backup_selections.py
--rw-rw-rw-   0        0        0    11912 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/chunk_reader.py
--rw-rw-rw-   0        0        0    39994 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/config.py
--rw-rw-rw-   0        0        0    25830 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/credentials.py
--rw-rw-rw-   0        0        0    27993 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/creds_cmdline.py
--rw-rw-rw-   0        0        0     3169 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/backup/list_items.py
--rw-rw-rw-   0        0        0    10173 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/recover.py
--rw-rw-rw-   0        0        0    19059 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/restore.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.962083 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/__init__.py
--rw-rw-rw-   0        0        0     4967 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/base.py
--rw-rw-rw-   0        0        0     7856 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/filesystem.py
--rw-rw-rw-   0        0        0    17394 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/google.py
--rw-rw-rw-   0        0        0     8216 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/storage_interface/libcloud.py
--rw-rw-rw-   0        0        0    12413 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/backup/verify.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.984098 atbu-pkg-0.0.8/src/atbu/common/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/common/__init__.py
--rw-rw-rw-   0        0        0     6128 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/aes_cbc.py
--rw-rw-rw-   0        0        0    45062 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/command_line.py
--rw-rw-rw-   0        0        0     5870 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/constants.py
--rw-rw-rw-   0        0        0    13416 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/exception.py
--rw-rw-rw-   0        0        0    36923 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/file_info.py
--rw-rw-rw-   0        0        0     3271 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/common/hasher.py
--rw-rw-rw-   0        0        0     9661 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/mp_global.py
--rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/multi_json_enc_dec.py
--rw-rw-rw-   0        0        0    10495 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/queued_worker.py
--rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/common/simple_report.py
--rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/singleton.py
--rw-rw-rw-   0        0        0     5576 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/common/util_helpers.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:03.990109 atbu-pkg-0.0.8/src/atbu/persisted_info/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.8/src/atbu/persisted_info/__init__.py
--rw-rw-rw-   0        0        0    23824 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/persisted_info/database.py
--rw-rw-rw-   0        0        0    33731 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/persisted_info/diff.py
--rw-rw-rw-   0        0        0     5846 2022-06-01 12:51:45.000000 atbu-pkg-0.0.8/src/atbu/persisted_info/update_digests.py
-drwxrwxrwx   0        0        0        0 2022-06-01 20:42:04.028108 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/
--rw-rw-rw-   0        0        0     1133 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      168 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-06-01 20:42:03.000000 atbu-pkg-0.0.8/src/atbu_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.162908 atbu-pkg-0.0.9/
+-rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1135 2022-06-01 20:44:31.161908 atbu-pkg-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0   265683 2022-06-01 20:38:39.000000 atbu-pkg-0.0.9/README.rst
+-rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-06-01 20:44:31.162908 atbu-pkg-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2590 2022-06-01 20:44:15.000000 atbu-pkg-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.072907 atbu-pkg-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.085909 atbu-pkg-0.0.9/src/atbu/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.107910 atbu-pkg-0.0.9/src/atbu/backup/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/backup/__init__.py
+-rw-rw-rw-   0        0        0    12123 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/backup_cmdline.py
+-rw-rw-rw-   0        0        0   130275 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/backup_core.py
+-rw-rw-rw-   0        0        0    24377 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/backup_selections.py
+-rw-rw-rw-   0        0        0    11912 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/chunk_reader.py
+-rw-rw-rw-   0        0        0    39994 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/config.py
+-rw-rw-rw-   0        0        0    25830 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/credentials.py
+-rw-rw-rw-   0        0        0    27993 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/creds_cmdline.py
+-rw-rw-rw-   0        0        0     3169 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/backup/list_items.py
+-rw-rw-rw-   0        0        0    10173 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/recover.py
+-rw-rw-rw-   0        0        0    19059 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/restore.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.115906 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/__init__.py
+-rw-rw-rw-   0        0        0     4967 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/base.py
+-rw-rw-rw-   0        0        0     7856 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/filesystem.py
+-rw-rw-rw-   0        0        0    17394 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/google.py
+-rw-rw-rw-   0        0        0     8216 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/storage_interface/libcloud.py
+-rw-rw-rw-   0        0        0    12413 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/backup/verify.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.133908 atbu-pkg-0.0.9/src/atbu/common/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/common/__init__.py
+-rw-rw-rw-   0        0        0     6128 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/aes_cbc.py
+-rw-rw-rw-   0        0        0    45062 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/command_line.py
+-rw-rw-rw-   0        0        0     5870 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/constants.py
+-rw-rw-rw-   0        0        0    13416 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/exception.py
+-rw-rw-rw-   0        0        0    36923 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/file_info.py
+-rw-rw-rw-   0        0        0     3271 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/common/hasher.py
+-rw-rw-rw-   0        0        0     9661 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/mp_global.py
+-rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/multi_json_enc_dec.py
+-rw-rw-rw-   0        0        0    10495 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/queued_worker.py
+-rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/common/simple_report.py
+-rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/singleton.py
+-rw-rw-rw-   0        0        0     5576 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/common/util_helpers.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.139909 atbu-pkg-0.0.9/src/atbu/persisted_info/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-pkg-0.0.9/src/atbu/persisted_info/__init__.py
+-rw-rw-rw-   0        0        0    23824 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/persisted_info/database.py
+-rw-rw-rw-   0        0        0    33731 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/persisted_info/diff.py
+-rw-rw-rw-   0        0        0     5846 2022-06-01 12:51:45.000000 atbu-pkg-0.0.9/src/atbu/persisted_info/update_digests.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:44:31.160911 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/
+-rw-rw-rw-   0        0        0     1135 2022-06-01 20:44:30.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2022-06-01 20:44:31.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-01 20:44:30.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2022-06-01 20:44:30.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      168 2022-06-01 20:44:30.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-06-01 20:44:30.000000 atbu-pkg-0.0.9/src/atbu_pkg.egg-info/top_level.txt
```

### Comparing `atbu-pkg-0.0.8/LICENSE` & `atbu-pkg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/PKG-INFO` & `atbu-pkg-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: ATBU package supports local/cloud backup/restore as well as local file integrity diff tool for helping in efforts to manage file integrity, duplication, and bitrot detection.
 Home-page: https://github.com/AshleyT3/atbu
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,8 +19,9 @@
 ATBU Backup & Persistent File Information is a local/cloud backup/restore
 command-line utility with optional deduplication and bitrot detection,
 plus a little utility with useful digest-based directory file diff'ing.
 
 Install: `pip install atbu-pkg`
 
 GitHub: https://github.com/AshleyT3/atbu
+
 Documentation: https://atbu.readthedocs.io/en/latest/
```

### Comparing `atbu-pkg-0.0.8/README.rst` & `atbu-pkg-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/setup.py` & `atbu-pkg-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Redirect from long_description to github README.rst since
 # PyPi chokes on this particular README.rst.
 # with open("README.rst", "r", encoding="utf-8") as fh:
 #    long_description = fh.read()
 
 setuptools.setup(
     name="atbu-pkg",
-    version="0.0.8",
+    version="0.0.9",
     author="Ashley R. Thomas",
     author_email="ashley.r.thomas.701@gmail.com",
     description= (
         "ATBU package supports local/cloud backup/restore "
         "as well as local file integrity diff tool for helping in "
         "efforts to manage file integrity, duplication, and bitrot detection."
     ),
@@ -36,14 +36,15 @@
 ATBU Backup & Persistent File Information is a local/cloud backup/restore
 command-line utility with optional deduplication and bitrot detection,
 plus a little utility with useful digest-based directory file diff'ing.
 
 Install: `pip install atbu-pkg`
 
 GitHub: https://github.com/AshleyT3/atbu
+
 Documentation: https://atbu.readthedocs.io/en/latest/
 """,
     long_description_content_type="text/markdown",
     url="https://github.com/AshleyT3/atbu",
     project_urls={
         "Bug Tracker": "https://github.com/AshleyT3/atbu/issues",
     },
```

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/backup_cmdline.py` & `atbu-pkg-0.0.9/src/atbu/backup/backup_cmdline.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/backup_core.py` & `atbu-pkg-0.0.9/src/atbu/backup/backup_core.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/backup_selections.py` & `atbu-pkg-0.0.9/src/atbu/backup/backup_selections.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/chunk_reader.py` & `atbu-pkg-0.0.9/src/atbu/backup/chunk_reader.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/config.py` & `atbu-pkg-0.0.9/src/atbu/backup/config.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/credentials.py` & `atbu-pkg-0.0.9/src/atbu/backup/credentials.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/creds_cmdline.py` & `atbu-pkg-0.0.9/src/atbu/backup/creds_cmdline.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/list_items.py` & `atbu-pkg-0.0.9/src/atbu/backup/list_items.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/recover.py` & `atbu-pkg-0.0.9/src/atbu/backup/recover.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/restore.py` & `atbu-pkg-0.0.9/src/atbu/backup/restore.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/storage_interface/base.py` & `atbu-pkg-0.0.9/src/atbu/backup/storage_interface/base.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/storage_interface/filesystem.py` & `atbu-pkg-0.0.9/src/atbu/backup/storage_interface/filesystem.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/storage_interface/google.py` & `atbu-pkg-0.0.9/src/atbu/backup/storage_interface/google.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/storage_interface/libcloud.py` & `atbu-pkg-0.0.9/src/atbu/backup/storage_interface/libcloud.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/backup/verify.py` & `atbu-pkg-0.0.9/src/atbu/backup/verify.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/aes_cbc.py` & `atbu-pkg-0.0.9/src/atbu/common/aes_cbc.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/command_line.py` & `atbu-pkg-0.0.9/src/atbu/common/command_line.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/constants.py` & `atbu-pkg-0.0.9/src/atbu/common/constants.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/exception.py` & `atbu-pkg-0.0.9/src/atbu/common/exception.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/file_info.py` & `atbu-pkg-0.0.9/src/atbu/common/file_info.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/hasher.py` & `atbu-pkg-0.0.9/src/atbu/common/hasher.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/mp_global.py` & `atbu-pkg-0.0.9/src/atbu/common/mp_global.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/multi_json_enc_dec.py` & `atbu-pkg-0.0.9/src/atbu/common/multi_json_enc_dec.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/queued_worker.py` & `atbu-pkg-0.0.9/src/atbu/common/queued_worker.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/simple_report.py` & `atbu-pkg-0.0.9/src/atbu/common/simple_report.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/singleton.py` & `atbu-pkg-0.0.9/src/atbu/common/singleton.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/common/util_helpers.py` & `atbu-pkg-0.0.9/src/atbu/common/util_helpers.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/persisted_info/database.py` & `atbu-pkg-0.0.9/src/atbu/persisted_info/database.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/persisted_info/diff.py` & `atbu-pkg-0.0.9/src/atbu/persisted_info/diff.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu/persisted_info/update_digests.py` & `atbu-pkg-0.0.9/src/atbu/persisted_info/update_digests.py`

 * *Files identical despite different names*

### Comparing `atbu-pkg-0.0.8/src/atbu_pkg.egg-info/PKG-INFO` & `atbu-pkg-0.0.9/src/atbu_pkg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: ATBU package supports local/cloud backup/restore as well as local file integrity diff tool for helping in efforts to manage file integrity, duplication, and bitrot detection.
 Home-page: https://github.com/AshleyT3/atbu
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,8 +19,9 @@
 ATBU Backup & Persistent File Information is a local/cloud backup/restore
 command-line utility with optional deduplication and bitrot detection,
 plus a little utility with useful digest-based directory file diff'ing.
 
 Install: `pip install atbu-pkg`
 
 GitHub: https://github.com/AshleyT3/atbu
+
 Documentation: https://atbu.readthedocs.io/en/latest/
```

### Comparing `atbu-pkg-0.0.8/src/atbu_pkg.egg-info/SOURCES.txt` & `atbu-pkg-0.0.9/src/atbu_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

