# Comparing `tmp/reconify-1.0.1.tar.gz` & `tmp/reconify-1.0.2.tar.gz`

## Comparing `reconify-1.0.1.tar` & `reconify-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reconify-1.0.1/src/reconify/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 reconify-1.0.1/src/reconify/reconifyOpenAIHandler.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 reconify-1.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 reconify-1.0.1/LICENSE
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 reconify-1.0.1/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 reconify-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 reconify-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reconify-1.0.2/src/reconify/__init__.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 reconify-1.0.2/src/reconify/reconifyOpenAIHandler.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 reconify-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 reconify-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 reconify-1.0.2/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 reconify-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 reconify-1.0.2/PKG-INFO
```

### Comparing `reconify-1.0.1/.gitignore` & `reconify-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `reconify-1.0.1/LICENSE` & `reconify-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reconify-1.0.1/README.md` & `reconify-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -40,15 +40,29 @@
    appKey = 'Your_App_Key', 
    apiKey = 'Your_Api_Key'
 )
 ```
 
 This is all that is needed for a basic integration. The module takes care of sending the correct data to Reconify when you call openai.Completion.create or openai.ChatCompletion.create. 
 
-There are additional optional parameters as well:
+#### Optional Config Parameters 
+There are additional optional parameters that can be passed in to the handler. 
+
++ debug: (default False) Enable/Disable console logging
++ trackImages: (default True) Turn on/off tracking of createImage 
+
+For example:
+
+```python
+reconifyOpenAIHandler.config(openai, 
+   appKey = 'Your_App_Key', 
+   apiKey = 'Your_Api_Key',
+   debug = True
+)
+```
 
 ### Optional methods
 
 You can optionally pass in a user object or session ID to be used in the analytics reporting. 
 The session ID will be used to group interactions together in the same session transcript.
 
 #### Set a user
@@ -132,7 +146,34 @@
 response = openai.Completion.create(
    model = "text-davinci-003",
    prompt = "write a haiku about cats",
    max_tokens = 100,
    temperature = 0,
 )
 ```
+
+### Image Example
+
+```python
+import os
+import openai
+from reconify import reconifyOpenAIHandler
+
+openai.api_key = 'YOUR_OPENAI_KEY'
+
+reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key')
+
+reconifyOpenAIHandler.setUser({
+   "userId": "12345",
+   "isAuthenticated": 1,
+   "firstName": "Jim",
+   "lastName": "Stand",
+   "gender": "male"
+})
+
+response = openai.Image.create(
+   prompt = "a cat on the moon",
+   n = 1,
+   size = "256x256"
+   response_format = "url"
+)
+```
```

### Comparing `reconify-1.0.1/pyproject.toml` & `reconify-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "reconify"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Reconify Team", email="services@reconify.com" },
 ]
 description = "A package for sending data to the Reconify platform"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `reconify-1.0.1/PKG-INFO` & `reconify-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconify
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for sending data to the Reconify platform
 Project-URL: Homepage, https://github.com/reconify-com/reconify-pip#readme
 Project-URL: Bug Tracker, https://github.com/reconify-com/reconify-pip/issues
 Author-email: Reconify Team <services@reconify.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,15 +54,29 @@
    appKey = 'Your_App_Key', 
    apiKey = 'Your_Api_Key'
 )
 ```
 
 This is all that is needed for a basic integration. The module takes care of sending the correct data to Reconify when you call openai.Completion.create or openai.ChatCompletion.create. 
 
-There are additional optional parameters as well:
+#### Optional Config Parameters 
+There are additional optional parameters that can be passed in to the handler. 
+
++ debug: (default False) Enable/Disable console logging
++ trackImages: (default True) Turn on/off tracking of createImage 
+
+For example:
+
+```python
+reconifyOpenAIHandler.config(openai, 
+   appKey = 'Your_App_Key', 
+   apiKey = 'Your_Api_Key',
+   debug = True
+)
+```
 
 ### Optional methods
 
 You can optionally pass in a user object or session ID to be used in the analytics reporting. 
 The session ID will be used to group interactions together in the same session transcript.
 
 #### Set a user
@@ -146,7 +160,34 @@
 response = openai.Completion.create(
    model = "text-davinci-003",
    prompt = "write a haiku about cats",
    max_tokens = 100,
    temperature = 0,
 )
 ```
+
+### Image Example
+
+```python
+import os
+import openai
+from reconify import reconifyOpenAIHandler
+
+openai.api_key = 'YOUR_OPENAI_KEY'
+
+reconifyOpenAIHandler.config(openai, 'Your_App_Key', 'Your_Api_Key')
+
+reconifyOpenAIHandler.setUser({
+   "userId": "12345",
+   "isAuthenticated": 1,
+   "firstName": "Jim",
+   "lastName": "Stand",
+   "gender": "male"
+})
+
+response = openai.Image.create(
+   prompt = "a cat on the moon",
+   n = 1,
+   size = "256x256"
+   response_format = "url"
+)
+```
```

