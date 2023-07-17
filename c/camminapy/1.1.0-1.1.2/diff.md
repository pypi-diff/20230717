# Comparing `tmp/camminapy-1.1.0.tar.gz` & `tmp/camminapy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-1.1.0.tar", max compression
+gzip compressed data, was "camminapy-1.1.2.tar", max compression
```

## Comparing `camminapy-1.1.0.tar` & `camminapy-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 08:57:11.658456 camminapy-1.1.0/LICENSE
--rw-r--r--   0        0        0      361 2023-05-26 08:44:24.292769 camminapy-1.1.0/README.md
--rw-r--r--   0        0        0      119 2023-05-26 08:04:14.503813 camminapy-1.1.0/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 09:40:51.581748 camminapy-1.1.0/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6299 2023-05-26 08:55:46.589484 camminapy-1.1.0/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 11:46:26.866899 camminapy-1.1.0/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 11:44:40.466282 camminapy-1.1.0/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6242 2023-05-26 07:23:10.045894 camminapy-1.1.0/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 12:58:34.534445 camminapy-1.1.0/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 08:57:11.673431 camminapy-1.1.0/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 08:57:11.672848 camminapy-1.1.0/camminapy/utils/config.py
--rw-r--r--   0        0        0      734 2023-05-26 07:23:10.046191 camminapy-1.1.0/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1138 2023-06-05 10:50:31.036043 camminapy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 camminapy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.2/LICENSE
+-rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.2/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.2/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.2/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6800 2023-07-17 19:29:59.439266 camminapy-1.1.2/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.2/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.2/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.2/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.2/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.2/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.2/camminapy/utils/config.py
+-rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.2/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1138 2023-07-17 19:37:43.619843 camminapy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 camminapy-1.1.2/PKG-INFO
```

### Comparing `camminapy-1.1.0/LICENSE` & `camminapy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/camminapy/data/resample.py` & `camminapy-1.1.2/camminapy/data/resample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import polars as pl
+import polars.selectors as cs
 
 from camminapy.utils.logger import logger
 
 
 def resample_dataframe_polars(
     df: pl.DataFrame,
     interpolation_column: str,
@@ -26,14 +27,15 @@
 
     Returns
     -------
     pl.DataFrame
         A dataframe with the same columns as the input dataframe and where
         `interpolation_column` is spaced as `interpolation_step` and all other
         data is interpolated onto that timeline.
+        **Note**: This will **NOT** extrapolate.
     """
     # Get the x-values onto which we want to interpolate the data.
     interpolation_points = pl.DataFrame(
         {
             interpolation_column: np.arange(
                 start=df.min()[0, interpolation_column],
                 stop=df.max()[0, interpolation_column] + interpolation_step,
@@ -58,14 +60,23 @@
     ).sort(interpolation_column)
 
     if to_log:
         n_input = len(df)
         n_output = len(df_with_data_only_at_interpolation_points)
         logger.info(f"Resampled from {n_input} rows to {n_output} rows.")
 
+    # Forward fill string columns because interpolation does not
+    # work on them. Only the first entry will be preserved and the others are none.
+    # This might need to be updated in the future to include columns
+    # other than pl.Utf8.
+    df_with_data_only_at_interpolation_points = (
+        df_with_data_only_at_interpolation_points.with_columns(
+            cs.by_dtype(pl.Utf8).forward_fill()
+        )
+    )
     return df_with_data_only_at_interpolation_points
 
 
 #######################################################################################
 #                       Everything below is just wrappers.                            #
 #######################################################################################
```

### Comparing `camminapy-1.1.0/camminapy/plot/altair_config.py` & `camminapy-1.1.2/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/camminapy/plot/altair_theme.py` & `camminapy-1.1.2/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/camminapy/plot/footer.py` & `camminapy-1.1.2/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/camminapy/utils/config.py` & `camminapy-1.1.2/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/camminapy/utils/logger.py` & `camminapy-1.1.2/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.0/pyproject.toml` & `camminapy-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "1.1.0"
+version = "1.1.2"
 description = "My personal code collection."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.md"
 repository = "https://github.com/thomascamminady/camminapy"
 homepage = "https://thomascamminady.github.io/camminapy/camminapy.html"
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-1.1.0/PKG-INFO` & `camminapy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 1.1.0
+Version: 1.1.2
 Summary: My personal code collection.
 Home-page: https://thomascamminady.github.io/camminapy/camminapy.html
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

