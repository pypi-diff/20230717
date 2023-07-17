# Comparing `tmp/mysql-mimic-2.2.6.tar.gz` & `tmp/mysql-mimic-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.6.tar", last modified: Wed Jul 12 22:47:51 2023, max compression
+gzip compressed data, was "mysql-mimic-2.2.7.tar", last modified: Mon Jul 17 18:24:14 2023, max compression
```

## Comparing `mysql-mimic-2.2.6.tar` & `mysql-mimic-2.2.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.080466 mysql-mimic-2.2.6/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.080466 mysql-mimic-2.2.6/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 22:47:51.000000 mysql-mimic-2.2.6/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:47:51.084466 mysql-mimic-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 22:47:21.000000 mysql-mimic-2.2.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.6/LICENSE` & `mysql-mimic-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/PKG-INFO` & `mysql-mimic-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.6
+Version: 2.2.7
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.6/README.md` & `mysql-mimic-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/auth.py` & `mysql-mimic-2.2.7/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/charset.py` & `mysql-mimic-2.2.7/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/connection.py` & `mysql-mimic-2.2.7/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/constants.py` & `mysql-mimic-2.2.7/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/errors.py` & `mysql-mimic-2.2.7/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/intercept.py` & `mysql-mimic-2.2.7/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/packets.py` & `mysql-mimic-2.2.7/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/results.py` & `mysql-mimic-2.2.7/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/schema.py` & `mysql-mimic-2.2.7/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/server.py` & `mysql-mimic-2.2.7/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/session.py` & `mysql-mimic-2.2.7/mysql_mimic/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,19 +260,28 @@
     def _set_var_hint(self, expression: exp.Expression) -> Iterator[None]:
         """Handles any SET_VAR hints, which set system variables for a single statement"""
         hint = expression.args.get("hint")
         if not hint:
             yield
             return
 
+        set_var_hint = None
         assignments = {}
         for e in hint.expressions:
             if isinstance(e, exp.Func) and e.name == "SET_VAR":
-                eq = e.expressions[0]
-                assignments[eq.left.name] = expression_to_value(eq.right)
+                set_var_hint = e
+                for eq in e.expressions:
+                    assignments[eq.left.name] = expression_to_value(eq.right)
+
+        if set_var_hint:
+            set_var_hint.pop()
+
+        # Remove the hint entirely if SET_VAR was the only expression
+        if not hint.expressions:
+            hint.pop()
 
         orig = {k: self.variables.get(k) for k in assignments}
         try:
             for k, v in assignments.items():
                 self.variables.set(k, v)
             yield
         finally:
```

### Comparing `mysql-mimic-2.2.6/mysql_mimic/stream.py` & `mysql-mimic-2.2.7/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/types.py` & `mysql-mimic-2.2.7/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/utils.py` & `mysql-mimic-2.2.7/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic/variables.py` & `mysql-mimic-2.2.7/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.2.7/mysql_mimic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.6
+Version: 2.2.7
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.6/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.2.7/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/setup.py` & `mysql-mimic-2.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/tests/test_auth.py` & `mysql-mimic-2.2.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/tests/test_query.py` & `mysql-mimic-2.2.7/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,22 @@
             "SELECT @@max_execution_time",
             [{"@@max_execution_time": 0}],
         ),
         (
             "SELECT /*+ SET_VAR(max_execution_time=1) */ @@max_execution_time",
             [{"@@max_execution_time": 1}],
         ),
+        (
+            "SELECT /*+ SET_VAR(max_execution_time=1, sql_mode = 'foo') */ @@max_execution_time, @@sql_mode",
+            [{"@@max_execution_time": 1, "@@sql_mode": "foo"}],
+        ),
+        (
+            "SELECT /*+ SET_VAR(max_execution_time=1, sql_mode = 'foo') EXECUTE_AS('barak_alon') */ @@max_execution_time, @@sql_mode",
+            [{"@@max_execution_time": 1, "@@sql_mode": "foo"}],
+        ),
         # SET names
         (
             """
             SET NAMES utf8;
             SELECT @@character_set_client, @@SESSION.character_set_connection, @@character_set_results, @@collation_connection""",
             [
                 {
```

### Comparing `mysql-mimic-2.2.6/tests/test_ssl.py` & `mysql-mimic-2.2.7/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/tests/test_stream.py` & `mysql-mimic-2.2.7/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/tests/test_types.py` & `mysql-mimic-2.2.7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.6/tests/test_variables.py` & `mysql-mimic-2.2.7/tests/test_variables.py`

 * *Files identical despite different names*

