# Comparing `tmp/dataflat-1.0.6.tar.gz` & `tmp/dataflat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflat-1.0.6.tar", last modified: Thu Jun 29 22:47:35 2023, max compression
+gzip compressed data, was "dataflat-1.1.0.tar", last modified: Mon Jul 17 21:41:48 2023, max compression
```

## Comparing `dataflat-1.0.6.tar` & `dataflat-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-29 22:47:25.000000 dataflat-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:47:35.411036 dataflat-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 22:47:25.000000 dataflat-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/dictionary/flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/flattener_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/pandas_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/pandas_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/pandas_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/spark_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/spark_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/spark_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:47:35.411036 dataflat-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-29 22:47:25.000000 dataflat-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.676391 dataflat-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-17 21:41:35.000000 dataflat-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-17 21:41:48.672391 dataflat-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-17 21:41:35.000000 dataflat-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/dictionary/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/flattener_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat/pandas_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/pandas_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/pandas_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat/spark_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/spark_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/spark_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-17 21:41:35.000000 dataflat-1.1.0/dataflat/utils/case_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:41:48.672391 dataflat-1.1.0/dataflat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-17 21:41:48.000000 dataflat-1.1.0/dataflat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-17 21:41:48.000000 dataflat-1.1.0/dataflat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:41:48.000000 dataflat-1.1.0/dataflat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 21:41:48.000000 dataflat-1.1.0/dataflat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 21:41:48.000000 dataflat-1.1.0/dataflat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:41:48.676391 dataflat-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-17 21:41:35.000000 dataflat-1.1.0/setup.py
```

### Comparing `dataflat-1.0.6/LICENSE` & `dataflat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.6/dataflat/commons.py` & `dataflat-1.1.0/dataflat/commons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-commons.py - a script file for common used functions
+dataflat/commons.py - a script file for common used functions
 
 Copyright (C) 2023 Juan ROJAS
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dataflat-1.0.6/dataflat/exceptions.py` & `dataflat-1.1.0/dataflat/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-exceptions.py - an exception classes script
+dataflat/exceptions.py - an exception classes script
 
 Copyright (C) 2023 Juan ROJAS
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dataflat-1.0.6/dataflat/pandas_df/flattener.py` & `dataflat-1.1.0/dataflat/pandas_df/flattener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-pandas_df/flattener.py - The processor script for pandas dataframes flattening process
+dataflat/pandas_df/flattener.py - The processor script for pandas dataframes flattening process
 
 Copyright (C) 2023 Juan ROJAS
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -19,75 +19,75 @@
 
 import pandas as pd
 from typeguard import typechecked
 from typing import List
 from dataflat.commons import init_logger
 from dataflat.exceptions import FlatteningException
 from dataflat.dictionary.flattener import CustomFlattener as DictionaryCustomFlattener
+from dataflat.utils.case_translator import CustomCaseTranslator
 
 logger = init_logger(__name__)
 
 @typechecked
 class CustomFlattener():
-    def __init__(self):
+    def __init__(self, case_translator:CustomCaseTranslator, replace_dots:bool):
         logger.info("CustomFlattener for Pandas Dataframes has been initiated")
+        self._case_translator = case_translator
+        self._replace_dots = replace_dots
 
 
-    def transform(self, dataframe:pd.DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", to_snake_case:bool = False, replace_dots:bool = False, chunk_size:int = 500) -> dict:
+    def transform(self, dataframe:pd.DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", chunk_size:int = 500) -> dict:
         """Receive a pandas Dataframe, and return a dictionary with the
         flattenend pandas Dataframes.
         If a black_list is provided then all the column names inside the black_list will
         be skipped. Notice that if ['name'] is provided as black list, then 
         all the 'name' columns will be skipped, even if they are under a nested
         column.
         The dataframe_name will be used to reference each resulting flattened dataframe
         under the processed_dataframes dictionary returned.
 
-        BEAWARE: This function will convert the dataframe to multiple dicitonaries (one per row) 
-        and process them using the DictionaryProcessor.
-        If you already have dictionaries before converting them to Dataframe, use DictionaryProcessor first, and later
-        convert the resulting dictionaries to Dataframes.
-
         Parameters
         ----------
         df: pandas.Dataframe
             The dataframe to be flattened.
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str], (default [])
             A list of keys to ignore and not to add to the resulting flattened dictionary.
         dataframe_name: str, (default 'df')
             A reference name for the dataframe, used to difference each
             resulting dataframe in the processed_dataframes return.
-        to_snake_case: bool
-            If True process the column name to Snake Case.
-        replace_dots: bool
-            If True replace the column name dots with underscores.
         chunk_size: int, (default 500)
             The chunk size used to process the dataframe in batches. 
             i.e. If dataframe size is 2000, and chunk_size is 500,
             then the dataframe will be processed in 4 batches.
 
         Returns
         -------
         processed_dicts : dict
         """
         dataframe_len = len(dataframe)
         if dataframe_len == 0:
             raise FlatteningException("The provided dataframe is empty.")
     
-        flattener = DictionaryCustomFlattener()
+        dict_flattener = DictionaryCustomFlattener(self._case_translator, self._replace_dots)
         processed_dataframes = {}
 
         for i in range(0, dataframe_len, chunk_size):
             records = dataframe[i:i+chunk_size].to_dict('records')
+            processed_dictionaries = {}
             for dictionary in records:
-                processed_dictionary = flattener.transform(dictionary, id_key, black_list, dataframe_name, 
-                                                           to_snake_case=to_snake_case,
-                                                           replace_dots=replace_dots)
-                for key, value in processed_dictionary.items():
-                    print(f"{key}: {value}")
-                    try:
-                        processed_dataframes[key].extend( processed_dictionary[key] )
-                    except:
-                        processed_dataframes[key] = processed_dictionary[key]
+                processed_data = dict_flattener.transform(dictionary, id_key, black_list, dataframe_name)
+                for key, value in processed_data.items():
+                    if  key not in processed_dictionaries:
+                        if isinstance(value, list):
+                            processed_dictionaries[key] = value
+                        else:
+                            processed_dictionaries[key] = [value]
+                    else:
+                        if isinstance(value, list):
+                            processed_dictionaries[key].extend(value)
+                        else:
+                            processed_dictionaries[key].extend([value])
+                for key, value in processed_dictionaries.items():
+                    processed_dataframes[key] = pd.DataFrame.from_dict(value)
         return processed_dataframes
```

### Comparing `dataflat-1.0.6/dataflat/spark_df/flattener.py` & `dataflat-1.1.0/dataflat/spark_df/flattener.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-spark_df/flattener.py - The processor script for spark dataframes flattening process
+dataflat/spark_df/flattener.py - The processor script for spark dataframes flattening process
 
 Copyright (C) 2023 Juan ROJAS
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -19,59 +19,41 @@
 
 import json
 import re
 from typeguard import typechecked
 from typing import List
 from dataflat.commons import init_logger
 from dataflat.exceptions import FlatteningException
+from dataflat.utils.case_translator import CustomCaseTranslator
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql.functions import posexplode
 
 logger = init_logger(__name__)
 
 @typechecked
 class CustomFlattener():
-    def __init__(self):
+    def __init__(self, case_translator:CustomCaseTranslator, replace_dots:bool):
         logger.info("CustomFlattener for PySpark Dataframes has been initiated")
+        self._case_translator = case_translator
+        self._reference_separator = "_" if replace_dots else "."
 
-    def _to_snake_case(self, process_col:bool, col_name:str):
-        if process_col:
-            pattern = re.compile(r'(?<!^)(?=[A-Z])')
-            return pattern.sub('_', col_name).lower().replace("__", "_").replace("._", ".")
-        return col_name
-    
-    def _replace_dots(self, process_col:bool, col_name:str):
-        if process_col:
-            return col_name.replace(".", "_")
-        return col_name
-
-    def _process_column_name(self, dataframe:DataFrame, to_snake_case:bool, replace_dots:bool):
-        """Receive a Spark Dataframe and return a snake_case columns like dataframe.
-        If replace_dots is True, then all the subcolumns like "Column.SubColumn" will be
-        renamed as "Column_SubColumn".
-        Parameters
-        ----------
-        dataframe: pyspark.Dataframe
-            The Spark Dataframe to rename each column to snake_case and replace dots with underscores.
-        to_snake_case: bool
-            If True rename the column to Snake Case column name like.
-        replace_dots: bool
-            If True replace the column name dots with underscores.
-        Returns
-        -------
-        dataframe: pyspark.Dataframe
-        """
+
+    def _process_strings(self, strings:List[str], join_key:str):
+        return join_key.join([self._case_translator.translate(string) for string in strings if string!=""])
+
+
+    def _process_dataframe_columns(self, dataframe_name:str, dataframe:DataFrame):
         for col in dataframe.columns:
-            renamed_col = self._to_snake_case(to_snake_case, col)
-            renamed_col = self._replace_dots(replace_dots, renamed_col)
-            if to_snake_case | replace_dots:
-                dataframe = dataframe.withColumnRenamed(col, renamed_col)
-        return dataframe
+            renamed_col = re.sub(f"{self._reference_separator}+", self._reference_separator, self._process_strings(col.split("."), self._reference_separator))
+            dataframe = dataframe.withColumnRenamed(col, renamed_col)
+        dataframe_name = re.sub(f"\\{self._reference_separator}\\{self._reference_separator}+", self._reference_separator, self._process_strings(dataframe_name.split("."), self._reference_separator))
+        return (dataframe_name, dataframe)
+
 
-    def _get_schema_struct(self, dataframe_schema:dict, id_key:str, black_list:List[str], dataframe_name:str, _ref:str = "", named_struct:dict = {}):
+    def _get_schema_struct(self, dataframe_schema:dict, id_key:str, dataframe_name:str, _ref:str = "", named_struct:dict = {}):
         """Receive Spark Dataframe Schema in dictionary format, and return 
         a dictionary[str, str] with the all required named_struct expressions
         to flatten de Dataframe.
         Parameters
         ----------
         dataframe_schema: dict
             A dictionary with the Dataframe schema.
@@ -86,35 +68,38 @@
         Returns
         -------
         named_struct: dict[str, str]
             A dictionary with all the named_struct expressions to flatten the
             provided Dataframe schema.
         """
         for field in dataframe_schema['fields']:
-            if field['name'] not in black_list:
+            if field['name'] not in self._black_list:
                 field_ref = _ref + f"`{field['name']}`"
                 field_name = field_ref.replace("`","").replace(f"{dataframe_name.split('.')[-1]}.","")
                 if type(field['type']) is dict:
                     if field['type']['type'] == "array":
+                        field_name_aux = 'value' if isinstance(field['type']['elementType'], str) else field_name
+                        
                         try:
-                            named_struct[f"{dataframe_name}.{field_name}"] += f"'{dataframe_name}_id',{id_key},'{field_name}',{field_ref},"
+                            named_struct[f"{dataframe_name}.{field_name}"] += f"'{self._parent_df_name}_{self._parent_id_key}',{id_key},'{field_name_aux}',{field_ref},"
                         except:
-                            named_struct[f"{dataframe_name}.{field_name}"] = f"'{dataframe_name}_id',{id_key},'{field_name}',{field_ref},"
+                            named_struct[f"{dataframe_name}.{field_name}"] = f"'{self._parent_df_name}_{self._parent_id_key}',{id_key},'{field_name_aux}',{field_ref},"
                     else:
-                        named_struct = self._get_schema_struct(field['type'], id_key, black_list, dataframe_name, f"{field_ref}.", named_struct)
+                        named_struct = self._get_schema_struct(field['type'], id_key, dataframe_name, f"{field_ref}.", named_struct)
                 elif field['type'] == "map":
-                    print(f"MapType is not supported, skipping column: {field_name}")
+                    logger.warning(f"MapType is not supported, skipping column: {field_name}")
                 else:
                     try:
                         named_struct[dataframe_name] += f"'{field_name}',{field_ref},"
                     except:
                         named_struct[dataframe_name] = f"'{field_name}',{field_ref},"
         return named_struct
 
-    def _processor(self, dataframe:DataFrame, id_key:str, black_list:List[str], dataframe_name:str):
+
+    def _processor(self, dataframe:DataFrame, id_key:str, dataframe_name:str):
         """Receive a pyspark.Dataframe and returns a Dictionary[str, pyspark.DataFrame]
         with all the processed dataframes.
         Parameters
         ----------
         dataframe: pyspark.DataFrame
             A Dataframe to be flattened
         id_key: str
@@ -129,40 +114,41 @@
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
         processed_data = {}
         schema = json.loads(dataframe.schema.json())
-        ns = self._get_schema_struct(schema, id_key, black_list, dataframe_name, _ref="", named_struct={})
-        parent_pos = f",'{dataframe_name}_pos',`pos`" if "'pos',`pos`" in ns[dataframe_name] else ""
+        ns = self._get_schema_struct(schema, id_key, dataframe_name, _ref="", named_struct={})
+        parent_pos = f",'{dataframe_name}_index',`index`" if "'index',`index`" in ns[dataframe_name] else ""
         for df_name, struct in ns.items():
             if df_name != dataframe_name:
                 selectExpr = f"named_struct( {struct[:-1]}{parent_pos} ) as Item"
                 aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
                 child_id_key = aux_df.columns[0] if "." not in aux_df.columns[0] else f"`{aux_df.columns[0]}`"
                 expld_col = aux_df.columns[1]
                 expld_expr = expld_col if "." not in expld_col else f"`{expld_col}`"
-                selected_cols = [child_id_key, posexplode(expld_expr).alias('pos', expld_col)]
+                selected_cols = [child_id_key, posexplode(expld_expr).alias('index', expld_col)]
                 if parent_pos:
-                    selected_cols.append(f'`{dataframe_name}_pos`')
+                    selected_cols.append(f'`{dataframe_name}_index`')
                 aux_df = aux_df.select(selected_cols) \
                     .withColumnRenamed(expld_col, expld_col.split(".")[-1])
                 processed_data[df_name] = aux_df
                 for types in aux_df.dtypes:
                     if "struct<" in types[1]:
-                        nested_dfs = self._processor(aux_df, child_id_key, black_list, df_name)
+                        nested_dfs = self._processor(aux_df, child_id_key, df_name)
                         processed_data.update(nested_dfs)
             else:
                 selectExpr = f"named_struct( {struct[:-1]} ) as Item"
                 aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
                 processed_data[df_name] = aux_df
         return processed_data
 
-    def transform(self, dataframe:DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", to_snake_case:bool = False, replace_dots:bool = False):
+
+    def transform(self, dataframe:DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df"):
         """Receive a pyspark.Dataframe and returns a Dictionary[str, pyspark.DataFrame]
         with all the processed dataframes.
         The ammount of dataframes on returned dictionary will depends on the number
         of ArrayType columns present on the input dataframe.
         If to_snake_case is set True, the column names on every processed Dataframe
         will be casted to snake_case.
         If replace_docts is set to True, all the dots present on a column name will
@@ -174,25 +160,28 @@
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str]
             A list of columns to ignore and not to add to the resulting flattened dictionary.
         dataframe_name: str
             A reference name for the dataframe, used to difference each
             resulting dataframe in the named_struct return.
-        to_snake_case: bool
-            If True rename the column to Snake Case column name like.
-        replace_dots: bool
-            If True replace the column name dots with underscores.
         Returns
         -------
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
         if len(dataframe.head(1)) == 0:
             raise FlatteningException("The provided dataframe is empty.")
-        processed_data = {}
-        processed_data = self._processor(dataframe, id_key, black_list, dataframe_name)
-        for processed_df_name, processed_df in processed_data.items():
-            processed_data[processed_df_name] = self._process_column_name(processed_df, to_snake_case, replace_dots)
-        return processed_data
+        elif id_key not in dataframe.columns:
+            raise FlatteningException(f"The provided id_key={id_key} does not exist in dataframe")
+        
+        self._parent_df_name = dataframe_name
+        self._parent_id_key = id_key
+        self._black_list = black_list
+        aux, self._processed_data = {}, {}
+        aux = self._processor(dataframe, id_key, dataframe_name)
+        for processed_df_name, processed_df in aux.items():
+            processed_aux = self._process_dataframe_columns(processed_df_name, processed_df)
+            self._processed_data[processed_aux[0]] = processed_aux[1]
+        return self._processed_data
```

### Comparing `dataflat-1.0.6/setup.py` & `dataflat-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,34 +24,35 @@
 PATH = path.abspath(path.dirname(__file__))
 
 with open(path.join(PATH, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
  
 setuptools.setup(
     name="dataflat",
-    version="1.0.6",
+    version="1.1.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JuanARojasA/dataflat',
     author="Juan Rojas",
     author_email="jarojasa97@gmail.com",
     license='Apache License 2.0',
     platforms='any',
     packages=setuptools.find_packages(),
     classifiers=[
-            'Development Status :: 4 - Beta',
+            'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'Intended Audience :: Information Technology',
             'Intended Audience :: Science/Research',
             'License :: OSI Approved :: Apache Software License',
             'Natural Language :: English',
             'Operating System :: OS Independent',
             'Programming Language :: Python :: 3',
             'Topic :: Scientific/Engineering',
             'Topic :: Software Development :: Libraries',
             'Topic :: Software Development :: Libraries :: Python Modules',
-            'Topic :: Software Development :: Pre-processors'
+            'Topic :: Software Development :: Pre-processors',
+            'Topic :: Utilities'
         ],
     python_requires='>=3.9',
     install_requires=["pandas","typeguard"],
     include_package_data=True
 )
```

