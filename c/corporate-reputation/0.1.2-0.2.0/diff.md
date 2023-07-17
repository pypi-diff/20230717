# Comparing `tmp/corporate_reputation-0.1.2.tar.gz` & `tmp/corporate_reputation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.1.2.tar", max compression
+gzip compressed data, was "corporate_reputation-0.2.0.tar", max compression
```

## Comparing `corporate_reputation-0.1.2.tar` & `corporate_reputation-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,59 @@
--rw-r--r--   0        0        0     1071 2023-07-11 02:40:48.250285 corporate_reputation-0.1.2/LICENSE
--rw-r--r--   0        0        0     3912 2023-07-11 02:40:48.250285 corporate_reputation-0.1.2/README.md
--rw-r--r--   0        0        0     3030 2023-07-11 02:41:12.890581 corporate_reputation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-11 02:41:12.834580 corporate_reputation-0.1.2/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      338 2023-07-11 02:41:12.834580 corporate_reputation-0.1.2/src/corprep/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      901 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      388 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/project/__init__.yaml
--rw-r--r--   0        0        0      185 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      305 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__init__.yaml
--rw-r--r--   0        0        0      208 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__test__.yaml
--rw-r--r--   0        0        0      114 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      113 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/py.typed
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 corporate_reputation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3912 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/README.md
+-rw-r--r--   0        0        0     3050 2023-07-17 20:56:47.606474 corporate_reputation-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-17 20:56:47.554474 corporate_reputation-0.2.0/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-17 20:56:47.554474 corporate_reputation-0.2.0/src/corprep/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      105 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/load_raw_dataset.yaml
+-rw-r--r--   0        0        0      241 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       88 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/save_dataset.yaml
+-rw-r--r--   0        0        0       90 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      387 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      377 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/datasets.yaml
+-rw-r--r--   0        0        0      746 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      193 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/__test__.yaml
+-rw-r--r--   0        0        0      221 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/corprep.yaml
+-rw-r--r--   0        0        0       38 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      183 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      145 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/datasets.yaml
+-rw-r--r--   0        0        0      124 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      148 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0      150 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/corprep.yaml
+-rw-r--r--   0        0        0      204 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/datasets/raw.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/py.typed
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 corporate_reputation-0.2.0/PKG-INFO
```

### Comparing `corporate_reputation-0.1.2/LICENSE` & `corporate_reputation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.2/README.md` & `corporate_reputation-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.2/pyproject.toml` & `corporate_reputation-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.1.2"
+version = "0.2.0"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.2"
+hyfi = "^1.2.13"
+ekonlpy = "^1.1.7"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/batch/__init__.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/batch/__init__.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-batch_name: ${oc.select:..batch_name,demo-batch}
+_config_name_: __init__
+batch_name: ${oc.select:..batch_name,__init__}
 batch_num:
-batch_root: ${oc.select:..path.batch_outputs,tmp/batch-outputs/${.batch_name}}
+batch_root: ${oc.select:..task_root,workspace}/${oc.select:..path.dirnames.outputs,outputs}
 output_suffix:
 output_extention:
 random_seed: true
 seed: -1
 resume_run: false
 resume_latest: false
 device: cpu
```

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/copier/conf.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/dotenv/__init__.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/hydra/help/help.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/mode/__init__.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/mode/__init__.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # @package _global_
 debug_mode: false
 resolve: true
 verbose: false
 ignore_warnings: true
-logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
-hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
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

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/path/__init__.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/path/__init__.yaml`

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

### Comparing `corporate_reputation-0.1.2/src/corprep/conf/project/__init__.yaml` & `corporate_reputation-0.2.0/src/corprep/conf/project/__init__.yaml`

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

### Comparing `corporate_reputation-0.1.2/PKG-INFO` & `corporate_reputation-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.1.2
+Version: 0.2.0
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.2.2,<2.0.0)
+Requires-Dist: ekonlpy (>=1.1.7,<2.0.0)
+Requires-Dist: hyfi (>=1.2.13,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

