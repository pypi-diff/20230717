# Comparing `tmp/AutoCarver-5.1.4.tar.gz` & `tmp/AutoCarver-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.4.tar", last modified: Mon Jul 17 09:08:07 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.5.tar", last modified: Mon Jul 17 12:11:46 2023, max compression
```

## Comparing `AutoCarver-5.1.4.tar` & `AutoCarver-5.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.231417 AutoCarver-5.1.4/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34722 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.235417 AutoCarver-5.1.4/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 09:08:07.000000 AutoCarver-5.1.4/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 09:08:07.243417 AutoCarver-5.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:08:07.239417 AutoCarver-5.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-17 09:07:41.000000 AutoCarver-5.1.4/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30592 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.841097 AutoCarver-5.1.5/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 12:11:46.000000 AutoCarver-5.1.5/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:11:46.845097 AutoCarver-5.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-17 12:11:21.000000 AutoCarver-5.1.5/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.4/AutoCarver/auto_carver.py` & `AutoCarver-5.1.5/AutoCarver/auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
         # min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
         output_dtype: str = "float",
         dropna: bool = True,
+        unknown_handling: str = "raises",
         copy: bool = False,
         verbose: bool = False,
         pretty_print: bool = False,
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
     ) -> None:
         """Initiates an ``AutoCarver``.
@@ -164,23 +165,31 @@
             quanti_feature not in self.qualitative_features
             for quanti_feature in self.quantitative_features
         ), "A feature of qualitative_features or ordinal_features also is in quantitative_features. Please, be carreful with your inputs!"
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
-        # self.min_carved_freq = min_carved_freq
+        # self.min_carved_freq = min_carved_freq  # TODO
         self.min_group_size = 1
         self.pretty_print = pretty_print
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
         assert (
             sort_by in measures
         ), f"""Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
 
+        assert unknown_handling in [
+            "drop",
+            "raises",
+            "best",
+            "worst",
+        ], "Wrong value for attribute unknown_handling. Choose from ['drop', 'raises', 'best', 'worst']."
+        self.unknown_handling = unknown_handling
+
     def _prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_dev: DataFrame = None,
         y_dev: Series = None,
     ) -> tuple[DataFrame, DataFrame]:
@@ -257,14 +266,15 @@
             quantitative_features=self.quantitative_features,
             qualitative_features=self.qualitative_features,
             min_freq=self.min_freq,
             ordinal_features=self.ordinal_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             str_default=self.str_default,
+            # unknwon_handling=self.unknown_handling,  # TODO
             copy=True,  # copying anyways, otherwise no discretization from start to finish
             verbose=self.verbose,
         )
         x_copy = discretizer.fit_transform(x_copy, y)
         if x_dev_copy is not None:
             x_dev_copy = discretizer.transform(x_dev_copy, y_dev)
         self.input_dtypes.update(discretizer.input_dtypes)  # saving data types
```

### Comparing `AutoCarver-5.1.4/AutoCarver/converters/converters.py` & `AutoCarver-5.1.5/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,30 +73,33 @@
         elif isinstance(iterable, list):
             # initiating the list with the provided list of keys
             super().__init__(iterable)
 
             # initiating the values with the provided list of keys
             self.content = {v: [v] for v in iterable}
 
-    def get(self, key: Any) -> list[Any]:
+    def get(self, key: Any, default: Any = None) -> list[Any]:
         """List of values content in key
 
         Parameters
         ----------
         key : Any
             Group.
+        default : Any, optional
+            Value to return if key was not found, by default None
 
         Returns
         -------
         list[Any]
             Values content in key
         """
-
         # default to fing an element
-        found = self.content.get(key)
+        if default is None:
+            default_value = []
+        found = self.content.get(key, default_value)
 
         return found
 
     def group(self, discarded: Any, kept: Any) -> None:
         """Groups the discarded value with the kept value
 
         Parameters
```

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     def __init__(
         self,
         qualitative_features: list[str],
         min_freq: float,
         chained_orders: list[GroupedList],
         *,
         values_orders: dict[str, GroupedList] = None,
-        remove_unknown: bool = True,
+        unknown_handling: str = "raise",
         copy: bool = False,
         verbose: bool = False,
         str_nan: str = "__NAN__",
     ) -> None:
         """Initiates a ChainedDiscretizer.
 
         Parameters
@@ -399,17 +399,19 @@
 
             **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
 
         values_orders : dict[str, GroupedList], optional
             Dict of feature's column names and there associated ordering.
             If lists are passed, a GroupedList will automatically be initiated, by default ``None``
 
-        remove_unknown : bool, optional
-            Whether or not to remove unknown values, by default True.
-            If ``True``, unknown values are grouped into the value ``str_nan``
+        unknown_handling : str, optional
+            Whether or not to remove unknown values, by default ``'raise'``.
+
+            * ``'raise'``, unknown values raise an ``AssertionError``.
+            * ``'drop'``, unknown values are grouped with ``str_nan``.
 
         copy : bool, optional
             If ``True``, feature processing at transform is applied to a copy of the provided DataFrame, by default ``False``
 
         verbose : bool, optional
             If ``True``, prints raw Discretizers Fit and Transform steps, by default ``False``
 
@@ -429,15 +431,19 @@
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
         self.chained_orders = [GroupedList(values) for values in chained_orders]
-        self.remove_unknown = remove_unknown
+        assert unknown_handling in [
+            "drop",
+            "raise",
+        ], "Wrong value for attribute unknown_handling. Choose from ['drop', 'raise']."
+        self.unknown_handling = unknown_handling
 
         # known_values: all ordered values describe in each level of the chained_orders
         # starting off with first level
         known_values = self.chained_orders[0].values()
         # adding each level
         for next_level in self.chained_orders[1:]:
             # highest value per group of the level
@@ -529,23 +535,66 @@
                 qualitative_features=features_to_convert, values_orders=self.values_orders
             )
             x_copy = stringer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
+        # filling nans
+        x_copy = x_copy.fillna(self.str_nan)
+
+        # adding nans and unknown values
+        for feature in self.features:
+            # adding NaNs to the order if any
+            order = self.values_orders[feature]
+            if any(x_copy[feature] == self.str_nan):
+                order.append(self.str_nan)
+
+            # checking for unknown values (missing from known_values)
+            unknown_values = [
+                value
+                for value in x_copy[feature].unique()
+                if value not in self.known_values and value != self.str_nan
+            ]
+
+            # converting unknown values to NaN
+            if len(unknown_values) > 0:
+                # raising an error
+                if self.unknown_handling == "raise":
+                    assert (
+                        not len(unknown_values) > 0
+                    ), f"Order for feature '{feature}' needs to be provided for values: {str(unknown_values)}, otherwise set remove_unknown='drop' (policy remove_unknown='raise')"
+
+                # dropping unknown value
+                else:  # unknown_handling='drop'
+                    # alerting user
+                    print(
+                        f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(unknown_values)}, these values will be converted to '{self.str_nan}' (policy remove_unknown='drop')"
+                    )
+
+                    # adding nan to the order if not already present
+                    if self.str_nan not in order:
+                        order.append(self.str_nan)
+
+                    # adding unknown to the order
+                    for unknown_value in unknown_values:
+                        order.append(unknown_value)
+                        # grouping unknown value with str_nan
+                        order.group(unknown_value, self.str_nan)
+                        x_copy[feature] = x_copy[feature].replace(unknown_value, self.str_nan)
+
+            # updating values_orders accordingly
+            self.values_orders.update({feature: order})
+
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
 
         # checking that all unique values in X are in values_orders
         check_new_values(x_copy, self.features, known_values, self.str_nan, self.str_default)
 
-        # filling nans
-        x_copy = x_copy.fillna(self.str_nan)
-
         return x_copy
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """Finds simple buckets of modalities of X.
 
         Parameters
         ----------
@@ -554,54 +603,27 @@
 
         y : Series
             Binary target feature, not used, by default None.
         """
         # filling nans
         x_copy = self._prepare_data(X, y)
 
-        # iterating over each feature
         if self.verbose:  # verbose if requested
             print(f" - [ChainedDiscretizer] Fit {str(self.features)}")
+
+        # iterating over each feature
         for feature in self.features:
             # computing frequencies of each modality
             frequencies = x_copy[feature].value_counts(normalize=True)
-            values, frequencies = frequencies.index, frequencies.values
-
-            # adding NaNs to the order if any
-            order = self.values_orders[feature]
-            if self.str_nan in values:
-                order.append(self.str_nan)
-
-            # checking for unknown values (missing from known_values)
-            missing = [
-                value
-                for value in values
-                if value not in self.known_values and value != self.str_nan
-            ]
-
-            # converting unknown values to NaN
-            if self.remove_unknown & (len(missing) > 0):
-                # alerting user
-                print(
-                    f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(missing)}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)"
-                )
-
-                # adding missing values to the order
-                order.update({self.str_nan: missing + order.get(self.str_nan)})
-
-            # alerting user
-            else:
-                assert (
-                    not len(missing) > 0
-                ), f"Order for feature '{feature}' needs to be provided for values: {str(missing)}, otherwise set remove_unknown=True"
 
             # iterating over each specified orders
-            for (
-                level_order
-            ) in self.chained_orders:  # TODO replace all of this with labels_per_orders
+            # TODO replace all of this with labels_per_orders
+            for level_order in self.chained_orders:
+                values, frequencies = frequencies.index, frequencies.values
+
                 # values that are frequent enough
                 to_keep = list(values[frequencies >= self.min_freq])
 
                 # values from the order to group (not frequent enough or absent)
                 values_to_group = [value for value in level_order.values() if value not in to_keep]
 
                 # values to group into discarded values
@@ -615,15 +637,14 @@
 
                 # historizing in the feature's order
                 for discarded, kept in zip(values_to_group, groups_value):
                     self.values_orders.get(feature).group(discarded, kept)
 
                 # updating frequencies of each modality for the next ordering
                 frequencies = x_copy[feature].value_counts(normalize=True)
-                values, frequencies = frequencies.index, frequencies.values
 
         super().fit(X, y)
 
         return self
 
 
 def find_common_modalities(
```

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.5/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.5/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.5/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/LICENSE` & `AutoCarver-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.4/setup.py` & `AutoCarver-5.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.4",
+    version="5.1.5",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.4/tests/test_auto_carver.py` & `AutoCarver-5.1.5/tests/test_auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     min_freq = 0.15
 
     chained_discretizer = ChainedDiscretizer(
         qualitative_features=chained_features,
         chained_orders=[level0_to_level1, level1_to_level2],
         min_freq=min_freq,
         values_orders=values_orders,
+        unknown_handling="drop",
         copy=copy,
     )
     x_discretized = chained_discretizer.fit_transform(x_train)
     values_orders.update(chained_discretizer.values_orders)
 
     # minimum frequency per modality
     min_freq = 0.06
```

