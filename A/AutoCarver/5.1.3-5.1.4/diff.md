# Comparing `tmp/AutoCarver-5.1.3.tar.gz` & `tmp/AutoCarver-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.3.tar", last modified: Sun Jul 16 23:28:03 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.4.tar", last modified: Mon Jul 17 09:08:07 2023, max compression
```

## Comparing `AutoCarver-5.1.3.tar` & `AutoCarver-5.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.397581 AutoCarver-5.1.3/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.231417 AutoCarver-5.1.4/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 09:08:07.243417 AutoCarver-5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.3/AutoCarver/auto_carver.py` & `AutoCarver-5.1.4/AutoCarver/auto_carver.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/converters/converters.py` & `AutoCarver-5.1.4/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.4/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.4/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.3
+Version: 5.1.4
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.3/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.4/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/LICENSE` & `AutoCarver-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/PKG-INFO` & `AutoCarver-5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.3
+Version: 5.1.4
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.3/README.md` & `AutoCarver-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.3/setup.py` & `AutoCarver-5.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.3",
+    version="5.1.4",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.3/tests/test_auto_carver.py` & `AutoCarver-5.1.4/tests/test_auto_carver.py`

 * *Files identical despite different names*

