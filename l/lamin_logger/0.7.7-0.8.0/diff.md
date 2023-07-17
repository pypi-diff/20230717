# Comparing `tmp/lamin_logger-0.7.7.tar.gz` & `tmp/lamin_logger-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.7.tar` & `lamin_logger-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.7/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.7/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.7/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.7/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.7/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.7/docs/api.md
--rw-r--r--   0        0        0     5269 2023-07-14 11:49:04.376377 lamin_logger-0.7.7/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.7/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.7/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.7/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-07-14 11:48:56.688696 lamin_logger-0.7.7/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.7/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.7/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.7.7/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.7.7/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7410 2023-07-14 11:45:47.889453 lamin_logger-0.7.7/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.7/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3524 2023-07-10 09:54:24.354688 lamin_logger-0.7.7/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.7/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.7/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.7/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.7/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.7/tests/test_lookup.py
--rw-r--r--   0        0        0     6153 2023-07-14 11:45:47.889627 lamin_logger-0.7.7/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.7/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.7/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.8.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.8.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.8.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.8.0/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.8.0/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.8.0/docs/api.md
+-rw-r--r--   0        0        0     5443 2023-07-17 18:29:21.249400 lamin_logger-0.8.0/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.8.0/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.8.0/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.8.0/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-07-17 18:29:12.752109 lamin_logger-0.8.0/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.8.0/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.8.0/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.8.0/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.8.0/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7410 2023-07-14 11:45:47.889453 lamin_logger-0.8.0/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.8.0/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3462 2023-07-17 18:27:14.475596 lamin_logger-0.8.0/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.8.0/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.8.0/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.8.0/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.8.0/tests/test_lookup.py
+-rw-r--r--   0        0        0     6153 2023-07-14 11:45:47.889627 lamin_logger-0.8.0/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.8.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2450 2023-07-17 18:27:14.475937 lamin_logger-0.8.0/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.8.0/PKG-INFO
```

### Comparing `lamin_logger-0.7.7/.github/workflows/build.yml` & `lamin_logger-0.8.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/.github/workflows/latest-changes.yml` & `lamin_logger-0.8.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/.gitignore` & `lamin_logger-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/.pre-commit-config.yaml` & `lamin_logger-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/LICENSE` & `lamin_logger-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/docs/changelog.md` & `lamin_logger-0.8.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Always return df for `search`, added `limit=` | [37](https://github.com/laminlabs/lamin-logger/pull/37) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-17 | 0.8.0
 🐛 Fix map_synonyms bug | [36](https://github.com/laminlabs/lamin-logger/pull/36) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-14 | 0.7.7
 ⚡️ Speed up search 150x | [35](https://github.com/laminlabs/lamin-logger/pull/35) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-10 | 0.7.6
 🐛 Fix existing_categories for map_synonyms | [34](https://github.com/laminlabs/lamin-logger/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-05 | 0.7.5
 🚑️ Fix for multiple matches in map_synonyms | [33](https://github.com/laminlabs/lamin-logger/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-02 | 0.7.4
 🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
```

### Comparing `lamin_logger-0.7.7/docs/quickstart.ipynb` & `lamin_logger-0.8.0/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_core.py` & `lamin_logger-0.8.0/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_inspect.py` & `lamin_logger-0.8.0/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_logger.py` & `lamin_logger-0.8.0/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_lookup.py` & `lamin_logger-0.8.0/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_map_synonyms.py` & `lamin_logger-0.8.0/lamin_logger/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_python_version.py` & `lamin_logger-0.8.0/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/lamin_logger/_search.py` & `lamin_logger-0.8.0/lamin_logger/_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,76 @@
-from typing import Any, Literal, Union
+from typing import Any, Literal, Optional, Union
 
 from lamin_logger import logger
 
 
 def search(
     df: Any,
     string: str,
     field: str = "name",
+    limit: Optional[int] = None,
     synonyms_field: Union[str, None] = "synonyms",
-    case_sensitive: bool = True,
-    return_ranked_results: bool = False,
+    case_sensitive: bool = False,
     synonyms_sep: str = "|",
     keep: Literal["first", "last", False] = "first",
-    tuple_name: str = "SearchResult",
 ) -> Any:
     """Search a given string against a field.
 
     Args:
         string: The input string to match against the field ontology values.
         field: The field against which the input string is matching.
         synonyms_field: Also map against in the synonyms
             If None, no mapping against synonyms.
         case_sensitive: Whether the match is case sensitive.
-        return_ranked_results: If True, return all entries ranked by matching ratios.
+        limit: maximum amount of top results to return.
+            If None, return all results.
 
     Returns:
-        Best match record of the input string.
+        A DataFrame of ranked results.
     """
     import pandas as pd
 
     from ._map_synonyms import explode_aggregated_column_to_map
 
-    def _fuzz_ratio(string: str, iterable: pd.Series, case_sensitive: bool = True):
-        from rapidfuzz import fuzz, utils
+    def _fuzz_ratio(
+        string: str,
+        iterable: pd.Series,
+        case_sensitive: bool = True,
+        limit: Optional[int] = None,
+    ):
+        from rapidfuzz import fuzz, process, utils
 
         processor = None if case_sensitive else utils.default_process
-        return iterable.apply(lambda x: fuzz.ratio(string, x, processor=processor))
+
+        results = process.extract(
+            string,
+            iterable,
+            scorer=fuzz.ratio,
+            limit=limit,
+            processor=processor,
+        )
+        return pd.DataFrame(results).set_index(2)[1]
 
     # empty DataFrame
     if df.shape[0] == 0:
-        if return_ranked_results:
-            return df
-        else:
-            return None
+        return df
 
     # search against each of the synonyms
     if (synonyms_field in df.columns) and (synonyms_field != field):
         # creates field_value:synonym
         mapper = explode_aggregated_column_to_map(
             df,
             agg_col=synonyms_field,  # type:ignore
             target_col=field,
             keep=keep,
             sep=synonyms_sep,
         )
         if keep is False:
             mapper = mapper.explode()
-        # adds field_value:field_value
+        # adds field_value:field_value to field_value:synonym
         df_field = pd.Series(df[field].values, index=df[field], name=field)
         df_field.index.name = synonyms_field
         df_field = df_field[df_field.index.difference(mapper.index)]
         mapper = pd.concat([mapper, df_field])
         df_exp = mapper.reset_index()
         target_column = synonyms_field
     else:
@@ -69,28 +79,25 @@
                 "Input field is the same as synonyms field, skipping synonyms matching"
             )
         df_exp = df[[field]].copy()
         target_column = field
 
     # add matching scores as a __ratio__ column
     df_exp["__ratio__"] = _fuzz_ratio(
-        string=string, iterable=df_exp[target_column], case_sensitive=case_sensitive
+        string=string,
+        iterable=df_exp[target_column],
+        case_sensitive=case_sensitive,
+        limit=limit,
     )
+    if limit is not None:
+        df_exp = df_exp[~df_exp["__ratio__"].isna()]
     # only keep the max score between field and synonyms for each entry
-    df_exp_grouped = (
-        df_exp.groupby(field).max("__ratio__").sort_values("__ratio__", ascending=False)
-    )
-    # subset to original field values (as synonyms were mixed in before)
-    df_exp_grouped = df_exp_grouped[df_exp_grouped.index.isin(df[field])]
+    if target_column == synonyms_field:
+        df_exp_grouped = df_exp.groupby(field).max("__ratio__")
+        # subset to original field values (as synonyms were mixed in before)
+        df_exp_grouped = df_exp_grouped[df_exp_grouped.index.isin(df[field])]
+    else:
+        df_exp_grouped = df_exp.set_index(field)
     df_scored = df.set_index(field).loc[df_exp_grouped.index]
     df_scored["__ratio__"] = df_exp_grouped["__ratio__"]
 
-    if return_ranked_results:
-        return df_scored.sort_values("__ratio__", ascending=False)
-    else:
-        res = df_scored[df_scored["__ratio__"] == df_scored["__ratio__"].max()]
-        res = res.drop(columns=["__ratio__"])
-        res_records = list(res.reset_index().itertuples(index=False, name=tuple_name))
-        if len(res_records) == 1:
-            return res_records[0]
-        else:
-            return res_records
+    return df_scored.sort_values("__ratio__", ascending=False)
```

### Comparing `lamin_logger-0.7.7/pyproject.toml` & `lamin_logger-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/tests/test_inspect.py` & `lamin_logger-0.8.0/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/tests/test_lookup.py` & `lamin_logger-0.8.0/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/tests/test_map_synonyms.py` & `lamin_logger-0.8.0/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.7/tests/test_search.py` & `lamin_logger-0.8.0/tests/test_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,61 +31,55 @@
             "synonyms": "cardiac pacemaker cell|myocytus nodalis|P cell",
             "children": ["CL:1000409", "CL:1000410"],
         },
     ]
     return pd.DataFrame.from_records(records)
 
 
-def test_search_name_default(df):
-    res = search(df=df, string="T cells", tuple_name="MyTuple")
-    assert res.name == "T cell"
-    assert res.ontology_id == "CL:0000084"
-    assert res.children == ["CL:0000798", "CL:0002420", "CL:0002419", "CL:0000789"]
-    assert res.synonyms == "T-cell|T lymphocyte|T-lymphocyte"
-    assert res.__class__.__name__ == "MyTuple"
-
-
 def test_search_synonyms(df):
     res = search(df=df, string="P cells")
-    assert res.name == "nodal myocyte"
+    assert res.index[0] == "nodal myocyte"
 
+    # without synonyms search
     res = search(df=df, synonyms_field=None, string="P cells")
-    assert res.name == "PP cell"
+    assert res.index[0] == "PP cell"
+
+
+def test_search_limit(df):
+    res = search(df=df, string="P cells", limit=1)
+    assert res.shape[0] == 1
 
 
 def test_search_keep(df):
+    # TODO: better test here
     res = search(df=df, string="enteroendocrine", keep=False)
-    assert res.name == "PP cell"
+    assert res.index[0] == "PP cell"
 
 
 def test_search_return_df(df):
-    res = search(df=df, string="P cells", return_ranked_results=True)
+    res = search(df=df, string="P cells")
     assert res.shape == (4, 4)
     assert res.iloc[0].name == "nodal myocyte"
 
 
 def test_search_return_tie_results(df):
     res = search(df=df, string="A cell", synonyms_field=None)
-    assert len(res) == 2
+    assert res.iloc[0].__ratio__ == res.iloc[1].__ratio__
 
 
 def test_search_non_default_field(df):
     res = search(df=df, string="type F enteroendocrine", field="synonyms")
-    res.synonyms == "type F enteroendocrine cell"
+    assert res.index[0] == "type F enteroendocrine cell"
 
 
 def test_search_case_sensitive(df):
     res = search(df=df, string="b cell", case_sensitive=True)
-    assert len(res) == 3
+    assert res.iloc[0].__ratio__ < 100
 
     res = search(df=df, string="b cell", case_sensitive=False)
-    assert res.name == "B cell"
+    assert res.index[0] == "B cell"
+    assert res.iloc[0].__ratio__ == 100
 
 
 def test_search_empty_df():
-    res = search(
-        pd.DataFrame(columns=["a", "b", "c"]), string="", return_ranked_results=True
-    )
-    assert res.shape == (0, 3)
-
     res = search(pd.DataFrame(columns=["a", "b", "c"]), string="")
-    assert res is None
+    assert res.shape == (0, 3)
```

### Comparing `lamin_logger-0.7.7/PKG-INFO` & `lamin_logger-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.7
+Version: 0.8.0
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

