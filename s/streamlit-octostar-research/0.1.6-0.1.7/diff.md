# Comparing `tmp/streamlit-octostar-research-0.1.6.tar.gz` & `tmp/streamlit-octostar-research-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-octostar-research-0.1.6.tar", last modified: Fri May 19 17:35:38 2023, max compression
+gzip compressed data, was "streamlit-octostar-research-0.1.7.tar", last modified: Mon Jul 17 10:54:53 2023, max compression
```

## Comparing `streamlit-octostar-research-0.1.6.tar` & `streamlit-octostar-research-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/desktop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/octostar-research-client.js
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/octostar-research.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/streamlit-component-lib.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/ontology/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-19 17:35:26.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:38.302506 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 17:35:38.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-19 17:35:38.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:35:38.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 17:35:38.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 17:35:38.000000 streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/desktop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/octostar-research-client.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/octostar-research.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/streamlit-component-lib.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-17 10:54:43.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:54:53.951702 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-17 10:54:53.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 10:54:53.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:54:53.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 10:54:53.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 10:54:53.000000 streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/top_level.txt
```

### Comparing `streamlit-octostar-research-0.1.6/LICENSE` & `streamlit-octostar-research-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/setup.py` & `streamlit-octostar-research-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-octostar-research",
-    version="0.1.6",
+    version="0.1.7",
     author="Octostar Research",
     author_email="developer@octostarresearch.com",
     description="Streamlit component that connects to the Octostar Research App",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/desktop/__init__.py` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/desktop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,7 +142,14 @@
 
 def set_open_workspace_ids(ids): 
     component_value = _component_func(
         call='octostar:desktop:setOpenWorkspaceIds',
         args=[ids]
     )
     return component_value
+
+def get_context(): 
+    component_value = _component_func(
+        subscribe='octostar:remoteapp:context',
+        args=[]
+    )
+    return component_value
```

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/extras/__init__.py` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/main.js` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/octostar-research-client.js` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/octostar-research-client.js`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/octostar-research.js` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/octostar-research.js`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/frontend/streamlit-component-lib.js` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research/ontology/__init__.py` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research/ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-octostar-research-0.1.6/src/streamlit_octostar_research.egg-info/SOURCES.txt` & `streamlit-octostar-research-0.1.7/src/streamlit_octostar_research.egg-info/SOURCES.txt`

 * *Files identical despite different names*

