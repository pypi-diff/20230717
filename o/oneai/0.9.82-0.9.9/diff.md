# Comparing `tmp/oneai-0.9.82.tar.gz` & `tmp/oneai-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneai-0.9.82.tar", last modified: Mon Jul 17 11:23:39 2023, max compression
+gzip compressed data, was "oneai-0.9.9.tar", last modified: Sun Jan 22 19:40:56 2023, max compression
```

## Comparing `oneai-0.9.82.tar` & `oneai-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,29 @@
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.226735 oneai-0.9.82/
--rw-r--r--   0 michaelgur   (501) staff       (20)     1084 2022-07-27 08:48:35.000000 oneai-0.9.82/LICENSE
--rw-r--r--   0 michaelgur   (501) staff       (20)     9131 2023-07-17 11:23:39.226832 oneai-0.9.82/PKG-INFO
--rw-r--r--   0 michaelgur   (501) staff       (20)     8694 2023-04-02 13:51:49.000000 oneai-0.9.82/README.md
--rw-r--r--   0 michaelgur   (501) staff       (20)      104 2022-07-27 08:49:02.000000 oneai-0.9.82/pyproject.toml
--rw-r--r--   0 michaelgur   (501) staff       (20)      824 2023-07-17 11:23:39.227266 oneai-0.9.82/setup.cfg
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.217590 oneai-0.9.82/src/
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.221954 oneai-0.9.82/src/oneai/
--rw-r--r--   0 michaelgur   (501) staff       (20)     1437 2023-07-17 11:19:30.000000 oneai-0.9.82/src/oneai/__init__.py
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.224152 oneai-0.9.82/src/oneai/api/
--rw-r--r--   0 michaelgur   (501) staff       (20)      438 2022-12-18 06:49:48.000000 oneai-0.9.82/src/oneai/api/__init__.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3568 2023-06-12 08:54:42.000000 oneai-0.9.82/src/oneai/api/clustering.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3360 2023-05-29 09:44:44.000000 oneai-0.9.82/src/oneai/api/output.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     5004 2023-05-29 09:43:06.000000 oneai-0.9.82/src/oneai/api/pipeline.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    14322 2023-06-20 11:39:50.000000 oneai-0.9.82/src/oneai/classes.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    10036 2023-06-12 08:55:24.000000 oneai-0.9.82/src/oneai/clustering.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     2583 2022-09-22 14:06:15.000000 oneai-0.9.82/src/oneai/exceptions.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     1008 2022-12-29 11:56:46.000000 oneai-0.9.82/src/oneai/logger.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3913 2023-05-29 10:14:02.000000 oneai-0.9.82/src/oneai/output.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     6996 2022-12-18 07:31:42.000000 oneai-0.9.82/src/oneai/parsing.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    10037 2023-05-29 10:16:02.000000 oneai-0.9.82/src/oneai/pipeline.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     8320 2023-06-20 11:39:50.000000 oneai-0.9.82/src/oneai/process_scheduler.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    19626 2023-07-17 11:22:29.000000 oneai-0.9.82/src/oneai/skills.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     1666 2023-04-10 16:16:55.000000 oneai-0.9.82/src/oneai/util.py
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.222931 oneai-0.9.82/src/oneai.egg-info/
--rwxrwxrwx   0 michaelgur   (501) staff       (20)     9131 2023-07-17 11:23:39.000000 oneai-0.9.82/src/oneai.egg-info/PKG-INFO
--rwxrwxrwx   0 michaelgur   (501) staff       (20)      684 2023-07-17 11:23:39.000000 oneai-0.9.82/src/oneai.egg-info/SOURCES.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)        1 2023-07-17 11:23:39.000000 oneai-0.9.82/src/oneai.egg-info/dependency_links.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)      192 2023-07-17 11:23:39.000000 oneai-0.9.82/src/oneai.egg-info/requires.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)        6 2023-07-17 11:23:39.000000 oneai-0.9.82/src/oneai.egg-info/top_level.txt
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-07-17 11:23:39.226407 oneai-0.9.82/tests/
--rw-r--r--   0 michaelgur   (501) staff       (20)     2258 2023-05-16 07:53:45.000000 oneai-0.9.82/tests/test_clustering.py
--rw-r--r--   0 michaelgur   (501) staff       (20)      611 2023-04-02 12:45:22.000000 oneai-0.9.82/tests/test_errors.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3105 2023-05-25 16:36:48.000000 oneai-0.9.82/tests/test_files.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     1232 2023-03-31 07:44:45.000000 oneai-0.9.82/tests/test_parsing.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     5599 2023-05-29 10:16:17.000000 oneai-0.9.82/tests/test_pipeline.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     2419 2023-05-03 10:53:39.000000 oneai-0.9.82/tests/test_skill.py
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.389530 oneai-0.9.9/
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1084 2022-07-27 08:48:35.000000 oneai-0.9.9/LICENSE
+-rw-r--r--   0 michaelgur   (501) staff       (20)     7579 2023-01-22 19:40:56.389616 oneai-0.9.9/PKG-INFO
+-rw-r--r--   0 michaelgur   (501) staff       (20)     7167 2022-08-27 22:48:27.000000 oneai-0.9.9/README.md
+-rw-r--r--   0 michaelgur   (501) staff       (20)      104 2022-07-27 08:49:02.000000 oneai-0.9.9/pyproject.toml
+-rw-r--r--   0 michaelgur   (501) staff       (20)      700 2023-01-22 19:40:56.389949 oneai-0.9.9/setup.cfg
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.378584 oneai-0.9.9/src/
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.382346 oneai-0.9.9/src/oneai/
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1325 2023-01-22 18:04:09.000000 oneai-0.9.9/src/oneai/__init__.py
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.389217 oneai-0.9.9/src/oneai/api/
+-rw-r--r--   0 michaelgur   (501) staff       (20)      438 2022-12-18 06:49:48.000000 oneai-0.9.9/src/oneai/api/__init__.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     3052 2022-12-18 06:49:48.000000 oneai-0.9.9/src/oneai/api/clustering.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     2914 2022-11-14 20:26:11.000000 oneai-0.9.9/src/oneai/api/output.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     3660 2023-01-02 10:24:42.000000 oneai-0.9.9/src/oneai/api/pipeline.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)    14098 2023-01-22 19:39:04.000000 oneai-0.9.9/src/oneai/classes.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6827 2023-01-03 13:45:25.000000 oneai-0.9.9/src/oneai/clustering.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     2583 2022-09-22 14:06:15.000000 oneai-0.9.9/src/oneai/exceptions.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1008 2022-12-29 11:56:46.000000 oneai-0.9.9/src/oneai/logger.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6996 2022-12-18 07:31:42.000000 oneai-0.9.9/src/oneai/parsing.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     9261 2023-01-22 19:37:16.000000 oneai-0.9.9/src/oneai/pipeline.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6499 2023-01-22 19:32:24.000000 oneai-0.9.9/src/oneai/process_scheduler.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)    20437 2023-01-19 13:40:49.000000 oneai-0.9.9/src/oneai/skills.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1522 2023-01-22 19:39:34.000000 oneai-0.9.9/src/oneai/util.py
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.383421 oneai-0.9.9/src/oneai.egg-info/
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)     7579 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/PKG-INFO
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)      533 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/SOURCES.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)        1 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/dependency_links.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)      101 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/requires.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)        6 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/top_level.txt
```

### Comparing `oneai-0.9.82/LICENSE` & `oneai-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oneai-0.9.82/PKG-INFO` & `oneai-0.9.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,38 @@
 Metadata-Version: 2.1
 Name: oneai
-Version: 0.9.82
+Version: 0.9.9
 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python
 Author: Michael Gur
 Author-email: devrel@oneai.com
 Project-URL: Bug Tracker, https://github.com/power-of-language/oneai-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
 
 <p align="left">
   <a href="https://oneai.com?utm_source=open_source&utm_medium=python_sdk_readme">
     <img src="./oneai_logo_light_cropped.svg" height="60">
   </a>
 </p>
 
-# Natural Language Processing API
-[![API Key](https://img.shields.io/badge/%20-Get%20Your%20API%20Key%20for%20Free-%231d1c29?logo=data:image/svg%2bxml;base64,PHN2ZyB3aWR0aD0iMTEyIiBoZWlnaHQ9Ijg4IiB2aWV3Qm94PSIwIDAgMTEyIDg4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTY5LjI5MTMgMzcuNTU4NkwzNi4xMTQzIDg3Ljc1MTZIMTAyLjQ2OEw2OS4yOTEzIDM3LjU1ODZaIiBmaWxsPSIjMDBGRkZGIi8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNODkuMzAwOCA1MC4yOTIxSDExMS4xNjRWMEg4OS4zMDA4VjUwLjI5MjFaIiBmaWxsPSIjRjIzREU5Ii8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjUuOTEwOCAxMS42NDc5QzExLjYwMDcgMTEuNjQ3OSAwIDIzLjI0ODYgMCAzNy41NTg3QzAgNTEuODY4OCAxMS42MDA3IDYzLjQ3MDEgMjUuOTEwOCA2My40NzAxQzQwLjIyMDkgNjMuNDcwMSA1MS44MjE2IDUxLjg2ODggNTEuODIxNiAzNy41NTg3QzUxLjgyMTYgMjMuMjQ4NiA0MC4yMjA5IDExLjY0NzkgMjUuOTEwOCAxMS42NDc5IiBmaWxsPSIjNEQ0REZGIi8+Cjwvc3ZnPgo=)](https://studio.oneai.com/settings/api-keys)
-![Build](https://github.com/oneai-nlp/oneai-python/actions/workflows/main.yml/badge.svg)
-[![Coverage Status](https://coveralls.io/repos/github/oneai-nlp/oneai-python/badge.svg?branch=main)](https://coveralls.io/github/oneai-nlp/oneai-python?branch=main)
-[![Version](https://img.shields.io/pypi/v/oneai)](https://pypi.org/project/oneai/)
-[![Downloads](https://img.shields.io/pypi/dm/oneai)](https://pypistats.org/packages/oneai)
-[![Discord](https://img.shields.io/discord/941458663493746698?logo=Discord)](https://discord.gg/ArpMha9n8H)
-
+# Python SDK
 One AI is a NLP as a service platform. Our API enables language comprehension in context, transforming texts from any source into structured data to use in code.
 
 This SDK provides safe and convenient access to One AI's API from a Python environment.
 
 ## Documentation
 See the [documentation](https://studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme)
 
 ## Getting started
 
 ### Requirements
-Python 3.7+ (PyPy supported)
+Python 3.6.1+ (PyPy supported)
 
 ### Installation
 `pip install oneai`
 
 ### Authentication
 You will need a valid API key for all requests. Register and create a key for your project [in the Studio](https://studio.oneai.com/?utm_source=open_source&utm_medium=python_sdk_readme).
```

#### html2text {}

```diff
@@ -1,36 +1,26 @@
-Metadata-Version: 2.1 Name: oneai Version: 0.9.82 Summary: NLP as a Service
+Metadata-Version: 2.1 Name: oneai Version: 0.9.9 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python Author:
 Michael Gur Author-email: devrel@oneai.com Project-URL: Bug Tracker, https://
 github.com/power-of-language/oneai-sdk-python/issues Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: testing License-File: LICENSE
+Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 [./oneai_logo_light_cropped.svg]
-# Natural Language Processing API [![API Key](https://img.shields.io/badge/%20-
-Get%20Your%20API%20Key%20for%20Free-%231d1c29?logo=data:image/
-svg%2bxml;base64,PHN2ZyB3aWR0aD0iMTEyIiBoZWlnaHQ9Ijg4IiB2aWV3Qm94PSIwIDAgMTEyIDg4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTY5LjI5MTMgMzcuNTU4NkwzNi4xMTQzIDg3Ljc1MTZIMTAyLjQ2OEw2OS4yOTEzIDM3LjU1ODZaIiBmaWxsPSIjMDBGRkZGIi8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNODkuMzAwOCA1MC4yOTIxSDExMS4xNjRWMEg4OS4zMDA4VjUwLjI5MjFaIiBmaWxsPSIjRjIzREU5Ii8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjUuOTEwOCAxMS42NDc5QzExLjYwMDcgMTEuNjQ3OSAwIDIzLjI0ODYgMCAzNy41NTg3QzAgNTEuODY4OCAxMS42MDA3IDYzLjQ3MDEgMjUuOTEwOCA2My40NzAxQzQwLjIyMDkgNjMuNDcwMSA1MS44MjE2IDUxLjg2ODggNTEuODIxNiAzNy41NTg3QzUxLjgyMTYgMjMuMjQ4NiA0MC4yMjA5IDExLjY0NzkgMjUuOTEwOCAxMS42NDc5IiBmaWxsPSIjNEQ0REZGIi8+Cjwvc3ZnPgo=)]
-(https://studio.oneai.com/settings/api-keys) ![Build](https://github.com/oneai-
-nlp/oneai-python/actions/workflows/main.yml/badge.svg) [![Coverage Status]
-(https://coveralls.io/repos/github/oneai-nlp/oneai-python/
-badge.svg?branch=main)](https://coveralls.io/github/oneai-nlp/oneai-
-python?branch=main) [![Version](https://img.shields.io/pypi/v/oneai)](https://
-pypi.org/project/oneai/) [![Downloads](https://img.shields.io/pypi/dm/oneai)]
-(https://pypistats.org/packages/oneai) [![Discord](https://img.shields.io/
-discord/941458663493746698?logo=Discord)](https://discord.gg/ArpMha9n8H) One AI
-is a NLP as a service platform. Our API enables language comprehension in
-context, transforming texts from any source into structured data to use in
-code. This SDK provides safe and convenient access to One AI's API from a
-Python environment. ## Documentation See the [documentation](https://
-studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme) ##
-Getting started ### Requirements Python 3.7+ (PyPy supported) ### Installation
-`pip install oneai` ### Authentication You will need a valid API key for all
-requests. Register and create a key for your project [in the Studio](https://
-studio.oneai.com/?utm_source=open_source&utm_medium=python_sdk_readme). ####
-Example ```python import oneai oneai.api_key = '' pipeline = oneai.Pipeline
-(steps=[ oneai.skills.Names(), oneai.skills.Summarize(min_length=20),
+# Python SDK One AI is a NLP as a service platform. Our API enables language
+comprehension in context, transforming texts from any source into structured
+data to use in code. This SDK provides safe and convenient access to One AI's
+API from a Python environment. ## Documentation See the [documentation](https:/
+/studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme) ##
+Getting started ### Requirements Python 3.6.1+ (PyPy supported) ###
+Installation `pip install oneai` ### Authentication You will need a valid API
+key for all requests. Register and create a key for your project [in the
+Studio](https://studio.oneai.com/
+?utm_source=open_source&utm_medium=python_sdk_readme). #### Example ```python
+import oneai oneai.api_key = '' pipeline = oneai.Pipeline(steps=
+[ oneai.skills.Names(), oneai.skills.Summarize(min_length=20),
 oneai.skills.Keywords() ]) my_text = 'analyze this text.' output = pipeline.run
 (my_text) print(output) ``` ## Pipeline API ### Language Skills A Language
 Skill is a package of trained NLP models, available via API. Skills accept text
 as an input in various formats, and respond with processed texts and extracted
 metadata. ### Pipelines Language AI pipelines allow invoking and chaining
 multiple Language Skills to process your input text with a single call.
 Pipelines are defined by listing the desired Skills. ### Language Studio The
```

### Comparing `oneai-0.9.82/README.md` & `oneai-0.9.9/src/oneai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+Metadata-Version: 2.1
+Name: oneai
+Version: 0.9.9
+Summary: NLP as a Service
+Home-page: https://github.com/power-of-language/oneai-sdk-python
+Author: Michael Gur
+Author-email: devrel@oneai.com
+Project-URL: Bug Tracker, https://github.com/power-of-language/oneai-sdk-python/issues
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="left">
   <a href="https://oneai.com?utm_source=open_source&utm_medium=python_sdk_readme">
     <img src="./oneai_logo_light_cropped.svg" height="60">
   </a>
 </p>
 
-# Natural Language Processing API
-[![API Key](https://img.shields.io/badge/%20-Get%20Your%20API%20Key%20for%20Free-%231d1c29?logo=data:image/svg%2bxml;base64,PHN2ZyB3aWR0aD0iMTEyIiBoZWlnaHQ9Ijg4IiB2aWV3Qm94PSIwIDAgMTEyIDg4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTY5LjI5MTMgMzcuNTU4NkwzNi4xMTQzIDg3Ljc1MTZIMTAyLjQ2OEw2OS4yOTEzIDM3LjU1ODZaIiBmaWxsPSIjMDBGRkZGIi8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNODkuMzAwOCA1MC4yOTIxSDExMS4xNjRWMEg4OS4zMDA4VjUwLjI5MjFaIiBmaWxsPSIjRjIzREU5Ii8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjUuOTEwOCAxMS42NDc5QzExLjYwMDcgMTEuNjQ3OSAwIDIzLjI0ODYgMCAzNy41NTg3QzAgNTEuODY4OCAxMS42MDA3IDYzLjQ3MDEgMjUuOTEwOCA2My40NzAxQzQwLjIyMDkgNjMuNDcwMSA1MS44MjE2IDUxLjg2ODggNTEuODIxNiAzNy41NTg3QzUxLjgyMTYgMjMuMjQ4NiA0MC4yMjA5IDExLjY0NzkgMjUuOTEwOCAxMS42NDc5IiBmaWxsPSIjNEQ0REZGIi8+Cjwvc3ZnPgo=)](https://studio.oneai.com/settings/api-keys)
-![Build](https://github.com/oneai-nlp/oneai-python/actions/workflows/main.yml/badge.svg)
-[![Coverage Status](https://coveralls.io/repos/github/oneai-nlp/oneai-python/badge.svg?branch=main)](https://coveralls.io/github/oneai-nlp/oneai-python?branch=main)
-[![Version](https://img.shields.io/pypi/v/oneai)](https://pypi.org/project/oneai/)
-[![Downloads](https://img.shields.io/pypi/dm/oneai)](https://pypistats.org/packages/oneai)
-[![Discord](https://img.shields.io/discord/941458663493746698?logo=Discord)](https://discord.gg/ArpMha9n8H)
-
+# Python SDK
 One AI is a NLP as a service platform. Our API enables language comprehension in context, transforming texts from any source into structured data to use in code.
 
 This SDK provides safe and convenient access to One AI's API from a Python environment.
 
 ## Documentation
 See the [documentation](https://studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme)
 
 ## Getting started
 
 ### Requirements
-Python 3.7+ (PyPy supported)
+Python 3.6.1+ (PyPy supported)
 
 ### Installation
 `pip install oneai`
 
 ### Authentication
 You will need a valid API key for all requests. Register and create a key for your project [in the Studio](https://studio.oneai.com/?utm_source=open_source&utm_medium=python_sdk_readme).
```

#### html2text {}

```diff
@@ -1,30 +1,26 @@
+Metadata-Version: 2.1 Name: oneai Version: 0.9.9 Summary: NLP as a Service
+Home-page: https://github.com/power-of-language/oneai-sdk-python Author:
+Michael Gur Author-email: devrel@oneai.com Project-URL: Bug Tracker, https://
+github.com/power-of-language/oneai-sdk-python/issues Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 [./oneai_logo_light_cropped.svg]
-# Natural Language Processing API [![API Key](https://img.shields.io/badge/%20-
-Get%20Your%20API%20Key%20for%20Free-%231d1c29?logo=data:image/
-svg%2bxml;base64,PHN2ZyB3aWR0aD0iMTEyIiBoZWlnaHQ9Ijg4IiB2aWV3Qm94PSIwIDAgMTEyIDg4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTY5LjI5MTMgMzcuNTU4NkwzNi4xMTQzIDg3Ljc1MTZIMTAyLjQ2OEw2OS4yOTEzIDM3LjU1ODZaIiBmaWxsPSIjMDBGRkZGIi8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNODkuMzAwOCA1MC4yOTIxSDExMS4xNjRWMEg4OS4zMDA4VjUwLjI5MjFaIiBmaWxsPSIjRjIzREU5Ii8+CjxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMjUuOTEwOCAxMS42NDc5QzExLjYwMDcgMTEuNjQ3OSAwIDIzLjI0ODYgMCAzNy41NTg3QzAgNTEuODY4OCAxMS42MDA3IDYzLjQ3MDEgMjUuOTEwOCA2My40NzAxQzQwLjIyMDkgNjMuNDcwMSA1MS44MjE2IDUxLjg2ODggNTEuODIxNiAzNy41NTg3QzUxLjgyMTYgMjMuMjQ4NiA0MC4yMjA5IDExLjY0NzkgMjUuOTEwOCAxMS42NDc5IiBmaWxsPSIjNEQ0REZGIi8+Cjwvc3ZnPgo=)]
-(https://studio.oneai.com/settings/api-keys) ![Build](https://github.com/oneai-
-nlp/oneai-python/actions/workflows/main.yml/badge.svg) [![Coverage Status]
-(https://coveralls.io/repos/github/oneai-nlp/oneai-python/
-badge.svg?branch=main)](https://coveralls.io/github/oneai-nlp/oneai-
-python?branch=main) [![Version](https://img.shields.io/pypi/v/oneai)](https://
-pypi.org/project/oneai/) [![Downloads](https://img.shields.io/pypi/dm/oneai)]
-(https://pypistats.org/packages/oneai) [![Discord](https://img.shields.io/
-discord/941458663493746698?logo=Discord)](https://discord.gg/ArpMha9n8H) One AI
-is a NLP as a service platform. Our API enables language comprehension in
-context, transforming texts from any source into structured data to use in
-code. This SDK provides safe and convenient access to One AI's API from a
-Python environment. ## Documentation See the [documentation](https://
-studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme) ##
-Getting started ### Requirements Python 3.7+ (PyPy supported) ### Installation
-`pip install oneai` ### Authentication You will need a valid API key for all
-requests. Register and create a key for your project [in the Studio](https://
-studio.oneai.com/?utm_source=open_source&utm_medium=python_sdk_readme). ####
-Example ```python import oneai oneai.api_key = '' pipeline = oneai.Pipeline
-(steps=[ oneai.skills.Names(), oneai.skills.Summarize(min_length=20),
+# Python SDK One AI is a NLP as a service platform. Our API enables language
+comprehension in context, transforming texts from any source into structured
+data to use in code. This SDK provides safe and convenient access to One AI's
+API from a Python environment. ## Documentation See the [documentation](https:/
+/studio.oneai.com/docs?utm_source=open_source&utm_medium=python_sdk_readme) ##
+Getting started ### Requirements Python 3.6.1+ (PyPy supported) ###
+Installation `pip install oneai` ### Authentication You will need a valid API
+key for all requests. Register and create a key for your project [in the
+Studio](https://studio.oneai.com/
+?utm_source=open_source&utm_medium=python_sdk_readme). #### Example ```python
+import oneai oneai.api_key = '' pipeline = oneai.Pipeline(steps=
+[ oneai.skills.Names(), oneai.skills.Summarize(min_length=20),
 oneai.skills.Keywords() ]) my_text = 'analyze this text.' output = pipeline.run
 (my_text) print(output) ``` ## Pipeline API ### Language Skills A Language
 Skill is a package of trained NLP models, available via API. Skills accept text
 as an input in various formats, and respond with processed texts and extracted
 metadata. ### Pipelines Language AI pipelines allow invoking and chaining
 multiple Language Skills to process your input text with a single call.
 Pipelines are defined by listing the desired Skills. ### Language Studio The
```

### Comparing `oneai-0.9.82/setup.cfg` & `oneai-0.9.9/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -9,36 +9,26 @@
 url = https://github.com/power-of-language/oneai-sdk-python
 project_urls = 
 	Bug Tracker = https://github.com/power-of-language/oneai-sdk-python/issues
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.6
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	aiohttp
 	validators
 	typing_extensions
 	dataclasses; python_version<"3.7"
 	requests
 	python-dateutil
 
-[options.extras_require]
-testing = 
-	pytest
-	pytest-cov
-	pytest-asyncio
-	pytest-dependency
-	mypy
-	python-dotenv
-	coveralls
-
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `oneai-0.9.82/src/oneai/__init__.py` & `oneai-0.9.9/src/oneai/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-__version__ = "0.9.82"
+__version__ = "0.9.9"
 __package__ = "oneai"
 
-import logging
-import oneai.logger
 from typing_extensions import Final
+import oneai.logger
 import oneai.skills as skills
 from oneai.classes import *
-from oneai.output import Output
 from oneai.pipeline import Pipeline
 import oneai.clustering as clustering
 import oneai.parsing as parsing
 import oneai.util as util
-import oneai.exceptions as exceptions
 
 URL: Final[str] = "https://api.oneai.com"
 """
 Base URL for the pipeline API. Only change if you know what you're doing.
 """
 
 api_key = None
@@ -29,17 +26,15 @@
 """
 
 MAX_CONCURRENT_REQUESTS: Final[int] = 2
 """
 Max number of allowed concurrent requests to be made by the SDK.
 Currently only enforced on `pipeline.run_batch`, other calls may be limited by the API
 """
-DEBUG_RAW_RESPONSES = False
+PRINT_PROGRESS = True
 """
-Debug flag, return raw API responses instead of structured `Output` object. Only enable if you know what you're doing
+Does nothing. Set `logging.get('oneai').propagate = False` to disable logging
 """
-DEBUG_LOG_REQUESTS = False
+DEBUG_RAW_RESPONSES = False
 """
-Debug flag, log all requests made by the SDK.
+Debug flag, return raw API responses instead of structured `Output` object. Only enable if you know what you're doing
 """
-
-logger: logging.Logger = logging.getLogger("oneai")
```

### Comparing `oneai-0.9.82/src/oneai/api/clustering.py` & `oneai-0.9.9/src/oneai/api/clustering.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         to_date = to_date.strftime(API_DATE_FORMAT)
 
     params = {
         "sort": sort,
         "limit": limit if limit else 20,
         "from-date": from_date,
         "to-date": to_date,
+        "include-phrases": False,
         "item-metadata": item_metadata,
-        "translate": True,
     }
-    return {k: v for k, v in params.items() if v is not None}
+    return urllib.parse.urlencode({k: v for k, v in params.items() if v})
 
 
 def get_clustering_paginated(
     path: str,
     api_key: str,
     result_key: str,
     parent: Any,
@@ -50,67 +50,55 @@
     sort: Literal["ASC", "DESC"] = None,
     limit: int = None,
     from_date: Union[datetime, str] = None,
     to_date: Union[datetime, str] = None,
     date_format: str = API_DATE_FORMAT,
     item_metadata: str = None,
 ):
-    params = build_query_params(
-        sort, limit, from_date, to_date, date_format, item_metadata
-    )
+    path_query = f"{path}?{build_query_params(sort, limit, from_date, to_date, date_format, item_metadata)}"
     page = 0
     counter = 0
     results = [None]
 
     while results and ((not limit) or counter < limit):
-        params["page"] = page
-        response = get_clustering(path, params, api_key)
+        response = get_clustering(f"{path_query}&page={page}", api_key)
         results = [
             (from_dict(parent, result) if parent else from_dict(result))
             for result in response[result_key]
         ]
         yield from results
         counter += len(results)
         page += 1
 
         if page >= response.get("total_pages", 0):
             break
 
 
-def get_clustering(path: str, params: dict, api_key: str = None):
+def get_clustering(path: str, api_key: str = None):
     api_key = api_key or oneai.api_key
     if not api_key:
         raise Exception("API key is required")
     headers = {
         "api-key": api_key,
         "Content-Type": "application/json",
         "User-Agent": f"python-sdk/{oneai.__version__}/{oneai.api.uuid}",
     }
-    if oneai.DEBUG_LOG_REQUESTS:
-        oneai.logger.debug(f"GET {oneai.URL}/{ENDPOINT}/{path}\n")
-        oneai.logger.debug(f"headers={json.dumps(headers, indent=4)}\n")
-        oneai.logger.debug(f"params={json.dumps(params, indent=4)}\n")
     response = requests.get(
         f"{oneai.URL}/{ENDPOINT}/{path}",
         headers=headers,
-        params=params,
     )
     return json.loads(response.content)
 
 
 def post_clustering(path: str, data: dict, api_key: str = None):
     api_key = api_key or oneai.api_key
     if not api_key:
         raise Exception("API key is required")
     headers = {
         "api-key": api_key,
         "Content-Type": "application/json",
         "User-Agent": f"python-sdk/{oneai.__version__}/{oneai.api.uuid}",
     }
-    if oneai.DEBUG_LOG_REQUESTS:
-        oneai.logger.debug(f"POST {oneai.URL}/{ENDPOINT}/{path}\n")
-        oneai.logger.debug(f"headers={json.dumps(headers, indent=4)}\n")
-        oneai.logger.debug(f"data={json.dumps(data, indent=4)}\n")
     response = requests.post(
         f"{oneai.URL}/{ENDPOINT}/{path}", headers=headers, json=data
     )
     return json.loads(response.content)
```

### Comparing `oneai-0.9.82/src/oneai/api/output.py` & `oneai-0.9.9/src/oneai/api/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from dataclasses import replace
+from copy import copy
 from typing import List
 
 import oneai
-from oneai.classes import Label, Labels, Skill, Utterance, TextContent
-from oneai.output import Output
+from oneai.classes import Label, Labels, Output, Skill, Utterance, TextContent
 
 
 def build_output(
     skills: List[Skill],
     raw_output: dict,
-    headers: dict = {},
 ) -> Output:
     if oneai.DEBUG_RAW_RESPONSES:
         return raw_output
 
     def get_text(index) -> TextContent:
         # get the input text for this Output object. use index=-1 to get the original input text
         # text can be returned as a simple str or parsed to match a given input type
@@ -28,66 +26,49 @@
         if len(text) > 1 or (text and "speaker" in text[0]):
             return [Utterance.from_dict(u) for u in text]
         return text[0]["utterance"]
 
     def split_pipeline(skills: List[Skill], i: int):
         # split pipeline at a generator Skill
         first, second = skills[: i + 1], skills[i + 1 :]
-        if skills[i].labels_attr:
+        if hasattr(skills[i], "output_attr1") and skills[i].output_attr1:
             # handle skills that create both text and labels
-            clone = replace(skills[i])
-            object.__setattr__(clone, "text_attr", None)
+            clone = copy(skills[i])
+            clone.is_generator = False
+            clone.output_attr = skills[i].output_attr1
             second = (clone, *second)
         return first, second
 
-    def build_internal(
-        output_index: int,
-        skills: List[Skill],
-        headers: dict = {},
-    ) -> "Output":
+    def build_internal(output_index: int, skills: List[Skill]) -> "Output":
         text = get_text(output_index)
         # temporary fix- if 1st skill is not a generator, use input_text, not output[0].text,
         # since output[0].text is corrupted (not parsable) for conversation inputs
         output_index = max(output_index, 0)
         labels = [
             Label.from_dict(label)
-            for label in raw_output["output"][output_index].get("labels", [])
+            for label in raw_output["output"][output_index]["labels"]
         ]
         data = []
         for i, skill in enumerate(skills):
-            if skill.text_attr:
+            if skill.is_generator:
                 skills, next_skills = split_pipeline(skills, i)
                 data.append(build_internal(output_index + 1, next_skills))
                 break
             else:
                 data.append(
-                    Labels(filter(lambda label: label.skill == skill.api_name, labels))
+                    Labels(filter(lambda label: label.type == skill.label_type, labels))
                 )
-        return Output(
-            text=text,
-            skills=list(skills),
-            data=data,
-            task_id=headers.get("x-oneai-request-id"),
-        )
-
-    # handle output lists
-    if "outputs" in raw_output:
-        return Output(
-            "",
-            outputs=[build_output(skills, o) for o in raw_output["outputs"]],
-            task_id=headers.get("x-oneai-request-id"),
-        )
+        return Output(text=text, skills=list(skills), data=data)
 
     generator = raw_output["output"][0].get("text_generated_by_step_id", 0) - 1
     if generator < 0:
-        return build_internal(-1, skills, headers)
+        return build_internal(-1, skills)
     else:
         # edge case- first Skill is a generator, or a generator preceded by Skills that didn't generate output
         # in this case the API will skip these Skills,
         # so we need to create filler objects to match the expected structure
         skills, next_skills = split_pipeline(skills, generator)
         return Output(
             text=get_text(-1),
             skills=list(skills),
             data=[Labels()] * generator + [build_internal(0, next_skills)],
-            task_id=headers.get("x-oneai-request-id"),
         )
```

### Comparing `oneai-0.9.82/src/oneai/api/pipeline.py` & `oneai-0.9.9/src/oneai/api/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,101 @@
 from datetime import timedelta
-import io
 import json
 import urllib.parse
 from typing import Awaitable, List
 
 import aiohttp
 import oneai, oneai.api
 from oneai.api.output import build_output
-from oneai.classes import Input, Skill, CSVParams
-from oneai.output import Output
+from oneai.classes import Input, Output, Skill
 from oneai.exceptions import handle_unsuccessful_response, validate_api_key
 
 endpoint_default = "api/v0/pipeline"
-endpoint_async = "api/v0/pipeline/async"
 endpoint_async_file = "api/v0/pipeline/async/file"
 endpoint_async_tasks = "api/v0/pipeline/async/tasks"
 
 
 def build_request(
-    input: Input,
-    steps: List[Skill],
-    multilingual: bool,
-    include_text: bool,
-    csv_params: CSVParams = None,
+    input: Input, steps: List[Skill], multilingual: bool, include_text: True
 ):
     def json_default(obj):
         if isinstance(obj, timedelta):
             return str(obj)
         if isinstance(obj, Skill):
             return obj.api_name
         return {k: v for k, v in obj.__dict__.items() if v is not None}
 
     # use input metadata for clustering
     if hasattr(input, "metadata"):
         for skill in steps:
             if skill.api_name == "clustering":
-                skill.params["user_metadata"] = input.metadata
+                skill._skill_params.append("user_metadata")
+                skill.user_metadata = input.metadata
                 break
 
     request = {
         "steps": [skill.asdict() for skill in steps],
         "output_type": "json",
         "multilingual": multilingual,
     }
     if include_text:
         request["text"] = input.text
-    if csv_params is not None:
-        request["csv_params"] = {
-            k: v for k, v in csv_params.asdict().items() if v is not None
-        }
-    if hasattr(input, "type") and input.type:
-        request["input_type"] = input.type
-    if hasattr(input, "content_type") and input.content_type:
-        request["content_type"] = input.content_type
-    if hasattr(input, "encoding") and input.encoding:
-        request["encoding"] = input.encoding
+    if isinstance(input, Input):
+        if input.type:
+            request["input_type"] = input.type
+        if hasattr(input, "content_type") and input.content_type:
+            request["content_type"] = input.content_type
+        if hasattr(input, "encoding") and input.encoding:
+            request["encoding"] = input.encoding
     return json.dumps(request, default=json_default)
 
 
 async def post_pipeline(
     session: aiohttp.ClientSession,
     input: Input,
     steps: List[Skill],
     api_key: str,
     multilingual: bool,
-    csv_params: CSVParams = None,
 ) -> Awaitable[Output]:
     validate_api_key(api_key)
 
-    request = build_request(input, steps, multilingual, True, csv_params)
+    request = build_request(input, steps, multilingual, True)
     url = f"{oneai.URL}/{endpoint_default}"
     headers = {
         "api-key": api_key,
         "Content-Type": "application/json",
         "User-Agent": f"python-sdk/{oneai.__version__}/{oneai.api.uuid}",
     }
 
-    if oneai.DEBUG_LOG_REQUESTS:
-        oneai.logger.debug(f"POST {url}\n")
-        oneai.logger.debug(f"headers={json.dumps(headers, indent=4)}\n")
-        oneai.logger.debug(f"data={json.dumps(json.loads(request), indent=4)}\n")
-
     async with session.post(url, headers=headers, data=request) as response:
         if response.status != 200:
             await handle_unsuccessful_response(response)
         else:
-            return build_output(steps, await response.json(), response.headers)
+            return build_output(steps, await response.json())
 
 
-async def post_pipeline_async(
+async def post_pipeline_async_file(
     session: aiohttp.ClientSession,
     input: Input,
     steps: List[Skill],
     api_key: str,
     multilingual: bool,
-    csv_params: CSVParams = None,
 ) -> Awaitable[str]:
     validate_api_key(api_key)
 
-    is_file = isinstance(input.text, io.IOBase)
-    endpoint = endpoint_async_file if is_file else endpoint_async
-    request = build_request(input, steps, multilingual, not is_file, csv_params)
-    endpoint += ("?pipeline=" + urllib.parse.quote(request)) if is_file else ""
-    url = f"{oneai.URL}/{endpoint}"
+    request = build_request(input, steps, multilingual, False)
+    url = f"{oneai.URL}/{endpoint_async_file}?pipeline=" + urllib.parse.quote(request)
     headers = {
         "api-key": api_key,
         "Content-Type": "application/json",
         "User-Agent": f"python-sdk/{oneai.__version__}/{oneai.api.uuid}",
     }
-    data = input.text if is_file else request
 
-    if oneai.DEBUG_LOG_REQUESTS:
-        oneai.logger.debug(f"POST {url}\n")
-        oneai.logger.debug(f"headers={json.dumps(headers, indent=4)}\n")
-        if is_file:
-            oneai.logger.debug(
-                f"decoded pipeline={json.dumps(json.loads(request), indent=4)}\n"
-            )
-            oneai.logger.debug(f"data={input.text}\n")
-        else:
-            oneai.logger.debug(f"data={json.dumps(json.loads(request), indent=4)}\n")
-
-    async with session.post(url, headers=headers, data=data) as response:
-        if response.status not in [200, 202]:
+    async with session.post(url, headers=headers, data=input.text) as response:
+        if response.status != 200:
             await handle_unsuccessful_response(response)
         else:
             return await response.json()
 
 
 async def get_task_status(
     session: aiohttp.ClientSession,
@@ -137,16 +106,12 @@
 
     url = f"{oneai.URL}/{endpoint_async_tasks}/{task_id}"
     headers = {
         "api-key": api_key,
         "User-Agent": f"python-sdk/{oneai.__version__}/{oneai.api.uuid}",
     }
 
-    if oneai.DEBUG_LOG_REQUESTS:
-        oneai.logger.debug(f"GET {url}\n")
-        oneai.logger.debug(f"headers={json.dumps(headers, indent=4)}\n")
-
     async with session.get(url, headers=headers) as response:
         if response.status != 200:
             await handle_unsuccessful_response(response)
         else:
             return await response.json()
```

### Comparing `oneai-0.9.82/src/oneai/classes.py` & `oneai-0.9.9/src/oneai/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,52 +2,57 @@
 from dateutil import parser as dateutil
 import io
 import os
 from base64 import b64encode
 import validators
 from dataclasses import dataclass, field
 from typing import (
+    TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     Generic,
+    Iterable,
     List,
     Optional,
     TextIO,
     Tuple,
+    Type,
     TypeVar,
     Union,
+    Hashable,
 )
-from typing_extensions import dataclass_transform, Literal
 from warnings import warn
 
+
 from oneai.exceptions import InputError
 
+if TYPE_CHECKING:
+    from oneai.skills import OutputAttrs
+
 
 @dataclass
 class Utterance:
     speaker: str
     utterance: str
     timestamp: Optional[timedelta] = None
 
     @classmethod
     def from_dict(cls, u: Dict[str, str]) -> "Utterance":
         return cls(
-            u.get("speaker", None),
+            u["speaker"],
             u["utterance"],
             timestamp_to_timedelta(u.get("timestamp", None)),
         )
 
     def __repr__(self) -> str:
         return (
             f"\n\t{self.timestamp} {self.speaker}: {self.utterance}"
             if self.timestamp
             else f"\n\t{self.speaker}: {self.utterance}"
-            if self.speaker
-            else f"\n\t{self.utterance}"
         )
 
 
 TextContent = TypeVar("TextContent", bound=Union[str, List["Utterance"]])
 PipelineInput = Union["Input[TextContent]", TextContent, TextIO, BinaryIO]
 
 # extension -> content_type, input_type
@@ -56,144 +61,108 @@
     ".txt": ("text/plain", "article"),
     ".srt": ("text/plain", "conversation"),
     ".wav": ("audio/wav", "conversation"),
     ".mp3": ("audio/mpeg", "conversation"),
     ".mp4": ("audio/mpeg", "conversation"),
     ".html": ("text/plain", "article"),
     ".pdf": ("text/pdf", "article"),
-    ".csv": ("text/csv", "article"),
 }
 
 
-@dataclass(frozen=True)
+@dataclass
 class Skill:
     """
     A base class for all Language Skills. Use predefined subclasses of this class, or use this class to define your own Skills.
 
     A Language Skill is a package of trained NLP models. Skills accept text and respond with processed texts and extracted metadata.
 
     Process texts with Skills using `Pipeline`s
 
     ### Skill types
-    * Generator Skills (`text_attr is not None`) process the input and produce a new text based on it. Examples include `Summarize`, `Proofread`.
-    * Analyzer Skills (`text_attr is None`) scan the input and extract structured data. Examples include `Emotions`, `Topics`.
+    * Generator Skills (`is_generator=True`) process the input and produce a new text based on it. Examples include `Summarize`, `TranscriptionEnhancer`.
+    * Analyzer Skills (`is_generator=False`) scan the input and extract structured data. Examples include `Emotions`, `Topics`.
 
     ## Attributes
 
     `api_name: str`
         The name of the Skill in the pipeline API.
-    `text_attr: str`
-        The attribute name of the Skill's output text in the Output object (Generator Skills only).
-    `labels_attr: str`
-        The attribute name of the Skill's output labels in the Output object.
-    `params: dict[str, Any]`
-        The parameters of the Skill. See the documentation for each Skill for a list of available parameters.
+    `is_generator: bool`
+        Whether the Skill is a generator Skill.
+    `skill_params: List[str]`
+        Names of the fields of the Skill object that should be passed as parameters to the API.
+    `label_type: str`
+        If the Skill generates labels, the type name of the label.
+    `output_attr: str`
+        The attribute name of the Skill's output in the Output object.
+    `output_attr1: str`
+        Only for Skills with 2 outputs (text / labels)
     """
 
     api_name: str = ""
-    text_attr: Optional[str] = None
-    labels_attr: Optional[str] = None
-    params: Dict[str, Any] = field(default_factory=dict)
-
-    def __post_init__(self):
-        # backwards compatibility
-        if self.labels_attr is None and self.text_attr is None:
-            object.__setattr__(self, "labels_attr", self.api_name)
+    is_generator: bool = False
+    _skill_params: List[str] = field(default_factory=list, repr=False, init=False)
+    # todo: replace all these w/ an output type object + parse conversations from t. enhancer etc.
+    label_type: str = ""
+    output_attr: str = ""
+    output_attr1: str = field(default="", repr=False)
 
     def asdict(self) -> dict:
         return {
             "skill": self.api_name,
-            "params": {k: v for k, v in self.params.items() if v is not None},
+            "params": {
+                p: self.__getattribute__(p)
+                for p in self._skill_params
+                if self.__getattribute__(p)
+            },
         }
 
 
-@dataclass_transform()
 def skillclass(
+    cls: Type = None,
     api_name: str = "",
-    text_attr: Optional[str] = None,
-    labels_attr: Optional[str] = None,
+    label_type: str = "",
+    is_generator: bool = False,
+    output_attr: str = "",
+    output_attr1: str = "",
 ):
     """
-    A decorator for defining a Language Skill class. Decorate subclasses of `Skill` with this to provide default values for instance attributes.
-
-    ## Example
-
-    >>> @skillclass(api_name="my-skill", text_attr="my_result")
-    ... class MySkill(Skill):
-    ...     ratio: float = 0.2
-    >>> s = Summarize(ratio=0.5)
-    >>> s.ratio
-    0.5
-    >>> pipeline = Pipeline([s])
-    >>> output = pipeline.run("Text to be processed with MySkill")
-    >>> output.my_result
-    "Result text, processed with MySkill"
+    A decorator for defining a Language Skill class. Decorate subclasses of `Skill` with this decorator to provide default values for instance attributes.
     """
 
-    def wrap(cls):
+    def wrap(cls) -> cls:
         if not issubclass(cls, Skill):
             warn(
                 f"warning: class {cls.__name__} decorated with @skillclass does not inherit Skill",
                 stacklevel=2,
             )
 
-        # remove class variables
-        classVars = {
-            k: getattr(cls, k, None)
-            for k in cls.__annotations__
-            if k not in Skill.__annotations__
-        }
-        for k in classVars:
-            if hasattr(cls, k):
-                delattr(cls, k)
-
-        def __init__(self, **params):
-            if "params" in params and isinstance(params["params"], dict):
-                params = {**params, **params["params"]}
-                del params["params"]
-
+        def __init__(self, *args, **kwargs):
+            cls_init(self, *args)
             Skill.__init__(
                 self,
-                api_name=params.pop("api_name", api_name),
-                text_attr=params.pop("text_attr", text_attr),
-                labels_attr=params.pop("labels_attr", labels_attr),
-                params=params,
+                api_name=api_name,
+                label_type=label_type,
+                is_generator=is_generator,
+                output_attr=output_attr,
+                output_attr1=output_attr1,
             )
+            self._skill_params = [
+                a
+                for a in {**self.__dict__, **kwargs}
+                if a not in Skill.__dataclass_fields__
+            ]
+            for param in self._skill_params:
+                if param in kwargs:
+                    self.__setattr__(param, kwargs[param])
 
-            for k, v in classVars.items():
-                if k not in self.params and k is not None:
-                    self.params[k] = v
-
-        def __getattr__(self, name):
-            if name in Skill.__annotations__:
-                return object.__getattribute__(self, name)
-
-            if name not in classVars:
-                raise AttributeError(
-                    f"'{self.__class__.__name__}' object has no attribute '{name}'"
-                )
-            return self.params.get(name, None)
-
-        def __setattr__(self, name, value):
-            if name in Skill.__annotations__:
-                return object.__setattr__(self, name, value)
-
-            if name not in classVars:
-                warn(
-                    f"warning: parameter '{name}' not defined in class {self.__class__.__name__}",
-                    stacklevel=2,
-                )
-            self.params[name] = value
-
+        cls_init = cls.__init__
         cls.__init__ = __init__
-        cls.__getattr__ = __getattr__
-        cls.__setattr__ = __setattr__
         return cls
 
-    return wrap
+    return wrap if cls is None else wrap(cls)
 
 
 class Input(Generic[TextContent]):
     """
     A base class for all input texts, allowing structured representations of inputs.
 
     ## Attributes
@@ -206,84 +175,74 @@
         The content type of the input.
     `encoding: str`
         The encoding of the input.
     `metadata: dict`
         Optional metadata to be associated with the input in clustering collections.
     `datetime: datetime`
         Optional datetime to be associated with the input in clustering collections.
-    `text_index: str`
-        Optional text index to be associated with the input in clustering collections.
     """
 
     def __init__(
         self,
         text: TextContent,
         *,
         type: str = None,
         content_type: str = None,
         encoding: str = None,
         metadata: Dict[str, any] = None,
         datetime: datetime = None,
-        text_index: str = None,
     ):
         self.text: TextContent = text
         self.type = type
         self.content_type = content_type
         self.encoding = encoding
         self.metadata = metadata
         self.datetime = datetime
-        self.text_index = text_index
 
     @classmethod
     def wrap(
-        cls,
-        text: PipelineInput[TextContent],
+        cls, text: PipelineInput[TextContent], sync: bool = True
     ) -> "Input[TextContent]":
         if isinstance(text, cls):
             return text
         elif isinstance(text, str):
             if validators.url(text):
                 return cls(text, type="article", content_type="text/uri-list")
             else:
                 return cls(text, type="article", content_type="text/plain")
         elif isinstance(text, list) and (
             len(text) == 0 or isinstance(text[0], Utterance)
         ):
             return cls(text, type="conversation", content_type="application/json")
         elif isinstance(text, io.IOBase):
-            _, ext = os.path.splitext(text.name)
+            name, mode = text.name, text.mode
+            _, ext = os.path.splitext(name)
             if ext not in CONTENT_TYPES:
                 raise InputError(
                     message=f"unsupported file extension {ext}",
                     details="see supported files in docs",
                 )
             content_type, input_type = CONTENT_TYPES[ext]
-            if ext == ".csv" and isinstance(text, io.TextIOBase):
-                text = io.BytesIO(text.read().encode("utf-8"))
-            return cls(text, type=input_type, content_type=content_type)
+            if "b" not in mode:
+                return cls(text.read(), type=input_type, content_type=content_type)
+            elif sync:
+                data = b64encode(text.read()).decode("ascii")
+                return cls(
+                    data, type=input_type, content_type=content_type, encoding="base64"
+                )
+            else:
+                return cls(text, type=input_type, content_type=content_type)
         else:
             raise ValueError(f"invalid content type {type(text)}")
 
-    def _make_sync(self) -> "Input[Union[str, List[Utterance]]]":
-        if isinstance(self.text, io.BufferedIOBase):
-            self.text = b64encode(self.text.read()).decode("ascii")
-            self.encoding = "base64"
-        elif isinstance(self.text, io.TextIOBase):
-            self.text = self.text.read()
-        return self
-
 
 def timestamp_to_timedelta(timestamp: str) -> timedelta:
     if not timestamp:
         return None
-    try:
-        dt = dateutil.parse(timestamp)
-    except Exception as e:
-        warn("Received invalid timestamp: {}, returning as str".format(timestamp))
-        return timestamp
+    dt = dateutil.parse(timestamp)
     return timedelta(
         hours=dt.hour, minutes=dt.minute, seconds=dt.second, microseconds=dt.microsecond
     )
 
 
 @dataclass
 class Span:
@@ -314,16 +273,14 @@
     """
     Represents a label, marking a part of the input text. Attribute values largely depend on the Skill the labels were produced by.
 
     ## Attributes
 
     `type: str`
         Label type, e.g. 'entity', 'topic', 'emotion'.
-    `skill: str`
-        The name of the Skill that produced the label.
     `name: str`
         Label class name, e.g. 'PERSON', 'happiness', 'POS'.
     `output_spans: list[Span]`
         The spans in the output text that are marked with the label.
     `input_spans: list[Span]`
         The spans in the input text that are relevant to the label. Only appears if the label was produced by a Skill that supports input spans.
     `span_text: str`
@@ -426,35 +383,63 @@
         return [l.output_spans for l in self]
 
     @property
     def span_texts(self) -> List[str]:
         return [l.span_text for l in self]
 
 
-CSVColumn = Union[
-    Literal[
-        # The text input to be processed
-        "input",
-        # Input timestamp
-        "timestamp",
-        # Input translation
-        "input_translated",
-        # Skip column
-        False,
-    ],
-    # Custom Metadata
-    str,
-]
+class Output(Input[TextContent], OutputAttrs if TYPE_CHECKING else object):
+    """
+    Represents the output of a pipeline. The structure of the output is dynamic, and corresponds to the Skills used and their order in the pipeline.
+    Skill outputs can be accessed as attributes, either with the `api_name` of the corresponding Skill or the `output_attr` field.
 
+    ## Attributes
 
-@dataclass
-class CSVParams:
-    columns: List[CSVColumn]
-    skip_rows: int = 0
-    max_rows: Optional[int] = None
+    `text: TextContent`
+        The input text from which this `Output` instance was produced.
+    `skills: List[Skill]`
+        The Skills used to process `text` and produce this `Output` instance.
+    See `OutputAttrs` for the attributes generated by different Skills.
+    """
 
-    def asdict(self) -> dict:
-        return {
-            "columns": self.columns,
-            "skip_rows": self.skip_rows,
-            "max_rows": self.max_rows,
-        }
+    def __init__(
+        self,
+        text: TextContent,
+        skills: List[Skill] = [],
+        data: List[Union[Labels, "Output"]] = [],
+    ):
+        super().__init__(
+            text,
+            type="article" if isinstance(text, str) else "conversation",
+            content_type="text/plain" if isinstance(text, str) else "application/json",
+        )
+
+        self.skills = skills
+        for skill, value in zip(skills, data):
+            setattr(self, skill.output_attr or skill.api_name, value)
+
+    def __dir__(self) -> Iterable[str]:
+        return super().__dir__() + [
+            skill.output_attr or skill.api_name for skill in self.skills
+        ]
+
+    def __repr__(self) -> str:
+        result = f"oneai.Output(text={repr(self.text)}"
+        for skill in self.skills:
+            attr = skill.output_attr or skill.api_name
+            result += f", {attr}={repr(getattr(self, attr))}"
+        return result + ")"
+
+
+class BatchResponse:
+    def __init__(self):
+        self._data: Dict[Input, Output] = {}
+
+    def __setitem__(self, key: Input, value: Output):
+        self._data[key] = value
+
+    def __getitem__(self, key: Input) -> Output:
+        return (
+            self._data[key]
+            if isinstance(key, Hashable) and key in self._data
+            else next(v for k, v in self._data.items() if k.text == key)
+        )
```

### Comparing `oneai-0.9.82/src/oneai/exceptions.py` & `oneai-0.9.9/src/oneai/exceptions.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.82/src/oneai/logger.py` & `oneai-0.9.9/src/oneai/logger.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.82/src/oneai/parsing.py` & `oneai-0.9.9/src/oneai/parsing.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.82/src/oneai/pipeline.py` & `oneai-0.9.9/src/oneai/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 import asyncio
 import concurrent.futures
+from io import IOBase
 import os
 import sys
-from typing import Awaitable, Callable, Iterable, List, Union
+from typing import Awaitable, Callable, Dict, Iterable, List
 
 import oneai
-from oneai.classes import (
-    PipelineInput,
-    Skill,
-    TextContent,
-    CSVParams,
-    Input,
-)
-from oneai.output import Output, BatchResponse
-from oneai.process_scheduler import (
-    process_single_input,
-    process_single_input_async,
-    process_batch,
-    task_polling,
-)
+from oneai.classes import BatchResponse, Output, PipelineInput, Skill, TextContent
+from oneai.process_scheduler import *
 
 
 class Pipeline:
     """
     Language AI pipelines allow invoking and chaining multiple Language Skills to process your input text with a single API call.
 
     ## Attributes
@@ -76,16 +65,14 @@
         self.multilingual = multilingual
 
     def run(
         self,
         input: PipelineInput[TextContent],
         api_key: str = None,
         multilingual: bool = False,
-        *,
-        csv_params: CSVParams = None,
     ) -> Output[TextContent]:
         """
         Runs the pipeline on the input text.
 
         ## Parameters
 
         `input: PipelineInput`
@@ -99,84 +86,66 @@
 
         ## Raises
 
         `InputError` if the input is is invalid or is of an incompatible type for the pipeline.
         `APIKeyError` if the API key is invalid, expired, or missing quota.
         `ServerError` if an internal server error occured.
         """
-        input = Input.wrap(input)
         return _async_run_nested(
             process_single_input(
                 input,
                 self.steps,
                 api_key or self.api_key or oneai.api_key,
                 multilingual or self.multilingual or oneai.multilingual,
-                csv_params=csv_params,
             )
         )
 
     async def run_async(
         self,
         input: PipelineInput[TextContent],
         api_key: str = None,
         interval: int = 1,
         multilingual: bool = False,
-        *,
-        csv_params: CSVParams = None,
-        polling: bool = True,
     ) -> Awaitable[Output[TextContent]]:
         """
         Runs the pipeline on the input text asynchronously.
 
         ## Parameters
 
         `input: PipelineInput`
             The input text (or multiple input texts) to be processed.
         `api_key: str, optional`
             An API key to be used in this API call. If not provided, `self.api_key` is used.
-        `interval: int, optional`
-            The number of seconds to wait between polling for results.
-        `polling: bool, optional`
-            Whether to poll for results. If `False`, will return an `Output` object with a `task_id`, and `None` for the rest of the fields.
 
         ## Returns
 
         An Awaitable with an `Output` object containing the results of the Skills in the pipeline.
 
         ## Raises
 
         `InputError` if the input is is invalid or is of an incompatible type for the pipeline.
         `APIKeyError` if the API key is invalid, expired, or missing quota.
         `ServerError` if an internal server error occured.
         """
-        input = Input.wrap(input)
-        return await process_single_input_async(
-            input,
-            self.steps,
-            api_key or self.api_key or oneai.api_key,
-            interval,
-            multilingual or self.multilingual or oneai.multilingual,
-            csv_params=csv_params,
-            polling=polling,
-        )
-
-    async def await_completion(
-        self,
-        task: Union[str, Output],
-        api_key: str = None,
-        interval: int = 1,
-    ) -> Awaitable[Output[TextContent]]:
-        if isinstance(task, Output):
-            task = task.task_id
-        return await task_polling(
-            task,
-            None,
-            api_key or self.api_key or oneai.api_key,
-            self.steps,
-            interval,
+        return await (
+            process_file_async(
+                input,
+                self.steps,
+                api_key or self.api_key or oneai.api_key,
+                interval,
+                multilingual or self.multilingual or oneai.multilingual,
+            )
+            if isinstance(input, io.IOBase)
+            or (isinstance(input, Input) and isinstance(input.text, io.IOBase))
+            else process_single_input(
+                input,
+                self.steps,
+                api_key or self.api_key or oneai.api_key,
+                multilingual or self.multilingual or oneai.multilingual,
+            )
         )
 
     def run_batch(
         self,
         batch: Iterable[PipelineInput[TextContent]],
         api_key: str = None,
         on_output: Callable[
@@ -245,15 +214,15 @@
 
         `InputError` if the input is is invalid or is of an incompatible type for the pipeline.
         `APIKeyError` if the API key is invalid, expired, or missing quota.
         `ServerError` if an internal server error occured.
         """
         outputs = BatchResponse()
         await process_batch(
-            (Input.wrap(i) for i in batch),
+            batch,
             self.steps,
             on_output if on_output else outputs.__setitem__,
             on_error if on_error else outputs.__setitem__,
             api_key=api_key or self.api_key or oneai.api_key,
             multilingual=multilingual or self.multilingual or oneai.multilingual,
         )
         return outputs
```

### Comparing `oneai-0.9.82/src/oneai/process_scheduler.py` & `oneai-0.9.9/src/oneai/process_scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import asyncio
-from datetime import datetime, timedelta
 import io
+from datetime import datetime, timedelta
 import logging
-from typing import Awaitable, Callable, Iterable, List, Tuple, TYPE_CHECKING
+from typing import Awaitable, Callable, Iterable, List
 
 import aiohttp
 
 import oneai
 from oneai.api.output import build_output
-from oneai.api.pipeline import post_pipeline, post_pipeline_async, get_task_status
-from oneai.classes import Input, PipelineInput, Skill, CSVParams
-from oneai.exceptions import ServerError, handle_unsuccessful_response, OneAIError
-from oneai.output import Output
+from oneai.api.pipeline import post_pipeline, post_pipeline_async_file, get_task_status
+from oneai.classes import Input, Output, PipelineInput, Skill
+from oneai.exceptions import ServerError, handle_unsuccessful_response
 
 logger = logging.getLogger("oneai")
 
 
 def time_format(time: timedelta):
     minutes = f"{time.seconds // 60}m " if time.seconds > 59 else ""
     return minutes + f"{time.seconds % 60}s {time.microseconds // 1000}ms"
@@ -23,108 +22,55 @@
 
 STATUS_COMPLETED = "COMPLETED"
 STATUS_FAILED = "FAILED"
 
 
 # open a client session and send a request
 async def process_single_input(
-    input: PipelineInput,
-    steps: List[Skill],
-    api_key: str,
-    multilingual: bool = False,
-    csv_params: CSVParams = None,
+    input: PipelineInput, steps: List[Skill], api_key: str, multilingual: bool = False
 ) -> Awaitable[Output]:
     timeout = aiohttp.ClientTimeout(total=6000)
     async with aiohttp.ClientSession(timeout=timeout) as session:
         return await _run_internal(
-            session, input, steps, api_key, multilingual, csv_params
+            session, Input.wrap(input), steps, api_key, multilingual
         )
 
 
-async def process_single_input_async(
+async def process_file_async(
     input: PipelineInput,
     steps: List[Skill],
     api_key: str,
     interval: int,
     multilingual: bool = False,
-    csv_params: CSVParams = None,
-    polling: bool = True,
 ) -> Awaitable[Output]:
-    if isinstance(input.text, io.TextIOBase):
-        input._make_sync()
+    input = Input.wrap(input, False)
     timeout = aiohttp.ClientTimeout(total=6000)
     async with aiohttp.ClientSession(timeout=timeout) as session:
-        name = f" '{input.text.name}'" if hasattr(input.text, "name") else ""
-        logger.debug(f"Uploading input{name}...")
+        name = input.text.name
+        logger.debug(f"Uploading file '{name}'")
         task_id = (
-            await post_pipeline_async(
-                session, input, steps, api_key, multilingual, csv_params
-            )
+            await post_pipeline_async_file(session, input, steps, api_key, multilingual)
         )["task_id"]
-        logger.debug(f"Upload of input{name} complete\n")
-        return (
-            await task_polling(task_id, session, api_key, steps, interval)
-            if polling
-            else Output(None, steps, task_id=task_id)
-        )
-
+        logger.debug(f"Upload of file '{name}' complete\n")
 
-async def task_polling(
-    task_id: str,
-    session: aiohttp.ClientSession,
-    api_key: str,
-    steps: List[Skill],
-    interval: int,
-) -> Awaitable[Output]:
-    timeout = aiohttp.ClientTimeout(total=6000)
-    close = session is None
-    if session == None:
-        session = aiohttp.ClientSession(timeout=timeout)
-    status, response = "", None
-    start = datetime.now()
-    while status != STATUS_COMPLETED:
-        status, response = await process_task_status(task_id, session, api_key, steps)
-        if status == STATUS_FAILED:
-            raise response
+        status = ""
+        start = datetime.now()
+        while status != STATUS_COMPLETED:
+            if status == STATUS_FAILED:
+                await handle_unsuccessful_response(response["result"])
+            response = await get_task_status(session, task_id, api_key)
+            status = response["status"]
+            logger.debug(
+                f"Processing file '{name}' - status {status} - {time_format(datetime.now() - start)}"
+            )
+            await asyncio.sleep(interval)
         logger.debug(
-            f"Processing input - status {status} - {time_format(datetime.now() - start)}"
+            f"Processing of file '{name}' complete - {time_format(datetime.now() - start)} total\n"
         )
-        await asyncio.sleep(interval)
-    logger.debug(
-        f"Processing of input complete - {time_format(datetime.now() - start)} total\n"
-    )
-    if close:
-        await session.close()
-    return response
-
-
-async def process_task_status(
-    task_id: str,
-    session: aiohttp.ClientSession,
-    api_key: str,
-    steps: List[Skill],
-) -> Awaitable[Tuple[str, Output]]:
-    timeout = aiohttp.ClientTimeout(total=6000)
-    close = session is None
-    if session == None:
-        session = aiohttp.ClientSession(timeout=timeout)
-    response = await get_task_status(session, task_id, api_key)
-    status = response["status"]
-    if status == STATUS_FAILED:
-        try:
-            await handle_unsuccessful_response(response["result"])
-        except OneAIError as e:
-            return status, e
-    elif status == STATUS_COMPLETED:
-        return status, build_output(
-            steps, response["result"], {"x-oneai-request-id": task_id}
-        )
-    if close:
-        await session.close()
-    return status, None
+        return build_output(steps, response["result"])
 
 
 # open a client session with multiple workers and send concurrent requests
 async def process_batch(
     batch: Iterable[PipelineInput],
     steps: List[Skill],
     on_output: Callable[[PipelineInput, Output], None],
@@ -136,15 +82,15 @@
     successful = 0  # total successful responses
     failed = 0  # number of exceptions occurred
     time_total = timedelta()  # total time spent on all requests
     # length = len(batch) if hasattr(batch, "__len__") else 0
 
     def next_input():  # distribute batch to workers
         try:
-            return next(iterator)
+            return Input.wrap(next(iterator))
         except StopIteration:
             return None  # we need to break loop for each worker, so we ignore StopIteration
 
     def log_progress(
         time_delta=timedelta(), start=False, end=False
     ):  # todo progress bar for iterables with __len__
         nonlocal successful, failed, time_total
@@ -156,17 +102,15 @@
             )
         elif end:
             logger.debug(
                 "Processed %d inputs - %s/input - %s total - %d successful - %d failed\n"
                 % (
                     successful + failed,
                     time_format(
-                        time_total
-                        / (successful + failed)
-                        / oneai.MAX_CONCURRENT_REQUESTS
+                        time_total / successful / oneai.MAX_CONCURRENT_REQUESTS
                     ),
                     time_format(time_total / oneai.MAX_CONCURRENT_REQUESTS),
                     successful,
                     failed,
                 )
             )
         else:
@@ -195,15 +139,16 @@
                 successful += 1
             except Exception as e:  # todo: break loop for some error types
                 logger.error(f"Input {successful + failed}: {repr(e)}")
                 on_error(input, e)
                 failed += 1
 
             time_end = datetime.now()
-            log_progress(time_end - time_start)
+            if oneai.PRINT_PROGRESS:
+                log_progress(time_end - time_start)
             time_start = time_end
             input = next_input()
 
     workers = []
     timeout = aiohttp.ClientTimeout(total=6000)
     async with aiohttp.ClientSession(timeout=timeout) as session:
         for _ in range(oneai.MAX_CONCURRENT_REQUESTS):
@@ -227,24 +172,15 @@
 
 async def _run_internal(
     session: aiohttp.ClientSession,
     input: Input,
     skills: List[Skill],
     api_key: str,
     multilingual: bool,
-    csv_params: CSVParams = None,
 ) -> Awaitable[Output]:
     if not skills:  # no skills
         return Output(input.text)
 
     if input.content_type == "text/uri-list":
-        if skills[0].api_name == "html-extract-article" and not skills[0].params.get(
-            "use_proxy"
-        ):
-            input = await fetch_url(session, input.text)
-        else:
-            input.content_type = "text/plain"
+        input = await fetch_url(session, input.text)
 
-    input._make_sync()  # make input compatible with sync API
-    return await post_pipeline(
-        session, input, skills, api_key, multilingual, csv_params
-    )
+    return await post_pipeline(session, input, skills, api_key, multilingual)
```

### Comparing `oneai-0.9.82/src/oneai/skills.py` & `oneai-0.9.9/src/oneai/skills.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,61 @@
+from dataclasses import dataclass
 from typing import List
 from typing_extensions import Literal
+from warnings import warn
 
-from oneai.classes import Labels, Skill, Utterance, skillclass
-from oneai.output import Output
+from oneai.classes import Labels, Skill, Utterance, skillclass, Output
 
 
 @skillclass(
     api_name="enhance",
-    text_attr="proofread",
-    labels_attr="replacements",
+    is_generator=True,
+    label_type="replacement",
+    output_attr="enhanced",
+    output_attr1="replacements",
+)
+class TranscriptionEnhancer(Skill):
+    """
+    Deprecated- use `Proofread` instead
+
+    ## Output Attributes
+
+    `enhanced: Output`
+        An `Output` object containing the enhanced conversation, and output of the following `Skill`s
+    `enhanced.text: str`
+        The enhanced conversation
+    `enhanced.replacements: list[Label]`
+        A list of `Label` objects, representing changes made to the text
+
+    ## Example
+
+    >>> conversation = [oneai.Utterance(...), ...]
+    >>> pipeline = oneai.Pipeline(steps=[
+    ...     oneai.skills.TranscriptionEnhancer()
+    ... ])
+    >>> output = pipeline.run(conversation)
+    >>> output.enhanced
+    oneai.Output(text='ENHANCED TRANSCRIPTION', replacements=[...])
+    """
+
+    def __new__(cls, *args, **kwargs):
+        warn(
+            "TranscriptionEnhancer Skill is deprecated- use `Proofread` instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return super().__new__(cls, *args, **kwargs)
+
+
+@skillclass(
+    api_name="enhance",
+    is_generator=True,
+    label_type="replacement",
+    output_attr="proofread",
+    output_attr1="replacements",
 )
 class Proofread(Skill):
     """
     Enhances conversations, removing fillers and mistakes. Only works with `Conversation` inputs
 
     ## Output Attributes
 
@@ -33,17 +76,20 @@
     >>> output.proofread
     oneai.Output(text='PROOFREAD TRANSCRIPTION', replacements=[...])
     """
 
 
 @skillclass(
     api_name="summarize",
-    text_attr="summary",
-    labels_attr="origins",
+    is_generator=True,
+    label_type="origin",
+    output_attr="summary",
+    output_attr1="origins",
 )
+@dataclass
 class Summarize(Skill):
     """
     Provides a summary of the input
 
     ##  Attributes
 
     `min_length: int`
@@ -68,20 +114,20 @@
     ...     oneai.skills.Summarize(min_length=10, find_origins=True)
     ... ])
     >>> output = pipeline.run('YOUR-TEXT')
     >>> output.summary
     oneai.Output(text='SUMMARY', origins=[...])
     """
 
-    min_length: int = None
-    max_length: int = None
+    min_length: int = 0
+    max_length: int = 0
     find_origins: bool = False
 
 
-@skillclass(api_name="emotions")
+@skillclass(api_name="emotions", label_type="emotion")
 class Emotions(Skill):
     """
     Detects emotions in the input. Supported emotions: [`happiness`, `sadness`, `fear`, `surprise`, `anger`]
 
     ## Output Attributes
 
     `emotions: list[Label]`
@@ -94,15 +140,44 @@
     ... ])
     >>> output = pipeline.run("I'm not interested. Don't call me again!")
     >>> output.emotions
     [oneai.Label(type=emotion, span=[20, 40], name=anger)]
     """
 
 
-@skillclass(api_name="keywords")
+@skillclass(api_name="entities", label_type="entity")
+class Entities(Skill):
+    """
+    Deprecated- use either `Names` or `Numbers` instead
+
+    ## Output Attributes
+
+    `entities: list[Label]`
+        A list of `Label` objects, with detected entities and their type
+
+    ## Example
+
+    >>> pipeline = oneai.Pipeline(steps=[
+    ...     oneai.skills.Entities()
+    ... ])
+    >>> output = pipeline.run('Jim bought shares of Acme Corp.')
+    >>> output.entities
+    [oneai.Label(type=entity, name=PERSON, span=[0, 3], value=Jim), oneai.Label(type=entity, name=ORG, span=[21, 31], value=Acme Corp.)]
+    """
+
+    def __new__(cls, *args, **kwargs):
+        warn(
+            "Entities Skill is deprecated- use either `Names` or `Numbers` instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return super().__new__(cls, *args, **kwargs)
+
+
+@skillclass(api_name="keywords", label_type="keyword")
 class Keywords(Skill):
     """
     Detects keywords in the input
 
     ## Output Attributes
 
     `keywords: list[Label]`
@@ -115,15 +190,15 @@
     ... ])
     >>> output = pipeline.run('I love this app, it helps me to organize my tasks')
     >>> output.keywords
     [oneai.Label(type=keyword, span=[12, 15], value=app), oneai.Label(type=keyword, span=[44, 49], value=tasks)]
     """
 
 
-@skillclass(api_name="highlights")
+@skillclass(api_name="highlights", label_type="highlight")
 class Highlights(Skill):
     """
     Detects highlights of the input
 
     ## Output Attributes
 
     `highlights: list[Label]`
@@ -136,15 +211,15 @@
     ... ])
     >>> output = pipeline.run('YOUR-TEXT')
     >>> output.keywords
     [oneai.Label(value='A-HIGHLIGHT'), ...]
     """
 
 
-@skillclass(api_name="sentiments")
+@skillclass(api_name="sentiments", label_type="sentiment")
 class Sentiments(Skill):
     """
     Detects sentiments in the input
 
     ## Output Attributes
 
     `sentiments: list[Label]`
@@ -157,15 +232,15 @@
     ... ])
     >>> output = pipeline.run('I love this app, it helps me to organize my tasks')
     >>> output.sentiments
     [oneai.Label(type=sentiment, span=[0, 49], value=POS)]
     """
 
 
-@skillclass(api_name="article-topics", labels_attr="topics")
+@skillclass(api_name="article-topics", label_type="topic", output_attr="topics")
 class Topics(Skill):
     """
     Detects topics of the input
 
     ## Output Attributes
 
     `topics: list[Label]`
@@ -179,33 +254,100 @@
     >>> output = pipeline.run('One AI is an NLP platform for developers')
     >>> output.topics
     [oneai.Label(type=topic, value=Machine Learning), oneai.Label(type=topic, value=Artificial Intelligence), ...]
     """
 
 
 @skillclass(
+    api_name="extract-html",
+    is_generator=True,
+    output_attr="html_article",
+)
+class HTMLExtractArticle(Skill):
+    """
+    Extracts the main text content of an HTML page. Accepts URLs or HTML strings
+
+    ## Output
+
+    Main text content from the HTML page
+
+    ## Example
+
+    >>> resp = requests.get('https://oneai.com/about-us/')
+    >>> pipeline = oneai.Pipeline(steps=[
+    ...     oneai.skills.HTMLExtractArticle()
+    ... ])
+    >>> output = pipeline.run(resp.text)
+    >>> output.html_article.text[:100] + '...'
+    One AI - About us
+    ABOUT ONE AI
+    // Bringing human-level language AI to everyday life, one developer a...
+    """
+
+    def __new__(cls, *args, **kwargs):
+        warn(
+            "HTMLExtractArticle Skill is deprecated- use `HtmlToArticle` instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return super().__new__(cls, *args, **kwargs)
+
+
+@skillclass(
     api_name="pdf-extract-text",
-    text_attr="pdf_text",
-    labels_attr="pdf_labels",
+    is_generator=True,
+    output_attr="pdf_text",
 )
 class PDFExtractText(Skill):
     """
     Extracts the text from PDF files.
 
-    ## Output Attributes
+    ## Output
+
+    Main text content from the PDF file
+    """
+
+
+@skillclass(
+    api_name="html-extract-text",
+    is_generator=True,
+    output_attr="html_text",
+)
+class HTMLExtractText(Skill):
+    """
+    Extracts all text content of an HTML page (including text from control elements). Accepts URLs or HTML strings. Use HTMLExtractArticle to extract the main content only
+
+    ## Output
+
+    Text content from the HTML page
 
-    `pdf_text: Output`
-        An `Output` object containing the extracted text, and output of the following `Skill`s
+    ## Example
+
+    >>> resp = requests.get('https://oneai.com/about-us/')
+    >>> pipeline = oneai.Pipeline(steps=[
+    ...     oneai.skills.HTMLExtractText()
+    ... ])
+    >>> output = pipeline.run(resp.text)
+    >>> output.html_text.text[:100] + '...'
+    One AI - About usSkip to main contentAPIStudioSkillsIndustriesPricingResearchAboutAbout UsLeadership...
     """
 
+    def __new__(cls, *args, **kwargs):
+        warn(
+            "HTMLExtractText Skill is deprecated- use `HtmlAllText` instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return super().__new__(cls, *args, **kwargs)
+
 
 @skillclass(
-    api_name="html-extract-article",
-    text_attr="html_article",
-    labels_attr="html_labels",
+    api_name="extract-html",
+    is_generator=True,
+    output_attr="html_article",
 )
 class HtmlToArticle(Skill):
     """
     Extracts the main text content of an HTML page. Accepts URLs or HTML strings
 
     ## Output
 
@@ -223,15 +365,16 @@
     ABOUT ONE AI
     // Bringing human-level language AI to everyday life, one developer a...
     """
 
 
 @skillclass(
     api_name="html-extract-text",
-    text_attr="html_text",
+    is_generator=True,
+    output_attr="html_text",
 )
 class HtmlAllText(Skill):
     """
     Extracts all text content of an HTML page (including text from control elements). Accepts URLs or HTML strings. Use HTMLExtractArticle to extract the main content only
 
     ## Output
 
@@ -245,15 +388,17 @@
     ... ])
     >>> output = pipeline.run(resp.text)
     >>> output.html_text.text[:100] + '...'
     One AI - About usSkip to main contentAPIStudioSkillsIndustriesPricingResearchAboutAbout UsLeadership...
     """
 
 
-@skillclass(api_name="action-items", labels_attr="action_items")
+@skillclass(
+    api_name="action-items", label_type="action-item", output_attr="action_items"
+)
 class ActionItems(Skill):
     """
     ### 'Labs' Skill- this Skill is still in beta and is may produce incorrect results in some cases
 
     Detects action items in the input
 
     ## Output Attributes
@@ -270,16 +415,18 @@
     >>> output.action_items
     [oneai.Label(type=action-item, span=[34, 78], value=Let's schedule another meeting for next Sun.)]
     """
 
 
 @skillclass(
     api_name="anonymize",
-    text_attr="anonymized",
-    labels_attr="anonymizations",
+    is_generator=True,
+    label_type="anonymized",
+    output_attr="anonymized",
+    output_attr1="anonymizations",
 )
 class Anonymize(Skill):
     """
     Anonymize texts, removing personal information
 
     ## Output Attributes
 
@@ -301,16 +448,18 @@
     >>> output.anonymized.anonymizations
     [oneai.Label(type=anonymized, span=[11, 14], value=Michael), oneai.Label(type=anonymized, span=[28, 31], value=michael@abcde.com)]
     """
 
 
 @skillclass(
     api_name="business-entities",
-    text_attr="labs",
-    labels_attr="pricing",
+    is_generator=True,
+    label_type="business-entity",
+    output_attr="labs",
+    output_attr1="pricing",
 )
 class Pricing(Skill):
     """
     ### 'Labs' Skill- this Skill is still in beta and is may produce incorrect results in some cases
 
     Detects pricing and quantities in the input
 
@@ -326,15 +475,16 @@
     ... ])
     >>> output = pipeline.run('it costs 10 USD per barrel')
     >>> output.labs.pricing
     [oneai.Label(name=pricing, data={'amount': 10.0, 'currency': 'USD', 'unit': 'barrel'}, span=[9, 26], value=10 USD per barrel)]
     """
 
 
-@skillclass(api_name="names")
+@skillclass(api_name="names", label_type="name")
+@dataclass
 class Names(Skill):
     """
     Detects and classifies names in the input
 
     ## Output Attributes
 
     `names: list[Label]`
@@ -350,15 +500,15 @@
     [oneai.Label(type=entity, name=PERSON, span=[0, 3], value=Jim), oneai.Label(type=entity, name=ORG, span=[21, 31], value=Acme Corp.)]
     """
 
     enrichment: bool = False
     amount: Literal["more", "less", "normal"] = None
 
 
-@skillclass(api_name="numbers")
+@skillclass(api_name="numbers", label_type="number")
 class Numbers(Skill):
     """
     Detects and classifies numbers and dates in the input
 
     ## Output Attributes
 
     `entities: list[Label]`
@@ -370,15 +520,15 @@
     ...     oneai.skills.Numbers()
     ... ])
     >>> output = pipeline.run('Jim bought shares of Acme Corp.')
     >>> output.numbers
     """
 
 
-@skillclass(api_name="sentences")
+@skillclass(api_name="sentences", label_type="sentence")
 class SplitBySentence(Skill):
     """
     Splits input by sentence
 
     ## Output Attributes
 
     `sentences: list[Label]`
@@ -392,16 +542,18 @@
     >>> output = pipeline.run('...')
     >>> output.sentences
     """
 
 
 @skillclass(
     api_name="dialogue-segmentation",
-    labels_attr="segments",
+    label_type="dialogue-segment",
+    output_attr="segments",
 )
+@dataclass
 class SplitByTopic(Skill):
     """
     Splits input by discussed topics
 
     ## Output Attributes
 
     `segments: list[Label]`
@@ -412,20 +564,22 @@
     >>> pipeline = oneai.Pipeline(steps=[
     ...     oneai.skills.SplitByTopic()
     ... ])
     >>> output = pipeline.run('...')
     >>> output.segments
     """
 
-    std_ratio: float = None
+    std_ratio: float = 0
     amount: Literal["more", "less", "normal"] = None
     use_discourse_parser: bool = False
 
 
-@skillclass(api_name="sales-insights", labels_attr="sales_insights")
+@skillclass(
+    api_name="sales-insights", label_type="sales-insights", output_attr="sales_insights"
+)
 class SalesInsights(Skill):
     """
     Splits input by discussed topics
 
     ## Output Attributes
 
     `sales_insights: list[Label]`
@@ -439,15 +593,16 @@
     >>> output = pipeline.run('...')
     >>> output.sales_insights
     """
 
 
 @skillclass(
     api_name="service-email-insights",
-    labels_attr="service_insights",
+    label_type="service-email-insights",
+    output_attr="service_insights",
 )
 class ServiceInsights(Skill):
     """
     Finds spans in the text with Service Insights.
 
     ## Output Attributes
 
@@ -462,15 +617,16 @@
     >>> output = pipeline.run('...')
     >>> output.service_insights
     """
 
 
 @skillclass(
     api_name="service-email-insights",
-    labels_attr="email_insights",
+    label_type="service-email-insights",
+    output_attr="email_insights",
 )
 class EmailInsights(Skill):
     """
     Finds spans in the text with Email Insights.
 
     ## Output Attributes
 
@@ -483,15 +639,17 @@
     ...     oneai.skills.EmailInsights()
     ... ])
     >>> output = pipeline.run('...')
     >>> output.email_insights
     """
 
 
-@skillclass(api_name="detect-language", labels_attr="language")
+@skillclass(
+    api_name="detect-language", label_type="detect-language", output_attr="language"
+)
 class DetectLanguage(Skill):
     """
     Detects language of input
 
     ## Output Attributes
 
     `language: list[Label]`
@@ -503,15 +661,15 @@
     ...     oneai.skills.DetectLanguage()
     ... ])
     >>> output = pipeline.run('...')
     >>> output.language[0]
     """
 
 
-@skillclass(api_name="headline")
+@skillclass(api_name="headline", label_type="headline")
 class Headline(Skill):
     """
     Generates a headline based on input
 
     ## Output Attributes
 
     `headline: list[Label]`
@@ -523,15 +681,15 @@
     ...     oneai.skills.Headline()
     ... ])
     >>> output = pipeline.run('...')
     >>> output.headline[0]
     """
 
 
-@skillclass(api_name="subheading")
+@skillclass(api_name="subheading", label_type="subheading", output_attr="subheading")
 class Subheading(Skill):
     """
     Generates a subheading based on input
 
     ## Output Attributes
 
     `subheading: list[Label]`
@@ -545,17 +703,19 @@
     >>> output = pipeline.run('...')
     >>> output.subheading[0]
     """
 
 
 @skillclass(
     api_name="transcribe",
-    text_attr="transcription",
-    labels_attr="words",
+    is_generator=True,
+    output_attr="transcription",
+    output_attr1="words",
 )
+@dataclass
 class Transcribe(Skill):
     """
     Transcribes audio files
 
     ## Output
 
     Speech-to-text transcription of the audio data
@@ -573,174 +733,43 @@
 
     speaker_detection: bool = True
     timestamp_per_word: bool = False
     engine: Literal["default", "whisper"] = "default"
 
 
 @skillclass(api_name="clustering")
+@dataclass
 class Clustering(Skill):
     """
     Automatically organizes various skill labels in clusters for later analytics
 
     ## Example
 
     >>> pipeline = oneai.Pipeline(steps=[
     ...     oneai.skills.Sentiments(),
     ...     oneai.skills.Clustering(),
     ... ])
     >>> pipeline.run(input)
     """
 
     collection: str = ""
-    """The name of the collection to insert the input into"""
-    input_skill: str = ""
-    """Use the output of a Skill as input for clustering, omit to use the input directly"""
-
-    def __post_init__(self):
-        if self.collection:
-            object.__setattr__(self, "labels_attr", "status")
-        else:
-            object.__setattr__(self, "labels_attr", "clusters")
-
-
-@skillclass(api_name="clustering", labels_attr="status")
-class CollectionInsert(Skill):
-    """
-    Insert input into a collection
-
-    ## Example
-
-    >>> pipeline = oneai.Pipeline(steps=[
-    ...     oneai.skills.Sentiments(),
-    ...     oneai.skills.Clustering(
-    ...         collection="my_collection",
-    ...         input_skill=oneai.skills.Sentiments(),
-    ...     ),
-    ... ])
-    >>> pipeline.run(input)
-    """
-
-    collection: str = ""
-    """The name of the collection to insert the input into"""
     input_skill: str = ""
-    """Use the output of a Skill as input for clustering, omit to use the input directly"""
-
-
-@skillclass(api_name="collection-search", labels_attr="matches")
-class CollectionSearch(Skill):
-    """
-    Find most matching items in a collection. Results are grouped in phrases.
-
-    ## Example
-
-    >>> pipeline = oneai.Pipeline(steps=[
-    ...     oneai.skills.CollectionSearch(
-    ...         collection="my_collection",
-    ...     ),
-    ... ])
-    >>> pipeline.run(input)
-    """
-
-    collection: str = ""
-    """The name of the collection to insert the input into"""
-    max_items: int = 1
-    """Maximum number of items per phrase to return"""
-    max_phrases: int = 3
-    """Maximum number of phrases to return"""
-    sort_by: Literal["similarity", "position"] = "similarity"
-    """Sort results by similarity to input or by position in original text when inserted"""
-
-
-@skillclass(api_name="gpt")
-class GPT(Skill):
-    """
-    Generate text using GPT-3
-
-    ## Output Attributes
-
-    `gpt_text: str`
-        The generated text
-
-    `gpt_labels: list[Label]`
-        Labels generated by GPT. Only available if `prompt_fields` is set.
-
-    ## Example
-
-    >>> pipeline = oneai.Pipeline(steps=[
-    ...     oneai.skills.GPT()
-    ... ])
-    >>> output = pipeline.run('...')
-    >>> output.gpt_text
-    """
-
-    model: Literal[
-        "text-davinci-003",
-        "text-curie-001",
-        "text-babbage-001",
-        "text-ada-001",
-        "gpt-3-5-turbo",
-        "gpt-4",
-    ] = "gpt-3-5-turbo"
-    input_skill: str = None
-    prompt: str = None
-    prompt_position: Literal["start", "end"] = "start"
-    temperature: float = None
-    get_api_key: str = None
-    prompt_fields: List[str] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        if self.prompt_fields is None:
-            self.text_attr = "gpt_text"
-        else:
-            self.labels_attr = "gpt_labels"
-
-
-@skillclass(api_name="classify", labels_attr="classification")
-class Classify(Skill):
-    """
-    Classifies input based on an analytics collection
-
-    ## Output Attributes
-
-    `classification: list[Label]`
-        A list of `Label` objects, containing the classification
-
-    ## Example
-
-    >>> pipeline = oneai.Pipeline(steps=[
-    ...     oneai.skills.Classify(collection='my_collection')
-    ... ])
-    >>> output = pipeline.run('...')
-    >>> output.classification[0]
-    """
-
-    collection: str = ""
-    """The name of the collection to use for classification"""
-    key: str = ""
-    """The key to use for classification"""
-    input_skill: str = ""
-    """Use the output of a Skill as input for classification, omit to use the input directly"""
 
 
 class OutputAttrs:
     summary: "Output[str]" = None
     proofread: "Output[List[Utterance]]" = None
     html_article: "Output[str]" = None
     html_text: "Output[str]" = None
-    html_labels: Labels = None
     pdf_text: "Output[str]" = None
-    pdf_labels: Labels = None
     transcription: "Output[List[Utterance]]" = None
     anonymized: "Output" = None
     words: Labels = None
     emotions: Labels = None
     names: Labels = None
-    clusters: Labels = None
-    status: Labels = None
     numbers: Labels = None
     keywords: Labels = None
     highlights: Labels = None
     sentiments: Labels = None
     topics: Labels = None
     sales_insights: Labels = None
     service_insights: Labels = None
@@ -750,13 +779,7 @@
     origins: Labels = None
     segments: Labels = None
     sentences: Labels = None
     anonymizations: Labels = None
     language: Labels = None
     headline: Labels = None
     subheading: Labels = None
-    classification: Labels = None
-    gpt_text: Output = None
-    gpt_labels: Labels = None
-    matches: Labels = None
-
-    outputs: List["Output"] = None
```

### Comparing `oneai-0.9.82/src/oneai/util.py` & `oneai-0.9.9/src/oneai/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import asyncio
 import oneai
-from typing import List, Optional, Union, Dict, Any
+from typing import List, Optional, Union
 from typing_extensions import Literal
 from dataclasses import dataclass
 
 
 @dataclass
 class Chapter:
     subheading: str
@@ -27,25 +26,22 @@
     ]
 
 
 def generate_chapters(
     input: oneai.PipelineInput,
     amount: Literal["more", "less", "normal"] = None,
     preprocessing: Optional[oneai.Skill] = None,
-    *,
-    params: Dict[str, Any] = None,
 ) -> List[Chapter]:
-    split_by_topic = oneai.skills.SplitByTopic(amount=amount, params=params)
-    output = asyncio.run(
-        oneai.Pipeline([split_by_topic]).run_async(input)
+    output = (
+        oneai.Pipeline([oneai.skills.SplitByTopic(amount=amount)]).run(input)
         if not preprocessing
-        else oneai.Pipeline([preprocessing, split_by_topic]).run_async(input)
+        else oneai.Pipeline([preprocessing, oneai.skills.SplitByTopic(amount=amount)])
+        .run(input)
+        .__getattribute__(preprocessing.output_attr)
     )
-    if preprocessing:
-        output = output.__getattribute__(preprocessing.output_attr)
     spans = [span_text(output.text, seg) for seg in output.segments]
     summaries = oneai.Pipeline([oneai.skills.Summarize()]).run_batch(spans)
     return [
         Chapter(
             subheading=seg.data["subheading"],
             text=span,
             summary=summaries[span].summary.text,
```

