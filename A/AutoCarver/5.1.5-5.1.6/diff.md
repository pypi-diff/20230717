# Comparing `tmp/AutoCarver-5.1.5.tar.gz` & `tmp/AutoCarver-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.5.tar", last modified: Mon Jul 17 12:11:46 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.6.tar", last modified: Mon Jul 17 18:34:12 2023, max compression
```

## Comparing `AutoCarver-5.1.5.tar` & `AutoCarver-5.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    30592 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35190 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35712 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.549298 AutoCarver-5.1.6/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 18:34:12.000000 AutoCarver-5.1.6/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:34:12.553298 AutoCarver-5.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-17 18:34:01.000000 AutoCarver-5.1.6/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.5/AutoCarver/auto_carver.py` & `AutoCarver-5.1.6/AutoCarver/auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             qualitative_features = []
         if ordinal_features is None:
             ordinal_features = []
         assert (
             len(quantitative_features) > 0
             or len(qualitative_features) > 0
             or len(ordinal_features) > 0
-        ), "No feature passed as input. Pleased provided column names to Carver by setting quantitative_features, quantitative_features or ordinal_features."
+        ), " - [AutoCarver] No feature passed as input. Pleased provided column names to Carver by setting quantitative_features, quantitative_features or ordinal_features."
         self.ordinal_features = list(set(ordinal_features))
         self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
 
         # initializing input_dtypes
         self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
@@ -156,38 +156,38 @@
             verbose=bool(max(verbose, pretty_print)),
         )
 
         # checking that qualitatitve and qualitative featues are distinct
         assert all(
             quali_feature not in self.quantitative_features
             for quali_feature in self.qualitative_features
-        ), "A feature of quantitative_features also is in qualitative_features or ordinal_features. Please, be carreful with your inputs!"
+        ), " - [AutoCarver] A feature of quantitative_features also is in qualitative_features or ordinal_features. Please, be carreful with your inputs!"
         assert all(
             quanti_feature not in self.qualitative_features
             for quanti_feature in self.quantitative_features
-        ), "A feature of qualitative_features or ordinal_features also is in quantitative_features. Please, be carreful with your inputs!"
+        ), " - [AutoCarver] A feature of qualitative_features or ordinal_features also is in quantitative_features. Please, be carreful with your inputs!"
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         # self.min_carved_freq = min_carved_freq  # TODO
         self.min_group_size = 1
         self.pretty_print = pretty_print
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
         assert (
             sort_by in measures
-        ), f"""Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
+        ), f""" - [AutoCarver] Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
 
         assert unknown_handling in [
             "drop",
             "raises",
             "best",
             "worst",
-        ], "Wrong value for attribute unknown_handling. Choose from ['drop', 'raises', 'best', 'worst']."
+        ], " - [AutoCarver] Wrong value for attribute unknown_handling. Choose from ['drop', 'raises', 'best', 'worst']."
         self.unknown_handling = unknown_handling
 
     def _prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_dev: DataFrame = None,
```

### Comparing `AutoCarver-5.1.5/AutoCarver/converters/converters.py` & `AutoCarver-5.1.6/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import Union
 
 from numpy import nan
 from pandas import DataFrame, Series, unique
 
-from .utils.base_discretizers import BaseDiscretizer, check_new_values, min_value_counts
+from .utils.base_discretizers import BaseDiscretizer, min_value_counts
 from .utils.grouped_list import GroupedList
 from .utils.qualitative_discretizers import DefaultDiscretizer, OrdinalDiscretizer
 from .utils.quantitative_discretizers import QuantileDiscretizer
 from .utils.type_discretizers import StringDiscretizer
 
 
 class Discretizer(BaseDiscretizer):
@@ -105,15 +105,15 @@
 
         # checking for missing orders
         no_order_provided = [
             feature for feature in self.ordinal_features if feature not in self.values_orders
         ]
         assert (
             len(no_order_provided) == 0
-        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+        ), f" - [Discretizer] No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
 
         # class specific attributes
         self.min_freq = min_freq
 
     def _remove_feature(self, feature: str) -> None:
         """Removes a feature from all `feature` attributes
 
@@ -304,15 +304,15 @@
 
         # checking for missing orders
         no_order_provided = [
             feature for feature in self.ordinal_features if feature not in self.values_orders
         ]
         assert (
             len(no_order_provided) == 0
-        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+        ), f" - [QualitativeDiscretizer] No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
 
         # non-ordinal qualitative features
         self.non_ordinal_features = [
             feature for feature in self.qualitative_features if feature not in self.ordinal_features
         ]
 
     def _prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
@@ -370,21 +370,16 @@
                 verbose=self.verbose,
             )
             x_copy = string_discretizer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(string_discretizer.values_orders)
 
-        # all known values for features
-        known_values = {feature: values.values() for feature, values in self.values_orders.items()}
-
         # checking that all unique values in X are in values_orders
-        check_new_values(
-            x_copy, self.ordinal_features, known_values, self.str_nan, self.str_default
-        )
+        self._check_new_values(x_copy, features=self.ordinal_features)
 
         return x_copy
 
     def _remove_feature(self, feature: str) -> None:
         """Removes a feature from all `feature` attributes
 
         Parameters
@@ -544,15 +539,15 @@
         x_copy = super()._prepare_data(X, y)
 
         # checking for quantitative columns
         dtypes = x_copy[self.features].applymap(type).apply(unique)
         not_numeric = dtypes.apply(lambda u: str in u)
         assert all(
             ~not_numeric
-        ), f"Non-numeric features: {str(list(not_numeric[not_numeric].index))}"
+        ), f" - [QuantitativeDiscretizer] Non-numeric features: {str(list(not_numeric[not_numeric].index))} in provided quantitative_features. Please check your inputs."
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Finds relevant buckets of modalities of X to provide the best association with y.
 
         Parameters
```

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,17 @@
         self.quantitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "float"
         ]
 
         # for each feature, getting label associated to each value
         self.labels_per_values: dict[str, dict[Any, Any]] = {}  # will be initiated during fit
 
+        # check if the discretizer has already been fitted
+        self.is_fitted = False
+
     def _get_labels_per_values(self, output_dtype: str) -> dict[str, dict[Any, Any]]:
         """Creates a dict that contains, for each feature, for each value, the associated label
 
         Parameters
         ----------
         output_dtype : str
             Whether or not to convert the output to float.
@@ -190,33 +193,77 @@
             Binary target feature, by default None.
 
         Returns
         -------
         DataFrame
             A formatted copy of X
         """
-        # copying X
+        # checking for previous fits of the discretizer that could cause unwanted errors
+        assert (
+            not self.is_fitted
+        ), " - [BaseDiscretizer] This Discretizer has already been fitted. Fitting it anew could break established orders. Please initialize a new one."
+
+        # checking for input columns
         x_copy = X
-        if self.copy and X is not None:
+        if X is not None:
             missing_columns = [feature for feature in self.features if feature not in X]
             assert (
                 len(missing_columns) == 0
-            ), f"Missing features from the provided DataFrame: {str(missing_columns)}"
-            x_copy = X.copy()
+            ), f" - [BaseDiscretizer] Missing features from the provided DataFrame: {str(missing_columns)}"
+
+            # copying X
+            x_copy = X
+            if self.copy:
+                x_copy = X.copy()
 
         # checking for binary target
         if y is not None:
             y_values = unique(y)
             assert (0 in y_values) & (
                 1 in y_values
-            ), "y must be a binary Series (int or float, not object)"
-            assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+            ), " - [BaseDiscretizer] y must be a binary Series (int or float, not object)"
+            assert (
+                len(y_values) == 2
+            ), " - [BaseDiscretizer] y must be a binary Series (int or float, not object)"
 
         return x_copy
 
+    def _check_new_values(self, X: DataFrame, features: list[str]) -> None:
+        """Checks for new, unexpected values, in X
+
+        Parameters
+        ----------
+        X : DataFrame
+            New DataFrame (at transform time)
+        features : list[str]
+            List of column names
+        """
+        # unique non-nan values in new dataframe
+        uniques = X[features].apply(
+            nan_unique,
+            axis=0,
+            result_type="expand",
+        )
+        uniques = applied_to_dict_list(uniques)
+
+        # checking for unexpected values for each feature
+        for feature in features:
+            unexpected = [
+                val for val in uniques[feature] if val not in self.values_orders[feature].values()
+            ]
+            assert (
+                self.str_nan not in unexpected
+            ), " - [BaseDiscretizer] It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
+            assert (
+                self.str_default not in unexpected
+            ), " - [BaseDiscretizer] It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
+            assert (
+                len(unexpected) == 0
+            ), f" - [BaseDiscretizer] Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
+
     def fit(self, X: DataFrame = None, y: Series = None) -> None:
         """Learns the labels associated to each value for each feature
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after ``BaseDiscretizer.features`` attribute, by default None
@@ -225,19 +272,22 @@
         """
         # checking that all features to discretize are in values_orders
         missing_features = [
             feature for feature in self.features if feature not in self.values_orders
         ]
         assert (
             len(missing_features) == 0
-        ), f"Missing values_orders for following features {str(missing_features)}."
+        ), f" - [BaseDiscretizer] Missing values_orders for following features {str(missing_features)}."
 
         # for each feature, getting label associated to each value
         self.labels_per_values = self._get_labels_per_values(self.output_dtype)
 
+        # setting fitted as True to raise alerts
+        self.is_fitted = True
+
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Applies discretization to a DataFrame's columns.
 
         * For each feature's modality, the associated group label is attributed as definid by ``values_orders``.
         * If ``output_dtype="float"``, converts labels into floats.
@@ -315,15 +365,15 @@
             # keeping track of nans
             nans = isna(X[feature])
 
             # converting nans to there corresponding quantile (if it was grouped to a quantile)
             if any(nans):
                 assert feature_values.contains(
                     self.str_nan
-                ), f"Unexpected value! Missing values found for feature '{feature}' at transform step but not during fit. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
+                ), f" - [BaseDiscretizer] Unexpected value! Missing values found for feature '{feature}' at transform step but not during fit. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
                 nan_value = feature_values.get_group(self.str_nan)
                 # checking that nans have been grouped to a quantile otherwise they are left as numpy.nan (for comparison purposes)
                 if nan_value != self.str_nan:
                     X.loc[nans, feature] = nan_value
 
             # list of masks of values to replace with there respective group
             values_to_group = [
@@ -366,21 +416,15 @@
             Discretized X.
         """
         # filling up nans with specified value
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
-        check_new_values(
-            X,
-            self.qualitative_features,
-            {feature: values.values() for feature, values in self.values_orders.items()},
-            self.str_nan,
-            self.str_default,
-        )
+        self._check_new_values(X, features=self.qualitative_features)
 
         # replacing values for there corresponding label
         X = X.replace(
             {
                 feature: label_per_value
                 for feature, label_per_value in self.labels_per_values.items()
                 if feature in self.qualitative_features
@@ -954,55 +998,14 @@
     # case when it's a DataFrame
     if isinstance(applied, DataFrame):
         converted = applied.to_dict(orient="list")
 
     return converted
 
 
-# TODO: remove known_values
-def check_new_values(
-    X: DataFrame,
-    features: list[str],
-    known_values: dict[str, list[Any]],
-    str_nan: str,
-    str_default: str,
-) -> None:
-    """Checks for new, unexpected values, in X
-
-    Parameters
-    ----------
-    X : DataFrame
-        New DataFrame (at transform time)
-    features : list[str]
-        List of column names
-    known_values : dict[str, list[Any]]
-        Dict of known values per column name
-    """
-    # unique non-nan values in new dataframe
-    uniques = X[features].apply(
-        nan_unique,
-        axis=0,
-        result_type="expand",
-    )
-    uniques = applied_to_dict_list(uniques)
-
-    # checking for unexpected values for each feature
-    for feature in features:
-        unexpected = [val for val in uniques[feature] if val not in known_values[feature]]
-        assert (
-            str_nan not in unexpected
-        ), "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
-        assert (
-            str_default not in unexpected
-        ), "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
-        assert (
-            len(unexpected) == 0
-        ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
-
-
 def check_missing_values(
     X: DataFrame, features: list[str], known_values: dict[str, list[Any]]
 ) -> None:
     """Checks for missing values from X, (unexpected values in values_orders)
 
     Parameters
     ----------
```

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Any, Union
 
 from numpy import argmin, nan, select
 from pandas import DataFrame, Series, isna, notna, unique
 
 from .base_discretizers import (
     BaseDiscretizer,
-    check_missing_values,
-    check_new_values,
     convert_to_labels,
     convert_to_values,
     nan_unique,
     target_rate,
     value_counts,
 )
 from .grouped_list import GroupedList
@@ -38,15 +36,15 @@
         *,
         values_orders: dict[str, GroupedList] = None,
         copy: bool = False,
         verbose: bool = False,
         str_default: str = "__OTHER__",
         str_nan: str = "__NAN__",
     ) -> None:
-        """Initiates a DefaultDiscretizer.
+        """Initiates a ``DefaultDiscretizer``.
 
         Parameters
         ----------
         qualitative_features : list[str]
             List of column names of qualitative features (non-ordinal) to be discretized
 
         min_freq : float
@@ -110,19 +108,18 @@
         # checks and initilizes values_orders
         for feature in self.qualitative_features:
             # initiating features missing from values_orders
             if feature not in self.values_orders:
                 self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
-        check_new_values(
-            x_copy, self.qualitative_features, self.values_orders, self.str_nan, self.str_default
-        )
+        self._check_new_values(x_copy, features=self.qualitative_features)
+
         # checking that all unique values in values_orders are in X
-        check_missing_values(x_copy, self.qualitative_features, self.values_orders)
+        # check_missing_values(x_copy, self.qualitative_features, self.values_orders)
 
         # adding NANS
         for feature in self.qualitative_features:
             if any(x_copy[feature].isna()):
                 self.values_orders[feature].append(self.str_nan)
 
         # filling up NaNs
@@ -156,14 +153,19 @@
 
             # checking for rare values
             values_to_group = [
                 val
                 for val, freq in frequencies[feature].items()
                 if freq < self.min_freq and val != self.str_nan
             ]
+
+            # adding values that are completly missing (no frequency in X)
+            values_to_group += [value for value in order if value not in frequencies[feature]]
+
+            # grouping values to str_default if any
             if any(values_to_group):
                 # adding default value to the order
                 order.append(self.str_default)
 
                 # grouping rare values in default value
                 order.group_list(values_to_group, self.str_default)
                 x_copy.loc[x_copy[feature].isin(values_to_group), feature] = self.str_default
@@ -265,15 +267,15 @@
 
         # checking for missong orders
         no_order_provided = [
             feature for feature in self.features if feature not in self.values_orders
         ]
         assert (
             len(no_order_provided) == 0
-        ), f"No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
+        ), f" - [OrdinalDiscretizer] No ordering was provided for following features: {str(no_order_provided)}. Please make sure you defined ``values_orders`` correctly."
 
         # class specific attributes
         self.min_freq = min_freq
 
     def _prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Validates format and content of X and y.
 
@@ -375,15 +377,15 @@
         *,
         values_orders: dict[str, GroupedList] = None,
         unknown_handling: str = "raise",
         copy: bool = False,
         verbose: bool = False,
         str_nan: str = "__NAN__",
     ) -> None:
-        """Initiates a ChainedDiscretizer.
+        """Initiates a ``ChainedDiscretizer``.
 
         Parameters
         ----------
         qualitative_features : list[str]
             List of column names of qualitative features (non-ordinal) to be discretized
 
         chained_orders : list[GroupedList]
@@ -424,59 +426,83 @@
         # Initiating BaseDiscretizer
         super().__init__(
             features=qualitative_features,
             values_orders=values_orders,
             input_dtypes="str",
             output_dtype="str",
             str_nan=str_nan,
+            dropna=False,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
         self.chained_orders = [GroupedList(values) for values in chained_orders]
         assert unknown_handling in [
             "drop",
             "raise",
-        ], "Wrong value for attribute unknown_handling. Choose from ['drop', 'raise']."
+        ], " - [ChainedDiscretizer] Wrong value for attribute unknown_handling. Choose from ['drop', 'raise']."
         self.unknown_handling = unknown_handling
 
         # known_values: all ordered values describe in each level of the chained_orders
         # starting off with first level
         known_values = self.chained_orders[0].values()
         # adding each level
-        for next_level in self.chained_orders[1:]:
-            # highest value per group of the level
-            highest_ranking_value = {
-                group: [value for value in values if value != group][-1]
-                for group, values in next_level.content.items()
-            }
-
-            # adding next_level group to the order
-            for group, highest_value in highest_ranking_value.items():
-                highest_index = known_values.index(highest_value)
+        for n, next_level in enumerate(self.chained_orders[1:]):
+            # iterating over each group of the next level
+            for next_group, next_values in next_level.content.items():
+                # looking for known and unknwon values in next_level
+
+                # checking for unknown values
+                next_unknown = [
+                    value
+                    for value in next_values
+                    if value not in known_values and value != next_group
+                ]
+                assert (
+                    len(next_unknown) == 0
+                ), f" - [ChainedDiscretizer] Values {str(next_unknown)}, provided in chained_orders[{n+1}] are missing from chained_orders[{n}]. Please make sure values are kept trhough each level."
+
+                # checking for known values
+                next_known = [
+                    value for value in next_values if value in known_values and value != next_group
+                ]
+                assert (
+                    len(next_known) > 0
+                ), f" - [ChainedDiscretizer] For key '{next_group}', the provided chained_orders[{n+1}] has no values from chained_orders[:{n+1}]. Please provide some values existing values."
+
+                # index of the highest ranked known value of the next_group
+                highest_index = known_values.index(next_known[-1])
+
+                # adding next_group to the order at the right place in the amongst known_values
                 known_values = (
-                    known_values[: highest_index + 1] + [group] + known_values[highest_index + 1 :]
+                    known_values[: highest_index + 1]
+                    + [next_group]
+                    + known_values[highest_index + 1 :]
                 )
+
+        # saving resulting known values
         self.known_values = known_values
 
         # adding known_values to each feature's order
         for feature in self.features:
             # checking for already known values of the feature
             if feature in self.values_orders:
                 order = self.values_orders[feature]
             # no known values for the feature
             else:
                 order = GroupedList([])
+
             # checking that all values from the order are in known_values
             for value in order:
                 assert (
                     value in self.known_values
-                ), f"Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
+                ), f" - [ChainedDiscretizer] Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
+
             # adding known values if missing from the order
             for value in self.known_values:
                 if value not in order.values():
                     order.append(value)
             order = order.sort_by(self.known_values)
             self.values_orders.update({feature: order})
 
@@ -497,14 +523,17 @@
         -------
         DataFrame
             A formatted copy of X
         """
         # copying dataframe
         x_copy = X.copy()
 
+        # checking for binary target and previous fit
+        x_copy = super()._prepare_data(x_copy, y)
+
         # checking for ids (unique value per row)
         max_frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
             axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
         all_features = self.features[:]
@@ -558,21 +587,21 @@
 
             # converting unknown values to NaN
             if len(unknown_values) > 0:
                 # raising an error
                 if self.unknown_handling == "raise":
                     assert (
                         not len(unknown_values) > 0
-                    ), f"Order for feature '{feature}' needs to be provided for values: {str(unknown_values)}, otherwise set remove_unknown='drop' (policy remove_unknown='raise')"
+                    ), f" - [ChainedDiscretizer] Order for feature '{feature}' needs to be provided for values: {str(unknown_values)}, otherwise set remove_unknown='drop' (policy unknown_handling='raise')"
 
                 # dropping unknown value
                 else:  # unknown_handling='drop'
                     # alerting user
                     print(
-                        f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(unknown_values)}, these values will be converted to '{self.str_nan}' (policy remove_unknown='drop')"
+                        f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(unknown_values)}, these values will be converted to '{self.str_nan}' (policy unknown_handling='drop')"
                     )
 
                     # adding nan to the order if not already present
                     if self.str_nan not in order:
                         order.append(self.str_nan)
 
                     # adding unknown to the order
@@ -581,19 +610,16 @@
                         # grouping unknown value with str_nan
                         order.group(unknown_value, self.str_nan)
                         x_copy[feature] = x_copy[feature].replace(unknown_value, self.str_nan)
 
             # updating values_orders accordingly
             self.values_orders.update({feature: order})
 
-        # all known values for features
-        known_values = {feature: values.values() for feature, values in self.values_orders.items()}
-
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.features, known_values, self.str_nan, self.str_default)
+        self._check_new_values(x_copy, features=self.features)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """Finds simple buckets of modalities of X.
 
         Parameters
@@ -612,15 +638,14 @@
 
         # iterating over each feature
         for feature in self.features:
             # computing frequencies of each modality
             frequencies = x_copy[feature].value_counts(normalize=True)
 
             # iterating over each specified orders
-            # TODO replace all of this with labels_per_orders
             for level_order in self.chained_orders:
                 values, frequencies = frequencies.index, frequencies.values
 
                 # values that are frequent enough
                 to_keep = list(values[frequencies >= self.min_freq])
 
                 # values from the order to group (not frequent enough or absent)
```

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.6/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.6/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.6/AutoCarver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.5
+Version: 5.1.6
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -25,15 +25,18 @@
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
     <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
-This is a work in progress.
+
+# ReadTheDocs
+
+Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
 # AutoCarver
 
 **AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
 
 It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
 As of today, this set of tools is available for binary classification problems only.
@@ -57,11 +60,7 @@
 
 AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 <pre>
 pip install autocarver
 </pre>
 
-
-## ReadTheDocs
-
-Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
```

### Comparing `AutoCarver-5.1.5/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.6/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/LICENSE` & `AutoCarver-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.5/PKG-INFO` & `AutoCarver-5.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.5
+Version: 5.1.6
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -25,15 +25,18 @@
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
     <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
-This is a work in progress.
+
+# ReadTheDocs
+
+Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
 # AutoCarver
 
 **AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
 
 It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
 As of today, this set of tools is available for binary classification problems only.
@@ -57,11 +60,7 @@
 
 AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 <pre>
 pip install autocarver
 </pre>
 
-
-## ReadTheDocs
-
-Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
```

### Comparing `AutoCarver-5.1.5/README.md` & `AutoCarver-5.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,18 @@
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
     <img src="https://github.com/mdefrance/AutoCarver/actions/workflows/pytest.yml/badge.svg">
     <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
-This is a work in progress.
+
+# ReadTheDocs
+
+Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
 # AutoCarver
 
 **AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
 
 It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
 As of today, this set of tools is available for binary classification problems only.
@@ -35,11 +38,7 @@
 
 AutoCarver can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 <pre>
 pip install autocarver
 </pre>
 
-
-## ReadTheDocs
-
-Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
```

### Comparing `AutoCarver-5.1.5/setup.py` & `AutoCarver-5.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.5",
+    version="5.1.6",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

