# Comparing `tmp/data-disaggregation-0.9.2.tar.gz` & `tmp/data-disaggregation-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-disaggregation-0.9.2.tar", last modified: Tue May  2 12:04:30 2023, max compression
+gzip compressed data, was "data-disaggregation-0.9.3.tar", last modified: Fri Jun 16 06:40:46 2023, max compression
```

## Comparing `data-disaggregation-0.9.2.tar` & `data-disaggregation-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/data_disaggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/data_disaggregation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/data_disaggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/data_disaggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/data_disaggregation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/data_disaggregation/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/data_disaggregation/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/data_disaggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/data_disaggregation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-16 06:40:46.000000 data-disaggregation-0.9.3/data_disaggregation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-16 06:40:46.000000 data-disaggregation-0.9.3/data_disaggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:40:46.000000 data-disaggregation-0.9.3/data_disaggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 06:40:46.000000 data-disaggregation-0.9.3/data_disaggregation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:40:46.000000 data-disaggregation-0.9.3/data_disaggregation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:40:46.585647 data-disaggregation-0.9.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-06-16 06:40:19.000000 data-disaggregation-0.9.3/test/test.py
```

### Comparing `data-disaggregation-0.9.2/LICENSE` & `data-disaggregation-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.2/PKG-INFO` & `data-disaggregation-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-disaggregation
-Version: 0.9.2
+Version: 0.9.3
 Author: Christian Winger
 License: MIT
 Project-URL: Documentation, https://wingechr.github.io/data-disaggregation
 Project-URL: Source, https://github.com/wingechr/data-disaggregation
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-disaggregation-0.9.2/README.md` & `data-disaggregation-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.2/data_disaggregation/base.py` & `data-disaggregation-0.9.3/data_disaggregation/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 """
 
 
 from typing import Mapping, Tuple
 
 from .classes import VT, F, T, V, VT_NumericExt
 from .utils import (
+    as_set,
     group_idx_first,
     group_idx_second,
     is_map,
     is_mapping,
     is_na,
     is_subset,
     is_unique,
@@ -114,17 +115,19 @@
         assert all(v > 0 for v in iter_values(size_out))
         # assert all(isinstance(v, (float, int)) for v in iter_values(size_out))
 
         # validate var
         assert is_mapping(data)
         assert is_unique(data)
 
-        assert is_subset(
-            data, size_in
-        ), "Variable index is not a subset of input dimension subset"
+        if not is_subset(data, size_in):
+            err = as_set(data) - as_set(size_in)
+            raise Exception(
+                f"Variable index is not a subset of input dimension subset: {err}"
+            )
 
         # validate map
         assert is_map(weight_map)
         assert is_unique(weight_map)
         assert all(v >= 0 for v in iter_values(weight_map))
         assert is_subset([x[0] for x in weight_map.keys()], size_in)
         assert is_subset([x[1] for x in weight_map.keys()], size_out)
@@ -134,15 +137,15 @@
 
     groups = get_groups(vtype=vtype, data=data, weight_map=weight_map, size_in=size_in)
 
     for t, vws in groups.items():
         # weights sum
         sumw = sum(w for _, w in vws)
         # TODO drop test
-        sumw <= size_out[t]
+        assert sumw <= size_out[t]
 
         # drop result?
         if threshold:
             if (sumw / size_out[t]) < threshold:
                 continue
 
         # normalize weights
```

### Comparing `data-disaggregation-0.9.2/data_disaggregation/classes.py` & `data-disaggregation-0.9.3/data_disaggregation/classes.py`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.2/data_disaggregation/ext.py` & `data-disaggregation-0.9.3/data_disaggregation/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,21 +59,44 @@
 
     if to_is_multindex:
         return MultiIndex.from_product(to_levels_values, names=to_levels_names)
     else:
         return Index(to_levels_values[0], name=to_levels_names[0])
 
 
+def as_index(x) -> Index:
+    if isinstance(x, Index):
+        return x
+    elif isinstance(x, Series):
+        return x.index
+
+    raise TypeError(f"Must be of type Index instead of {type(x).__name__}")
+
+
+def as_series(x) -> Series:
+    if isinstance(x, Series):
+        return x
+    elif isinstance(x, Index):
+        return Series(1.0, index=x)
+
+    raise TypeError("Must be of type Series")
+
+
 def create_weight_map(
     weights: Series,
     idx_in: Index,
     idx_out: Index = None,
 ) -> Mapping[Tuple[F, T], float]:
+    weights = as_series(weights)
+    idx_in = as_index(idx_in)
+
     if idx_out is None:
         idx_out = get_idx_out(weights, idx_in)
+    # else:
+    #    idx_out = as_index(idx_out)
 
     map_levels = get_dimension_levels(weights)
     map_is_multindex = is_multindex(weights)
 
     from_levels = get_dimension_levels(idx_in)
     from_levels_names = [x[0] for x in from_levels]
     from_is_multindex = is_multindex(idx_in)
@@ -119,14 +142,19 @@
         if is_na(val_map):
             continue
 
         # get in/out keys
         key_in = get_key(row, from_level_idcs, from_is_multindex)
         key_out = get_key(row, to_level_idcs, to_is_multindex)
 
+        if key_in not in idx_in:
+            continue
+        if key_out not in idx_out:
+            continue
+
         key = (key_in, key_out)
         result[key] = val_map
 
     from_name = (
         tuple(from_levels_names) if len(from_levels_names) > 1 else from_levels_names[0]
     )
     to_name = tuple(to_levels_names) if len(to_levels_names) > 1 else to_levels_names[0]
```

### Comparing `data-disaggregation-0.9.2/data_disaggregation/utils.py` & `data-disaggregation-0.9.3/data_disaggregation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
 
 
 def iter_values(x):
     for k in x.keys():
         yield x[k]
 
 
+def as_set(x) -> set:
+    return set(as_list(x))
+
+
 def as_list(x) -> List:
     # meaning: is index
     if is_list(x):
         return x
     elif is_mapping(x):
         if hasattr(x, "index"):
             return x.index
```

### Comparing `data-disaggregation-0.9.2/data_disaggregation.egg-info/PKG-INFO` & `data-disaggregation-0.9.3/data_disaggregation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-disaggregation
-Version: 0.9.2
+Version: 0.9.3
 Author: Christian Winger
 License: MIT
 Project-URL: Documentation, https://wingechr.github.io/data-disaggregation
 Project-URL: Source, https://github.com/wingechr/data-disaggregation
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-disaggregation-0.9.2/setup.py` & `data-disaggregation-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         packages=["data_disaggregation"],
         name="data-disaggregation",
         install_requires=["pandas"],
         keywords=[],
         description="",
         long_description=long_description_md,
         long_description_content_type="text/markdown",
-        version="0.9.2",
+        version="0.9.3",
         author="Christian Winger",
         platforms=["any"],
         license="MIT",
         project_urls={
             "Documentation": "https://wingechr.github.io/data-disaggregation",
             "Source": "https://github.com/wingechr/data-disaggregation",
         },
```

### Comparing `data-disaggregation-0.9.2/test/test.py` & `data-disaggregation-0.9.3/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,30 +112,27 @@
         d1m = MultiIndex.from_product([d1])
         d2 = Index([2, 3], name="d2")
         d2m = MultiIndex.from_product([d2])
         d12 = MultiIndex.from_product([d1, d2])
         d3 = Index([4], name="d3")
         d23 = MultiIndex.from_product([d2, d3])
 
-        res = create_weight_map(Series(1, index=d12), d1, d2)
+        res = create_weight_map(Series(1, index=d12), idx_in=d1, idx_out=d2)
         self.assertEqual(res[(1, 2)], 1)
 
-        res = create_weight_map(Series(1, index=d12), d1m, d2)
+        res = create_weight_map(Series(1, index=d12), idx_in=d1m, idx_out=d2)
         self.assertEqual(res[((1,), 2)], 1)
 
-        res = create_weight_map(Series(1, index=d12), d1m, d2m)
+        res = create_weight_map(Series(1, index=d12), idx_in=d1m, idx_out=d2m)
         self.assertEqual(res[((1,), (2,))], 1)
 
-        res = create_weight_map(Series(1, index=d23), d12, d23)
+        res = create_weight_map(Series(1, index=d23), idx_in=d12, idx_out=d23)
         self.assertEqual(res[((1, 2), (2, 4))], 1)
 
-        res = create_weight_map(Series(1, index=d1), 0, d1)
-        self.assertEqual(res[(SCALAR_INDEX_KEY, 1)], 1)
-
-        res = create_weight_map(Series(1, index=d1), d1, d0)
+        res = create_weight_map(Series(1, index=d1), idx_in=d1, idx_out=d0)
         self.assertEqual(res[(1, SCALAR_INDEX_KEY)], 1)
 
     def test_is_scalar(self):
         for x in [1, None, "xyz", True]:
             res = (is_scalar(x), is_list(x), is_mapping(x))
             self.assertEqual(res, (True, False, False), x)
```

