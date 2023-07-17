# Comparing `tmp/pollination-daylight-factor-0.8.8.tar.gz` & `tmp/pollination-daylight-factor-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-daylight-factor-0.8.8.tar", last modified: Thu Jan 19 20:54:27 2023, max compression
+gzip compressed data, was "dist/pollination-daylight-factor-0.8.9.tar", last modified: Mon Jul 17 12:17:44 2023, max compression
```

## Comparing `pollination-daylight-factor-0.8.8.tar` & `pollination-daylight-factor-0.8.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination/daylight_factor/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/pollination/daylight_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/pollination/daylight_factor/_postprocess_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/pollination/daylight_factor/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/pollination/daylight_factor/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 20:53:48.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:54:27.000000 pollination-daylight-factor-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-19 20:53:26.000000 pollination-daylight-factor-0.8.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination/daylight_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/pollination/daylight_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/pollination/daylight_factor/_postprocess_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/pollination/daylight_factor/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/pollination/daylight_factor/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:17:07.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:17:44.000000 pollination-daylight-factor-0.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 12:16:46.000000 pollination-daylight-factor-0.8.9/tests/validation_test.py
```

### Comparing `pollination-daylight-factor-0.8.8/.github/workflows/ci.yaml` & `pollination-daylight-factor-0.8.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-daylight-factor-0.8.8/.github/workflows/tests.yaml` & `pollination-daylight-factor-0.8.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-daylight-factor-0.8.8/LICENSE` & `pollination-daylight-factor-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-daylight-factor-0.8.8/PKG-INFO` & `pollination-daylight-factor-0.8.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pollination-daylight-factor
-Version: 0.8.8
+Version: 0.8.9
 Summary: Daylight factor recipe for Pollination.
 Home-page: https://github.com/pollination/daylight-factor
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/dfrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # daylight-factor
-        
-        Daylight factor recipe for Pollination
-        
-        Use this recipe to calculate daylight factor for a Honeybee model or zipped
-        honeybee-radiance folder.
-        
-        You can only use a Honeybee model when using the `-viz` tag.
-        
-        [Daylight factor recipe on Pollination](https://app.pollination.cloud/ladybug-tools/recipes/daylight-factor/latest?tab=graph)
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,daylight-factor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: viz
+License-File: LICENSE
+
+# daylight-factor
+
+Daylight factor recipe for Pollination
+
+Use this recipe to calculate daylight factor for a Honeybee model or zipped
+honeybee-radiance folder.
+
+You can only use a Honeybee model when using the `-viz` tag.
+
+[Daylight factor recipe on Pollination](https://app.pollination.cloud/ladybug-tools/recipes/daylight-factor/latest?tab=graph)
```

### Comparing `pollination-daylight-factor-0.8.8/pollination/daylight_factor/_postprocess_results.py` & `pollination-daylight-factor-0.8.9/pollination/daylight_factor/_postprocess_results.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 from pollination_dsl.dag import Inputs, GroupedDAG, task, Outputs
 from dataclasses import dataclass
 
 from pollination.path.copy import CopyFile
 
 from pollination.honeybee_radiance.grid import MergeFolderData
+from pollination.honeybee_radiance_postprocess.post_process import GridSummaryMetrics
 
 
 @dataclass
 class DaylightFactorPostProcessResults(GroupedDAG):
     """Daylight factor results post-process."""
 
+    model = Inputs.file(
+        description='Input Honeybee model.',
+        extensions=['json', 'hbjson', 'pkl', 'hbpkl', 'zip']
+    )
+
     results_folder = Inputs.folder(
         description='Daylight factor results input folder.'
     )
 
     grids_info = Inputs.file(
         description='Grids information from the original model.'
     )
 
+    grid_metrics = Inputs.file(
+        description='A JSON file with additional custom metrics to calculate.',
+        path='grid_metrics.json', optional=True
+    )
+
     @task(template=MergeFolderData, annotations={'main_task': True})
     def restructure_results(self, input_folder=results_folder, extension='res'):
         return [
             {
                 'from': MergeFolderData()._outputs.output_folder,
                 'to': 'results'
             }
@@ -32,11 +43,31 @@
         return [
             {
                 'from': CopyFile()._outputs.dst,
                 'to': 'results/grids_info.json'
             }
         ]
 
+    @task(
+        template=GridSummaryMetrics,
+        needs=[restructure_results]
+    )
+    def grid_summary_metrics(
+        self, folder=restructure_results._outputs.output_folder,
+        model=model, grids_info=grids_info, grid_metrics=grid_metrics,
+        folder_level='main-folder'
+    ):
+        return [
+            {
+                'from': GridSummaryMetrics()._outputs.grid_summary,
+                'to': 'grid_summary.csv'
+            }
+        ]
+
     results = Outputs.folder(
         source='results',
         description='Daylight factor results.'
     )
+
+    grid_summary = Outputs.file(
+        source='grid_summary.csv', description='grid summary.'
+    )
```

### Comparing `pollination-daylight-factor-0.8.8/pollination/daylight_factor/_prepare_folder.py` & `pollination-daylight-factor-0.8.9/pollination/daylight_factor/_prepare_folder.py`

 * *Files identical despite different names*

### Comparing `pollination-daylight-factor-0.8.8/pollination/daylight_factor/entry.py` & `pollination-daylight-factor-0.8.9/pollination/daylight_factor/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pollination.honeybee_radiance.raytrace import RayTracingDaylightFactor
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.radiancepar import rad_par_daylight_factor_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
+from pollination.alias.inputs.postprocess import grid_metrics_input
 from pollination.alias.outputs.daylight import daylight_factor_results
 
 
 from ._prepare_folder import DaylightFactorPrepareFolder
 from ._postprocess_results import DaylightFactorPostProcessResults
 
 
@@ -56,14 +57,19 @@
         'of the model that are simulated. For instance, first_floor_* will simulate '
         'only the sensor grids that have an identifier that starts with '
         'first_floor_. By default, all grids in the model will be simulated.',
         default='*',
         alias=grid_filter_input
     )
 
+    grid_metrics = Inputs.file(
+        description='A JSON file with additional custom metrics to calculate.',
+        extensions=['json'], optional=True, alias=grid_metrics_input
+    )
+
     @task(template=DaylightFactorPrepareFolder)
     def prepare_daylight_factor_folder(
             self, cpu_count=cpu_count, min_sensor_count=min_sensor_count,
             grid_filter=grid_filter, model=model
     ):
         return [
             {
@@ -109,22 +115,31 @@
         ]
 
     @task(
         template=DaylightFactorPostProcessResults,
         needs=[daylight_factor_ray_tracing]
     )
     def post_process_results(
-            self, results_folder='initial_results',
-            grids_info='resources/grids_info.json'
+        self, results_folder='initial_results',
+        grids_info='resources/grids_info.json',
+        model=model, grid_metrics=grid_metrics
     ):
         return [
             {
                 'from': DaylightFactorPostProcessResults()._outputs.results,
                 'to': 'results'
+            },
+            {
+                'from': DaylightFactorPostProcessResults()._outputs.grid_summary,
+                'to': 'grid_summary.csv'
             }
         ]
 
     results = Outputs.folder(
         source='results', description='Folder with raw result files '
         '(.res) that contain daylight factor values for each sensor.',
         alias=daylight_factor_results
     )
+
+    grid_summary = Outputs.file(
+        source='grid_summary.csv', description='grid summary.'
+    )
```

### Comparing `pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/PKG-INFO` & `pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pollination-daylight-factor
-Version: 0.8.8
+Version: 0.8.9
 Summary: Daylight factor recipe for Pollination.
 Home-page: https://github.com/pollination/daylight-factor
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_components/honeybee/png/dfrecipe.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
-Description: # daylight-factor
-        
-        Daylight factor recipe for Pollination
-        
-        Use this recipe to calculate daylight factor for a Honeybee model or zipped
-        honeybee-radiance folder.
-        
-        You can only use a Honeybee model when using the `-viz` tag.
-        
-        [Daylight factor recipe on Pollination](https://app.pollination.cloud/ladybug-tools/recipes/daylight-factor/latest?tab=graph)
-        
 Keywords: honeybee,radiance,ladybug-tools,daylight,daylight-factor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: viz
+License-File: LICENSE
+
+# daylight-factor
+
+Daylight factor recipe for Pollination
+
+Use this recipe to calculate daylight factor for a Honeybee model or zipped
+honeybee-radiance folder.
+
+You can only use a Honeybee model when using the `-viz` tag.
+
+[Daylight factor recipe on Pollination](https://app.pollination.cloud/ladybug-tools/recipes/daylight-factor/latest?tab=graph)
```

### Comparing `pollination-daylight-factor-0.8.8/pollination_daylight_factor.egg-info/SOURCES.txt` & `pollination-daylight-factor-0.8.9/pollination_daylight_factor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-daylight-factor-0.8.8/setup.py` & `pollination-daylight-factor-0.8.9/setup.py`

 * *Files identical despite different names*

