# Comparing `tmp/rest_framework_simplejwt_byforde2-0.1.1.tar.gz` & `tmp/rest_framework_simplejwt_byforde2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-ocbqk4yw\rest_framework_simplejwt_byford", last modified: Mon Jul 17 07:55:16 2023, max compression
+gzip compressed data, was "C:\Users\Lenovo PARKSON\Desktop\New folder\rest_framework_simplejwt_byforde2\dist\.tmp-bihisyu6\rest_framework_simplejwt_byford", last modified: Mon Jul 17 08:01:43 2023, max compression
```

## Comparing `rest_framework_simplejwt_byforde2-0.1.1.tar` & `rest_framework_simplejwt_byforde2-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.761914 rest_framework_simplejwt_byforde2-0.1.1/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 rest_framework_simplejwt_byforde2-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      634 2023-07-17 07:55:16.762913 rest_framework_simplejwt_byforde2-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-17 07:14:11.000000 rest_framework_simplejwt_byforde2-0.1.1/README.md
--rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 rest_framework_simplejwt_byforde2-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.643342 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.686637 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/
--rw-rw-rw-   0        0        0      230 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/__init__.py
--rw-rw-rw-   0        0        0     5387 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/authentication.py
--rw-rw-rw-   0        0        0     4666 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/backends.py
--rw-rw-rw-   0        0        0     1300 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/compat.py
--rw-rw-rw-   0        0        0      994 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/exceptions.py
--rw-rw-rw-   0        0        0     3010 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/models.py
--rw-rw-rw-   0        0        0     4928 2023-07-17 07:34:59.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/serializers.py
--rw-rw-rw-   0        0        0     3306 2023-07-17 07:34:41.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/settings.py
--rw-rw-rw-   0        0        0      327 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/state.py
--rw-rw-rw-   0        0        0       68 2023-07-17 07:47:52.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/test.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.716332 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/
--rw-rw-rw-   0        0        0      168 2023-07-17 07:32:27.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/admin.py
--rw-rw-rw-   0        0        0      290 2023-07-17 07:32:08.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.717428 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/management/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.720841 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/__init__.py
--rw-rw-rw-   0        0        0      379 2023-07-17 07:33:07.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/flushexpiredtokens.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.760913 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/
--rw-rw-rw-   0        0        0     2004 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      367 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
--rw-rw-rw-   0        0        0      907 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0003_auto_20171017_2007.py
--rw-rw-rw-   0        0        0      370 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0004_auto_20171017_2013.py
--rw-rw-rw-   0        0        0      294 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
--rw-rw-rw-   0        0        0      339 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0006_auto_20171017_2113.py
--rw-rw-rw-   0        0        0      760 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0007_auto_20171017_2214.py
--rw-rw-rw-   0        0        0      692 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0008_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      693 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
--rw-rw-rw-   0        0        0      578 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0011_linearizes_history.py
--rw-rw-rw-   0        0        0      699 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
--rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/__init__.py
--rw-rw-rw-   0        0        0     1636 2023-07-17 07:31:58.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/models.py
--rw-rw-rw-   0        0        0    11067 2023-07-17 07:34:13.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/tokens.py
--rw-rw-rw-   0        0        0      651 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/utils.py
--rw-rw-rw-   0        0        0     3265 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/views.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:55:16.709332 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/
--rw-rw-rw-   0        0        0      634 2023-07-17 07:55:16.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3638 2023-07-17 07:55:16.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:55:16.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 07:55:16.000000 rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      835 2023-07-17 07:55:16.770007 rest_framework_simplejwt_byforde2-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.245422 rest_framework_simplejwt_byforde2-0.1.2/
+-rw-rw-rw-   0        0        0        0 2023-07-16 16:26:36.000000 rest_framework_simplejwt_byforde2-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-07-17 08:01:43.245422 rest_framework_simplejwt_byforde2-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-17 07:14:11.000000 rest_framework_simplejwt_byforde2-0.1.2/README.md
+-rw-rw-rw-   0        0        0      109 2023-07-16 16:31:27.000000 rest_framework_simplejwt_byforde2-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.181566 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.209592 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-07-17 08:01:43.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1960 2023-07-17 08:01:43.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:01:43.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 08:01:43.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.217416 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/
+-rw-rw-rw-   0        0        0      168 2023-07-17 07:32:27.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-07-17 07:08:30.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/admin.py
+-rw-rw-rw-   0        0        0      290 2023-07-17 07:32:08.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.219610 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/management/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.222613 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-07-17 07:33:07.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/management/commands/flushexpiredtokens.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:01:43.243978 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/
+-rw-rw-rw-   0        0        0     2004 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      367 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-rw-rw-   0        0        0      907 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-rw-rw-   0        0        0      370 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-rw-rw-   0        0        0      294 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-rw-rw-   0        0        0      339 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-rw-rw-   0        0        0      760 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-rw-rw-   0        0        0      692 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      693 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-rw-rw-   0        0        0      578 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0011_linearizes_history.py
+-rw-rw-rw-   0        0        0      699 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:37:25.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1636 2023-07-17 07:31:58.000000 rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/models.py
+-rw-rw-rw-   0        0        0      835 2023-07-17 08:01:43.249435 rest_framework_simplejwt_byforde2-0.1.2/setup.cfg
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/PKG-INFO` & `rest_framework_simplejwt_byforde2-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest_framework_simplejwt_byforde2
-Version: 0.1.1
+Version: 0.1.2
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/admin.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0001_initial.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0003_auto_20171017_2007.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0003_auto_20171017_2007.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0007_auto_20171017_2214.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0007_auto_20171017_2214.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0008_migrate_to_bigautofield.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0008_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0011_linearizes_history.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0011_linearizes_history.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0012_alter_outstandingtoken_user.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/migrations/0012_alter_outstandingtoken_user.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2/token_blacklist/models.py` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/token_blacklist/models.py`

 * *Files identical despite different names*

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO` & `rest_framework_simplejwt_byforde2-0.1.2/rest_framework_simplejwt_byforde2/rest_framework_simplejwt_byforde2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-simplejwt-byforde2
-Version: 0.1.1
+Version: 0.1.2
 Summary: fixed _id fields to work with pymongo and djongo, error for blacklist app.
 Home-page: https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde
 Author: Forde
 Author-email: for.dev@outlook.com
 Project-URL: Bug Tracker, https://github.com/Siliphon/rest_framework_simplejwt_djongo_byforde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_framework_simplejwt_byforde2-0.1.1/setup.cfg` & `rest_framework_simplejwt_byforde2-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6573 745f 6672 616d 6577 6f72   = rest_framewor
 00000020: 6b5f 7369 6d70 6c65 6a77 745f 6279 666f  k_simplejwt_byfo
 00000030: 7264 6532 0d0a 7665 7273 696f 6e20 3d20  rde2..version = 
-00000040: 302e 312e 310d 0a61 7574 686f 7220 3d20  0.1.1..author = 
+00000040: 302e 312e 320d 0a61 7574 686f 7220 3d20  0.1.2..author = 
 00000050: 466f 7264 650d 0a61 7574 686f 725f 656d  Forde..author_em
 00000060: 6169 6c20 3d20 666f 722e 6465 7640 6f75  ail = for.dev@ou
 00000070: 746c 6f6f 6b2e 636f 6d0d 0a64 6573 6372  tlook.com..descr
 00000080: 6970 7469 6f6e 203d 2066 6978 6564 205f  iption = fixed _
 00000090: 6964 2066 6965 6c64 7320 746f 2077 6f72  id fields to wor
 000000a0: 6b20 7769 7468 2070 796d 6f6e 676f 2061  k with pymongo a
 000000b0: 6e64 2064 6a6f 6e67 6f2c 2065 7272 6f72  nd djongo, error
```

