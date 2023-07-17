# Comparing `tmp/entelecheia-0.2.7.tar.gz` & `tmp/entelecheia-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.2.7.tar", max compression
+gzip compressed data, was "entelecheia-0.2.8.tar", max compression
```

## Comparing `entelecheia-0.2.7.tar` & `entelecheia-0.2.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1071 2023-07-16 20:00:48.869239 entelecheia-0.2.7/LICENSE
--rw-r--r--   0        0        0     1591 2023-07-16 20:00:48.869239 entelecheia-0.2.7/README.md
--rw-r--r--   0        0        0     3065 2023-07-16 20:01:12.725675 entelecheia-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      292 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-07-16 20:01:12.669674 entelecheia-0.2.7/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      353 2023-07-16 20:01:12.669674 entelecheia-0.2.7/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0       83 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      969 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      554 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      880 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      125 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       85 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__external__.yaml
--rw-r--r--   0        0        0       70 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       51 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__instance__.yaml
--rw-r--r--   0        0        0       49 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/__lambda__.yaml
--rw-r--r--   0        0        0      236 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      388 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0      160 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      298 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0      183 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/task/__test__.yaml
--rw-r--r--   0        0        0      124 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      148 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-16 20:00:48.873239 entelecheia-0.2.7/src/entelecheia/py.typed
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 entelecheia-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-17 02:31:40.753071 entelecheia-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1591 2023-07-17 02:31:40.753071 entelecheia-0.2.8/README.md
+-rw-r--r--   0        0        0     3065 2023-07-17 02:32:09.058838 entelecheia-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-17 02:32:08.994834 entelecheia-0.2.8/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-17 02:32:08.998834 entelecheia-0.2.8/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      554 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      846 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      125 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       85 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0       70 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      236 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      388 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      746 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      193 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      298 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      183 2023-07-17 02:31:40.757071 entelecheia-0.2.8/src/entelecheia/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      124 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      148 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0        0 2023-07-17 02:31:40.761072 entelecheia-0.2.8/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 entelecheia-0.2.8/PKG-INFO
```

### Comparing `entelecheia-0.2.7/LICENSE` & `entelecheia-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/README.md` & `entelecheia-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/pyproject.toml` & `entelecheia-0.2.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.2.7"
+version = "0.2.8"
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
-hyfi = "^1.2.10"
+hyfi = "^1.2.11"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/batch/__init__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/copier/conf.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/mode/__init__.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # @package _global_
 debug_mode: false
 resolve: true
 verbose: false
 ignore_warnings: true
-logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
-hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}/logs/hydra
+logging_level: WARNING
+hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}/logs/hydra
 
 hydra:
   job:
-    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
+    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}}
     chdir: true
   run:
     dir: ${hydra_log_dir}/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
     dir: ${hydra_log_dir}/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
```

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/path/__init__.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -5,13 +5,13 @@
   - dirnames: __init__
 
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
-global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}
-global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}
+global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}
+global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}
 # project specific paths
-project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}
+project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}
 project_root: ${oc.select:..project_root,${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}}
-project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}}
+project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},workspace}}
```

### Comparing `entelecheia-0.2.7/src/entelecheia/conf/project/__init__.yaml` & `entelecheia-0.2.8/src/entelecheia/conf/project/__init__.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 _config_name_: __init__
-project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
+project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},${oc.select:about.__package_name__,hyfi}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
-project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
-global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
-global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
+project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},workspace}
+global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}
+global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
 use_wandb: false
 verbose: ${alt:${oc.env:HYFI_VERBOSE,null},false}
```

### Comparing `entelecheia-0.2.7/PKG-INFO` & `entelecheia-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.2.7
+Version: 0.2.8
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
-Requires-Dist: hyfi (>=1.2.10,<2.0.0)
+Requires-Dist: hyfi (>=1.2.11,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![home-img]][home-url]
 [![course-img]][course-url]
```

