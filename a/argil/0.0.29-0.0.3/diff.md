# Comparing `tmp/argil-0.0.29.tar.gz` & `tmp/argil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.29.tar", last modified: Mon Jul 17 05:49:30 2023, max compression
+gzip compressed data, was "argil-0.0.3.tar", last modified: Mon Jul 17 06:32:42 2023, max compression
```

## Comparing `argil-0.0.29.tar` & `argil-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:49:30.895614 argil-0.0.29/
--rw-rw-r--   0 charles   (1000) charles   (1000)    34600 2023-07-05 16:58:03.000000 argil-0.0.29/LICENCE.md
--rw-rw-r--   0 charles   (1000) charles   (1000)       26 2023-07-17 05:18:04.000000 argil-0.0.29/MANIFEST.in
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:49:30.895614 argil-0.0.29/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      655 2023-07-05 16:40:12.000000 argil-0.0.29/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:49:30.895614 argil-0.0.29/argil/
--rw-rw-r--   0 charles   (1000) charles   (1000)      251 2023-07-05 16:40:12.000000 argil-0.0.29/argil/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)       39 2023-07-17 05:48:49.000000 argil-0.0.29/argil/config.json
--rw-rw-r--   0 charles   (1000) charles   (1000)      197 2023-07-17 05:06:16.000000 argil-0.0.29/argil/types.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      792 2023-07-17 05:28:04.000000 argil-0.0.29/argil/workflowRuns.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      646 2023-07-17 05:28:00.000000 argil-0.0.29/argil/workflows.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 05:49:30.895614 argil-0.0.29/argil.egg-info/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1255 2023-07-17 05:49:30.000000 argil-0.0.29/argil.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      277 2023-07-17 05:49:30.000000 argil-0.0.29/argil.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 05:49:30.000000 argil-0.0.29/argil.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        9 2023-07-17 05:49:30.000000 argil-0.0.29/argil.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        6 2023-07-17 05:49:30.000000 argil-0.0.29/argil.egg-info/top_level.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-07-17 05:49:30.895614 argil-0.0.29/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)     1197 2023-07-17 05:49:06.000000 argil-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:32:42.101669 argil-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-07-17 06:32:30.000000 argil-0.0.3/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 06:32:30.000000 argil-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-17 06:32:42.101669 argil-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 06:32:30.000000 argil-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:32:42.097669 argil-0.0.3/argil/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 06:32:30.000000 argil-0.0.3/argil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 06:32:30.000000 argil-0.0.3/argil/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 06:32:30.000000 argil-0.0.3/argil/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-17 06:32:30.000000 argil-0.0.3/argil/workflowRuns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-17 06:32:30.000000 argil-0.0.3/argil/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:32:42.101669 argil-0.0.3/argil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-17 06:32:42.000000 argil-0.0.3/argil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 06:32:42.000000 argil-0.0.3/argil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:32:42.000000 argil-0.0.3/argil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 06:32:42.000000 argil-0.0.3/argil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:32:42.000000 argil-0.0.3/argil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:32:42.101669 argil-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-17 06:32:41.000000 argil-0.0.3/setup.py
```

### Comparing `argil-0.0.29/LICENCE.md` & `argil-0.0.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.29/PKG-INFO` & `argil-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.29
+Version: 0.0.3
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.29/README.md` & `argil-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `argil-0.0.29/argil/workflowRuns.py` & `argil-0.0.3/argil/workflowRuns.py`

 * *Files identical despite different names*

### Comparing `argil-0.0.29/argil/workflows.py` & `argil-0.0.3/argil/workflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 
 class Workflows:
     def __init__(self, apiKey: str) -> None:
         self.headers: Dict[str, str] = {'authorization': f'Bearer {apiKey}'}
         config = json.loads(resource_string(__name__, 'config.json').decode('utf-8'))
         self.apiUrl: str = config['apiUrl']
 
+    # Run a workflow providing its id and input
     def run(self, id: str, input: Dict[str, Any]) -> WorkflowRun:
         response = requests.post(f'{self.apiUrl}/runWorkflow', json={'id': id, 'input': input}, headers=self.headers)
         response.raise_for_status()
         return response.json()
```

### Comparing `argil-0.0.29/argil.egg-info/PKG-INFO` & `argil-0.0.3/argil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argil
-Version: 0.0.29
+Version: 0.0.3
 Summary: SDK for the Argil API
 Home-page: https://github.com/argildotai/argil-sdk-python
 Author: Brivael Le Pogam
 Author-email: briva@argil.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `argil-0.0.29/setup.py` & `argil-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='argil',
-    version='0.0.29',#'{{VERSION_PLACEHOLDER}}',
+    version='0.0.3',
     author="Brivael Le Pogam",
     author_email="briva@argil.ai",
     description='SDK for the Argil API',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/argildotai/argil-sdk-python',
     packages=find_packages(),
```

