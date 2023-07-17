# Comparing `tmp/h2o_mlops_scoring_client-0.0.8b1-py3-none-any.whl.zip` & `tmp/h2o_mlops_scoring_client-0.0.9b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 8752 bytes, number of entries: 8
--rw-r--r--  2.0 unx        8 b- defN 23-May-31 16:47 h2o_mlops_scoring_client/VERSION
--rw-r--r--  2.0 unx     9820 b- defN 23-May-31 16:46 h2o_mlops_scoring_client/__init__.py
--rw-r--r--  2.0 unx    14230 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_utils.py
--rw-r--r--  2.0 unx      228 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_version.py
--rw-r--r--  2.0 unx     3044 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      737 b- defN 23-May-31 16:47 h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD
-8 files, 28184 bytes uncompressed, 7438 bytes compressed:  73.6%
+Zip file size: 10283 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client/VERSION
+-rw-r--r--  2.0 unx    10937 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client/__init__.py
+-rw-r--r--  2.0 unx    14124 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client/_utils.py
+-rw-r--r--  2.0 unx      497 b- defN 23-Jun-06 23:42 h2o_mlops_scoring_client/_version.py
+-rw-r--r--  2.0 unx     1635 b- defN 23-Jun-06 23:42 h2o_mlops_scoring_client/log4j.properties
+-rw-r--r--  2.0 unx     3054 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client-0.0.9b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client-0.0.9b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client-0.0.9b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      836 b- defN 23-Jul-17 20:21 h2o_mlops_scoring_client-0.0.9b1.dist-info/RECORD
+9 files, 31208 bytes uncompressed, 8811 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: h2o_mlops_scoring_client/_utils.py
 Comment: 
 
 Filename: h2o_mlops_scoring_client/_version.py
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA
+Filename: h2o_mlops_scoring_client/log4j.properties
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/WHEEL
+Filename: h2o_mlops_scoring_client-0.0.9b1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/top_level.txt
+Filename: h2o_mlops_scoring_client-0.0.9b1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD
+Filename: h2o_mlops_scoring_client-0.0.9b1.dist-info/top_level.txt
+Comment: 
+
+Filename: h2o_mlops_scoring_client-0.0.9b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_mlops_scoring_client/VERSION

```diff
@@ -1 +1 @@
-0.0.8b1
+0.0.9b1
```

## h2o_mlops_scoring_client/__init__.py

```diff
@@ -1,13 +1,14 @@
 import datetime as _datetime
 import logging as _logging
 import os as _os
 import typing as _typing
 
 import pandas as _pandas
+import pyspark as _pyspark
 
 from h2o_mlops_scoring_client import _utils
 from h2o_mlops_scoring_client._utils import Format
 from h2o_mlops_scoring_client._utils import WriteMode
 from h2o_mlops_scoring_client._version import version as __version__  # noqa: F401
 
 
@@ -16,14 +17,29 @@
     datefmt="%y/%m/%d %H:%M:%S",
     level=_logging.INFO,
 )
 logger = _logging.getLogger(__name__)
 spark_conf_dir = _os.environ.get("SPARK_CONF_DIR")
 spark_master = _os.environ.get("MASTER", "local[*]")
 if spark_master.startswith("local"):
+    # quiet spark warnings
+    import importlib.resources
+
+    try:
+        resource = importlib.resources.files(  # type: ignore
+            "h2o_mlops_scoring_client"
+        ).joinpath("log4j.properties")
+    except AttributeError:
+        # fallback for Python < 3.9
+        with importlib.resources.path(
+            "h2o_mlops_scoring_client", "log4j.properties"
+        ) as resource:
+            pass
+    _os.environ["LOG4J_CONFIGURATION_FILE"] = str(resource)
+    # ignore local SPARK_HOME
     _os.environ.pop("SPARK_HOME", None)
 
 
 def get_capabilities(
     mlops_endpoint_url: str, passphrase: _typing.Optional[str] = None
 ) -> _typing.List[str]:
     """Capabilities of the scoring endpoint.
@@ -55,14 +71,39 @@
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
         passphrase: passphrase for protected MLOps endpoints
     """
     return _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase).schema
 
 
+def get_spark_session(
+    app_name: str = "h2o_mlops_scoring_client",
+    mini_batch_size: int = 1000,
+    spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
+) -> _pyspark.sql.SparkSession:
+    """Get or create a Spark session configured for the scoring client.
+
+    Args:
+        app_name: name of application in Spark
+        mini_batch_size: number of rows per scorer call
+        spark_config_overrides: pass Spark configuration options to the Spark context
+    """
+
+    if spark_master.startswith("local") and spark_conf_dir:
+        _utils.preflight(spark_conf_dir)
+        _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
+    spark = _utils.get_spark_session(
+        app_name=app_name,
+        master=spark_master,
+        mini_batch_size=mini_batch_size,
+        spark_config=spark_config_overrides,
+    )
+    return spark
+
+
 def score_source_sink(
     *,
     mlops_endpoint_url: str,
     id_column: str,
     source_data: str,
     source_format: Format,
     sink_location: str,
@@ -98,24 +139,17 @@
             after scoring
         mini_batch_size: number of rows per scorer call
         spark_config_overrides: pass Spark configuration options to the Spark context
     """
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
-        if spark_master.startswith("local") and spark_conf_dir:
-            _utils.preflight(spark_conf_dir)
-            _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
-
-        logger.info("Starting Spark context")
-        spark = _utils.get_spark_session(
-            app_name="h2o_mlops_scoring_client",
-            master=spark_master,
+        spark = get_spark_session(
             mini_batch_size=mini_batch_size,
-            spark_config=spark_config_overrides,
+            spark_config_overrides=spark_config_overrides,
         )
 
         logger.info(f"Connecting to H2O.ai MLOps scorer at '{mlops_endpoint_url}'")
         mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase)
 
         sdf = _utils.read_source(spark, source_data, source_format, source_config)
 
@@ -140,56 +174,58 @@
 
         logger.info(f"Total run time: {stop - start}")
         logger.info(f"Scoring run time: {stop - start_scoring}")
 
     finally:
         if spark_master.startswith("local"):
             try:
-                logger.info("Stopping Spark context")
                 spark.stop()
             except UnboundLocalError:
                 pass
 
 
 def score_data_frame(
     *,
     mlops_endpoint_url: str,
     id_column: str,
-    data_frame: _pandas.DataFrame,
+    data_frame: _typing.Union[_pandas.DataFrame, _pyspark.sql.DataFrame],
     mini_batch_size: int = 1000,
     passphrase: _typing.Optional[str] = None,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
-) -> _pandas.DataFrame:
+) -> _typing.Union[_pandas.DataFrame, _pyspark.sql.DataFrame]:
     """Do scoring of a data frame against a MLOps deployment. Parallelized mini-batch
     scoring with Spark is done if the data frame row count is more than mini_batch_size.
 
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
         id_column: name of column in data to be scored
             - column should contain unique row identifiers
         data_frame: Pandas DataFrame
         mini_batch_size: number of rows per scorer call
         passphrase: passphrase for protected MLOps endpoint
         spark_config_overrides: pass Spark configuration options to the Spark context
     """
-    if data_frame.shape[0] > mini_batch_size:
-        return _score_data_frame_spark(
+    if (
+        isinstance(data_frame, _pandas.DataFrame)
+        and data_frame.shape[0] <= mini_batch_size
+    ):
+        return _score_data_frame_direct(
             mlops_endpoint_url=mlops_endpoint_url,
             passphrase=passphrase,
             id_column=id_column,
             data_frame=data_frame,
-            mini_batch_size=mini_batch_size,
-            spark_config_overrides=spark_config_overrides,
         )
     else:
-        return _score_data_frame_direct(
+        return _score_data_frame_spark(
             mlops_endpoint_url=mlops_endpoint_url,
             passphrase=passphrase,
             id_column=id_column,
             data_frame=data_frame,
+            mini_batch_size=mini_batch_size,
+            spark_config_overrides=spark_config_overrides,
         )
 
 
 def _score_data_frame_direct(
     *,
     mlops_endpoint_url: str,
     id_column: str,
@@ -214,52 +250,54 @@
     return scored_df
 
 
 def _score_data_frame_spark(
     *,
     mlops_endpoint_url: str,
     id_column: str,
-    data_frame: _pandas.DataFrame,
+    data_frame: _typing.Union[_pandas.DataFrame, _pyspark.sql.DataFrame],
     mini_batch_size: int = 1000,
     passphrase: _typing.Optional[str] = None,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
-) -> _pandas.DataFrame:
+) -> _typing.Union[_pandas.DataFrame, _pyspark.sql.DataFrame]:
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
-        if spark_master.startswith("local") and spark_conf_dir:
-            _utils.preflight(spark_conf_dir)
-            _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
-
-        logger.info("Starting Spark context")
-        spark = _utils.get_spark_session(
-            app_name="h2o_mlops_scoring_client",
-            master=spark_master,
+        is_pandas = isinstance(data_frame, _pandas.DataFrame)
+
+        spark = get_spark_session(
             mini_batch_size=mini_batch_size,
-            spark_config=spark_config_overrides,
+            spark_config_overrides=spark_config_overrides,
         )
 
         logger.info(f"Connecting to H2O.ai MLOps scorer at '{mlops_endpoint_url}'")
         mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase)
 
-        sdf = spark.createDataFrame(data_frame)
+        if is_pandas:
+            sdf = spark.createDataFrame(data_frame)
+        else:
+            sdf = data_frame
 
         logger.info("Starting scoring data frame")
         start_scoring = _datetime.datetime.now().replace(microsecond=0)
         scored_sdf = mlops_endpoint.score_spark_dataframe(sdf, id_column=id_column)
-        scored_df = scored_sdf.toPandas()
 
         logger.info("Scoring complete")
+
+        if is_pandas:
+            scored_df = scored_sdf.toPandas()
+        else:
+            scored_df = scored_sdf
+
         stop = _datetime.datetime.now().replace(microsecond=0)
 
         logger.info(f"Total run time: {stop - start}")
         logger.info(f"Scoring run time: {stop - start_scoring}")
 
         return scored_df
 
     finally:
-        if spark_master.startswith("local"):
+        if is_pandas and spark_master.startswith("local"):
             try:
-                logger.info("Stopping Spark context")
                 spark.stop()
             except UnboundLocalError:
                 pass
```

## h2o_mlops_scoring_client/_utils.py

```diff
@@ -323,18 +323,16 @@
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
     ] and not _source_config.get("url"):
         raise RuntimeError("JDBC connection URL required for source.")
     if source_format in [Format.SNOWFLAKE_QUERY, Format.SNOWFLAKE_TABLE]:
         required_sf_options = {
             "sfDatabase",
-            "sfPassword",
             "sfURL",
             "sfUser",
-            "sfWarehouse",
         }
         missing_sf_options = required_sf_options.difference(_source_config.keys())
         if missing_sf_options:
             raise RuntimeError(
                 f"Snowflake option(s) {missing_sf_options} required for source."
             )
 
@@ -367,18 +365,16 @@
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
     ] and not _sink_config.get("url"):
         raise RuntimeError("JDBC connection URL required for sink.")
     if sink_format in [Format.SNOWFLAKE_QUERY, Format.SNOWFLAKE_TABLE]:
         required_sf_options = {
             "sfDatabase",
-            "sfPassword",
             "sfURL",
             "sfUser",
-            "sfWarehouse",
         }
         missing_sf_options = required_sf_options.difference(_sink_config.keys())
         if missing_sf_options:
             raise RuntimeError(
                 f"Snowflake option(s) {missing_sf_options} required for sink."
             )
```

## h2o_mlops_scoring_client/_version.py

```diff
@@ -1,9 +1,17 @@
 import importlib.resources
 
 
 version = "0.0.0"
 
-if importlib.resources.is_resource("h2o_mlops_scoring_client", "VERSION"):
-    version = importlib.resources.read_text(
-        "h2o_mlops_scoring_client", "VERSION"
-    ).strip()
+try:
+    resource = importlib.resources.files(  # type: ignore
+        "h2o_mlops_scoring_client"
+    ).joinpath("VERSION")
+    if resource.is_file():
+        version = resource.read_text().strip()
+except AttributeError:
+    # fallback for Python < 3.9
+    if importlib.resources.is_resource("h2o_mlops_scoring_client", "VERSION"):
+        version = importlib.resources.read_text(
+            "h2o_mlops_scoring_client", "VERSION"
+        ).strip()
```

## Comparing `h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA` & `h2o_mlops_scoring_client-0.0.9b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-mlops-scoring-client
-Version: 0.0.8b1
+Version: 0.0.9b1
 Summary: A Python client library to simplify robust mini-batch scoring against an H2O MLOps scoring endpoint.
 Author: H2O.ai
 Author-email: support@h2o.ai
 License: Proprietary License
 Project-URL: Documentation, https://docs.h2o.ai/mlops/mlops-scoring-client/overview
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
     source_format=h2o_mlops_scoring_client.Format.CSV,
     sink_location="file:///.../output/",
     sink_format=h2o_mlops_scoring_client.Format.PARQUET,
     sink_write_mode=h2o_mlops_scoring_client.WriteMode.OVERWRITE
 )
 ```
 
-Or if you want to work with Pandas DataFrames:
+Or if you want to work with Pandas or Spark data frames:
 
 ```python
 scores_df = h2o_mlops_scoring_client.score_data_frame(
     mlops_endpoint_url="https://.../model/score",
     id_column="ID",
     data_frame=input_df,
 )
```

## Comparing `h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD` & `h2o_mlops_scoring_client-0.0.9b1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-h2o_mlops_scoring_client/VERSION,sha256=5BCbE0YEZ7BdpBwDfmQSMrRVCAdycpy7RZkg7E5Y1OM,8
-h2o_mlops_scoring_client/__init__.py,sha256=qyFWf4r4ZqD4h09fNMuTKtPHHb76TKf0G4-qHj72ddc,9820
-h2o_mlops_scoring_client/_utils.py,sha256=oXY-dL325duYATlU6idk73OGCQCaeMolfa91OG-Pygs,14230
-h2o_mlops_scoring_client/_version.py,sha256=1zDsuRRqsnIsxWZY4--3dDuaB3D82cfPyw541E-uOic,228
-h2o_mlops_scoring_client-0.0.8b1.dist-info/METADATA,sha256=co5TwLae1Il0LI_nC_zOxYil8WgKQup4ksQokmUkGek,3044
-h2o_mlops_scoring_client-0.0.8b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-h2o_mlops_scoring_client-0.0.8b1.dist-info/top_level.txt,sha256=QqsGjPwyloWBgEOjck-e-Bdmk2YW_AaAcX7YWz40UKg,25
-h2o_mlops_scoring_client-0.0.8b1.dist-info/RECORD,,
+h2o_mlops_scoring_client/VERSION,sha256=YZQZvgsV3d68t-tj1-f7qYPlGYTpxmLkHu0jCIAx_qY,8
+h2o_mlops_scoring_client/__init__.py,sha256=ChZnP0zQRngNWhoiJadRwy549UbuhtN9YoPvAPixxtM,10937
+h2o_mlops_scoring_client/_utils.py,sha256=u2Rugn7rBO1QJHIV_1Ezu6G1XQau3D14E8X3cmZnbnk,14124
+h2o_mlops_scoring_client/_version.py,sha256=xSFev2acw6sH4HhRIFTczsDXl8HZlO172zFY8jjbdLs,497
+h2o_mlops_scoring_client/log4j.properties,sha256=VFvumzeQUxBHEfFvxJ4AqHTX0wQXxdWEt8ifMMgZSCM,1635
+h2o_mlops_scoring_client-0.0.9b1.dist-info/METADATA,sha256=GFONhQdMFudagy0k75jgtpVOETrIMvk4B8eswdckJE0,3054
+h2o_mlops_scoring_client-0.0.9b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+h2o_mlops_scoring_client-0.0.9b1.dist-info/top_level.txt,sha256=QqsGjPwyloWBgEOjck-e-Bdmk2YW_AaAcX7YWz40UKg,25
+h2o_mlops_scoring_client-0.0.9b1.dist-info/RECORD,,
```

