# Comparing `tmp/cleanvision-0.3.1.tar.gz` & `tmp/cleanvision-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanvision-0.3.1.tar", last modified: Fri Jul  7 19:58:16 2023, max compression
+gzip compressed data, was "cleanvision-0.3.2.tar", last modified: Mon Jul 17 03:23:13 2023, max compression
```

## Comparing `cleanvision-0.3.1.tar` & `cleanvision-0.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.090724 cleanvision-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-07 19:58:04.000000 cleanvision-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-07 19:58:04.000000 cleanvision-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-07 19:58:04.000000 cleanvision-0.3.1/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 19:58:04.000000 cleanvision-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 19:58:04.000000 cleanvision-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50513 2023-07-07 19:58:16.090724 cleanvision-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-07-07 19:58:04.000000 cleanvision-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-07 19:58:04.000000 cleanvision-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:58:16.090724 cleanvision-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.078724 cleanvision-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.082724 cleanvision-0.3.1/src/cleanvision/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/folder_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/imagelab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/issue_managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/duplicate_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/image_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/issue_managers/image_property_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.086724 cleanvision-0.3.1/src/cleanvision/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/base_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-07 19:58:04.000000 cleanvision-0.3.1/src/cleanvision/utils/viz_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.082724 cleanvision-0.3.1/src/cleanvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50513 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 19:58:16.000000 cleanvision-0.3.1/src/cleanvision.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:58:16.090724 cleanvision-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_duplicate_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_image_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_image_property_issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 19:58:05.000000 cleanvision-0.3.1/tests/test_viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.913138 cleanvision-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-17 03:23:02.000000 cleanvision-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-17 03:23:02.000000 cleanvision-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-17 03:23:02.000000 cleanvision-0.3.2/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-17 03:23:02.000000 cleanvision-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 03:23:02.000000 cleanvision-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-07-17 03:23:13.913138 cleanvision-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-17 03:23:02.000000 cleanvision-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 03:23:02.000000 cleanvision-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:23:13.913138 cleanvision-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.909138 cleanvision-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.909138 cleanvision-0.3.2/src/cleanvision/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.913138 cleanvision-0.3.2/src/cleanvision/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/folder_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27057 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/imagelab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.913138 cleanvision-0.3.2/src/cleanvision/issue_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/issue_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/issue_managers/duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/issue_managers/image_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/issue_managers/image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.913138 cleanvision-0.3.2/src/cleanvision/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/base_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-17 03:23:02.000000 cleanvision-0.3.2/src/cleanvision/utils/viz_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.909138 cleanvision-0.3.2/src/cleanvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-07-17 03:23:13.000000 cleanvision-0.3.2/src/cleanvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-17 03:23:13.000000 cleanvision-0.3.2/src/cleanvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:23:13.000000 cleanvision-0.3.2/src/cleanvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 03:23:13.000000 cleanvision-0.3.2/src/cleanvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 03:23:13.000000 cleanvision-0.3.2/src/cleanvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:23:13.913138 cleanvision-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_duplicate_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_image_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_image_property_issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-17 03:23:02.000000 cleanvision-0.3.2/tests/test_viz_manager.py
```

### Comparing `cleanvision-0.3.1/CODE_OF_CONDUCT.md` & `cleanvision-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/CONTRIBUTING.md` & `cleanvision-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/DEVELOPMENT.md` & `cleanvision-0.3.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/LICENSE` & `cleanvision-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/PKG-INFO` & `cleanvision-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.3.1
+Version: 0.3.2
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -787,14 +787,16 @@
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
 
 * The best place to learn is [our Slack community](https://cleanlab.ai/slack). Join the discussion there to see how
   folks are using this library, discuss upcoming features, or ask for private support.
 
+* Need professional help with CleanVision?  Join our [\#help Slack channel](https://cleanlab.ai/slack) and message us there, or reach out via email: team@cleanlab.ai
+
 * Interested in contributing? See the [contributing guide](CONTRIBUTING.md). An easy starting point is to
   consider [issues](https://github.com/cleanlab/cleanvision/labels/good%20first%20issue) marked `good first issue` or
   simply reach out in [Slack](https://cleanlab.ai/slack). We welcome your help building a standard open-source library
   for data-centric computer vision!
 
 * Ready to start adding your own code? See the [development guide](DEVELOPMENT.md).
```

### Comparing `cleanvision-0.3.1/README.md` & `cleanvision-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
 
 * The best place to learn is [our Slack community](https://cleanlab.ai/slack). Join the discussion there to see how
   folks are using this library, discuss upcoming features, or ask for private support.
 
+* Need professional help with CleanVision?  Join our [\#help Slack channel](https://cleanlab.ai/slack) and message us there, or reach out via email: team@cleanlab.ai
+
 * Interested in contributing? See the [contributing guide](CONTRIBUTING.md). An easy starting point is to
   consider [issues](https://github.com/cleanlab/cleanvision/labels/good%20first%20issue) marked `good first issue` or
   simply reach out in [Slack](https://cleanlab.ai/slack). We welcome your help building a standard open-source library
   for data-centric computer vision!
 
 * Ready to start adding your own code? See the [development guide](DEVELOPMENT.md).
```

### Comparing `cleanvision-0.3.1/pyproject.toml` & `cleanvision-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cleanvision"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     { name = "Cleanlab Inc.", email = "team@cleanlab.ai" },
 ]
 description = "Find issues in image datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["computer_vision", "cv", "image_data", "issue_detection", "data_quality", "image_quality", "machine_learning", "data_cleaning", "image_deduplication"]
```

### Comparing `cleanvision-0.3.1/src/cleanvision/dataset/base_dataset.py` & `cleanvision-0.3.2/src/cleanvision/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/dataset/folder_dataset.py` & `cleanvision-0.3.2/src/cleanvision/dataset/folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/dataset/hf_dataset.py` & `cleanvision-0.3.2/src/cleanvision/dataset/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/dataset/torch_dataset.py` & `cleanvision-0.3.2/src/cleanvision/dataset/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/dataset/utils.py` & `cleanvision-0.3.2/src/cleanvision/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/imagelab.py` & `cleanvision-0.3.2/src/cleanvision/imagelab.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,15 @@
     def report(
         self,
         issue_types: Optional[List[str]] = None,
         max_prevalence: Optional[float] = None,
         num_images: Optional[int] = None,
         verbosity: int = 1,
         print_summary: bool = True,
+        show_id: bool = False,
     ) -> None:
         """Prints summary of the issues found in your dataset.
         By default, this method depicts the images representing top-most severe instances of each issue type.
 
         Parameters
         ----------
         issue_types : List[str], optional
@@ -387,14 +388,17 @@
 
         verbosity : int, {1, 2, 3, 4}
             Increasing verbosity increases the detail of the report. Set this to 1 to report less information, or to 4 to report the most information.
 
         print_summary : bool, default=True
             If True, prints the summary of issues found in the dataset.
 
+        show_id: bool, default=False
+            If True, prints the dataset ID of each image shown in the report.
+
         Examples
         --------
         Default usage
 
         .. code-block:: python
 
             imagelab.report()
@@ -442,14 +446,15 @@
                     f"Number of examples with this issue: {self.issues[get_is_issue_colname(issue_type)].sum()}\n"
                     f"Examples representing most severe instances of this issue:\n"
                 )
                 self._visualize(
                     issue_type,
                     report_args["num_images"],
                     report_args["cell_size"],
+                    show_id,
                 )
         else:
             print(
                 "Please specify some issue_types to check for in imagelab.find_issues()."
             )
 
     def _pprint_issue_summary(self, issue_summary: pd.DataFrame) -> None:
@@ -467,75 +472,76 @@
             return self._issue_managers[issue_type_str]
 
     def _visualize(
         self,
         issue_type: str,
         num_images: int,
         cell_size: Tuple[int, int],
+        show_id: bool,
     ) -> None:
         # todo: remove dependency on issue manager
         issue_manager = self._get_issue_manager(issue_type)
         viz_name = issue_manager.visualization
 
         if viz_name == "individual_images":
             sorted_df = self.issues.sort_values(by=get_score_colname(issue_type))
             sorted_df = sorted_df[sorted_df[get_is_issue_colname(issue_type)] == 1]
 
             scores = sorted_df.head(num_images)[get_score_colname(issue_type)]
             indices = scores.index.tolist()
             images = [self._dataset[i] for i in indices]
 
-            titles = [f"score : {x:.4f}" for x in scores]
-
-            # Add size information for odd sized images
-            additional_info = None
+            # construct title info
+            title_info = {"scores": [f"score : {x:.4f}" for x in scores]}
+            if show_id:
+                title_info["ids"] = [f"id : {i}" for i in indices]
             if issue_type == IssueType.ODD_SIZE.value:
-                additional_info = []
-                for image in images:
-                    additional_info.append(f"original size: {image.size}")
+                title_info["size"] = [
+                    f"original size: {image.size}" for image in images
+                ]
 
             if images:
                 VizManager.individual_images(
                     images=images,
-                    titles=titles,
+                    title_info=title_info,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
-                    additional_info=additional_info,
                 )
 
         elif viz_name == "image_sets":
             image_sets_indices = sorted(
                 self.info[issue_type][SETS], key=len, reverse=True
             )
             image_sets_indices = image_sets_indices[:num_images]
             image_sets = []
             for indices in image_sets_indices:
                 image_sets.append([self._dataset[index] for index in indices])
 
-            title_sets = [
-                [self._dataset.get_name(index) for index in s]
-                for s in image_sets_indices
-            ]
+            title_info_sets = []
+            for s in image_sets_indices:
+                title_info = {"name": [self._dataset.get_name(index) for index in s]}
+                title_info_sets.append(title_info)
 
             if image_sets:
                 VizManager.image_sets(
                     image_sets,
-                    title_sets,
+                    title_info_sets,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
     # todo: compress this code
     def visualize(
         self,
         image_files: Optional[List[str]] = None,
         indices: Optional[List[str | int]] = None,
         issue_types: Optional[List[str]] = None,
         num_images: int = 4,
         cell_size: Tuple[int, int] = (2, 2),
+        show_id: bool = False,
     ) -> None:
         """Show specific images.
 
         Can be used for visualizing either:
         1. Particular images with paths given in `image_files`.
         2. Images representing top-most severe instances of given `issue_types` detected the dataset.
         3. If no `image_files` or `issue_types` are given, random images will be shown from the dataset.
@@ -595,47 +601,49 @@
             imagelab.visualize(issue_types=issue_types)
 
         """
         if issue_types is not None:
             if len(issue_types) == 0:
                 raise ValueError("issue_types list is empty")
             for issue_type in issue_types:
-                self._visualize(issue_type, num_images, cell_size)
+                self._visualize(issue_type, num_images, cell_size, show_id)
         elif image_files is not None:
             if len(image_files) == 0:
                 raise ValueError("image_files list is empty.")
             images = [Image.open(path) for path in image_files]
-            titles = [path.split("/")[-1] for path in image_files]
+            title_info = {"path": [path.split("/")[-1] for path in image_files]}
             VizManager.individual_images(
                 images,
-                titles,
+                title_info,
                 ncols=self._config["visualize_num_images_per_row"],
                 cell_size=cell_size,
             )
         elif indices:
             images = [self._dataset[i] for i in indices]
-            titles = [self._dataset.get_name(i) for i in indices]
+            title_info = {"name": [self._dataset.get_name(i) for i in indices]}
             VizManager.individual_images(
                 images,
-                titles,
+                title_info,
                 ncols=self._config["visualize_num_images_per_row"],
                 cell_size=cell_size,
             )
         else:
             print("Sample images from the dataset")
 
             if image_files is None:
                 image_indices = random.sample(
                     self._dataset.index, min(num_images, len(self._dataset))
                 )
                 images = [self._dataset[i] for i in image_indices]
-                titles = [self._dataset.get_name(i) for i in image_indices]
+                title_info = {
+                    "name": [self._dataset.get_name(i) for i in image_indices]
+                }
                 VizManager.individual_images(
                     images,
-                    titles,
+                    title_info,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
     # Todo: Improve mypy dict typechecking so this does not return any
     def get_stats(self) -> Any:
         """Returns dict of statistics computed from images when auditing the data such as: brightness, color space, aspect ratio, etc.
```

### Comparing `cleanvision-0.3.1/src/cleanvision/issue_managers/__init__.py` & `cleanvision-0.3.2/src/cleanvision/issue_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/issue_managers/duplicate_issue_manager.py` & `cleanvision-0.3.2/src/cleanvision/issue_managers/duplicate_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/issue_managers/image_property.py` & `cleanvision-0.3.2/src/cleanvision/issue_managers/image_property.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/issue_managers/image_property_issue_manager.py` & `cleanvision-0.3.2/src/cleanvision/issue_managers/image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/utils/base_issue_manager.py` & `cleanvision-0.3.2/src/cleanvision/utils/base_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/utils/constants.py` & `cleanvision-0.3.2/src/cleanvision/utils/constants.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/utils/serialize.py` & `cleanvision-0.3.2/src/cleanvision/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/utils/utils.py` & `cleanvision-0.3.2/src/cleanvision/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/src/cleanvision/utils/viz_manager.py` & `cleanvision-0.3.2/src/cleanvision/utils/viz_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,106 @@
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Dict
 
 import math
 import matplotlib.axes
 import matplotlib.pyplot as plt
 from PIL import Image
 
 
 class VizManager:
     @staticmethod
     def individual_images(
         images: List[Image.Image],
-        titles: List[str],
+        title_info: Dict[str, List[str]],
         ncols: int,
         cell_size: Tuple[int, int],
-        additional_info: Optional[List[str]] = None,
     ) -> None:
         """Plots a list of images in a grid."""
-        plot_image_grid(images, titles, ncols, cell_size, additional_info)
+        plot_image_grid(images, title_info, ncols, cell_size)
 
     @staticmethod
     def image_sets(
         image_sets: List[List[Image.Image]],
-        title_sets: List[List[str]],
+        title_info_sets: List[Dict[str, List[str]]],
         ncols: int,
         cell_size: Tuple[int, int],
     ) -> None:
         for i, s in enumerate(image_sets):
             print(f"Set: {i}")
-            plot_image_grid(s, title_sets[i], ncols, cell_size)
+            plot_image_grid(s, title_info_sets[i], ncols, cell_size)
 
 
 def set_image_on_axes(image: Image.Image, ax: matplotlib.axes.Axes, title: str) -> None:
     cmap = "gray" if image.mode == "L" else None
     ax.get_xaxis().set_visible(False)
     ax.get_yaxis().set_visible(False)
     ax.set_title(title, fontsize=7)
     ax.imshow(image, cmap=cmap, vmin=0, vmax=255)
 
 
+def truncate_titles(cell_width: int, titles: List[str]) -> List[str]:
+    """Converts font size of 7 into inches"""
+    CHARACTER_SIZE_INCHES = 7 * (1 / 72)
+
+    chars_allowed = math.ceil(cell_width / CHARACTER_SIZE_INCHES) - 4
+
+    k1 = 1
+    while k1 <= chars_allowed and titles[0][:k1] == titles[1][:k1]:
+        k1 += 1
+    k2 = 1
+    while (
+        k2 <= chars_allowed
+        and titles[0][(len(titles[0]) - k2) :] == titles[1][(len(titles[1]) - k2) :]
+    ):
+        k2 += 1
+
+    if k1 > k2:
+        truncate_from_front = True
+    else:
+        truncate_from_front = False
+
+    for i in range(len(titles)):
+        title_width = len(titles[i]) * CHARACTER_SIZE_INCHES
+        if title_width >= cell_width:
+            titles[i] = (
+                ("..." + titles[i][len(titles[i]) - chars_allowed :])
+                if truncate_from_front
+                else (titles[i][:chars_allowed] + "...")
+            )
+    return titles
+
+
+def construct_titles(title_info: Dict[str, List[str]], cell_width: int) -> List[str]:
+    keys = list(title_info.keys())
+    nimages = len(title_info[keys[0]])
+
+    # truncate longer lines
+    if nimages > 1:
+        for key in keys:
+            title_info[key] = truncate_titles(cell_width, title_info[key])
+
+    # join all keys
+    titles = []
+    for i in range(nimages):
+        titles.append("\n".join(title_info[key][i] for key in keys))
+    return titles
+
+
 def plot_image_grid(
     images: List[Image.Image],
-    titles: List[str],
+    title_info: Dict[str, List[str]],
     ncols: int,
     cell_size: Tuple[int, int],
-    additional_info: Optional[List[str]] = None,
 ) -> None:
     nrows = math.ceil(len(images) / ncols)
     ncols = min(ncols, len(images))
     fig, axes = plt.subplots(
         nrows, ncols, figsize=(cell_size[0] * ncols, cell_size[1] * nrows)
     )
-
-    """Converts font size of 7 into inches"""
-    CHARACTER_SIZE_INCHES = 7 * (1 / 72)
-
-    chars_allowed = math.ceil(cell_size[0] / CHARACTER_SIZE_INCHES) - 4
-
-    if len(images) > 1:
-        k1 = 1
-        while k1 <= chars_allowed and titles[0][:k1] == titles[1][:k1]:
-            k1 += 1
-        k2 = 1
-        while (
-            k2 <= chars_allowed
-            and titles[0][(len(titles[0]) - k2) :] == titles[1][(len(titles[1]) - k2) :]
-        ):
-            k2 += 1
-
-        if k1 > k2:
-            truncate_from_front = True
-        else:
-            truncate_from_front = False
-
-        for i in range(len(images)):
-            title_width = len(titles[i]) * CHARACTER_SIZE_INCHES
-            if title_width >= cell_size[0]:
-                titles[i] = (
-                    ("..." + titles[i][len(titles[i]) - chars_allowed :])
-                    if truncate_from_front
-                    else (titles[i][:chars_allowed] + "...")
-                )
-    if additional_info is not None:
-        for i in range(len(images)):
-            titles[i] = f"{titles[i]}\n{additional_info[i]}"
+    titles = construct_titles(title_info, cell_size[0])
     if nrows > 1:
         idx = 0
         for i in range(nrows):
             for j in range(ncols):
                 idx = i * ncols + j
                 if idx >= len(images):
                     axes[i, j].axis("off")
```

### Comparing `cleanvision-0.3.1/src/cleanvision.egg-info/PKG-INFO` & `cleanvision-0.3.2/src/cleanvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.3.1
+Version: 0.3.2
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -787,14 +787,16 @@
 CleanVision supports Linux, macOS, and Windows and runs on Python 3.7+.
 
 ## Join our community
 
 * The best place to learn is [our Slack community](https://cleanlab.ai/slack). Join the discussion there to see how
   folks are using this library, discuss upcoming features, or ask for private support.
 
+* Need professional help with CleanVision?  Join our [\#help Slack channel](https://cleanlab.ai/slack) and message us there, or reach out via email: team@cleanlab.ai
+
 * Interested in contributing? See the [contributing guide](CONTRIBUTING.md). An easy starting point is to
   consider [issues](https://github.com/cleanlab/cleanvision/labels/good%20first%20issue) marked `good first issue` or
   simply reach out in [Slack](https://cleanlab.ai/slack). We welcome your help building a standard open-source library
   for data-centric computer vision!
 
 * Ready to start adding your own code? See the [development guide](DEVELOPMENT.md).
```

### Comparing `cleanvision-0.3.1/src/cleanvision.egg-info/SOURCES.txt` & `cleanvision-0.3.2/src/cleanvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_dataset.py` & `cleanvision-0.3.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_duplicate_issue_manager.py` & `cleanvision-0.3.2/tests/test_duplicate_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_image_property_helpers.py` & `cleanvision-0.3.2/tests/test_image_property_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_image_property_issue_manager.py` & `cleanvision-0.3.2/tests/test_image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_run.py` & `cleanvision-0.3.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_save_load.py` & `cleanvision-0.3.2/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_utils.py` & `cleanvision-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_visualize.py` & `cleanvision-0.3.2/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.3.1/tests/test_viz_manager.py` & `cleanvision-0.3.2/tests/test_viz_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 from cleanvision.utils.viz_manager import VizManager
 
 
 class TestVizManager:
     @pytest.mark.usefixtures("set_plt_show")
     @pytest.mark.parametrize(
-        ("images", "titles"),
+        ("images", "title_info"),
         [
-            ([Image.new("L", (100, 100))], ["image_title"]),
-            ([Image.new("L", (100, 100))] * 2, ["image_title"] * 4),
-            ([Image.new("L", (100, 100))] * 6, ["imaxge_title"] * 6),
+            ([Image.new("L", (100, 100))], {"name": ["image_title"]}),
+            ([Image.new("L", (100, 100))] * 2, {"name": ["image_title"] * 4}),
+            ([Image.new("L", (100, 100))] * 6, {"name": ["imaxge_title"] * 6}),
         ],
         ids=["plot single image", "plot <=4 images", "plt > 4 images"],
     )
-    def test_individual_images(self, images, titles):
-        VizManager.individual_images(images, titles, 4, (2, 2))
+    def test_individual_images(self, images, title_info):
+        VizManager.individual_images(images, title_info, 4, (2, 2))
 
     @pytest.mark.usefixtures("set_plt_show")
     @pytest.mark.parametrize(
-        ("image_sets", "title_sets"),
+        ("image_sets", "title_info_sets"),
         [
             (
                 [[Image.new("L", (100, 100))], [Image.new("L", (100, 100))] * 2],
-                [["image_title"], ["image_title"] * 2],
+                [{"name": ["image_title"]}, {"name": ["image_title"] * 2}],
             ),
         ],
     )
-    def test_image_sets(self, image_sets, title_sets):
-        VizManager.image_sets(image_sets, title_sets, 4, (2, 2))
+    def test_image_sets(self, image_sets, title_info_sets):
+        VizManager.image_sets(image_sets, title_info_sets, 4, (2, 2))
```

