# Comparing `tmp/macrometa-target-oracle-0.0.8.tar.gz` & `tmp/macrometa-target-oracle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.8.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.9.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.8.tar` & `macrometa-target-oracle-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35198 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 09:29:05.041839 macrometa-target-oracle-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.8/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35237 2023-07-06 09:40:54.271446 macrometa-target-oracle-0.0.9/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 09:40:54.523401 macrometa-target-oracle-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.9/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.9/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.8/LICENSE` & `macrometa-target-oracle-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.8/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.9/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.8/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.9/macrometa_target_oracle/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,14 +564,15 @@
                     merge_sql, droptable = self.merge_upsert_from_table(
                                                 from_table_name=tmp_table_name,
                                                 to_table_name=full_table_name,
                                                 schema=schema,
                                                 join_keys=join_keys,
                                             )
                     cur.execute(merge_sql)
+                    connection.commit()
                     cur.execute(droptable)
                     connection.commit()
                     self.logger.info("Merge complete.")
                 else:
                     insert_query, values = self.bulk_insert_records(
                                                 full_table_name=full_table_name,
                                                 schema=schema,
@@ -617,15 +618,15 @@
             USING {from_table_name} temp
             ON ({join_condition})
             WHEN MATCHED THEN
                 UPDATE SET
                     { update_stmt }
             WHEN NOT MATCHED THEN
                 INSERT ({", ".join(columns)})
-                VALUES ({", ".join([f"temp.{key}" for key in columns])});
+                VALUES ({", ".join([f"temp.{key}" for key in columns])})
         """  # nosec
 
         droptable = f"DROP TABLE {from_table_name}"
         return merge_sql, droptable
 
     def column_names(self):
         return [safe_column_name(name) for name in self.flatten_schema]
```

### Comparing `macrometa-target-oracle-0.0.8/pyproject.toml` & `macrometa-target-oracle-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.8'
+version='0.0.9'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.8/setup.py` & `macrometa-target-oracle-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.8/PKG-INFO` & `macrometa-target-oracle-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

