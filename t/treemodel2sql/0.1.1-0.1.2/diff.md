# Comparing `tmp/treemodel2sql-0.1.1.tar.gz` & `tmp/treemodel2sql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treemodel2sql-0.1.1.tar", last modified: Mon Jul 17 12:43:55 2023, max compression
+gzip compressed data, was "dist/treemodel2sql-0.1.2.tar", last modified: Mon Jul 17 12:57:51 2023, max compression
```

## Comparing `treemodel2sql-0.1.1.tar` & `treemodel2sql-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.editorconfig
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/.github/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.gitignore
--rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/.travis.yml
--rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/AUTHORS.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-17 12:41:25.000000 treemodel2sql-0.1.1/HISTORY.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/LICENSE
--rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/MANIFEST.in
--rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)    32641 2023-07-17 12:39:53.000000 treemodel2sql-0.1.1/README.md
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/docs/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/authors.rst
--rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/conf.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/contributing.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/history.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/index.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/installation.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/make.bat
--rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/readme.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/docs/usage.rst
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/examples/
--rw-r--r--   0 ryanzheng   (501) staff       (20)   115765 2023-07-17 12:40:38.000000 treemodel2sql-0.1.1/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
--rw-r--r--   0 ryanzheng   (501) staff       (20)   100911 2023-07-17 12:40:39.000000 treemodel2sql-0.1.1/examples/tutorial_code_xgboost_model_transform_sql.ipynb
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/images/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.1/images/干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.1/images/魔都数据干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.1/requirements.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/setup.cfg
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-17 12:40:47.000000 treemodel2sql-0.1.1/setup.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/tests/
--rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/tests/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.1/tests/test_treemodel2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-16 06:49:05.000000 treemodel2sql-0.1.1/treemodel2sql/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4656 2023-07-16 05:19:29.000000 treemodel2sql-0.1.1/treemodel2sql/lgb2sql.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 treemodel2sql-0.1.1/treemodel2sql/xgboost2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/not-zip-safe
--rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/requires.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-17 12:43:55.000000 treemodel2sql-0.1.1/treemodel2sql.egg-info/top_level.txt
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.editorconfig
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/.github/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.gitignore
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.travis.yml
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/AUTHORS.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-17 12:54:41.000000 treemodel2sql-0.1.2/HISTORY.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/LICENSE
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/MANIFEST.in
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    32641 2023-07-17 12:39:53.000000 treemodel2sql-0.1.2/README.md
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/docs/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/conf.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/contributing.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/history.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/index.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/installation.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/make.bat
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/readme.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/usage.rst
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/examples/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   115765 2023-07-17 12:40:38.000000 treemodel2sql-0.1.2/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   100911 2023-07-17 12:40:39.000000 treemodel2sql-0.1.2/examples/tutorial_code_xgboost_model_transform_sql.ipynb
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/images/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.2/images/干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.2/images/魔都数据干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.2/requirements.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/setup.cfg
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-17 12:54:31.000000 treemodel2sql-0.1.2/setup.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/tests/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/tests/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/tests/test_treemodel2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-17 12:54:28.000000 treemodel2sql-0.1.2/treemodel2sql/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4656 2023-07-16 05:19:29.000000 treemodel2sql-0.1.2/treemodel2sql/lgb2sql.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 treemodel2sql-0.1.2/treemodel2sql/xgboost2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/not-zip-safe
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/requires.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/top_level.txt
```

### Comparing `treemodel2sql-0.1.1/.gitignore` & `treemodel2sql-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/.travis.yml` & `treemodel2sql-0.1.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/CONTRIBUTING.rst` & `treemodel2sql-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/LICENSE` & `treemodel2sql-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/Makefile` & `treemodel2sql-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/PKG-INFO` & `treemodel2sql-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treemodel2sql
-Version: 0.1.1
+Version: 0.1.2
 Summary: tree model transform to sql
 Home-page: https://github.com/ZhengRyan/treemodel2sql
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Keywords: treemodel2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `treemodel2sql-0.1.1/README.md` & `treemodel2sql-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/docs/Makefile` & `treemodel2sql-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/docs/conf.py` & `treemodel2sql-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/docs/installation.rst` & `treemodel2sql-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/docs/make.bat` & `treemodel2sql-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/examples/tutorial_code_lightgbm_model_transform_sql.ipynb` & `treemodel2sql-0.1.2/examples/tutorial_code_lightgbm_model_transform_sql.ipynb`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/examples/tutorial_code_xgboost_model_transform_sql.ipynb` & `treemodel2sql-0.1.2/examples/tutorial_code_xgboost_model_transform_sql.ipynb`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/images/干饭人.png` & `treemodel2sql-0.1.2/images/干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/images/魔都数据干饭人.png` & `treemodel2sql-0.1.2/images/魔都数据干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/setup.py` & `treemodel2sql-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     include_package_data=True,
     keywords='treemodel2sql',
     name=NAME,
     packages=find_packages(include=['treemodel2sql', 'treemodel2sql.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZhengRyan/treemodel2sql',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `treemodel2sql-0.1.1/tests/test_treemodel2sql.py` & `treemodel2sql-0.1.2/tests/test_treemodel2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/treemodel2sql/lgb2sql.py` & `treemodel2sql-0.1.2/treemodel2sql/lgb2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/treemodel2sql/xgboost2sql.py` & `treemodel2sql-0.1.2/treemodel2sql/xgboost2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.1/treemodel2sql.egg-info/PKG-INFO` & `treemodel2sql-0.1.2/treemodel2sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treemodel2sql
-Version: 0.1.1
+Version: 0.1.2
 Summary: tree model transform to sql
 Home-page: https://github.com/ZhengRyan/treemodel2sql
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Keywords: treemodel2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `treemodel2sql-0.1.1/treemodel2sql.egg-info/SOURCES.txt` & `treemodel2sql-0.1.2/treemodel2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

