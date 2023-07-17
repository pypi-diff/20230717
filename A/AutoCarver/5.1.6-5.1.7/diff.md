# Comparing `tmp/AutoCarver-5.1.6.tar.gz` & `tmp/AutoCarver-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.6.tar", last modified: Mon Jul 17 18:34:12 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.7.tar", last modified: Mon Jul 17 21:00:50 2023, max compression
```

## Comparing `AutoCarver-5.1.6.tar` & `AutoCarver-5.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35190 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35712 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.353508 AutoCarver-5.1.7/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35190 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.357508 AutoCarver-5.1.7/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.357508 AutoCarver-5.1.7/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.353508 AutoCarver-5.1.7/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.6/AutoCarver/auto_carver.py` & `AutoCarver-5.1.7/AutoCarver/auto_carver.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/converters/converters.py` & `AutoCarver-5.1.7/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,14 +307,22 @@
             Discretized X.
         """
         # copying dataframes
         x_copy = X
         if self.copy:
             x_copy = X.copy()
 
+        # applying default discretization for concerned features
+        for feature in self.features:
+            known_values = self.values_orders[feature].values()
+            if self.str_default in known_values:
+                known_values_index = x_copy[feature].isin(known_values)
+                nans = (x_copy[feature].isna()) | (x_copy[feature] == self.str_nan)
+                x_copy.loc[(~known_values_index) & (~nans), feature] = self.str_default
+
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print(
                     f" - [BaseDiscretizer] Transform Quantitative {str(self.quantitative_features)}"
                 )
             x_copy = self._transform_quantitative(x_copy, y)
```

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.7/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.7/AutoCarver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.6
-Summary: Automatic Bucketizing of Features with Optimal Association
+Version: 5.1.7
+Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.1.6/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.7/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/LICENSE` & `AutoCarver-5.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/PKG-INFO` & `AutoCarver-5.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.6
-Summary: Automatic Bucketizing of Features with Optimal Association
+Version: 5.1.7
+Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.1.6/README.md` & `AutoCarver-5.1.7/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.6/setup.py` & `AutoCarver-5.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.6",
+    version="5.1.7",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
-    description="Automatic Bucketizing of Features with Optimal Association",
+    description="Automatic Discretization of Features with Optimal Target Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
         "Documentation": "https://autocarver.readthedocs.io/en/latest/index.html",
         "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues",
     },
```

### Comparing `AutoCarver-5.1.6/tests/test_auto_carver.py` & `AutoCarver-5.1.7/tests/test_auto_carver.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 def test_auto_carver(
     x_train: DataFrame,
     x_train_wrong_1: DataFrame,
     x_train_wrong_2: DataFrame,
     x_dev_1: DataFrame,
     x_dev_wrong_1: DataFrame,
     x_dev_wrong_2: DataFrame,
+    x_dev_wrong_3: DataFrame,
     output_dtype: str,
     dropna: bool,
     sort_by: str,
     copy: bool,
 ) -> None:
     """Tests AutoCarver
 
@@ -214,22 +215,25 @@
     json_serialized_auto_carver = dumps(auto_carver.to_json())
     loaded_carver = load_carver(loads(json_serialized_auto_carver))
 
     assert all(
         loaded_carver.summary() == auto_carver.summary()
     ), "Non-identical AutoCarver when loading JSON"
 
-    # testing to transform dev set with unexpected modality
-    with raises(AssertionError):
-        auto_carver.transform(x_dev_wrong_1)
+    # testing to transform dev set with unexpected modality for a feature that passed through DefaultDiscretizer
+    auto_carver.transform(x_dev_wrong_1)
 
-    # testing to transform dev set with unexpected nans
+    # testing to transform dev set with unexpected nans for a feature that passed through DefaultDiscretizer
     with raises(AssertionError):
         auto_carver.transform(x_dev_wrong_2)
 
+    # testing to transform dev set with unexpected modality for a feature that did not pass through DefaultDiscretizer
+    with raises(AssertionError):
+        auto_carver.transform(x_dev_wrong_3)
+
     # testing with unknown values in chained discretizer
     chained_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
     values_orders = {
         "Qualitative_Ordinal_lownan": [
             "Low+",
             "Medium-",
             "Medium",
```

