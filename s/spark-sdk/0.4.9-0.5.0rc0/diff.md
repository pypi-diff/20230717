# Comparing `tmp/spark_sdk-0.4.9-py3-none-any.whl.zip` & `tmp/spark_sdk-0.5.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 32225 bytes, number of entries: 14
--rw-rw-r--  2.0 unx     1202 b- defN 22-Oct-25 06:41 spark_sdk/__init__.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Jul-07 02:56 spark_sdk/_version.py
+Zip file size: 35572 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Jul-17 10:04 spark_sdk/__init__.py
+-rw-rw-r--  2.0 unx      772 b- defN 23-Jul-16 08:13 spark_sdk/conf.py
 -rw-rw-r--  2.0 unx     4469 b- defN 22-Aug-12 12:38 spark_sdk/create_yaml_file.py
+-rw-rw-r--  2.0 unx     6309 b- defN 23-Mar-24 03:02 spark_sdk/datahub_api.py
 -rw-rw-r--  2.0 unx     9905 b- defN 22-Jun-06 02:01 spark_sdk/hive_metastore.py
--rw-rw-r--  2.0 unx     2433 b- defN 22-Jun-23 03:02 spark_sdk/ingest_hive_datahub.py
--rw-rw-r--  2.0 unx     1766 b- defN 22-Jun-14 08:33 spark_sdk/pandas_decrypt.py
--rw-rw-r--  2.0 unx    44328 b- defN 22-Oct-18 04:07 spark_sdk/pandas_to_dwh.py
--rw-rw-r--  2.0 unx    45110 b- defN 22-Nov-01 06:38 spark_sdk/pyspark_add_on.py
--rw-rw-r--  2.0 unx     3758 b- defN 22-Oct-17 02:00 spark_sdk/utils.py
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-10 08:46 spark_sdk-0.4.9.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-rw-r--  2.0 unx     6066 b- defN 22-Nov-01 06:42 spark_sdk-0.4.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-01 06:42 spark_sdk-0.4.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 22-Nov-01 06:42 spark_sdk-0.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-01 06:42 spark_sdk-0.4.9.dist-info/RECORD
-14 files, 120401 bytes uncompressed, 30275 bytes compressed:  74.9%
+-rw-rw-r--  2.0 unx     3319 b- defN 23-Apr-26 04:20 spark_sdk/ingest_hive_datahub.py
+-rw-rw-r--  2.0 unx     2300 b- defN 23-Apr-24 07:08 spark_sdk/magics.py
+-rw-rw-r--  2.0 unx     1767 b- defN 23-Feb-13 06:42 spark_sdk/pandas_decrypt.py
+-rw-rw-r--  2.0 unx    34923 b- defN 23-Jul-17 08:41 spark_sdk/pylineage.py
+-rw-rw-r--  2.0 unx    51893 b- defN 23-Jul-17 10:05 spark_sdk/pyspark_add_on.py
+-rw-rw-r--  2.0 unx     4100 b- defN 23-Mar-12 15:53 spark_sdk/utils.py
+-rw-rw-r--  2.0 unx       92 b- defN 22-Oct-10 08:46 spark_sdk-0.5.0rc0.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-r--  2.0 unx     8526 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1335 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/RECORD
+16 files, 131193 bytes uncompressed, 33370 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,43 +1,49 @@
 Filename: spark_sdk/__init__.py
 Comment: 
 
-Filename: spark_sdk/_version.py
+Filename: spark_sdk/conf.py
 Comment: 
 
 Filename: spark_sdk/create_yaml_file.py
 Comment: 
 
+Filename: spark_sdk/datahub_api.py
+Comment: 
+
 Filename: spark_sdk/hive_metastore.py
 Comment: 
 
 Filename: spark_sdk/ingest_hive_datahub.py
 Comment: 
 
+Filename: spark_sdk/magics.py
+Comment: 
+
 Filename: spark_sdk/pandas_decrypt.py
 Comment: 
 
-Filename: spark_sdk/pandas_to_dwh.py
+Filename: spark_sdk/pylineage.py
 Comment: 
 
 Filename: spark_sdk/pyspark_add_on.py
 Comment: 
 
 Filename: spark_sdk/utils.py
 Comment: 
 
-Filename: spark_sdk-0.4.9.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
+Filename: spark_sdk-0.5.0rc0.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
 Comment: 
 
-Filename: spark_sdk-0.4.9.dist-info/METADATA
+Filename: spark_sdk-0.5.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: spark_sdk-0.4.9.dist-info/WHEEL
+Filename: spark_sdk-0.5.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: spark_sdk-0.4.9.dist-info/top_level.txt
+Filename: spark_sdk-0.5.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_sdk-0.4.9.dist-info/RECORD
+Filename: spark_sdk-0.5.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_sdk/__init__.py

```diff
@@ -1,40 +1,48 @@
 from .pyspark_add_on import PySpark, PyArrow, Utf8Encoder
 from .pyspark_add_on import to_dwh, drop_table, drop_table_and_delete_data, read_table, sql, refresh_table, spark_dataframe_to_dwh
 from .pyspark_add_on import ls, mkdir, cat, exists, info, open
 from .pyspark_add_on import read_dwh_pd, read_csv, read_json, write_json, read_parquet, read_dwh
 from .pyspark_add_on import show, refresh_table
 from .pyspark_add_on import limit_timestamp
-from .pyspark_add_on import info as spark_dataframe_info
+from .pyspark_add_on import spark_dataframe_info
 from .create_yaml_file import CreateYamlDWH
 from .pandas_decrypt import decrypt, decrypt_column
+from spark_sdk.pylineage import PandasConversionMixin
+
+from .magics import *
+try:
+    from IPython import get_ipython
+    load_ipython_extension(get_ipython())
+except:
+    pass
+
 
-# from .pyspark_add_on.PySpark import to_dwh
 from .utils import modulereload, choose_num_core
 from pandas.core.series import Series
 
 
 import pandas as pd
 from pandas import DataFrame
 
 
 DataFrame.to_dwh = to_dwh
+#DataFrame._repr_html_ = PandasDataFrame_repr_html_
 modulereload(pd)
 
 Series.decrypt_column = decrypt_column
 pd.read_dwh = read_dwh_pd
 modulereload(pd)
 
 
 from pyspark.sql import DataFrame as SparkDataFrame
 SparkDataFrame.to_dwh = spark_dataframe_to_dwh
 SparkDataFrame.info = spark_dataframe_info
+SparkDataFrame.toPandas = PandasConversionMixin.toPandasLineage
 
 
 SparkDataFrame.show = show
 
-
-
-__version__ = '0.4.9'
-__all__ = ["PySpark", "CreateYamlDWH", "decrypt", "decrypt_column", "PyArrow", "to_dwh", "sql"]
+__version__ = '0.5.0rc0'
+__all__ = ["PySpark", "PyArrow"]
```

## spark_sdk/ingest_hive_datahub.py

```diff
@@ -2,81 +2,111 @@
 import sys, argparse
 
 def getOptions(args=sys.argv[1:]):
     parser = argparse.ArgumentParser(description='Function run yaml file datahub')
     parser.add_argument("-d", "--database_name", help="database_name")
     parser.add_argument("--allow", nargs="+", help='list table pattern allow')
     parser.add_argument("--deny", nargs="+", help='list table pattern deny')
+    parser.add_argument("--file_password", help='Path file to file have user and password')
     parser.add_argument("--user", help='User name')
+    parser.add_argument("--profiling", help="Enable profiling")
     parser.add_argument("--password", help='PassWord')
 
     options = parser.parse_args(args)
     return options
 
-def create_yaml_file(username, password, database_name, table_pattern_allow = [], table_pattern_deny = []):
+def create_yaml_file(username, password, database_name, table_pattern_allow = [], table_pattern_deny = [], profiling=False):
     if table_pattern_allow:
-        table_pattern_allow_txt = '            allow'
+        table_pattern_allow_txt = '            allow:\n'
+
+        for i in table_pattern_allow:
+            table_pattern_allow_txt += "                - " + database_name + '.' + i +'$\n'
     else:
         table_pattern_allow_txt = ''
-    for i in table_pattern_allow:
-        table_pattern_allow_txt += "                - " + database_name + '.' + i +'\n'
         
     if table_pattern_deny:
-        table_pattern_deny_txt = '            deny'
+        table_pattern_deny_txt = '\n'
+    
+        for i in table_pattern_deny:
+            table_pattern_deny_txt += "                - " + database_name + '.' + i +'\n'
     else:
         table_pattern_deny_txt = ''
-    for i in table_pattern_deny:
-        table_pattern_deny_txt += "                - " + database_name + '.' + i +'\n'
-        
         
+    if profiling:
+        profiling = """
+        profiling:
+            enabled: true 
+        """
+    else:
+        profiling = ""
+
     yaml = f"""
 source:
     type: sqlalchemy
     config:
         platform: hive
-        connect_uri: "hive://{username}:{password}@master02-dc9c14u41.bigdata.local:10000/{database_name}"
+        connect_uri: "hive://{username}:{password}@172.24.178.40:10009/{database_name}"
         include_views: False
         table_pattern:
 {table_pattern_allow_txt}
             deny:
                 - "{database_name}.test.*"
-                - "{database_name}.backup_*"
-{table_pattern_allow_txt}
+                - "{database_name}.tmp.*"
+                - "{database_name}.bk.*"
+                - "{database_name}.backup.*"
+                - "{database_name}.view_.*"
+                
+                - ".*test.*"
+                - ".*backup.*"
+                - ".*tmp.*"
+{table_pattern_deny_txt}
         schema_pattern:
             allow:
                 - "{database_name}"
             deny:
                 - "information_schema"
         options:
             connect_args:
                 auth: 'LDAP'
+
+{profiling}
 sink:
     type: "datahub-rest"
     config:
-        server: "http://gms.datahub.bigdata.local"
+        server: "http://gms-dev-datahub.cads.live"
     
     """
     
     
     with open(f'datahub_ingest_{database_name}.yaml', 'w') as file:
         file.write(yaml)
     
     return f'datahub_ingest_{database_name}.yaml'
     
 def run_yaml_file(yaml_file_name):
     os.system(f'datahub ingest -c {yaml_file_name}')
 
-if __name__ = '__main__':
-
+if __name__ == '__main__':
     options = getOptions()
+    file_password = options.file_password
+    password = options.password
+    profiling = options.profiling
+
+    if file_password:
+        f = open(options.file_password, "r")
+        PASSWORD = f.read()
+        PASSWORD = PASSWORD.strip()
 
+    elif password:
+        PASSWORD = password
 
     yaml_file_name = create_yaml_file(
         username = options.user,
-        password = options.password,
+        password = PASSWORD,
         database_name = options.database_name,
-        table_pattern_deny=options.deny
-    )
+        table_pattern_allow=options.allow,
+        table_pattern_deny=options.deny,
+        profiling=profiling
+     )
 
 
     run_yaml_file(yaml_file_name)
-
```

## spark_sdk/pandas_decrypt.py

```diff
@@ -18,14 +18,15 @@
     """
     check = str(x)
     if check and check != "None":
         x_bytes = base64.b64decode(x)
         encryption = AES.new(base64.b64decode(key), AES.MODE_CBC, x_bytes[0:16])
         return unpad(encryption.decrypt(x_bytes[16:]),16).decode('utf-8')
 
+
 def decrypt_column(self, key):
     """
      Parameters
     ----------
 
     df: pandas.DataFrame
     col: str column want to decrypt
```

## spark_sdk/pyspark_add_on.py

```diff
@@ -1,21 +1,38 @@
 import os
-import sys
-from .utils import choose_num_core, choose_executor_memory, choose_driver_memory, _check_series_convert_timestamps_internal, _get_local_timezone, contains_duplicates, modulereload
-from .hive_metastore import HiveMetastoreClient
-
 # for yarn support
 os.environ['SPARK_HOME']="/opt/spark/spark-3.3.0-bin-hadoop2"
 os.environ['JAVA_HOME'] = "/usr/jdk64/jdk1.8.0_112/"
 os.environ['SPARK_CONF_DIR'] = "/opt/spark/spark-3.3.0-bin-hadoop2/conf"
-#os.environ['SPARK_CONF_DIR'] = "/opt/spark/spark-3.0.2-bin-hadoop2.7/conf"
 
+import sys
+from .utils import choose_num_core, choose_executor_memory, choose_driver_memory, _check_series_convert_timestamps_internal, _get_local_timezone, contains_duplicates, modulereload
+from .hive_metastore import HiveMetastoreClient
 
 import findspark
-findspark.init("/opt/spark/spark-3.3.0-bin-hadoop2")
+findspark.init(os.getenv("SPARK_HOME"))
+
+# exist_old_pyspark = False
+# for _idx, path in enumerate(sys.path):
+#     if path == '/opt/spark/spark-3.0.2-bin-hadoop2.7/python':
+#         sys.path[_idx] = '/opt/spark/spark-3.3.0-bin-hadoop2/python'
+#         exist_old_pyspark = True
+#     elif path == '/opt/spark/spark-3.0.2-bin-hadoop2.7/python/lib/py4j-0.10.9-src.zip':
+#         sys.path[_idx] = '/opt/spark/spark-3.3.0-bin-hadoop2/python/lib/py4j-0.10.9.5-src.zip'
+#         exist_old_pyspark = True
+
+
+# if exist_old_pyspark:
+#     import sys
+#     from copy import copy
+#     all_modules = copy(sys.modules)
+#     for m in all_modules:
+#         if 'pyspark.' in m or m=='pyspark':
+#             sys.modules.pop(m)
+#             import pyspark
 
 import json
 
 import pandas as pd
 import pyarrow.parquet as pq
 import pyarrow as pa
 import subprocess
@@ -60,15 +77,15 @@
 
 pd.options.display.max_columns = 50
 
 
 from typing import (Union)
 
 class PySpark:
-    def __init__(self, driver_memory='1G', num_executors='1', executor_memory='1G', port='', yarn=False, **spark_configs):
+    def __init__(self, driver_memory='1G', num_executors='1', executor_memory='4G', port='', yarn=False, **spark_configs):
         """
          Parameters
         ----------
 
         driver_memory: memory for spark driver and executor memory, must less than 8Gb. 8Gb is handle table 10 milion rows
         executor_memory: memeory for core spark, must less than 8G
         core: executor core, must less than 10 cores
@@ -96,46 +113,52 @@
         conf = SparkConf()
 
         # config spark application name
         import getpass
         conf.setAppName(f"spark_sdk_{getpass.getuser()}")
 
         # config location for spark finding metadata from hive metadata server
-        conf.set("hive.metastore.uris",
-                 "thrift://master01-dc9c14u40.bigdata.local:9083,thrift://master02-dc9c14u41.bigdata.local:9083")
+        conf.set("hive.metastore.uris", "thrift://master01-dc9c14u40.bigdata.local:9083,thrift://master02-dc9c14u41.bigdata.local:9083")
         conf.set("spark.sql.hive.metastore.jars", "/opt/spark/spark-3.0.2-bin-hadoop2.7/*")
 
-        # config directory to use for "scratch" space in Spark, including map output files and RDDs that get stored on disk
-        if os.path.exists('./tmp/'):
-            pass
-        else:
-            os.mkdir('./tmp/')
-        conf.set('spark.local.dir', './tmp/')
+
         # config in-memory columnar data format that is used in Spark to efficiently transfer data between JVM and Python processes
         conf.set("spark.kryoserializer.buffer.max", "2000")
         conf.set("spark.sql.execution.arrow.pyspark.enabled", "true")
         # conf.set("spark.sql.execution.arrow.enabled", "true") # remove in future
-        conf.set("spark.sql.execution.arrow.maxRecordsPerBatch", "10000")
+        conf.set("spark.sql.execution.arrow.maxRecordsPerBatch", "50000")
         
         if self.yarn == 'yarn':
             #queue
             conf.set("spark.yarn.queue", "batch")
             
             # config spark dynamicAllocation
             conf.set("spark.dynamicAllocation.enabled", "true")
             conf.set("spark.dynamicAllocation.shuffleTracking.enabled", "true")
             conf.set("spark.dynamicAllocation.minExecutors", 1)
             conf.set("spark.dynamicAllocation.maxExecutors", 8)
             conf.set("spark.dynamicAllocation.executorIdleTimeout", "300s")
             conf.set("spark.dynamicAllocation.shuffleTracking.enabled", "true")
             conf.set("spark.dynamicAllocation.shuffleTracking.timeout", "300s")
+        else:
+            # config directory to use for "scratch" space in Spark, including map output files and RDDs that get stored on disk
+            conf.set('spark.local.dir', '/tmp/')
+            
+            conf.set("spark.dynamicAllocation.enabled", "true")
+            conf.set("spark.dynamicAllocation.shuffleTracking.enabled", "true")
+            conf.set("spark.dynamicAllocation.minExecutors", 1)
+            conf.set("spark.dynamicAllocation.maxExecutors", 10)
+            conf.set("spark.dynamicAllocation.executorIdleTimeout", "300s")
+            conf.set("spark.dynamicAllocation.shuffleTracking.enabled", "true")
+            conf.set("spark.dynamicAllocation.shuffleTracking.timeout", "300s")
+
 
         # config partition Size
         # conf.set('spark.sql.adaptive.coalescePartitions.minPartitionSize', '128MB')
-        conf.set('spark.sql.files.minPartitionNum', 100000)
+        # conf.set('spark.sql.files.minPartitionNum', 100000)
 
         # config spark driver memory
         conf.set("spark.driver.memory", self.driver_memory)
         conf.set('spark.executor.memory', self.executor_memory)
         conf.set('spark.driver.maxResultSize', '10G')
 
         if int(self.num_executors) > 1:
@@ -144,82 +167,86 @@
         conf.set('spark.rpc.message.maxSize', '1000')
 
         # conf.set("spark.ui.enabled", "false")
         if not port:
             port = 0
             for j,i in enumerate(getpass.getuser()):
                 port+=ord(i) * 1 if j//2 == 1 else -1
-            port +=4000
+            port +=4300
         conf.set("spark.ui.port", port)
 
         # config for write append parquet
         conf.set("spark.sql.parquet.compression.codec", "snappy")
 
         # set metastore.client.capability.check to false
         conf.set("hive.metastore.client.capability.check", "false")
 
         # config for descrypt data
-        conf.set("spark.jars", "hdfs:///shared/jars/hotpot_2.12-0.0.3.jar")
+        conf.set("spark.jars", "hdfs:///shared/jars/hotpot_2.12-0.0.3.jar,hdfs:/shared/jars/datahub-spark-lineage-0.10.11-SNAPSHOT.jar")
+        # conf.set("spark.jars", "hdfs:///shared/jars/hotpot_2.12-0.0.3.jar")
         conf.set("spark.sql.redaction.string.regex", ".{22}==")
         
         # delta format
         conf.set("spark.sql.catalog.spark_catalog","org.apache.spark.sql.delta.catalog.DeltaCatalog")
         conf.set("spark.sql.extensions","io.delta.sql.DeltaSparkSessionExtension")
+        conf.set("spark.sql.catalogImplementation","hive")
         conf.set('spark.sql.hive.metastorePartitionPruningFallbackOnException', True)
         conf.set('spark.sql.hive.metastorePartitionPruningFastFallback', True)
         conf.set("spark.databricks.delta.optimize.maxFileSize", 268435456) # 256MB
         conf.set('spark.databricks.delta.retentionDurationCheck.enabled', False)
         # conf.set('spark.jars.packages', "io.delta:delta-core_2.12:2.1.0")
         # conf.set("spark.driver.extraJavaOptions", "-Dhttps.proxyHost=proxy.hcm.fpt.vn -Dhttps.proxyPort=80 -Dhttp.proxyHost=proxy.hcm.fpt.vn -Dhttp.proxyPort=80")
         # conf.set("spark.executor.extraJavaOptions", "-Dhttps.proxyHost=proxy.hcm.fpt.vn -Dhttps.proxyPort=80 -Dhttp.proxyHost=proxy.hcm.fpt.vn -Dhttp.proxyPort=80")
         
         # fix legacy parquet timestamp error
         conf.set("spark.sql.parquet.int96RebaseModeInRead", "CORRECTED")
         conf.set("spark.sql.parquet.int96RebaseModeInWrite", "CORRECTED")
         conf.set("spark.sql.parquet.datetimeRebaseModeInRead", "CORRECTED")
         conf.set("spark.sql.parquet.datetimeRebaseModeInWrite", "CORRECTED")
+        
+        # lineage
+        from spark_sdk.conf import GMS_URL_KEY, GMS_AUTH_TOKEN
+        conf.set("spark.extraListeners","datahub.spark.DatahubSparkListener")
+        conf.set("spark.datahub.rest.server", GMS_URL_KEY)
+        conf.set("spark.datahub.rest.token", GMS_AUTH_TOKEN)
+        
 
-
+        all_config = {c[0]:c[1] for c in conf.getAll()}
         for k_c in spark_configs.keys():
             if len(spark_configs[k_c]) == 2:
-                
-                conf.set(spark_configs[k_c][0], spark_configs[k_c][1])
+                if spark_configs[k_c][0] in ['spark.repl.local.jars', 'spark.sql.hive.metastore.jars', 'spark.jars']:
+                    conf.set(spark_configs[k_c][0], all_config[spark_configs[k_c][0]]+','+spark_configs[k_c][1])
+                else:
+                    conf.set(spark_configs[k_c][0], spark_configs[k_c][1])
             else:
                 raise TypeError(f"PySpark got an unexpected keyword argument {k_c}")
         
         self.spark = SparkSession.builder.config(conf=conf).master(self.yarn).enableHiveSupport().getOrCreate()
-        
-        # TRY to turn off old spark
-        # print("Spark UI URL %s" % self.spark.sparkContext.uiWebUrl)
-#         if str(self.spark.version)!='3.3.0':
-#             print(os.environ['SPARK_HOME'])
-#             modulereload(pyspark)
-#             self.spark.stop()
-            
-#             self.spark = SparkSession.builder.config(conf=conf).master(self.yarn).enableHiveSupport().getOrCreate()
             
         # config timezone
         self.spark.conf.set('spark.sql.session.timeZone', '+07:00')
 
         # config show pandas dataframe format on notebook
         self.spark.conf.set("spark.sql.repl.eagerEval.enabled", True)
         self.spark.conf.set("spark.sql.repl.eagerEval.truncate", 200)
 
         self.spark.conf.get("hive.metastore.uris")
 
         # defing decrypt function
         try:
             self.spark._jvm.vn.fpt.insights.utils.Helper.registerUdf("fdecrypt", "fdecrypt")
             self.spark._jvm.vn.fpt.insights.utils.Helper.registerUdf("fencrypt", "fencrypt")
+            self.spark._jvm.vn.fpt.insights.utils.Helper.registerUdf("fmask", "fmask")
         except:
             pass
         
         # dont print WARN
         self.spark.sparkContext.setLogLevel("ERROR")
         
+        
     
 
     def get_fs(self):
         # get hadoop file system
         return self.spark._jvm.org.apache.hadoop.fs.FileSystem.get(self.spark._jsc.hadoopConfiguration())
 
     def check_is_file(self, hdfs_path):
@@ -260,24 +287,64 @@
         import re
         if re.search('json$', keys_path):
             return True
         else:
             raise Exception("keys_path must end with '.json'")
 
     def autogenerate_key(self, length_key=22):
+        """
+        Input length of string key
+        return random string (contains string upper case and string lower case) and digits 
+        """
         import string
         import random
 
         key = ''.join(
             random.choice(string.ascii_uppercase + string.digits + string.ascii_lowercase) for _ in range(length_key))
         key = key + "=="
         return key
 
+    def auto_generate_list_keys(self, table_name, column_name='', keys_path='keys.json'):
+        """
+        Input
+        table_name: Name of table that need encrypt
+        column_name: list string seperate by ',', ex: a,b,c
+        keys_path: path file of key if want to append key to file
+        
+        return list of keys ready to be copy
+        """
+        from datetime import datetime
+        import json
 
+        if self.check_is_file(keys_path):
+            list_keys = self.read_json(keys_path)
+        else:
+            list_keys = []
+
+        for c in column_name.split(','):
+            if c:
+                keys = {}
+
+                keys["name"] = f"secret_for_{table_name}_{c}"
+                keys["description"] = f"This is secret_for_{table_name}_{c}"
+                keys["created"] = round(datetime.timestamp(datetime.now()))
+                keys["material"] = self.autogenerate_key()
+
+                list_keys.append(keys)
+        return list_keys
+    
     def encrypt_column(self, sparkDF, table_name, column_names=[], keys_path=''):
+        """
+        Input
+        : sparkDF: spark.sql.DataFrame
+        : table_name: name of table example: table1
+        : column_names: list column name need encrypt
+        : keys_path: json path example: /path/to/keys.json
+        return: spark.sql.DataFrame have encrypted column
+        """
         # check file keys exist
         if self.check_is_file(keys_path):
             # Opening JSON file
             list_keys = PyArrow().read_json(keys_path)
         else:
             list_keys = []
 
@@ -323,39 +390,56 @@
         """
 
         sparkDF.createOrReplaceTempView(f"{table_name}")
         print('Start encrypt column')
 
         return self.spark.sql(sql)
 
-    def read_first_file(self, database, table_name):
+    def read_first_file(self, database, table_name, hdfs_path):
         '''
         Read schema hive
         '''
-        return self.spark.sql(f"""SELECT * FROM {database}.{table_name} LIMIT 5""")
+        try:
+            df = self.spark.sql(f"""SELECT * FROM {database}.{table_name} LIMIT 5""")
+        except:
+            if 'parquet' in hdfs_path:
+                df = self.spark.sql(f"""SELECT * FROM parquet.`{hdfs_path}` LIMIT 5""")
+            else:
+                raise AnalysisException(f"Table or view not found {database}.{table_name}")
+        return df
 
     def compare_data_type(self, first_sparkDF, second_sparkDF):
         """
         Function to check when write data second time
-        """
+        """                             
+        def get_data_type(datatype):
+            mapping = {'LongType()': 'IntegerType()', 'IntegerType()': 'LongType()'}
+            if datatype in mapping.keys():
+                return mapping[datatype]
+            else:
+                return datatype
+            
         error = {}
         if len(first_sparkDF.schema) == len(second_sparkDF.schema):
             for c in second_sparkDF.schema:
                 c_name = c.name
                 second_type = second_sparkDF.schema[c_name].dataType
+                second_type = str(second_type)
                 first_type = first_sparkDF.schema[c_name].dataType
+                first_type = str(first_type)
 
                 if first_type != second_type:
-                    error[c_name] = {'first_time': first_type, 'second_time': second_type}
+                    if first_type != get_data_type(second_type):
+                        error[c_name] = {'first_time': first_type, 'second_time': second_type}
                              
                 if error.keys():
                     print('Error', error)
                     first_sparkDF.unpersist()
                     second_sparkDF.unpersist()
-                    raise TypeError(f"DataType of Columns this time store is not like first time")
+                    raise TypeError(f"DataType of Columns this time store is not like first time {error}")
         else:
             print(f'First time have columns', first_sparkDF.schema.names)
             print(f'Second time have columns', second_sparkDF.schema.names)
             
             raise ValueError(f"First time have {len(first_sparkDF.schema)} columns but second time have {len(second_sparkDF.schema)} columns")
         
                              
@@ -390,14 +474,23 @@
                 return valid[default]
             elif choice in valid:
                 return valid[choice]
             else:
                 sys.stdout.write("Please respond with 'yes' or 'no' " "(or 'y' or 'n').\n")
 
     def create_table_and_metadata(self, database, table_name, hdfs_path, partition_by=''):
+        """
+        Create table in catalog and MSCK (update metadata) if partitioned table
+        Input:
+        :param database: database name, example: default
+        :param table_name: table name, example: test1
+        :param hdfs_path: path to data, example /path/to/data.parquet
+        Return:
+        nothing
+        """
         if database and table_name:
             try:
                 self.spark.catalog.createTable(database + '.' + table_name, "hdfs://" + hdfs_path)
             except:
                 # AnalysisException table aready exists
                 print('Cannot create table, this table already exists ==> repair data')
 
@@ -410,15 +503,16 @@
         if partition_by:
             print('MSCK REPAIR DATA FOR PARTITION TABLE')
             self.spark.sql(f'msck REPAIR TABLE {database}.{table_name}')
             
         self.spark.sql(f"""REFRESH TABLE {database}.{table_name}""")
 
     def store_spark_dataframe_to_dwh(self, data, hdfs_path, repartition=False, numPartitions=None, partition_by='',
-                                     partition_date='', database='', table_name='', encrypt_columns=[], keys_path=''):
+                                     partition_date='', compression = 'snappy', 
+                                     database='', table_name='', encrypt_columns=[], keys_path=''):
         """
          Parameters
         ----------
         data: pyspark.sql.dataframe.DataFrame
         hdfs_path : Path hdfs user want to store. EX: /data/fpt/ftel/cads/opt_customer/dm/
         partition_by: columns user want to partition, if None do not partition
         database : If user want to store to database must have database
@@ -472,56 +566,62 @@
 
             print('HDFS path: ', hdfs_path)
             
 
                 
             # if table exist compare datatype before store
             if self.check_is_file(hdfs_path):
-                self.compare_data_type(self.read_first_file(database, table_name), sparkDF)
+                self.compare_data_type(self.read_first_file(database, table_name, hdfs_path), sparkDF)
 
             self.spark.sql("SET spark.sql.sources.partitionOverwriteMode = dynamic")
 
             if repartition and numPartitions:
-                sparkDF.repartition(numPartitions).write.format(file_format).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(database + '.' + table_name)
+                sparkDF.repartition(numPartitions).write.format(file_format).option('compression', compression).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(database + '.' + table_name)
             elif repartition:
                 numPartitions = self.num_repartition(sparkDF)
-                sparkDF.repartition(numPartitions).write.format(file_format).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(database + '.' + table_name)
+                sparkDF.repartition(numPartitions).write.format(file_format).option('compression', compression).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(database + '.' + table_name)
             else:
-                sparkDF.write.format(file_format).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(
+                sparkDF.write.format(file_format).option('compression', compression).mode("overwrite").partitionBy(partition_by).option("path", hdfs_path).saveAsTable(
                     database + '.' + table_name)
 
         else:
             if repartition and numPartitions:
                 sparkDF.repartition(numPartitions).write.format(file_format).mode("overwrite").option("path", hdfs_path).saveAsTable(database + '.' + table_name)
             elif repartition:
                 numPartitions = self.num_repartition(sparkDF)
                 sparkDF.repartition(numPartitions).write.format(file_format).mode("overwrite").option("path", hdfs_path).saveAsTable(database + '.' + table_name)
             else:
                 sparkDF.write.format(file_format).mode("overwrite").option("path", hdfs_path).saveAsTable(database + '.' + table_name)
         
         self.spark.sql(f"""REFRESH TABLE {database}.{table_name}""")
         
+        from spark_sdk.pylineage import addLineageAfterToDwh
+        try:
+            addLineageAfterToDwh(database+'.'+table_name)
+        except Exception as e: 
+            print(e)
+        
 
-    def to_dwh_spark(self, data, hdfs_path, repartition=False, numPartitions=None, partition_by='', partition_date='',
+    def to_dwh_spark(self, data, hdfs_path, repartition=False, numPartitions=None, partition_by='', partition_date='',compression='snappy',
                      database='', table_name='', encrypt_columns=[], keys_path=''):
         """
         Parameters
         ----------
         data: pandas dataframe
         hdfs_path : Path hdfs user want to store. EX: /data/fpt/ftel/cads/opt_customer/dm/
         partition_by: columns user want to partition, if None do not partition
         database : If user want to store to database must have database
         table_name: If user want to map data hdfs to table must have table_name
         """
-        # =====================================================
         sparkDF = self.spark.createDataFrame(data)
         self.store_spark_dataframe_to_dwh(sparkDF, hdfs_path=hdfs_path, repartition=repartition,
                                           numPartitions=numPartitions, partition_by=partition_by,
                                           partition_date=partition_date, database=database, table_name=table_name,
-                                          encrypt_columns=encrypt_columns, keys_path=keys_path)
+                                          encrypt_columns=encrypt_columns, keys_path=keys_path, compression=compression)
+        
 
         
     def read_csv(self, path, sep=',', header=True):
         return self.spark.read.option("header",header).options(delimiter=sep).csv(path)
         
     def read_parquet(self, path):
         return self.spark.read.parquet(path)
@@ -549,17 +649,18 @@
         return True
 
 
 class PyArrow:
     def __init__(self, existing_data_behavior='overwrite_or_ignore'):
         # Install latest Pyarrow version
         import os
+        from spark_sdk.conf import (HADOOP_HOST, HADOOP_PORT)
 
 
-        self.hdfs = fs.HadoopFileSystem(host="hdfs://hdfs-cluster.datalake.bigdata.local", port=8020)
+        self.hdfs = fs.HadoopFileSystem(host=HADOOP_HOST, port=HADOOP_PORT)
         
         self.existing_data_behavior = existing_data_behavior
         
     def check_keys_path_format(self, keys_path):
         import re
         if re.search('json$', keys_path):
             return True
@@ -600,15 +701,36 @@
         keys["description"] = ""
         keys["created"] = round(datetime.timestamp(datetime.now()))
         keys["material"] = self.autogenerate_key()
         list_keys.append(keys)
 
         with self.hdfs.open_output_stream(keys_path) as file:
             json.dump(list_keys, Utf8Encoder(file))
-        
+
+    def auto_generate_list_keys(self, table_name, column_name='', keys_path='keys.json'):
+        from datetime import datetime
+        import json
+
+        if self.check_is_file(keys_path):
+            list_keys = self.read_json(keys_path)
+        else:
+            list_keys = []
+
+        for c in column_name.split(','):
+            if c:
+                keys = {}
+
+                keys["name"] = f"secret_for_{table_name}_{c}"
+                keys["description"] = f"This is secret_for_{table_name}_{c}"
+                keys["created"] = round(datetime.timestamp(datetime.now()))
+                keys["material"] = self.autogenerate_key()
+
+                list_keys.append(keys)
+        return list_keys
+            
     def encrypt_column(self, data, table_name, column_names=[], keys_path=''):
         # check file keys exist
         if self.check_is_file(keys_path):
             # Opening JSON file
             list_keys = self.read_json(keys_path)
         else:
             list_keys = []
@@ -804,89 +926,37 @@
             database=database, table_name=table_name, partition_by=partition_by, hdfs_path=hdfs_path)
         
         PySpark(driver_memory='1g', num_executors='1', executor_memory='1G').spark.sql(f"""REFRESH TABLE {database}.{table_name}""")
         
 
         
 
-
-        
         
 ######################
-def to_dwh(self, hdfs_path, database, table_name, repartition=False, numPartitions=None, partition_by='',
-           partition_date='', encrypt_columns=[], keys_path='',
-           driver_memory='8G', executor_memory='4g', num_executors='1', parallel=True, port='', yarn=False,
-           engine='pyarrow',
-           use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
-    
-    if repartition:
-        engine='spark'
-    
-    df_memory = self.memory_usage(index=True).sum() / 1024 / 1024
-
-
-    if engine == 'spark' or 'delta' in hdfs_path.lower():
-        if parallel:
-            num_executors = choose_num_core(df_memory)
-
-        driver_memory = choose_driver_memory(df_memory)
-        executor_memory = choose_executor_memory(df_memory, int(num_executors))
-
-        PySpark(driver_memory=driver_memory, executor_memory=executor_memory, num_executors=num_executors, port=port,
-                yarn=yarn).to_dwh_spark(data=self, hdfs_path=hdfs_path, repartition=repartition,
-                                        numPartitions=numPartitions, partition_by=partition_by,
-                                        partition_date=partition_date, database=database, table_name=table_name,
-                                        encrypt_columns=encrypt_columns, keys_path=keys_path)
-    else:
-        PyArrow().to_dwh_pyarrow(data=self, hdfs_path=hdfs_path, database=database, table_name=table_name,
-                                 partition_by=partition_by, partition_date=partition_date,
-                                 use_deprecated_int96_timestamps=True, existing_data_behavior=existing_data_behavior, encrypt_columns=encrypt_columns, keys_path=keys_path)
-
-
 def read_table(full_table_name, engine='spark',
               driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False):
     PS = PySpark(driver_memory=driver_memory, executor_memory=executor_memory, num_executors=num_executors, port=port, yarn=yarn)
     return PS.spark.sql(f"select * from {full_table_name}")
 
 
-def drop_table(full_table_name, engine='spark', yarn=False):
-    PS = PySpark(driver_memory='1G', num_executors='1', executor_memory='1G', yarn=yarn)
-    PS.spark.sql(f"""ALTER TABLE {full_table_name} SET TBLPROPERTIES('external.table.purge' = 'false')""")
-    PS.spark.sql(f"DROP TABLE {full_table_name}")
-
-
-def drop_table_and_delete_data(full_table_name, yarn=False):
-    PS = PySpark(driver_memory='1G', num_executors='1', executor_memory='1G', yarn=yarn)
-    provider = get_provider_from_table(full_table_name)
-    if provider == 'delta':
-        import pandas as pd
-
-        df = PS.spark.sql(f"DESCRIBE FORMATTED {full_table_name}").toPandas()
-        location = df[df['col_name']=='Location']['data_type'].values[0]
-        
-        print(f"DELETE DATA {location}")
-        os.system(f"hdfs dfs -rm -r {location}")
-#         PS.spark.sql(f"""DELETE FROM {full_table_name} WHERE 1=1""")
-#         PS.spark.sql(f"""VACUUM {full_table_name} RETAIN 0 HOURS""")
-        PS.spark.sql(f"DROP TABLE {full_table_name}")
-    else:
-        PS.spark.sql(f"""ALTER TABLE {full_table_name} SET TBLPROPERTIES('external.table.purge' = 'true')""")
-        PS.spark.sql(f"DROP TABLE {full_table_name}")
-
 
 def sql(query, driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False):
     PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
     return PS.spark.sql(query)
 
 def refresh_table(full_table_name, driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False):
     PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
     return PS.spark.sql(f"""REFRESH TABLE {full_table_name}""")
 
 
 def read_dwh_pd(full_table_name, filters='', engine='spark', driver_memory='8G', num_executors='4', executor_memory='4G', port='', yarn=False):
+    # ========================LINEAGE======================
+    from spark_sdk.pylineage import emitPythonJob
+    emitPythonJob(full_table_name = full_table_name, outputNode=False)
+    # =====================================================
     if engine == 'pyarrow':
         df_arrow = PyArrow().read_table(source=get_location_from_table(full_table_name), filters=render_filters_pyarrow(filters))
         df = df_arrow.to_pandas()
             
     if engine == 'spark':
         PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
         if filters:
@@ -901,140 +971,166 @@
     PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
     if filters:
         filters = 'where ' + filters
     df_spark = PS.spark.sql(f"select * from {full_table_name} {filters}")
     return df_spark
 
 
-def get_location_from_table(full_table_name):
-    HIVE = HiveMetastoreClient(hmss_ro_addrs=["master01-dc9c14u40.bigdata.local:9083","master02-dc9c14u41.bigdata.local:9083"])
-    d, t = full_table_name.split('.')
-
-    location = HIVE.get_table(db_name=d, tb_name=t).__dict__['sd'].__dict__['location']
-    import re
-
-    pattern = re.compile('/data/')
-    x = pattern.search(location)
-
-    location = location[x.start():]
-    return location
-
-def get_provider_from_table(full_table_name):
-    HIVE = HiveMetastoreClient(hmss_ro_addrs=["master01-dc9c14u40.bigdata.local:9083","master02-dc9c14u41.bigdata.local:9083"])
-    d, t = full_table_name.split('.')
-
-    return HIVE.get_table(db_name=d, tb_name=t).parameters['spark.sql.sources.provider']
-
-
-def render_filters_pyarrow(sql):
-    if sql:
-        import sqlglot
-        sql = sqlglot.transpile(sql, write='spark', identify=True, pretty=True)[0]
-        list_bool_expression = sql.split('\n')
-
-
-        import re
-
-        pattern_column = re.compile('`(.*?)`')
-        pattern_operator = re.compile('[<>=]')
-
-
-        list_filters = []
-        for b in list_bool_expression:
-            x1 = pattern_column.search(b)
-            column_name = b[x1.start()+1: x1.end()-1]
-
-            x2 = pattern_operator.search(b)
-            operator = b[x2.start(): x2.end()]
-
-            value = b[x2.end()+2: -1]
-
-            list_filters.append((column_name, operator, value))
-
-        return list_filters
-    else:
-        return ''
-
-
-def spark_dataframe_to_dwh(self, hdfs_path, database, table_name, repartition=False, numPartitions=None, partition_by='',
-           partition_date='', encrypt_columns=[], keys_path='',
-           driver_memory='8G', executor_memory='5g', num_executors='1', parallel=True, port='', yarn=False
-           ):
-
-    PySpark(driver_memory=driver_memory, executor_memory=executor_memory, num_executors=num_executors, port=port,
-            yarn=yarn).store_spark_dataframe_to_dwh(data=self, hdfs_path=hdfs_path, database=database, table_name=table_name, repartition=repartition, numPartitions=numPartitions, partition_by=partition_by, partition_date=partition_date, encrypt_columns=encrypt_columns, keys_path=keys_path)
-    
-    
     
 def read_csv(path, sep=',', header=True,
            driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False,
            engine='spark',
            use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
     PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
     return PS.read_csv(path=path, sep=sep, header=header)
 
 
 def read_parquet(path,
            driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False,
            engine='spark',
            use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
+
     PS = PySpark(driver_memory=driver_memory, num_executors=num_executors, executor_memory=executor_memory, port=port, yarn=yarn)
     return PS.read_parquet(path=path)
 
 
 def read_json(path,
            driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False,
            engine='pyarrow',
            use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
     return PyArrow().read_json(path)
 
+
 def write_json(data, path,
            driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False,
            engine='pyarrow',
            use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
+    # ========================LINEAGE======================
+    from spark_sdk.pylineage import emitPythonJob
+    emitPythonJob(hdfs_path = path, outputNode=True)
+    # =====================================================
     return PyArrow().write_json(data = data, path = path)
 
 
+def spark_dataframe_to_dwh(self, hdfs_path, database, table_name, repartition=False, numPartitions=None, partition_by='',
+           partition_date='', compression='snappy', encrypt_columns=[], keys_path='',
+           driver_memory='8G', executor_memory='5g', num_executors='1', parallel=True, port='', yarn=False
+           ):
+
+    PySpark(driver_memory=driver_memory, executor_memory=executor_memory, num_executors=num_executors, port=port,
+            yarn=yarn).store_spark_dataframe_to_dwh(data=self, hdfs_path=hdfs_path, database=database, table_name=table_name, 
+                                                    repartition=repartition, numPartitions=numPartitions, partition_by=partition_by, partition_date=partition_date, compression=compression,
+                                                    encrypt_columns=encrypt_columns, keys_path=keys_path)
+    
+    
+def to_dwh(self, hdfs_path, database, table_name, repartition=False, numPartitions=None, compression = 'snappy', partition_by='',
+           partition_date='', encrypt_columns=[], keys_path='',
+           driver_memory='8G', executor_memory='4g', num_executors='1', parallel=True, port='', yarn=False,
+           engine='spark',
+           use_deprecated_int96_timestamps=True, existing_data_behavior='overwrite_or_ignore'):
+    # ========================LINEAGE======================
+    from spark_sdk.pylineage import emitPythonJob
+    emitPythonJob(full_table_name = database + "." + table_name, outputNode=True)
+    # =====================================================
+    
+    if repartition:
+        engine='spark'
+    
+    df_memory = self.memory_usage(index=True).sum() / 1024 / 1024
+
+
+    if engine == 'spark' or 'delta' in hdfs_path.lower():
+        if parallel:
+            num_executors = choose_num_core(df_memory)
+
+        driver_memory = choose_driver_memory(df_memory)
+        executor_memory = choose_executor_memory(df_memory, int(num_executors))
+
+        PySpark(driver_memory=driver_memory, executor_memory=executor_memory, num_executors=num_executors, port=port,
+                yarn=yarn).to_dwh_spark(data=self, hdfs_path=hdfs_path, repartition=repartition,
+                                        numPartitions=numPartitions, partition_by=partition_by,
+                                        partition_date=partition_date, compression=compression, database=database, table_name=table_name,
+                                        encrypt_columns=encrypt_columns, keys_path=keys_path)
+    else:
+        PyArrow().to_dwh_pyarrow(data=self, hdfs_path=hdfs_path, database=database, table_name=table_name,
+                                 partition_by=partition_by, partition_date=partition_date,
+                                 use_deprecated_int96_timestamps=True, existing_data_behavior=existing_data_behavior, encrypt_columns=encrypt_columns, keys_path=keys_path)
+
+def drop_table(full_table_name, engine='spark', yarn=False):
+    PS = PySpark(driver_memory='1G', num_executors='1', executor_memory='1G', yarn=yarn)
+    if PS.query_yes_no("Are you sure you want to drop table?", default='no'):
+        provider = get_provider_from_table(full_table_name)
+        if provider != 'delta':
+            PS.spark.sql(f"""ALTER TABLE {full_table_name} SET TBLPROPERTIES('external.table.purge' = 'false')""")
+        PS.spark.sql(f"DROP TABLE {full_table_name}")
+
+
+def drop_table_and_delete_data(full_table_name, yarn=False):
+    PS = PySpark(driver_memory='1G', num_executors='1', executor_memory='1G', yarn=yarn)
+    if PS.query_yes_no("Are you sure you want to drop table and delete data?", default='no'):
+        provider = get_provider_from_table(full_table_name)
+        if provider == 'delta':
+            import pandas as pd
+
+            df = PS.spark.sql(f"DESCRIBE FORMATTED {full_table_name}").toPandas()
+            location = df[df['col_name']=='Location']['data_type'].values[0]
+
+            print(f"MOVE DATA {location} to /shared/trash")
+            base_name = os.path.basename(location)
+            if exists(f"/shared/trash/{base_name}"):
+                os.system(f"hdfs dfs -rm -r /shared/trash/{base_name}")
+            os.system(f"hdfs dfs -mv {location} /shared/trash")
+            PS.spark.sql(f"DROP TABLE {full_table_name}")
+        else:
+            import pandas as pd
+
+            df = PS.spark.sql(f"DESCRIBE FORMATTED {full_table_name}").toPandas()
+            location = df[df['col_name']=='Location']['data_type'].values[0]
+
+            print(f"MOVE DATE {location} to /shared/trash")
+            base_name = os.path.basename(location)
+            if exists(f"/shared/trash/{base_name}"):
+                os.system(f"hdfs dfs -rm -r /shared/trash/{base_name}")
+            os.system(f"hdfs dfs -mv {location} /shared/trash")
+            PS.spark.sql(f"""ALTER TABLE {full_table_name} SET TBLPROPERTIES('external.table.purge' = 'false')""")
+            PS.spark.sql(f"DROP TABLE {full_table_name}")
+
+        
 ###############
 def ls(path, detail=False):
-    return pa.HadoopFileSystem().ls(path, detail=detail)
+    if "file:" in path:
+        import os
+        return os.listdir(path.replace('file:', ''))
+    else:
+        return pa.HadoopFileSystem().ls(path, detail=detail)
 
 
 def mkdir(path):
     return pa.HadoopFileSystem().mkdir(path)
 
 
 def cat(path):
     return pa.HadoopFileSystem().cat(path)
 
 
 def exists(path):
-    return pa.HadoopFileSystem().exists(path)    
+    if "file:" in path:
+        import os
+        return os.path.exists(path.replace('file:', ''))
+    else:
+        return pa.HadoopFileSystem().exists(path)    
 
 
 def info(path):
     return pa.HadoopFileSystem().info(path) 
 
 
 def open(path, mode='rb'):
     return pa.HadoopFileSystem().open(path, mode=mode)
-#     if mode == 'rb':
-#         return pa.HadoopFileSystem().open(path, mode=mode)
-#     else:
-#         print('Write wb')
-#         def write(self, data):
-#             print("DEBUG using Utf8Encoder")
-#             if not isinstance(data, bytes):
-#                 print("DEBUG using not isinstance")
-#                 data = data.encode('utf-8')
-#             self.fp.write(data)
-        
-#         from pyarrow.hdfs.HadoopFileSystem import open as o
-#         o.write = write
-#         return pa.HadoopFileSystem().open(path, mode=mode)
+
 
 def show(self, n: int = 20, truncate: Union[bool, int] = 50, vertical: bool = False) -> None:
     """Prints the first ``n`` rows to the console.
     .. versionadded:: 1.3.0
     Parameters
     ----------
     n : int, optional
@@ -1087,16 +1183,16 @@
         except ValueError:
             raise TypeError(
                 "Parameter 'truncate={}' should be either bool or int.".format(truncate)
             )
 
         print(self._jdf.showString(n, int_truncate, vertical))
         
-### new function
-def info(self, driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False):
+### dataframe function
+def spark_dataframe_info(self, driver_memory='8G', num_executors='4', executor_memory='4G', parallel=True, port='', yarn=False):
     sdf = self
     sdf.createOrReplaceTempView('info_table')
     sql = ''
     
     column_names = sdf.schema.names
     
     if len(column_names) > 1:
@@ -1126,8 +1222,63 @@
     for c in sparkDF.schema:
         if str(c.dataType) in ['TimestampType()', 'DateType()']:
             sql += f"AND {c.name} between '1900-01-01' AND '2300-01-01' \n"
     PS = PySpark()
     print("Filter")
     print(sql)
     sparkDF.createOrReplaceTempView('df')
-    return PS.spark.sql(f"""SELECT * FROM df WHERE 1=1 {sql}""")
+    return PS.spark.sql(f"""SELECT * FROM df WHERE 1=1 {sql}""")
+
+
+############ other table functions 
+def get_location_from_table(full_table_name):
+    from spark_sdk import HIVE_IP_NODE1,HIVE_IP_NODE2 
+    HIVE = HiveMetastoreClient(hmss_ro_addrs=[HIVE_IP_NODE1,HIVE_IP_NODE2])
+    d, t = full_table_name.split('.')
+
+    location = HIVE.get_table(db_name=d, tb_name=t).__dict__['sd'].__dict__['location']
+    import re
+
+    pattern = re.compile('/data/')
+    x = pattern.search(location)
+
+    location = location[x.start():]
+    return location
+
+def get_provider_from_table(full_table_name):
+    HIVE = HiveMetastoreClient(hmss_ro_addrs=["master01-dc9c14u40.bigdata.local:9083","master02-dc9c14u41.bigdata.local:9083"])
+    d, t = full_table_name.split('.')
+
+    return HIVE.get_table(db_name=d, tb_name=t).parameters['spark.sql.sources.provider']
+
+
+def render_filters_pyarrow(sql):
+    """
+    function support read_dwh() by pyarrow engine, render sql where clause
+    """
+    if sql:
+        import sqlglot
+        sql = sqlglot.transpile(sql, write='spark', identify=True, pretty=True)[0]
+        list_bool_expression = sql.split('\n')
+
+
+        import re
+
+        pattern_column = re.compile('`(.*?)`')
+        pattern_operator = re.compile('[<>=]')
+
+
+        list_filters = []
+        for b in list_bool_expression:
+            x1 = pattern_column.search(b)
+            column_name = b[x1.start()+1: x1.end()-1]
+
+            x2 = pattern_operator.search(b)
+            operator = b[x2.start(): x2.end()]
+
+            value = b[x2.end()+2: -1]
+
+            list_filters.append((column_name, operator, value))
+
+        return list_filters
+    else:
+        return ''
```

## spark_sdk/utils.py

```diff
@@ -106,7 +106,19 @@
     """
     import os
     return os.environ.get('TZ', 'dateutil/:')
 
 def contains_duplicates(X):
     import numpy as np
     return len(np.unique(X)) != len(X)
+
+
+def import_or_install(package):
+    try:
+        __import__(package)
+    except ImportError:
+        import os
+        import pip
+        os.environ['http_proxy'] = "http://proxy.hcm.fpt.vn:80" 
+        os.environ['https_proxy'] = "http://proxy.hcm.fpt.vn:80"
+        pip.main(['install', package])
+        modulereload(__import__(package))
```

## Comparing `spark_sdk-0.4.9.dist-info/METADATA` & `spark_sdk-0.5.0rc0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,103 @@
 Metadata-Version: 2.1
 Name: spark-sdk
-Version: 0.4.9
+Version: 0.5.0rc0
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark (>=3.0.2)
-Requires-Dist: pyarrow (>=8.0.0)
+Requires-Dist: pyarrow (>=4.0.0)
 Requires-Dist: pycryptodome
-Requires-Dist: pandas (>=1.3.4)
 Requires-Dist: thrift
 Requires-Dist: hmsclient
 Requires-Dist: sqlglot
 Requires-Dist: findspark
+Requires-Dist: acryl-datahub (>=0.10.4)
 
-# Install package
-```bash
-pip install spark-sdk --upgrade
+-----------------
+
+# spark-sdk: Function to help Data Scientist work more effectively with DataLake
+[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.4.21-blue)](https://pypi.org/project/spark-sdk/)
+[![Package Status](https://img.shields.io/badge/status-stable-green)](https://pypi.org/project/spark-sdk/)
+[![Downloads](https://static.pepy.tech/personalized-badge/spark-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/spark-sdk)
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-CADS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://blog.cads.live/)
+
+
+
+## What is it?
+
+**spark-sdk** Function to help Data Scientist work more effectively with DataLake. Include different function work with spark, pyarrow
+
+## Main Features
+Here are just a few of the things that spark-sdk does well:
+  - Get your spark with newest version update,
+    PySpark() function to get your spark requirement.
+  - Easy to read and write data to data lake.
+  - Support user using key to encrypt or decrypt data
+  - Support function to work with distributed system (datalake)
+
+
+## Install
+Binary installers for the latest released version are available at the [Python
+Package Index (PyPI)](https://pypi.org/project/spark-sdk).
+
+
+```sh
+# with PyPI
+pip install spark-sdk
 ```
 
-# Get Spark
+## Dependencies
+- [pyspark - Apache Spark Python API](https://spark.apache.org/docs/latest/api/python/)
+- [pyarrow - Python library for Apache Arrow](https://arrow.apache.org/docs/python/index.html)
+- [pandas - Powerful data structures for data analysis, time series, and statistics](https://pandas.pydata.org/)
+
+
+## Installation from sources
+To install spark-sdk from source you need [Cython](http://git.bigdata.local/data-engineers/sdk/utilities/-/tree/master/spark_sdk) in addition to the normal
+dependencies above. Cython can be installed from PyPI:
+
+```sh
+pip install cython
+```
+
+In the `spark-sdk` directory (same one where you found this file after
+cloning the git repo), execute:
+
+```sh
+python setup.py install
+```
+
+
+
+
+## Get Spark
 ```python
 import spark_sdk as ss
-spark = ss.PySpark(yarn=False, num_executors=4, executor_memory='4G').spark
+spark = ss.PySpark(yarn=False, num_executors=4, driver_memory='8G').spark
 
 # Yarn mode
-spark = ss.PySpark(yarn=True, driver_memory='3G', num_executors=4, executor_memory='4G').spark
+spark = ss.PySpark(yarn=True, driver_memory='2G', num_executors=4, executor_memory='4G').spark
 
 # Add more spark config
 spark = ss.PySpark(yarn=False, driver_memory='8G', num_executors=4, executor_memory='4G',
                   add_on_config1=("spark.sql.catalog.spark_catalog","org.apache.spark.sql.delta.catalog.DeltaCatalog"),
                   add_on_config2=('spark.databricks.delta.retentionDurationCheck.enabled', 'false')
                   ).spark
 ```
-# Store data to dwh
+## Store data to dwh
 ```python
 
 # step 1 read data
 ELT_DATE = '2021-12-01'
 ELT_STR = ELT_DATE[:7]
 import pandas as pd
 df1 = pd.read_csv('./data.csv', sep='\t')
@@ -96,16 +148,16 @@
 # When to drop it also delete data
 ss.drop_table_and_delete_data('database_name.test1')
 
 # IF JUST WANT TO DELETE TABLE NOT DELETE DATA
 ss.drop_table('database_name.test1')
 
 ```
-# Delta format
-# function to store to dwh
+## Delta format
+### function to store to dwh
 ```python
 df1.to_dwh(
     # just end path with delta then table will be store in delta format
     hdfs_path="path/to/data/test1.delta/", 
     partition_by="m", # column time want to partition
     partition_date=ELT_DATE, # partition date
     database="database_name", # database name
@@ -119,48 +171,48 @@
 FROM database_name.table1
 WHERE m='2022-04-01'
 """)
 
 ```
 
 
-# Decrypt Data
+## Decrypt Data
 
-## method 1: sql
+### method 1: sql
 Using Spark SQL
 ```python
 import spark_sdk as ps
 
 key = '1234' # contact Data Owner to get key
 
 df = ps.sql(f"""
 select fdecrypt(column_name, "{key}") column_name
 from database_name.table_name
 limit 50000
 """).toPandas()
 ```
 
 
-## method 2: using pandas
+### method 2: using pandas
 Using pandas
 ```python
 import spark_sdk as ss
 df['new_column'] = df['column'].decrypt_column(key)
 
-# function will return dataframe with column_decrypted
+## function will return dataframe with column_decrypted
 ```
 
-# method 3
+## method 3
 Using pandas apply function
 ```python
 from spark_sdk import decrypt
 df['decrypted'] = df['encrypted'].apply(decrypt,args=("YOUR_KEY",))
 ```
 
-# Encrypt data
+## Encrypt data
 ```python
 import spark_sdk as ss
 
 
 # function to store to dwh
 df.to_dwh(    
     hdfs_path="path/to/data/test1.parquet/", # path hdfs
@@ -171,30 +223,30 @@
     encrypt_columns=['column1','column2'], # list column name need to encrypt
     keys_path = '/path/to/store/keys.json' # if you add encrypt_columns, you need to have keys_path to store keys
 )
 
 ss.PySpark().stop()
 ```
 
-# Create Yaml File Mapping data from CSV to DWH
+## Create Yaml File Mapping data from CSV to DWH
 ```python
 from spark_sdk import CreateYamlDWH
 create_yaml = CreateYamlDWH(
 csv_file = 'data.csv',
 hdfs_path = '/path/to/data/table_name.parquet',
 sep = '\t',
 database_name = 'database_name',
 table_name = 'table_name',
 yaml_path = '/path/to/yaml/file/'
 )
 
 create_yaml.generate_yaml_file()
 ```
 
-# Store spark.sql.DataFrame
+## Store spark.sql.DataFrame
 ```python
 from spark_sdk.src import spark_sdk as ss
 sparkDF = ss.sql("""select * from database.table_name limit 1000""")
 
 ELT_DATE = '2022-06-10'
 sparkDF.to_dwh(
     hdfs_path="path/to/data/test6.parquet/", # path hdfs
@@ -203,46 +255,71 @@
     database="database_name", # database name
     table_name="test6", # table name
     repartition=True,
     driver_memory='4G', executor_memory='4g', num_executors='1', port='4090', yarn=True
 )
 ```
 
-# Working with hdfs
+## Read data
+###
+```python
+# sql
+import spark_sdk as ss
+sparkDF = ss.sql("""select * from database.table_name limit 1000""")
+
+# function
+sparkDF = ss.read_parquet("hdfs:/path/to/file.parquet")
+sparkDF = ss.read_csv("hdfs:/path/to/file.csv")
+sparkDF = ss.read_json("hdfs:/path/to/file.json")
+
+```
+
+## Working with hdfs
 ```python
 mkdir, cat, exists, info, open
+```
 
-# list file
+### list file
+```python
 ss.ls('/path/data')
+```
 
-# create new path 
+### create new path
+```python
 ss.mkdir('/path/create/')
+```
 
-# create new path 
+### create new path
+```python
 ss.exists('/check/path/exists') # return True if exists
+```
 
-# print info
+### print info
+```python
 ss.info('/path/info/')
+```
 
-# open file like normal file
+### open file like local file
+```python
 import json
 with ss.open('/path/to/file.json', mode='rb') as file:
     data = json.load(file)
-
+```
+```python
 import json
 from spark_sdk import Utf8Encoder
 data = {'user': 1, 'code': '456'}
 with ss.open('/path/to/file.json', mode='wb') as file:
     json.dump(data, Utf8Encoder(file), indent=4)
 
 
 json__file = ss.read_json('/path/to/file.json')
 ss.write_json(data, '/path/to_file.json')
 
 sparkDF = ss.read_csv("file:///path/to/data.csv", sep='\t') # with local file
 sparkDF = ss.read_csv("/path/to/data.csv", sep='\t') # with hdfs file
 
-# mode in ['rb', 'wb', 'ab']
+#### mode in ['rb', 'wb', 'ab']
 ```
```

