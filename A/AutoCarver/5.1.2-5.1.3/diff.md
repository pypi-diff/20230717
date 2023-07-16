# Comparing `tmp/AutoCarver-5.1.2.tar.gz` & `tmp/AutoCarver-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.2.tar", last modified: Sun Jul 16 21:50:57 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.3.tar", last modified: Sun Jul 16 23:28:03 2023, max compression
```

## Comparing `AutoCarver-5.1.2.tar` & `AutoCarver-5.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34702 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.566622 AutoCarver-5.1.2/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 21:50:57.000000 AutoCarver-5.1.2/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:50:57.570623 AutoCarver-5.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 21:50:46.000000 AutoCarver-5.1.2/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.397581 AutoCarver-5.1.3/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.405582 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.401581 AutoCarver-5.1.3/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 23:28:03.000000 AutoCarver-5.1.3/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:28:03.409582 AutoCarver-5.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-16 23:27:47.000000 AutoCarver-5.1.3/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.2/AutoCarver/auto_carver.py` & `AutoCarver-5.1.3/AutoCarver/auto_carver.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,18 +55,18 @@
 
             * Features whose most frequent modality is less frequent than ``min_freq`` will not be carved.
             * Sets the number of quantiles in which to discretize the continuous features.
             * Sets the minimum frequency of a quantitative feature's modality.
 
             **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
 
-        quantitative_features : list[str]
+        quantitative_features : list[str], optional
             List of column names of quantitative features (continuous and discrete) to be carved, by default ``None``
 
-        qualitative_features : list[str]
+        qualitative_features : list[str], optional
             List of column names of qualitative features (non-ordinal) to be carved, by default ``None``
 
         ordinal_features : list[str], optional
             List of column names of ordinal features to be carved. For those features a list of
             values has to be provided in the ``values_orders`` dict, by default ``None``
 
         values_orders : dict[str, GroupedList], optional
```

### Comparing `AutoCarver-5.1.2/AutoCarver/converters/converters.py` & `AutoCarver-5.1.3/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.3/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/feature_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,112 +6,98 @@
 from IPython.display import display_html
 from pandas import DataFrame, Series
 
 from .filters import cramerv_filter, spearman_filter, thresh_filter
 from .measures import cramerv_measure, dtype_measure, kruskal_measure, mode_measure, nans_measure
 
 
-# TODO: add thresh_mode, thresh_nan to the class parameters
-# TODO: add parameter to shut down displayed info
 class FeatureSelector:
-    """A pipeline of measures to perform EDA and feature pre-selection
+    """A pipeline of measures to perform a feature pre-selection that maximizes association
+    with a binary target.
 
-     - best features are the n_best of each measure
-     - selected features are stored in FeatureSelector.best_features
-
-    Parameters
-    ----------
-    features: list[str]
-        Features on which to compute association.
-    n_best, int:
-        Number of features to be selected
-    sample_size: float, default 1.
-        Should be set between ]0, 1]
-        Size of sampled list of features speeds up computation.
-        By default, all features are used. For sample_size=0.5,
-        FeatureSelector will search for the best features in
-        features[:len(features)//2] and then in features[len(features)//2:]
-    measures, list[Callable]: default list().
-        List of association measures to be used.
-        Implemented measures are:
-            [Quantitative Features]
-             - For association evaluation: `kruskal_measure`, `R_measure`
-             - For outlier detection: `zscore_measure`, `iqr_measure`
-            [Qualitative Features]
-             - For correlation: `chi2_measure`, `cramerv_measure`, `tschuprowt_measure`
-        Ranks features based on last measure of the list.
-    filters, list[Callable]: default list().
-        List of filters to be used.
-        Implemented filters are:
-            [Quantitative Features]
-             - For linear correlation: `spearman_filter`, `pearson_filter`
-             - For multicoloinearity: `vif_filter`
-            [Qualitative Features]
-             - For correlation: `cramerv_filter`, `tschuprowt_filter`
-
-    Thresholds (to be passed as kwargs)
-    ----------
-    thresh_measure, float: default 0.
-        Minimum association between target and features
-        To be used with: `measure_filter`
-    name_measure, str
-        Measure to be used for minimum association filtering
-        To be used with: `measure_filter`
-    thresh_nan, float: default 1.
-        Maximum percentage of NaNs in a feature
-        To be used with: `nans_measure`
-    thresh_mode, float: default 1.
-        Maximum percentage of the mode of a feature
-        To be used with: `mode_measure`
-    thresh_outlier, float: default 1.
-        Maximum percentage of Outliers in a feature
-        To be used with: `iqr_measure`, `zscore_measure`
-    thresh_corr, float: default 1.
-        Maximum association between features
-        To be used with: `spearman_filter`, `pearson_filter`, `cramerv_filter`, `tschuprowt_filter`
-    thresh_vif, float: default inf
-        Maximum VIF between features
-        To be used with: `vif_filter`
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
+    * Best features are the n_best of each measure
+    * Get your best features with ``FeatureSelector.select()``!
     """
 
     def __init__(
         self,
         n_best: int,
         *,
         quantitative_features: list[str] = None,
         qualitative_features: list[str] = None,
         measures: list[Callable] = None,
         filters: list[Callable] = None,
         sample_size: float = 1.0,
         verbose: bool = False,
-        pretty_print: bool = False,  # TODO
+        pretty_print: bool = False,
         **params,
     ) -> None:
         """Initiates a ``FeatureSelector``.
 
         Parameters
         ----------
-        features : list[str]
-            _description_
         n_best : int
-            _description_
+            Number of features to select.
+
+        quantitative_features : list[str], optional
+            List of column names of quantitative features to chose from, by default ``None``
+            Must be set if ``qualitative_features=None``.
+
+        qualitative_features : list[str], optional
+            List of column names of qualitative features to chose from, by default ``None``
+            Must be set if ``quantitative_features=None``.
+
         measures : list[Callable], optional
-            _description_, by default list()
+            List of association measures to be used, by default ``None``.
+            Ranks features based on last provided measure of the list.
+            See :ref:`Measures`.
+            Implemented measures are:
+
+            * [Quantitative Features] For association evaluation: ``kruskal_measure``, ``R_measure``
+            * [Quantitative Features] For outlier detection: ``zscore_measure``, ``iqr_measure``
+            * [Qualitative Features] For correlation: ``chi2_measure``, ``cramerv_measure``, ``tschuprowt_measure``
+
         filters : list[Callable], optional
-            _description_, by default list()
+            List of filters to be used, by default ``None``.
+            See :ref:`Filters`.
+            Implemented filters are:
+
+            * [Quantitative Features] For linear correlation: ``spearman_filter``, ``pearson_filter``
+            * [Quantitative Features] For multicoloinearity: ``vif_filter``
+            * [Qualitative Features] For correlation: ``cramerv_filter``, ``tschuprowt_filter``
+
         sample_size : float, optional
-            _description_, by default 1.0
-        copy : bool, optional
-            _description_, by default True
+            _description_, by default ``1.0``
+
         verbose : bool, optional
-            _description_, by default True
+            If ``True``, prints raw Discretizers Fit and Transform steps, as long as
+            information on AutoCarver's processing and tables of target rates and frequencies for
+            X, by default ``False``
+
+        pretty_print : bool, optional
+            If ``True``, adds to the verbose some HTML tables of target rates and frequencies for X and, if provided, X_dev.
+            Overrides the value of ``verbose``, by default ``False``
+
+        **params
+            Sets thresholds for ``measures`` and ``filters``, passed as keyword arguments.
+
+            * thresh_measure, float, minimum association between target and features, by default ``0``. To be used with: ``measure_filter``.
+            * name_measure, str, measure to be used for minimum association filtering. To be used with: ``measure_filter``.
+            * thresh_nan, float,aximum percentage of NaNs in a feature, by default ``1``. To be used with: ``nans_measure``.
+            * thresh_mode, float, maximum percentage of the mode of a feature, by default ``1``. To be used with: ``mode_measure``.
+            * thresh_outlier, float, maximum percentage of Outliers in a feature, by default ``1``. To be used with: ``iqr_measure``, ``zscore_measure``.
+            * thresh_corr, float, Maximum association between features, by default ``1``. To be used with: ``spearman_filter``, ``pearson_filter``, ``cramerv_filter``, ``tschuprowt_filter``.
+            * thresh_vif, float, maximum VIF between features, by default ``inf``. To be used with: ``vif_filter``.
+            * ascending, bool default ``False``
+                * ``True``: Lower values of the measure are to be considered as more associated to the target
+                * ``False``: Higher values of the measure are to be considered as more associated to the target
+
+        Examples
+        --------
+        See `FeatureSelector examples <https://autocarver.readthedocs.io/en/latest/index.html>`_
         """
         # settinp up list of features
         if quantitative_features is None:
             quantitative_features = []
         if qualitative_features is None:
             qualitative_features = []
         assert (
@@ -120,15 +106,17 @@
         assert (len(quantitative_features) > 0 and len(qualitative_features) == 0) or (
             len(qualitative_features) > 0 and len(quantitative_features) == 0
         ), "Mixed quantitative and qualitative features. One only of quantitative_features and qualitative_features should be set."
         self.features = list(set(qualitative_features + quantitative_features))
 
         # number of features selected
         self.n_best = n_best
-        assert n_best <= len(self.features) + 1, "Must set n_best <= len(features)"
+        assert (
+            0 < int(n_best // 2) <= len(self.features) + 1
+        ), "Must set 0 < n_best // 2 <= len(features)"
 
         # feature sample size per iteration
         self.sample_size = sample_size
 
         # initiating measures
         if measures is None:
             if any(quantitative_features):  # quantitative feature association measure
@@ -151,17 +139,14 @@
         # wether or not to print tables
         self.verbose = bool(max(verbose, pretty_print))
         self.pretty_print = pretty_print
 
         # keyword arguments
         self.params = params
 
-        self.associations = None
-        self.filtered_associations = None
-
     def _select_features(
         self, X: DataFrame, y: Series, features: list[str], n_best: int
     ) -> list[str]:
         """Selects the n_best features amongst the specified ones
 
         Parameters
         ----------
@@ -245,15 +230,16 @@
 
     def select(self, X: DataFrame, y: Series) -> list[str]:
         """Selects the ``n_best`` features of the DataFrame, by association with the binary target
 
         Parameters
         ----------
         X : DataFrame
-            _description_
+            Dataset used to measure association between features and target.
+            Needs to have columns has specified in ``FeatureSelector.features``.
         y : Series
             Binary target feature with wich the association is maximized.
 
         Returns
         -------
         list[str]
             List of selected features
@@ -282,15 +268,16 @@
                 best_features += self._select_features(X, y, features, int(self.n_best // 2))
 
         # splitting in chunks not requested
         else:
             best_features = self.features[:]
 
         # final selection with all best_features selected
-        best_features = self._select_features(X, y, best_features, self.n_best)
+        if any(best_features):
+            best_features = self._select_features(X, y, best_features, self.n_best)
 
         return best_features
 
 
 def print_associations(association: DataFrame, pretty_print: bool = False) -> None:
     """EDA of fitted associations
 
@@ -306,15 +293,15 @@
         print(association)
 
     # adding colors and displaying DataFrame as html
     else:
         # finding columns with indicators to colorize
         subset = [
             column
-            for column in association
+            for column in association.columns
             # checking for an association indicator
             if any(indic in column for indic in ["pct_", "_measure", "_filter"])
         ]
         # getting prettier association table
         nicer_association = association.style.background_gradient(cmap="coolwarm", subset=subset)
         nicer_association = nicer_association.set_table_attributes("style='display:inline'")
```

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 
 from ..measures import cramerv_measure, tschuprowt_measure
 
 
 def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
     """Computes max Cramer's V between X and X (qualitative) excluding features
     that are correlated to a feature more associated with the target
-    (defined by the ranks).
+    (defined by the ``ranks``).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
 
     # applying quantitative filter with Cramer's V correlation
     return qualitative_filter(X, ranks, cramerv_measure, **params)
 
 
 def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> dict[str, Any]:
-    """Computes max Tschuprow's T between X and X (qualitative) excluding
-     features that are correlated to a feature more associated with the target
-    (defined by the ranks).
+    """Computes max Tschuprow's T between X and X (qualitative) excluding features that are
+    correlated to a feature more associated with the target (defined by the ``ranks``).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
```

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.3/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.3/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.2
+Version: 5.1.3
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.2/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.3/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/LICENSE` & `AutoCarver-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/PKG-INFO` & `AutoCarver-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.2
+Version: 5.1.3
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
```

### Comparing `AutoCarver-5.1.2/README.md` & `AutoCarver-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.2/setup.py` & `AutoCarver-5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.2",
+    version="5.1.3",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.2/tests/test_auto_carver.py` & `AutoCarver-5.1.3/tests/test_auto_carver.py`

 * *Files identical despite different names*

