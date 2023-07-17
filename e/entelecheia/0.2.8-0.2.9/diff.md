# Comparing `tmp/entelecheia-0.2.8.tar.gz` & `tmp/entelecheia-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.2.8.tar", max compression
+gzip compressed data, was "entelecheia-0.2.9.tar", max compression
```

## Comparing `entelecheia-0.2.8.tar` & `entelecheia-0.2.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1071 2023-07-17 02:31:40.753071 entelecheia-0.2.8/LICENSE
--rw-r--r--   0        0        0     1591 2023-07-17 02:31:40.753071 entelecheia-0.2.8/README.md
--rw-r--r--   0        0        0     3065 2023-07-17 02:32:09.058838 entelecheia-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      292 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-07-17 02:32:08.994834 entelecheia-0.2.8/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      353 2023-07-17 02:32:08.998834 entelecheia-0.2.8/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0       83 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      554 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      846 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      125 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       85 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__external__.yaml
--rw-r--r--   0        0        0       70 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       51 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__instance__.yaml
--rw-r--r--   0        0        0       49 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__lambda__.yaml
--rw-r--r--   0        0        0      236 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      388 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      746 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0      193 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      298 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0      183 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__test__.yaml
--rw-r--r--   0        0        0      124 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      148 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/py.typed
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 entelecheia-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-17 10:50:38.583870 entelecheia-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1591 2023-07-17 10:50:38.583870 entelecheia-0.2.9/README.md
+-rw-r--r--   0        0        0     3065 2023-07-17 10:51:07.094296 entelecheia-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-17 10:51:07.030290 entelecheia-0.2.9/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-17 10:51:07.034291 entelecheia-0.2.9/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      554 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      846 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       85 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0       70 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      236 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      387 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      746 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      193 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      183 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      124 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      148 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0        0 2023-07-17 10:50:38.587870 entelecheia-0.2.9/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 entelecheia-0.2.9/PKG-INFO
```

### Comparing `entelecheia-0.2.8/LICENSE` & `entelecheia-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/README.md` & `entelecheia-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/pyproject.toml` & `entelecheia-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.2.8"
+version = "0.2.9"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.11"
+hyfi = "^1.2.13"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/batch/__init__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/copier/conf.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/src/entelecheia/conf/project/__init__.yaml` & `entelecheia-0.2.9/src/entelecheia/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.8/PKG-INFO` & `entelecheia-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.2.8
+Version: 0.2.9
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.2.11,<2.0.0)
+Requires-Dist: hyfi (>=1.2.13,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![home-img]][home-url]
 [![course-img]][course-url]
```

