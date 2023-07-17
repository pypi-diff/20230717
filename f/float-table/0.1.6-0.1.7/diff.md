# Comparing `tmp/float_table-0.1.6.tar.gz` & `tmp/float_table-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.6.tar", max compression
+gzip compressed data, was "float_table-0.1.7.tar", max compression
```

## Comparing `float_table-0.1.6.tar` & `float_table-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.6/README.md
--rw-r--r--   0        0        0      165 2023-07-16 21:40:31.971112 float_table-0.1.6/float_table/__init__.py
--rw-r--r--   0        0        0     3046 2023-07-16 23:00:28.137583 float_table-0.1.6/float_table/fmt.py
--rw-r--r--   0        0        0      824 2023-07-16 23:10:39.833827 float_table-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     2763 2023-07-16 21:40:33.068136 float_table-0.1.6/tests/test.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.7/README.md
+-rw-r--r--   0        0        0      178 2023-07-17 09:50:19.103444 float_table-0.1.7/float_table/__init__.py
+-rw-r--r--   0        0        0     4645 2023-07-17 11:39:05.920922 float_table-0.1.7/float_table/fmt.py
+-rw-r--r--   0        0        0      844 2023-07-17 11:47:07.068481 float_table-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-17 11:23:41.558571 float_table-0.1.7/tests/test.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.7/PKG-INFO
```

### Comparing `float_table-0.1.6/pyproject.toml` & `float_table-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.6"
+version = "0.1.7"
 homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
@@ -24,14 +24,15 @@
 bump2version = "*"
 coverage = "*"
 pytest = ">=7.2.0"
 pytest-pycharm = "*"
 sigfig = "*"
 
 black = {extras = ["d"], version = "*"}
+tabulate = "^0.9.0"
 
 
 
 [tool.black]
 line-length = 100
 
 [build-system]
```

### Comparing `float_table-0.1.6/tests/test.py` & `float_table-0.1.7/tests/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             # Find the last digit
             idx_last_digit = len(x.rstrip()) - 1
             int(x[idx_last_digit])  # Make sure it's a digit
             pos_decimals.append(idx_last_digit + 1)
     assert min(pos_decimals) == max(pos_decimals)
 
 
-def test_exponent(num_column):
+def test_exponent_is_eng(num_column):
     exponent = determine_eng_exponent(num_column)
     assert exponent % 3 == 0
 
 
 def test_all_zeros():
     num_column = pd.Series([0, 0, 0])
     exponent = determine_eng_exponent(num_column)
@@ -76,14 +76,18 @@
         msg = f"For '{num_column.iloc[i]}', got '{actual.iloc[i]}', expected '{expected.iloc[i]}'"
         assert actual.iloc[i] == expected.iloc[i], msg
 
 
 def test_format_df():
     df = pd.DataFrame(
         {
-            "a": [1, 2, 3],
-            "b": ["not a number", 1.23456789, 1.23456789e-10],
+            "ints": [1, 2, 3],
+            "floats": [1.0, 2.0, 3.0],
+            "ints_and_floats": [1, 2.0, 3],
+            "string": ["not a number", 1.23456789, 1.23456789e-10],
         }
     )
     formatted = format_df(df, 2)
-    assert all(formatted["a"] == ["1.0", "2.0", "3.0"])
-    assert all(formatted["b"] == df["b"])
+    assert all(formatted["ints"] == ["1", "2", "3"])
+    assert all(formatted["floats"] == ["1.0", "2.0", "3.0"])
+    assert all(formatted["ints_and_floats"] == ["1.0", "2.0", "3.0"])
+    assert all(formatted["string"] == df["string"])
```

### Comparing `float_table-0.1.6/PKG-INFO` & `float_table-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: float-table
-Version: 0.1.6
+Version: 0.1.7
 Summary: Top-level package for float-table.
 Home-page: https://github.com/tadamcz/float-table
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

