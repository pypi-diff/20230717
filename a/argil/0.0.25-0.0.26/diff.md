# Comparing `tmp/argil-0.0.25.tar.gz` & `tmp/argil-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.25.tar", last modified: Mon Jul 17 05:14:04 2023, max compression
+gzip compressed data, was "argil-0.0.26.tar", last modified: Mon Jul 17 05:22:01 2023, max compression
```

## Comparing `argil-0.0.25.tar` & `argil-0.0.26.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:14:04.034493 argil-0.0.25/
--rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.25/LICENCE.md
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:14:04.034493 argil-0.0.25/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.25/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:14:04.034493 argil-0.0.25/argil/
--rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.25/argil/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.25/argil/types.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      957 2023-07-17 05:13:40.000000 argil-0.0.25/argil/workflowRuns.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      693 2023-07-17 05:13:58.000000 argil-0.0.25/argil/workflows.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:14:04.034493 argil-0.0.25/argil.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:14:03.000000 argil-0.0.25/argil.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      247 2023-07-17 05:14:04.000000 argil-0.0.25/argil.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:14:03.000000 argil-0.0.25/argil.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:14:03.000000 argil-0.0.25/argil.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:14:03.000000 argil-0.0.25/argil.egg-info/top_level.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:14:04.034493 argil-0.0.25/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1166 2023-07-17 05:11:56.000000 argil-0.0.25/setup.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:22:01.167317 argil-0.0.26/
+-rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.26/LICENCE.md
+-rw-rw-r--   0 charles   (1000) charles   (1000)       26 2023-07-17 05:18:04.000000 argil-0.0.26/MANIFEST.in
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:22:01.167317 argil-0.0.26/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.26/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:22:01.167317 argil-0.0.26/argil/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.26/argil/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-05 17:08:31.000000 argil-0.0.26/argil/config.json
+-rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.26/argil/types.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      894 2023-07-17 05:21:38.000000 argil-0.0.26/argil/workflowRuns.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      630 2023-07-17 05:20:57.000000 argil-0.0.26/argil/workflows.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:22:01.167317 argil-0.0.26/argil.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:22:01.000000 argil-0.0.26/argil.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      277 2023-07-17 05:22:01.000000 argil-0.0.26/argil.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:22:01.000000 argil-0.0.26/argil.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:22:01.000000 argil-0.0.26/argil.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:22:01.000000 argil-0.0.26/argil.egg-info/top_level.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:22:01.167317 argil-0.0.26/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1197 2023-07-17 05:21:51.000000 argil-0.0.26/setup.py
```

### Comparing `argil-0.0.25/LICENCE.md` & `argil-0.0.26/LICENCE.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.25/PKG-INFO` & `argil-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.25
+Version: 0.0.26
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.25/README.md` & `argil-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.25/argil/workflowRuns.py` & `argil-0.0.26/argil/workflowRuns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import requests, os, json
+import requests, json
 from typing import List
 from .types import WorkflowRun
-
-config_file_path = os.path.join(os.path.dirname(__file__), 'config.json')
+from pkg_resources import resource_string
 
 class WorkflowRuns:
     def __init__(self, apiKey: str) -> None:
         self.headers: Dict[str, str] = {'authorization': f'Bearer {apiKey}'}
-        with open(config_file_path) as config_file:
-            config = json.load(config_file)
+        config = json.loads(resource_string(__name__, 'config.json'))
         self.apiUrl: str = config['apiUrl']
 
         response = requests.post(f'{self.apiUrl}/runWorkflow', json={'id': id, 'input': input}, headers=self.headers)
     def list(self) -> List[WorkflowRun]:
         response = requests.get(f'{self.apiUrl}/getWorkflowRuns', headers=self.headers)
         response.raise_for_status()
         return response.json()
```

### Comparing `argil-0.0.25/argil.egg-info/PKG-INFO` & `argil-0.0.26/argil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.25
+Version: 0.0.26
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.25/setup.py` & `argil-0.0.26/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='argil',
-    version='0.0.25',#'{{VERSION_PLACEHOLDER}}',
+    version='0.0.26',#'{{VERSION_PLACEHOLDER}}',
     author="Brivael Le Pogam",
     author_email="briva@argil.ai",
     description='SDK for the Argil API',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/argildotai/argil-sdk-python',
     packages=find_packages(),
@@ -24,14 +24,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'requests',
     ],
+    include_package_data=True,
     package_data={
         'argil': ['config.json'],
     },
     # package_dir = {"": "src"},
     # packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.8"
 )
```

