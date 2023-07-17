# Comparing `tmp/smarterai-1.3.0.tar.gz` & `tmp/smarterai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smarterai-1.3.0.tar", last modified: Mon Jul 17 16:06:16 2023, max compression
+gzip compressed data, was "dist/smarterai-1.3.1.tar", last modified: Mon Jul 17 16:49:37 2023, max compression
```

## Comparing `smarterai-1.3.0.tar` & `smarterai-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-17 16:05:58.000000 smarterai-1.3.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:06:16.000000 smarterai-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5307 2023-07-17 16:05:58.000000 smarterai-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-17 16:05:58.000000 smarterai-1.3.0/VERSION.txt
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-17 16:05:58.000000 smarterai-1.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-17 16:06:16.000000 smarterai-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-17 16:05:58.000000 smarterai-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30853 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterApi.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8025 2023-07-17 16:05:58.000000 smarterai-1.3.0/smarterai/smarterStore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 16:06:16.000000 smarterai-1.3.0/smarterai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:49:37.000000 smarterai-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-17 16:49:21.000000 smarterai-1.3.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:49:37.000000 smarterai-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2023-07-17 16:49:21.000000 smarterai-1.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-17 16:49:21.000000 smarterai-1.3.1/VERSION.txt
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-17 16:49:21.000000 smarterai-1.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-17 16:49:37.000000 smarterai-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-17 16:49:21.000000 smarterai-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-17 16:49:21.000000 smarterai-1.3.1/smarterai/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30835 2023-07-17 16:49:21.000000 smarterai-1.3.1/smarterai/smarterApi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-17 16:49:21.000000 smarterai-1.3.1/smarterai/smarterInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8025 2023-07-17 16:49:21.000000 smarterai-1.3.1/smarterai/smarterStore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 16:49:37.000000 smarterai-1.3.1/smarterai.egg-info/top_level.txt
```

### Comparing `smarterai-1.3.0/LICENSE.txt` & `smarterai-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/PKG-INFO` & `smarterai-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterai
-Version: 1.3.0
+Version: 1.3.1
 Summary: smarter.ai Python API
 Home-page: https://www.smarter.ai/
 Author: Nevine Soliman and Carlos Medina
 Author-email: dev@smarter.ai
 License: UNKNOWN
 Description: [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip/)
```

### Comparing `smarterai-1.3.0/README.md` & `smarterai-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/setup.cfg` & `smarterai-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/setup.py` & `smarterai-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/smarterai/smarterApi.py` & `smarterai-1.3.1/smarterai/smarterApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,24 +444,24 @@
             schema_name: the schema for the table. If not provided it will default to the current user's ID.
 
         Returns:
             True if the schema_name.table_name exits, False otherwise
         """
         if not schema_name:
             return_message = self.send_message(message=SmarterMessage(), port="#user")
-            current_schema_id = return_message.get("user", {}).get("currentSchema")
+            schema_name = return_message.get("user", {}).get("currentSchema")
         if "." in table_name:
             s_t = table_name.split(".")
             if len(s_t) != 2:
                 return False
-            current_schema_id = s_t[0]
+            schema_name = s_t[0]
             table_name = s_t[1]
         query = f"SELECT EXISTS (" \
                 f"SELECT FROM pg_tables " \
-                f"WHERE schemaname = '{current_schema_id}'" \
+                f"WHERE schemaname = '{schema_name}'" \
                 f"AND tablename  = '{table_name}')"
         res = self.query_data_lake(sql_query=query, commit=False)
         return res[0][0] if res else False
 
     def get_user_data(self, user_id: str = None, data_type_filter: str = None) -> Tuple:
         """
            Gets the current user's previously persisted data.
```

### Comparing `smarterai-1.3.0/smarterai/smarterInterface.py` & `smarterai-1.3.1/smarterai/smarterInterface.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/smarterai/smarterStore.py` & `smarterai-1.3.1/smarterai/smarterStore.py`

 * *Files identical despite different names*

### Comparing `smarterai-1.3.0/smarterai.egg-info/PKG-INFO` & `smarterai-1.3.1/smarterai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarterai
-Version: 1.3.0
+Version: 1.3.1
 Summary: smarter.ai Python API
 Home-page: https://www.smarter.ai/
 Author: Nevine Soliman and Carlos Medina
 Author-email: dev@smarter.ai
 License: UNKNOWN
 Description: [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip/)
```

