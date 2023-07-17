# Comparing `tmp/npgbq-2.1.8.tar.gz` & `tmp/npgbq-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npgbq-2.1.8.tar", last modified: Mon Apr 24 10:57:29 2023, max compression
+gzip compressed data, was "npgbq-2.1.9.tar", last modified: Fri May 12 10:40:30 2023, max compression
```

## Comparing `npgbq-2.1.8.tar` & `npgbq-2.1.9.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.484221 npgbq-2.1.8/
--rw-rw-rw-   0        0        0     1083 2023-04-12 05:59:51.000000 npgbq-2.1.8/LICENSE
--rw-rw-rw-   0        0        0     2771 2023-04-24 10:57:29.484221 npgbq-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2023-04-24 10:56:16.000000 npgbq-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.459718 npgbq-2.1.8/npgbq/
--rw-rw-rw-   0        0        0      677 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.477718 npgbq-2.1.8/npgbq/connectors/
--rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/__init__.py
--rw-rw-rw-   0        0        0     4052 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/dtype_mapper.py
--rw-rw-rw-   0        0        0      475 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/mssql.py
--rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/mysql.py
--rw-rw-rw-   0        0        0      386 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/postgres.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.480219 npgbq-2.1.8/npgbq/core/
--rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/__init__.py
--rw-rw-rw-   0        0        0     7842 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/helper_phone_number_th.py
--rw-rw-rw-   0        0        0     1298 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/log_table_schema.py
--rw-rw-rw-   0        0        0    39415 2023-04-24 10:54:15.000000 npgbq-2.1.8/npgbq/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.474719 npgbq-2.1.8/npgbq.egg-info/
--rw-rw-rw-   0        0        0     2771 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 10:57:29.484719 npgbq-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-04-24 10:54:37.000000 npgbq-2.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.483219 npgbq-2.1.8/tests/
--rw-rw-rw-   0        0        0     1951 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_insert_excel.py
--rw-rw-rw-   0        0        0     1674 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_load_scbpt_mediaperf.py
--rw-rw-rw-   0        0        0     3342 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_load_scbpt_saleorder.py
--rw-rw-rw-   0        0        0     6165 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_oracle_ingest.py
--rw-rw-rw-   0        0        0     1334 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_script.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.619066 npgbq-2.1.9/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 05:59:51.000000 npgbq-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2771 2023-05-12 10:40:30.619066 npgbq-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2023-04-24 10:56:16.000000 npgbq-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.591567 npgbq-2.1.9/npgbq/
+-rw-rw-rw-   0        0        0      677 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.609569 npgbq-2.1.9/npgbq/connectors/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     4052 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/connectors/dtype_mapper.py
+-rw-rw-rw-   0        0        0      475 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/connectors/mssql.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/connectors/mysql.py
+-rw-rw-rw-   0        0        0      386 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/connectors/postgres.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.612069 npgbq-2.1.9/npgbq/core/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/core/__init__.py
+-rw-rw-rw-   0        0        0     7842 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/core/helper_phone_number_th.py
+-rw-rw-rw-   0        0        0     1298 2023-04-12 05:59:51.000000 npgbq-2.1.9/npgbq/core/log_table_schema.py
+-rw-rw-rw-   0        0        0    39273 2023-05-12 10:36:44.000000 npgbq-2.1.9/npgbq/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.606569 npgbq-2.1.9/npgbq.egg-info/
+-rw-rw-rw-   0        0        0     2771 2023-05-12 10:40:30.000000 npgbq-2.1.9/npgbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2023-05-12 10:40:30.000000 npgbq-2.1.9/npgbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:40:30.000000 npgbq-2.1.9/npgbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-05-12 10:40:30.000000 npgbq-2.1.9/npgbq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 10:40:30.000000 npgbq-2.1.9/npgbq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:40:30.619569 npgbq-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1718 2023-05-12 10:39:44.000000 npgbq-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:40:30.618068 npgbq-2.1.9/tests/
+-rw-rw-rw-   0        0        0      478 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_create_biglake.py
+-rw-rw-rw-   0        0        0     1645 2023-04-12 07:07:05.000000 npgbq-2.1.9/tests/test_encrypt_table.py
+-rw-rw-rw-   0        0        0      518 2023-04-12 07:06:59.000000 npgbq-2.1.9/tests/test_encrypt_table_read_data.py
+-rw-rw-rw-   0        0        0     1951 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_insert_excel.py
+-rw-rw-rw-   0        0        0     1674 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_load_scbpt_mediaperf.py
+-rw-rw-rw-   0        0        0     3342 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_load_scbpt_saleorder.py
+-rw-rw-rw-   0        0        0     6165 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_oracle_ingest.py
+-rw-rw-rw-   0        0        0      185 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_random.py
+-rw-rw-rw-   0        0        0     1334 2023-04-12 05:59:51.000000 npgbq-2.1.9/tests/test_script.py
```

### Comparing `npgbq-2.1.8/LICENSE` & `npgbq-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/PKG-INFO` & `npgbq-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgbq
-Version: 2.1.8
+Version: 2.1.9
 Summary: A package designed for helping everyone in the team to work with data ingestion
 Home-page: https://github.com/noppGithub/npgbq
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `npgbq-2.1.8/README.md` & `npgbq-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/npgbq/__init__.py` & `npgbq-2.1.9/npgbq/__init__.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/npgbq/connectors/dtype_mapper.py` & `npgbq-2.1.9/npgbq/connectors/dtype_mapper.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/npgbq/core/helper_phone_number_th.py` & `npgbq-2.1.9/npgbq/core/helper_phone_number_th.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/npgbq/core/log_table_schema.py` & `npgbq-2.1.9/npgbq/core/log_table_schema.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/npgbq/core/tools.py` & `npgbq-2.1.9/npgbq/core/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         for table in tables:
             table_name = table.split(".")[-1]
             self.delete_bq_table(dataset_name, table_name)
         try:
             dataset_name = f"{self.client.project}.{dataset_name}"
             dataset = bigquery.Dataset(dataset_name)
             dataset.location = "asia-southeast1"
-            dataset = self.client.delete_dataset(dataset, timeout=30)
+            self.client.delete_dataset(dataset, timeout=30)
         except Exception as e:
             print(f"Can not create the dataset: {e}")
         else:
             print(f"Deleted dataset: {dataset_name}")
 
     def create_bq_table(self, dataset_id, table_id, schema):
         try:
@@ -782,18 +782,17 @@
 
     def convert_dtype(self, df: pd.DataFrame, schema_bq: List[bigquery.SchemaField]):
         for sch in schema_bq:
             print(f"Converting: {sch.name}")
             data_type = sch.field_type
             if data_type in ("NUMERIC", "BIGNUMERIC"):
                 df[sch.name] = df[sch.name].apply(self.convert_to_decimal)  # type: ignore it can handle None
-            elif data_type in ("TIMESTAMP"):
+            elif data_type in ("TIMESTAMP","DATETIME"):
                 df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce")
             elif data_type in ("DATE"):
-                # https://stackoverflow.com/questions/64317195/python-google-cloud-bigquery-parquet-column-date-has-type-int64-which-does-not
                 df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce").dt.date
             elif data_type in ("TIME"):
                 df[sch.name] = df[sch.name].apply(self.convert_time)  # type: ignore it can handle None
             elif data_type in ("STRING"):
                 df[sch.name] = df[sch.name].astype(str)
             elif data_type in ("INTEGER"):
                 df[sch.name] = df[sch.name].astype("float")
```

### Comparing `npgbq-2.1.8/npgbq.egg-info/PKG-INFO` & `npgbq-2.1.9/npgbq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgbq
-Version: 2.1.8
+Version: 2.1.9
 Summary: A package designed for helping everyone in the team to work with data ingestion
 Home-page: https://github.com/noppGithub/npgbq
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `npgbq-2.1.8/npgbq.egg-info/SOURCES.txt` & `npgbq-2.1.9/npgbq.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,12 +12,16 @@
 npgbq/connectors/mssql.py
 npgbq/connectors/mysql.py
 npgbq/connectors/postgres.py
 npgbq/core/__init__.py
 npgbq/core/helper_phone_number_th.py
 npgbq/core/log_table_schema.py
 npgbq/core/tools.py
+tests/test_create_biglake.py
+tests/test_encrypt_table.py
+tests/test_encrypt_table_read_data.py
 tests/test_insert_excel.py
 tests/test_load_scbpt_mediaperf.py
 tests/test_load_scbpt_saleorder.py
 tests/test_oracle_ingest.py
+tests/test_random.py
 tests/test_script.py
```

### Comparing `npgbq-2.1.8/setup.py` & `npgbq-2.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Read long description from the readme.md file
-with open("README.md") as f:
+with open("README.md",encoding='utf-8') as f:
     readme = f.read()
 
-with open("LICENSE") as f:
-    license = f.read()
+with open("LICENSE",encoding='utf-8') as f:
+    license_text = f.read()
 
 setup(
     name="npgbq",
-    version="2.1.8",
+    version="2.1.9",
     description="A package designed for helping everyone in the team to work with data ingestion",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Nopporn Phantawee",
     author_email="n.phantawee@gmail.com",
     url="https://github.com/noppGithub/npgbq",
     license="MIT",
```

### Comparing `npgbq-2.1.8/tests/test_insert_excel.py` & `npgbq-2.1.9/tests/test_insert_excel.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/tests/test_load_scbpt_mediaperf.py` & `npgbq-2.1.9/tests/test_load_scbpt_mediaperf.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/tests/test_load_scbpt_saleorder.py` & `npgbq-2.1.9/tests/test_load_scbpt_saleorder.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/tests/test_oracle_ingest.py` & `npgbq-2.1.9/tests/test_oracle_ingest.py`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.8/tests/test_script.py` & `npgbq-2.1.9/tests/test_script.py`

 * *Files identical despite different names*

