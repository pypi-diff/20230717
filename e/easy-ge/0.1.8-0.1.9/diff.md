# Comparing `tmp/easy_ge-0.1.8.tar.gz` & `tmp/easy_ge-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.8.tar", max compression
+gzip compressed data, was "easy_ge-0.1.9.tar", max compression
```

## Comparing `easy_ge-0.1.8.tar` & `easy_ge-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1059 2023-07-14 04:28:31.312322 easy_ge-0.1.8/LICENSE
--rw-r--r--   0        0        0       95 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/__init__.py
--rw-r--r--   0        0        0      308 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/docker_entry.py
--rw-r--r--   0        0        0     6297 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     4468 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/helpers.py
--rw-r--r--   0        0        0     2335 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     4535 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     5091 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1137 2023-07-14 04:28:31.316322 easy_ge-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 04:28:31.316322 easy_ge-0.1.8/readme.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 easy_ge-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-14 05:54:57.135529 easy_ge-0.1.9/LICENSE
+-rw-r--r--   0        0        0       41 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/__init__.py
+-rw-r--r--   0        0        0      308 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/entrypoint.py
+-rw-r--r--   0        0        0     6411 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     4468 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/helpers.py
+-rw-r--r--   0        0        0     2166 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     4535 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     5091 2023-07-14 05:54:57.135529 easy_ge-0.1.9/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1137 2023-07-14 05:54:57.139530 easy_ge-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 05:54:57.139530 easy_ge-0.1.9/readme.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 easy_ge-0.1.9/PKG-INFO
```

### Comparing `easy_ge-0.1.8/LICENSE` & `easy_ge-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.8/easy_ge/expectation_manager.py` & `easy_ge-0.1.9/easy_ge/expectation_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s [%(levelname)s] %(message)s",
     handlers=[
         logging.StreamHandler()
     ]
 )
+logging.getLogger('great_expectations.data_context.data_context.abstract_data_context').setLevel(logging.WARNING)
 
 class ExpectationManager:
     """
     A class for managing Great Expectations operations.
     """
 
     def __init__(self, ge_template_handler: TemplateHandler, cp_template_handler: TemplateHandler, generate_docs: bool):
```

### Comparing `easy_ge-0.1.8/easy_ge/helpers.py` & `easy_ge-0.1.9/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.8/easy_ge/main.py` & `easy_ge-0.1.9/easy_ge/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,37 +3,33 @@
 """
 
 import importlib.resources
 import logging
 from datetime import datetime
 
 try:
-    from expectation_manager import ExpectationManager
-    from helpers import ConfigLoader, TemplateHandler
-except:
     from easy_ge.expectation_manager import ExpectationManager
     from easy_ge.helpers import ConfigLoader, TemplateHandler  
+except:
+    from expectation_manager import ExpectationManager
+    from helpers import ConfigLoader, TemplateHandler
 
 ###############################
 # ONLY FOR LOCAL Testing
 ###############################
-GCP_KEY_PATH = "gcp_key_spark.json"
-JAVA_HOME = "/usr/lib/jvm/java-11-openjdk-amd64"
-import os
-
-os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = GCP_KEY_PATH
-os.environ["JAVA_HOME"] = JAVA_HOME
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s [%(levelname)s] %(message)s",
     handlers=[
         logging.StreamHandler()
     ]
 )
+logging.getLogger('great_expectations.data_context.data_context.abstract_data_context').setLevel(logging.WARNING)
+
 
 def easy_validation(config: str):
     schema_path = importlib.resources.files("easy_ge.templates").joinpath("schema.json")
     ge_template_path = importlib.resources.files("easy_ge.templates").joinpath("great_expectations.tpl")
     cp_template_path = importlib.resources.files("easy_ge.templates").joinpath("checkpoint.tpl")
 
     user_config = ConfigLoader(config, str(schema_path)).load_config()
@@ -49,15 +45,11 @@
     cp_result = expectation_manager.run_checkpoint(user_config, data_context)
     success_threshold = user_config["Outputs"].get("FailureThreshold", None)
     df = expectation_manager.generate_summary_table(cp_result, success_threshold)
 
     if user_config["Outputs"]["SaveSummaryTableAsCSV"]:
         logging.info("Saving summary table as CSV...")
         filename = f"{user_config['Backend']['ExpectationSuiteName']}-{datetime.today().strftime('%Y-%m-%d')}.csv"
-        df.to_csv(filename)
+        df.to_csv(filename, index=False)
     logging.info("Validation complete.")
 
     return df  # return the summary table
-
-if __name__ == "__main__":
-    config_path = "sample_config.yaml"
-    df = easy_validation(config_path)
```

### Comparing `easy_ge-0.1.8/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.9/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.8/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.9/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.8/easy_ge/templates/schema.json` & `easy_ge-0.1.9/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.8/pyproject.toml` & `easy_ge-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_ge"
-version = "0.1.8"
+version = "0.1.9"
 description = "A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "readme.md"
 packages = [{include = "easy_ge"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `easy_ge-0.1.8/PKG-INFO` & `easy_ge-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases.
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

