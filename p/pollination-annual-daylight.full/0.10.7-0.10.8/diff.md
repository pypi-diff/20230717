# Comparing `tmp/pollination-annual-daylight.full-0.10.7.tar.gz` & `tmp/pollination-annual-daylight.full-0.10.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollination-annual-daylight.full-0.10.7.tar", last modified: Thu Jul  6 12:34:30 2023, max compression
+gzip compressed data, was "pollination-annual-daylight.full-0.10.8.tar", last modified: Mon Jul 17 12:05:40 2023, max compression
```

## Comparing `pollination-annual-daylight.full-0.10.7.tar` & `pollination-annual-daylight.full-0.10.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.468236 pollination-annual-daylight.full-0.10.7/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.653005 pollination-annual-daylight.full-0.10.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.645005 pollination-annual-daylight.full-0.10.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.645005 pollination-annual-daylight.full-0.10.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-17 12:05:40.653005 pollination-annual-daylight.full-0.10.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.641005 pollination-annual-daylight.full-0.10.8/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.649005 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.649005 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:05:40.000000 pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 12:05:40.653005 pollination-annual-daylight.full-0.10.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:40.653005 pollination-annual-daylight.full-0.10.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 12:04:59.000000 pollination-annual-daylight.full-0.10.8/tests/validation_test.py
```

### Comparing `pollination-annual-daylight.full-0.10.7/.github/workflows/ci.yaml` & `pollination-annual-daylight.full-0.10.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/.github/workflows/tests.yaml` & `pollination-annual-daylight.full-0.10.8/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/LICENSE` & `pollination-annual-daylight.full-0.10.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/PKG-INFO` & `pollination-annual-daylight.full-0.10.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.full
-Version: 0.10.7
+Version: 0.10.8
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight.full-0.10.7/README.md` & `pollination-annual-daylight.full-0.10.8/README.md`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_post_process.py` & `pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_post_process.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Post-process DAG for annual daylight."""
 from dataclasses import dataclass
 from pollination_dsl.dag import Inputs, GroupedDAG, task, Outputs
 from pollination.honeybee_radiance_postprocess.grid import MergeFolderMetrics
+from pollination.honeybee_radiance_postprocess.post_process import GridSummaryMetrics
 from pollination.honeybee_display.translate import ModelToVis
 
 
 @dataclass
 class AnnualDaylightPostProcess(GroupedDAG):
     """Post-process for annual daylight."""
 
@@ -27,14 +28,19 @@
     )
 
     grids_info = Inputs.file(
         description='Grid information file.',
         path='grids_info.json'
     )
 
+    grid_metrics = Inputs.file(
+        description='A JSON file with additional custom metrics to calculate.',
+        path='grid_metrics.json', optional=True
+    )
+
     @task(
         template=MergeFolderMetrics
     )
     def restructure_metrics(
         self, input_folder=initial_results,
         dist_info=dist_info,
         grids_info=grids_info
@@ -42,14 +48,30 @@
         return [
             {
                 'from': MergeFolderMetrics()._outputs.output_folder,
                 'to': 'metrics'
             }
         ]
 
+    @task(
+        template=GridSummaryMetrics,
+        needs=[restructure_metrics]
+    )
+    def grid_summary_metrics(
+        self, folder=restructure_metrics._outputs.output_folder,
+        model=model, grids_info=grids_info, grid_metrics=grid_metrics,
+        folder_level='sub-folder'
+    ):
+        return [
+            {
+                'from': GridSummaryMetrics()._outputs.grid_summary,
+                'to': 'grid_summary.csv'
+            }
+        ]
+
     @task(template=ModelToVis, needs=[restructure_metrics])
     def create_vsf(
         self, model=model, grid_data='metrics', active_grid_data='udi',
         output_format='vsf'
     ):
         return [
             {
@@ -62,7 +84,11 @@
         source='visualization.vsf',
         description='Annual daylight result visualization in VisualizationSet format.'
     )
 
     metrics = Outputs.folder(
         source='metrics', description='metrics folder.'
     )
+
+    grid_summary = Outputs.file(
+        source='grid_summary.csv', description='grid summary.'
+    )
```

### Comparing `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_prepare_folder.py` & `pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_prepare_folder.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_raytracing.py` & `pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/entry.py` & `pollination-annual-daylight.full-0.10.8/pollination/annual_daylight/entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pollination.alias.inputs.wea import wea_input_timestep_check
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
 from pollination.alias.inputs.schedule import schedule_csv_input
+from pollination.alias.inputs.postprocess import grid_metrics_input
 from pollination.alias.outputs.daylight import daylight_autonomy_results, \
     continuous_daylight_autonomy_results, \
     udi_results, udi_lower_results, udi_upper_results
 
 
 from ._prepare_folder import AnnualDaylightPrepareFolder
 from ._raytracing import AnnualDaylightRayTracing
@@ -94,14 +95,19 @@
         'threshold. The default is -t 300 -lt 100 -ut 3000. The order of the keys is '
         'not important and you can include one or all of them. For instance if you only '
         'want to change the upper threshold to 2000 lux you should use -ut 2000 as '
         'the input.', default='-t 300 -lt 100 -ut 3000',
         alias=daylight_thresholds_input
     )
 
+    grid_metrics = Inputs.file(
+        description='A JSON file with additional custom metrics to calculate.',
+        extensions=['json'], optional=True, alias=grid_metrics_input
+    )
+
     @task(template=AnnualDaylightPrepareFolder)
     def prepare_folder_annual_daylight(
         self, north=north, cpu_count=cpu_count, min_sensor_count=min_sensor_count,
         grid_filter=grid_filter, model=model, wea=wea
         ):
         return [
             {
@@ -159,15 +165,16 @@
             'grids_info': 'grids_info.json'
         }
     )
     def post_process_annual_daylight(
         self, initial_results='initial_results/metrics',
         dist_info=prepare_folder_annual_daylight._outputs.resources,
         grids_info=prepare_folder_annual_daylight._outputs.results,
-        model=model
+        model=model,
+        grid_metrics=grid_metrics
         ):
         return [
             {
                 'from': AnnualDaylightPostProcess()._outputs.metrics,
                 'to': 'metrics'
             },
             {
@@ -205,14 +212,18 @@
         'contain illuminance matrices for each sensor at each timestep of the analysis.'
     )
 
     metrics = Outputs.folder(
         source='metrics', description='Annual metrics folder.'
     )
 
+    grid_summary = Outputs.file(
+        source='grid_summary.csv', description='grid summary.'
+    )
+
     da = Outputs.folder(
         source='metrics/da', description='Daylight autonomy results.',
         alias=daylight_autonomy_results
     )
 
     cda = Outputs.folder(
         source='metrics/cda', description='Continuous daylight autonomy results.',
```

### Comparing `pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/PKG-INFO` & `pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.full
-Version: 0.10.7
+Version: 0.10.8
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/SOURCES.txt` & `pollination-annual-daylight.full-0.10.8/pollination_annual_daylight.full.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.7/setup.py` & `pollination-annual-daylight.full-0.10.8/setup.py`

 * *Files identical despite different names*

