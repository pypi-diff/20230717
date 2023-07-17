# Comparing `tmp/cyberwatch_api-0.3.0.tar.gz` & `tmp/cyberwatch_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyberwatch_api-0.3.0.tar", last modified: Mon Jun 26 08:01:07 2023, max compression
+gzip compressed data, was "dist/cyberwatch_api-0.3.1.tar", last modified: Mon Jul 17 09:30:11 2023, max compression
```

## Comparing `cyberwatch_api-0.3.0.tar` & `cyberwatch_api-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/cyberwatch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-17 09:30:01.000000 cyberwatch_api-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-17 09:30:01.000000 cyberwatch_api-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/cyberwatch_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-17 09:30:01.000000 cyberwatch_api-0.3.1/cyberwatch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:30:11.000000 cyberwatch_api-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 09:30:01.000000 cyberwatch_api-0.3.1/setup.py
```

### Comparing `cyberwatch_api-0.3.0/LICENSE` & `cyberwatch_api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberwatch_api-0.3.0/PKG-INFO` & `cyberwatch_api-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberwatch_api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Api client for the Cyberwatch software
 Author: CyberWatch SAS
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cyberwatch API
@@ -101,43 +101,55 @@
 ## Usage
 **Swagger documentation**
 
 Cyberwatch API provides a Swagger documentation.
 
 Using it, you can :
  * Select the action you want to perform in the documentation
- * Update the "method", "endpoint" and parameters ("params") in you script according to the documentation 
+ * Update the "method", "endpoint" and parameters ("body_params") in you script according to the documentation 
  * Add any required logic
 
 Note that the `request` method provided by this module always outputs a generator. This is intended to allow building of high performance scripts. If the request you perform returns a single result and not a list, you will find the result in the first row of this generator.
 
 **Location of the Swagger's documentation**
 
 You can find it while clicking on the </> logo on the top right of the Cyberwatch interface.
 
-**Request body parameters**
+**Request parameters**
 
-When using this API, you need to distinguish between GET/DELETE and POST/PUT methods.
+When using this API, you can use the `body_params` variable to send parameters to your endpoint.
 
-For the GET/DELETE methods you need to use the `params` variable, while for the POST/PUT methods, you need to use the `body_params` variable as follows:
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="get",
-    endpoint="/api/v3/assets/servers/{id}",
-    params={'id' : 7}
+    endpoint="/api/v3/vulnerabilities/servers/{id}",
+    body_params={'id' : 7}
 )
 ```
+
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
     body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
 
+**Paginate the response**
+
+You can select how many elements are returned per-page using the `per_page` parameter. If you need only a single page to be returned, you may specify it using the `page` parameter. 
+
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/agents",
+    body_params={'per_page' : 50, 'page' : 3}
+)
+```
+
 ## FAQs
 
 **What if I don't want to verify the SSL certificate?**
 
 Error example:
```

### Comparing `cyberwatch_api-0.3.0/README.md` & `cyberwatch_api-0.3.1/cyberwatch_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: cyberwatch-api
+Version: 0.3.1
+Summary: Python Api client for the Cyberwatch software
+Author: CyberWatch SAS
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cyberwatch API
 
 Python Api client for the Cyberwatch software
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 **Table of Contents** 
 
@@ -92,43 +101,55 @@
 ## Usage
 **Swagger documentation**
 
 Cyberwatch API provides a Swagger documentation.
 
 Using it, you can :
  * Select the action you want to perform in the documentation
- * Update the "method", "endpoint" and parameters ("params") in you script according to the documentation 
+ * Update the "method", "endpoint" and parameters ("body_params") in you script according to the documentation 
  * Add any required logic
 
 Note that the `request` method provided by this module always outputs a generator. This is intended to allow building of high performance scripts. If the request you perform returns a single result and not a list, you will find the result in the first row of this generator.
 
 **Location of the Swagger's documentation**
 
 You can find it while clicking on the </> logo on the top right of the Cyberwatch interface.
 
-**Request body parameters**
+**Request parameters**
 
-When using this API, you need to distinguish between GET/DELETE and POST/PUT methods.
+When using this API, you can use the `body_params` variable to send parameters to your endpoint.
 
-For the GET/DELETE methods you need to use the `params` variable, while for the POST/PUT methods, you need to use the `body_params` variable as follows:
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="get",
-    endpoint="/api/v3/assets/servers/{id}",
-    params={'id' : 7}
+    endpoint="/api/v3/vulnerabilities/servers/{id}",
+    body_params={'id' : 7}
 )
 ```
+
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
     body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
 
+**Paginate the response**
+
+You can select how many elements are returned per-page using the `per_page` parameter. If you need only a single page to be returned, you may specify it using the `page` parameter. 
+
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/agents",
+    body_params={'per_page' : 50, 'page' : 3}
+)
+```
+
 ## FAQs
 
 **What if I don't want to verify the SSL certificate?**
 
 Error example:
```

### Comparing `cyberwatch_api-0.3.0/cyberwatch_api.egg-info/PKG-INFO` & `cyberwatch_api-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: cyberwatch-api
-Version: 0.3.0
-Summary: Python Api client for the Cyberwatch software
-Author: CyberWatch SAS
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cyberwatch API
 
 Python Api client for the Cyberwatch software
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 **Table of Contents** 
 
@@ -101,43 +92,55 @@
 ## Usage
 **Swagger documentation**
 
 Cyberwatch API provides a Swagger documentation.
 
 Using it, you can :
  * Select the action you want to perform in the documentation
- * Update the "method", "endpoint" and parameters ("params") in you script according to the documentation 
+ * Update the "method", "endpoint" and parameters ("body_params") in you script according to the documentation 
  * Add any required logic
 
 Note that the `request` method provided by this module always outputs a generator. This is intended to allow building of high performance scripts. If the request you perform returns a single result and not a list, you will find the result in the first row of this generator.
 
 **Location of the Swagger's documentation**
 
 You can find it while clicking on the </> logo on the top right of the Cyberwatch interface.
 
-**Request body parameters**
+**Request parameters**
 
-When using this API, you need to distinguish between GET/DELETE and POST/PUT methods.
+When using this API, you can use the `body_params` variable to send parameters to your endpoint.
 
-For the GET/DELETE methods you need to use the `params` variable, while for the POST/PUT methods, you need to use the `body_params` variable as follows:
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="get",
-    endpoint="/api/v3/assets/servers/{id}",
-    params={'id' : 7}
+    endpoint="/api/v3/vulnerabilities/servers/{id}",
+    body_params={'id' : 7}
 )
 ```
+
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
     body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
 
+**Paginate the response**
+
+You can select how many elements are returned per-page using the `per_page` parameter. If you need only a single page to be returned, you may specify it using the `page` parameter. 
+
+```python
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/agents",
+    body_params={'per_page' : 50, 'page' : 3}
+)
+```
+
 ## FAQs
 
 **What if I don't want to verify the SSL certificate?**
 
 Error example:
```

### Comparing `cyberwatch_api-0.3.0/cyberwatch_api.py` & `cyberwatch_api-0.3.1/cyberwatch_api.py`

 * *Files identical despite different names*

