# Comparing `tmp/azure_speech_tools-0.0.1.tar.gz` & `tmp/azure_speech_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_speech_tools-0.0.1.tar", last modified: Mon Jul 17 14:29:15 2023, max compression
+gzip compressed data, was "azure_speech_tools-0.0.2.tar", last modified: Mon Jul 17 14:47:15 2023, max compression
```

## Comparing `azure_speech_tools-0.0.1.tar` & `azure_speech_tools-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.1/MANIFEST.in
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/PKG-INFO
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/azure_speech_tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.1/azure_speech_tools/__init__.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/azure_speech_tools/tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.1/azure_speech_tools/tools/__init__.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.1/azure_speech_tools/tools/azure_speech_tts.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      503 2023-07-17 10:04:13.000000 azure_speech_tools-0.0.1/azure_speech_tools/tools/utils.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/azure_speech_tools/yamls/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      601 2023-07-17 14:17:18.000000 azure_speech_tools-0.0.1/azure_speech_tools/yamls/azure_speech_tts.yaml
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/PKG-INFO
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      468 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/entry_points.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       90 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/requires.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-17 14:29:15.000000 azure_speech_tools-0.0.1/azure_speech_tools.egg-info/top_level.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-17 14:29:15.265032 azure_speech_tools-0.0.1/setup.cfg
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      579 2023-07-17 13:42:10.000000 azure_speech_tools-0.0.1/setup.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.2/MANIFEST.in
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/PKG-INFO
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.2/azure_speech_tools/__init__.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/__init__.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/azure_speech_tts.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      503 2023-07-17 10:04:13.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/utils.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/yamls/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      601 2023-07-17 14:17:18.000000 azure_speech_tools-0.0.2/azure_speech_tools/yamls/azure_speech_tts.yaml
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      468 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       65 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/requires.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/top_level.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/setup.cfg
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      543 2023-07-17 14:46:41.000000 azure_speech_tools-0.0.2/setup.py
```

### Comparing `azure_speech_tools-0.0.1/azure_speech_tools/tools/azure_speech_tts.py` & `azure_speech_tools-0.0.2/azure_speech_tools/tools/azure_speech_tts.py`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.1/azure_speech_tools/yamls/azure_speech_tts.yaml` & `azure_speech_tools-0.0.2/azure_speech_tools/yamls/azure_speech_tts.yaml`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.1/setup.py` & `azure_speech_tools-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name="azure_speech_tools",
-    version="0.0.1",
+    version="0.0.2",
     description="This is the Azure Speech Services tools package",
     packages=find_packages(),
     install_requires=[
-        "promptflow-sdk[builtins]",
         "azure-cognitiveservices-speech",
         "azure-storage-blob",
         "azure-identity",
     ],
     entry_points={
         "package_tools": ["my_tools = azure_speech_tools.tools.utils:list_package_tools"],
     },
```

