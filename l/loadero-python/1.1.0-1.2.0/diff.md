# Comparing `tmp/loadero_python-1.1.0.tar.gz` & `tmp/loadero_python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadero_python-1.1.0.tar", last modified: Tue Jan  3 09:18:08 2023, max compression
+gzip compressed data, was "loadero_python-1.2.0.tar", last modified: Mon Jul 17 15:25:39 2023, max compression
```

## Comparing `loadero_python-1.1.0.tar` & `loadero_python-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 09:18:08.011491 loadero_python-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34754 2023-01-03 09:17:47.000000 loadero_python-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-03 09:17:47.000000 loadero_python-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-01-03 09:18:08.011491 loadero_python-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-01-03 09:17:47.000000 loadero_python-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 09:18:08.007492 loadero_python-1.1.0/loadero_python/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 09:18:08.011491 loadero_python-1.1.0/loadero_python/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/assert_precondition.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/assert_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/classificator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/metric_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    32353 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/run_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-01-03 09:17:47.000000 loadero_python-1.1.0/loadero_python/resources/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 09:18:08.007492 loadero_python-1.1.0/loadero_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-01-03 09:18:07.000000 loadero_python-1.1.0/loadero_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-03 09:18:08.000000 loadero_python-1.1.0/loadero_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 09:18:07.000000 loadero_python-1.1.0/loadero_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-03 09:18:07.000000 loadero_python-1.1.0/loadero_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-03 09:18:07.000000 loadero_python-1.1.0/loadero_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-03 09:17:47.000000 loadero_python-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-03 09:18:08.011491 loadero_python-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-03 09:17:47.000000 loadero_python-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:39.856951 loadero_python-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34754 2023-07-17 15:25:30.000000 loadero_python-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 15:25:30.000000 loadero_python-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-07-17 15:25:39.856951 loadero_python-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-17 15:25:30.000000 loadero_python-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:39.852951 loadero_python-1.2.0/loadero_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:39.856951 loadero_python-1.2.0/loadero_python/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17206 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/assert_precondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/assert_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/classificator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30849 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/metric_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21557 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/run_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24883 2023-07-17 15:25:30.000000 loadero_python-1.2.0/loadero_python/resources/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:39.852951 loadero_python-1.2.0/loadero_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-07-17 15:25:39.000000 loadero_python-1.2.0/loadero_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 15:25:39.000000 loadero_python-1.2.0/loadero_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:25:39.000000 loadero_python-1.2.0/loadero_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 15:25:39.000000 loadero_python-1.2.0/loadero_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 15:25:39.000000 loadero_python-1.2.0/loadero_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 15:25:30.000000 loadero_python-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 15:25:39.856951 loadero_python-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 15:25:30.000000 loadero_python-1.2.0/setup.py
```

### Comparing `loadero_python-1.1.0/LICENSE.md` & `loadero_python-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `loadero_python-1.1.0/PKG-INFO` & `loadero_python-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadero_python
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python client for Loadero API
 Home-page: https://github.com/loadero/loadero-python
 Author: Loadero Team
 Author-email: support@loadero.com
 License: GPLv3
 Project-URL: Documentation, https://loadero.github.io/loadero-python/
 Project-URL: Source, https://github.com/loadero/loadero-python
@@ -72,21 +72,15 @@
 ```
 
 ## Usage
 
 ### API Access
 
 Before using the Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting support. More information about the
-API can be found in the
-[Loadero wiki](https://wiki.loadero.com/loadero-usage/api/).
-
-Before using Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting
-[support](mailto:support@loadero.com?subject=I%20want%20to%20request%20project%20access%20token%20for%20API).
+This can be done in the projects settings page in Loadero web-app.
 More information about the API can be found in the
 [Loadero wiki](https://wiki.loadero.com/loadero-usage/api/)
 
 **Note** Access tokens are project specific and cannot be used across multiple
 projects. Make sure to specify the project ID in the request for an access
 token.
```

### Comparing `loadero_python-1.1.0/README.md` & `loadero_python-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,15 @@
 ```
 
 ## Usage
 
 ### API Access
 
 Before using the Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting support. More information about the
-API can be found in the
-[Loadero wiki](https://wiki.loadero.com/loadero-usage/api/).
-
-Before using Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting
-[support](mailto:support@loadero.com?subject=I%20want%20to%20request%20project%20access%20token%20for%20API).
+This can be done in the projects settings page in Loadero web-app.
 More information about the API can be found in the
 [Loadero wiki](https://wiki.loadero.com/loadero-usage/api/)
 
 **Note** Access tokens are project specific and cannot be used across multiple
 projects. Make sure to specify the project ID in the request for an access
 token.
```

### Comparing `loadero_python-1.1.0/loadero_python/api_client.py` & `loadero_python-1.2.0/loadero_python/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,14 +165,50 @@
             raise APIException(f"Loadero API request failed: {resp.data}")
 
         if len(resp.data) == 0:
             return None
 
         return json.loads(resp.data)
 
+    def get_raw(self, url, dest):
+        """Sends a HTTP GET request to Loadero API. Writes raw response to
+        destination
+
+        Args:
+            url (str): URL to a Loadero resource.
+
+            dest: Destination where request response is going to be written.
+                Must implement write method from file interface.
+
+        Raises:
+            APIException: When Loadero API request fails. Either because of
+                client error or server error.
+        """
+
+        req = self.__http.request(
+            method="GET",
+            url=url,
+            headers=self._build_headers(),
+            preload_content=False,
+        )
+
+        while True:
+            data = req.read(256)
+            if not data:
+                break
+
+            dest.write(data)
+
+        req.release_conn()
+
+        if req.status // 100 != 2:
+            raise APIException(
+                f"Loadero API request failed with status code {req.status}"
+            )
+
     def post(self, route: str, body: dict) -> dict or None:
         """Sends a HTTP POST request to Loadero API.
 
         Args:
             route (str): Loadero API route.
 
             body (dict): Request JSON body decoded as dictionary.
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/__init__.py` & `loadero_python-1.2.0/loadero_python/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `loadero_python-1.1.0/loadero_python/resources/assert_precondition.py` & `loadero_python-1.2.0/loadero_python/resources/assert_precondition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Loadero assert resource.
 
 Assert resource is seperated into three parts
-    - AssertPreconditionParams class describes assert preconditions attributes
+    AssertPreconditionParams class describes assert preconditions attributes
 
-    - AssertPreconditionAPI class that groups all API operations with assert
+    AssertPreconditionAPI class that groups all API operations with assert
     preconditions attributes.
 
-    - AssertPrecondition class combines AssertPreconditionParams and
+    AssertPrecondition class combines AssertPreconditionParams and
     AssertPreconditionAPI.
 
 Single AssertPrecondition object coresponds to a single assert precondition in
 Loadero.
 """
 
 from __future__ import annotations
@@ -262,19 +262,20 @@
         super().__init__(self.params)
 
     def create(self) -> AssertPrecondition:
         """Creates new assert precondition with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
-            - expected
-            - operator
-            - property
+
+        - test_id
+        - assert_id
+        - expected
+        - operator
+        - property
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -287,17 +288,18 @@
         return self
 
     def read(self) -> AssertPrecondition:
         """Reads information about an existing assert precondition.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
-            - assert_precondition_id
+
+        - test_id
+        - assert_id
+        - assert_precondition_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -310,20 +312,21 @@
         return self
 
     def update(self) -> AssertPrecondition:
         """Updates assert precondition with given parameters.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
-            - assert_precondition_id
-            - expected
-            - operator
-            - property
+
+        - test_id
+        - assert_id
+        - assert_precondition_id
+        - expected
+        - operator
+        - property
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -336,17 +339,18 @@
         return self
 
     def delete(self) -> AssertPrecondition:
         """Deletes and existing assert precondition.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
-            - assert_precondition_id
+
+        - test_id
+        - assert_id
+        - assert_precondition_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
         """
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/assert_resource.py` & `loadero_python-1.2.0/loadero_python/resources/assert_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loadero assert resource.
 
 Assert resource is seperated into three parts
-    - AssertParams class describes assert attributes
+    AssertParams class describes assert attributes
 
-    - AssertAPI class that groups all API operations with assert resource.
+    AssertAPI class that groups all API operations with assert resource.
 
-    - Assert class that combines AssertParams and AssertAPI.
+    Assert class that combines AssertParams and AssertAPI.
 
 Single Assert object coresponds to single assert in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from dateutil import parser
@@ -232,18 +232,19 @@
         super().__init__(self.params)
 
     def create(self) -> Assert:
         """Creates new assert with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - expected
-            - operator
-            - path
+
+        - test_id
+        - expected
+        - operator
+        - path
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -256,16 +257,17 @@
         return self
 
     def read(self) -> Assert:
         """Reads information about an existing assert.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
+
+        - test_id
+        - assert_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -278,19 +280,20 @@
         return self
 
     def update(self) -> Assert:
         """Updates assert with given parameters.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
-            - expected
-            - operator
-            - path
+
+        - test_id
+        - assert_id
+        - expected
+        - operator
+        - path
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -303,16 +306,17 @@
         return self
 
     def delete(self) -> None:
         """Deletes and existing assert.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
+
+        - test_id
+        - assert_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
         """
@@ -320,16 +324,17 @@
         AssertAPI.delete(self.params)
 
     def duplicate(self) -> Assert:
         """Duplicates and existing assert.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
+
+        - test_id
+        - assert_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -349,16 +354,17 @@
     def preconditions(
         self, query_params: QueryParams or None = None
     ) -> list[AssertPrecondition]:
         """Read all preconditions of assert.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - assert_id
+
+        - test_id
+        - assert_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Assert.params.test_id must be a valid int
 
@@ -401,15 +407,16 @@
         """Create a new assert resource.
 
         Args:
             params (AssertParams): Describes the assert resource to be created.
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
-                resource or resource params required attributes are None.
+            resource or resource params required attributes are None.
+
             APIException: If API call fails.
 
         Returns:
             AssertParams: Created assert resource.
         """
 
         AssertAPI.__validate_identifiers(params, False)
@@ -423,15 +430,16 @@
         """Read an existing assert resource.
 
         Args:
             params (AssertParams): Describes the assert resource to read.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource.
+            resource.
+
             APIException: If API call fails.
 
         Returns:
             AssertParams: Read assert resource.
         """
 
         AssertAPI.__validate_identifiers(params)
@@ -445,15 +453,16 @@
         """Update an existing assert resource.
 
         Args:
             params (AssertParams): Describes the assert resource to update.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource or resource params required attributes are None.
+            resource or resource params required attributes are None.
+
             APIException: If API call fails.
 
         Returns:
             AssertParams: Updated assert resource.
         """
 
         AssertAPI.__validate_identifiers(params)
@@ -470,15 +479,16 @@
         """Delete an existing assert resource.
 
         Args:
             params (AssertParams): Describes the assert resource to delete.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource.
+            resource.
+
             APIException: If API call fails.
         """
 
         AssertAPI.__validate_identifiers(params)
 
         APIClient().delete(AssertAPI.route(params.test_id, params.assert_id))
 
@@ -488,15 +498,16 @@
 
         Args:
             params (AssertParams): Describe the assert resource to duplicate and
             the name of duplicate assert resource.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource.
+            resource.
+
             APIException: If API call fails.
 
         Returns:
             AssertParams: Duplicate assert resource.
         """
 
         AssertAPI.__validate_identifiers(params)
@@ -537,16 +548,17 @@
 
     @staticmethod
     def route(test_id: int, assert_id: int or None = None) -> str:
         """Build assert resource url route.
 
         Args:
             test_id (int): Test resource id.
-            assert_id (int, optional): Assert resource id. Defaults to None. If
-                omitted the route will point to all assert resources.
+
+            assert_id (int, optional): Assert resource id. Defaults to None.
+            If omitted the route will point to all assert resources.
 
         Returns:
             str: Route to assert resource/s.
         """
 
         r = APIClient().project_route + f"tests/{test_id}/asserts/"
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/classificator.py` & `loadero_python-1.2.0/loadero_python/resources/classificator.py`

 * *Files identical despite different names*

### Comparing `loadero_python-1.1.0/loadero_python/resources/file.py` & `loadero_python-1.2.0/loadero_python/resources/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loadero file resource.
 
 File resource is seperated into three parts
-    - FileParams class describes file attributes
+    FileParams class describes file attributes
 
-    - FileAPI class groups file related API calls
+    FileAPI class groups file related API calls
 
-    - File class combines FileParams and FileAPI
+    File class combines FileParams and FileAPI
 
 Single File object coresponds to single file in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from dateutil import parser
@@ -146,16 +146,17 @@
         super().__init__(self.params)
 
     def create(self) -> File:
         """Creates a new file.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - content
-            - file_type
+
+        - content
+        - file_type
 
         Raises:
             APIException: If API call fails.
 
         Returns:
             File: Created file resource.
         """
@@ -164,15 +165,16 @@
         return self
 
     def read(self) -> File:
         """Reads information about an existing file.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - file_id
+
+        - file_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -184,17 +186,18 @@
         return self
 
     def update(self) -> File:
         """Update information about an existing file.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - file_id
-            - content
-            - file_type
+
+        - file_id
+        - content
+        - file_type
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -206,15 +209,16 @@
         return self
 
     def delete(self) -> None:
         """Delete an existing file.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - file_id
+
+        - file_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
         """
@@ -248,14 +252,15 @@
         """Read an existing file resource.
 
         Args:
             params (FileParams): Describes the file resource to read.
 
         Raises:
             Exception: FileParams.file_id was not defined.
+
             APIException: If API call fails.
 
         Returns:
             FileParams: Read file resource params.
         """
 
         FileAPI.__validate_identifiers(params)
@@ -269,14 +274,15 @@
         """Update an existing file resource.
 
         Args:
             params (FileParams): Describes the file and the changes to apply.
 
         Raises:
             Exception: FileParams.file_id was not defined.
+
             APIException: If API call fails.
 
         Returns:
             FileParams: Read file resource.
         """
 
         FileAPI.__validate_identifiers(params)
@@ -290,14 +296,15 @@
         """Delete an existing file resource.
 
         Args:
             params (FileParams): Describes the file to delete.
 
         Raises:
             Exception: FileParams.file_id was not defined.
+
             APIException: If API call fails.
 
         Returns:
             FileParams: Read file resource.
         """
 
         FileAPI.__validate_identifiers(params)
@@ -328,15 +335,15 @@
 
     @staticmethod
     def route(file_id: int or None = None) -> str:
         """Build file resource url route.
 
         Args:
             file_id (int, optional): File resource id. Defaults to None. If
-                omitted the route will point to all file resources
+            omitted the route will point to all file resources
 
         Returns:
             str: Route to file resource.
         """
 
         r = APIClient().project_route + "files/"
 
@@ -347,16 +354,18 @@
 
     @staticmethod
     def __validate_identifiers(params: FileParams, single: bool = True):
         """Validate file resource identifiers.
 
         Args:
             params (FileParams): File params.
+
             single (bool, optional): Indicates if the resource identifiers
-                should be validated as pointing to a single resource.
-                Defaults to True.
+            should be validated as pointing to a single resource.
+            Defaults to True.
+
         Raises:
             ValueError: FileParams.file_id must be a valid int.
         """
 
         if single and params.file_id is None:
             raise ValueError("FileParams.file_id must be a valid int")
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/group.py` & `loadero_python-1.2.0/loadero_python/resources/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loadero group resource.
 
 Group resource is seperated into three parts
-    - GroupParams class describes groups attributes
+    GroupParams class describes groups attributes
 
-    - GroupAPI class groups all API operations related to groups.
+    GroupAPI class groups all API operations related to groups.
 
-    - Group class combined GroupParams and GroupAPI
+    Group class combined GroupParams and GroupAPI
 
 Single group object coresponds to single group in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from dateutil import parser
@@ -237,17 +237,18 @@
         super().__init__(self.params)
 
     def create(self) -> Group:
         """Creates new group with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - count
-            - name
+
+        - test_id
+        - count
+        - name
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -260,16 +261,17 @@
         return self
 
     def read(self) -> Group:
         """Reads information about an existing group.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - group_id
+
+        - test_id
+        - group_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -282,18 +284,19 @@
         return self
 
     def update(self) -> Group:
         """Updates group with given parameters.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - group_id
-            - test_id
-            - count
-            - name
+
+        - group_id
+        - test_id
+        - count
+        - name
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -306,16 +309,17 @@
         return self
 
     def delete(self) -> None:
         """Deletes and existing group.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - group_id
-            - test_id
+
+        - group_id
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
         """
@@ -323,16 +327,17 @@
         GroupAPI.delete(self.params)
 
     def duplicate(self, name: str) -> Group:
         """Duplicates and existing group.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - group_id
-            - test_id
+
+        - group_id
+        - test_id
 
         Args:
             name (str): New name for the duplicate group.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
@@ -348,16 +353,17 @@
     def participants(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Participant], PaginationParams, dict[any, any]]:
         """Read all participants in group.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - group_id
-            - test_id
+
+        - group_id
+        - test_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Test.params.test_id must be a valid int.
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/metric_path.py` & `loadero_python-1.2.0/loadero_python/resources/metric_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,18 +805,27 @@
 
     WEBRTC_VIDEO_RTT_MAX = "webrtc/video/rtt/max"
 
     WEBRTC_VIDEO_RTT_RSTDDEV = "webrtc/video/rtt/rstddev"
 
     WEBRTC_VIDEO_RTT_STDDEV = "webrtc/video/rtt/stddev"
 
+    UNKNOWN = "unknown"
+
     # pylint: disable=arguments-differ
     @staticmethod
     def from_dict(jv: str) -> MetricPath:
-        return MetricPath(jv)
+        m = None
+
+        try:
+            m = MetricPath(jv)
+        except:  # pylint: disable=bare-except
+            m = MetricPath.UNKNOWN
+
+        return m
 
     def to_dict(self) -> str:
         return self.value
 
     def to_dict_full(self) -> str:
         return self.to_dict()
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/pagination.py` & `loadero_python-1.2.0/loadero_python/resources/pagination.py`

 * *Files identical despite different names*

### Comparing `loadero_python-1.1.0/loadero_python/resources/participant.py` & `loadero_python-1.2.0/loadero_python/resources/participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loadero participant resource.
 
 Participant resources is seperated into three parts
-    - ParticipantParams class describes participant attributes
+    ParticipantParams class describes participant attributes
 
-    - ParticipantAPI groups all API operations with participant resource.
+    ParticipantAPI groups all API operations with participant resource.
 
-    - Participant class combines ParticipantParams and ParticipantAPI.
+    Participant class combines ParticipantParams and ParticipantAPI.
 
 Single Participant object coresponds to single participant in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from dateutil import parser
@@ -403,24 +403,25 @@
         super().__init__(self.params)
 
     def create(self) -> Participant:
         """Creates new participant with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - name
-            - count
-            - compute_unit
-            - record_audio
-            - audio_feed
-            - browser
-            - location
-            - network
-            - video_feed
+
+        - test_id
+        - name
+        - count
+        - compute_unit
+        - record_audio
+        - audio_feed
+        - browser
+        - location
+        - network
+        - video_feed
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -433,16 +434,17 @@
         return self
 
     def read(self) -> Participant:
         """Reads information about an existing participant.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - participant_id
-            - test_id
+
+        - participant_id
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -455,25 +457,26 @@
         return self
 
     def update(self) -> Participant:
         """Updates particpant with given parameters.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - participant_id
-            - test_id
-            - name
-            - count
-            - compute_unit
-            - record_audio
-            - audio_feed
-            - browser
-            - location
-            - network
-            - video_feed
+
+        - participant_id
+        - test_id
+        - name
+        - count
+        - compute_unit
+        - record_audio
+        - audio_feed
+        - browser
+        - location
+        - network
+        - video_feed
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -486,16 +489,17 @@
         return self
 
     def delete(self) -> None:
         """Deletes and existing participant.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - participant_id
+
+        - test_id
+        - participant_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
         """
@@ -503,16 +507,17 @@
         ParticipantAPI.delete(self.params)
 
     def duplicate(self, name: str) -> Participant:
         """Duplicates and existing participant.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - participant_id
+
+        - test_id
+        - participant_id
 
         Args:
             name (str): New name for the duplicate participant.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/project.py` & `loadero_python-1.2.0/loadero_python/resources/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Loadero project resource.
 
 Project resource is seperated into three parts
-    - ProjectParams class describes projects attributes
-    - ProjectAPI class groups all API operations related to projects.
-    - Project class combines ProjectParams and ProjectAPI.
+    ProjectParams class describes projects attributes
+
+    ProjectAPI class groups all API operations related to projects.
+
+    Project class combines ProjectParams and ProjectAPI.
 
 Single Project object coresponds to single project in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from typing import Dict, List, Tuple
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/resource.py` & `loadero_python-1.2.0/loadero_python/resources/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """Describes generics and utility functions of Loadero resources."""
 
 from __future__ import annotations
 from enum import Enum
-from typing import Callable, Dict, List, Tuple
+from typing import Callable, Dict, List, Tuple, Any
 import json
 from datetime import datetime
 
+from loadero_python.api_client import APIClient
+
 
 class Serializable:
     """Base class for serializable objects. Serializable objects can be
     converted to and from JSON using Python dictionary as a JSON representation.
     """
 
-    def to_dict(self) -> Dict[str, any]:
+    def to_dict(self) -> Dict[str, Any]:
         """Returns a dictionary representation of the object."""
         raise NotImplementedError
 
-    def to_dict_full(self) -> Dict[str, any]:
+    def to_dict_full(self) -> Dict[str, Any]:
         """Returns a dictionary representation of the object that contains all
         of the objects attributes."""
         raise NotImplementedError
 
-    def from_dict(self, json_dict: Dict[str, any]) -> Serializable:
+    def from_dict(self, _: Dict[str, Any]) -> Serializable:
         """Returns an instance of the object from a dictionary."""
         raise NotImplementedError
 
 
 class ParamsSerializer(Serializable):
     """ParamsSerializer implements Serializable for Loadero resource params."""
 
     # pylint: disable=dangerous-default-value
     def __init__(
         self,
         attribute_map: dict[str, str] = {},
-        custom_deserializers: dict[str, any] = {},
+        custom_deserializers: dict[str, Any] = {},
         body_attributes: list[str] = [],
         required_body_attributes: list[str] = [],
     ):
         """Initializes the resource params serializer.
 
         Args:
             attribute_map (dict[str, str], optional): Mapping of JSON field
@@ -62,15 +64,15 @@
         self.__body_attributes = body_attributes
         self.__required_body_attributes = required_body_attributes
 
         self.__reverse_attribute_map = {}
         for k, v in self.__attribute_map.items():
             self.__reverse_attribute_map[v] = k
 
-    def to_dict(self) -> Dict[str, any]:
+    def to_dict(self) -> Dict[str, Any]:
         """Converts the resource params object to a dictionary JSON
         representation that contains only the body attributes.
 
         Raises:
             ValueError: If one or more required attributes is missing.
 
         Returns:
@@ -128,15 +130,15 @@
                     v, full
                 )
                 for k, v in attribute.items()
             }
 
         return attribute
 
-    def to_dict_full(self) -> Dict[str, any]:
+    def to_dict_full(self) -> Dict[str, Any]:
         """Returns a dictionary representation of the object that contains all
         of the objects attributes.
 
         Returns:
             dict[str, any]: dictionary representation of the object.
         """
 
@@ -158,15 +160,15 @@
 
             json_dict[json_attribute_name] = self.__get_attribute_dict(
                 python_attribute_value, full=True
             )
 
         return json_dict
 
-    def from_dict(self, json_dict: Dict[str, any]) -> ParamsSerializer:
+    def from_dict(self, json_dict: Dict[str, Any]) -> ParamsSerializer:
         """Sets the attributes of the resource params object from a JSON
         representation.
 
         Args:
             json_dict (dict[str, any]): JSON parsed as dictionary
             representation of the resource.
 
@@ -190,27 +192,27 @@
                 self.__dict__[python_attribute_name] = json_attribute_value
 
         return self
 
 
 def from_dict_as_list(
     resource_params_class: type,
-) -> Callable[[Dict[str, any]], List[LoaderoResourceParams]]:
+) -> Callable[[Dict[str, Any]], List[LoaderoResourceParams]]:
     """Returns a function that deserializes a dictionary to a list of new
     instances of the resource params class
 
     Args:
         resource_params_class (type): Loadero resource params class.
 
     Returns:
         function: Function that deserializes a json dictionary to a list of new
         LoaderoResourceParams objects.
     """
 
-    def func(json_value: dict[str, any]) -> list[LoaderoResourceParams]:
+    def func(json_value: dict[str, Any]) -> list[LoaderoResourceParams]:
         if json_value is None:
             return []
 
         resources = []
 
         for jv in json_value:
             r = resource_params_class()
@@ -219,27 +221,27 @@
         return resources
 
     return func
 
 
 def from_dict_as_new(
     resource_params_class: type,
-) -> Callable[[Dict[str, any]], LoaderoResourceParams]:
+) -> Callable[[Dict[str, Any]], LoaderoResourceParams]:
     """Returns a function that deserializes a dictionary to a new instance of
     the resource params class.
 
     Args:
         resource_params_class (type): Loadero resource params class.
 
     Returns:
         function: Function that deserializes a json dictionary to a new
         LoaderoResourceParams object.
     """
 
-    def func(json_value: dict[str, any]) -> LoaderoResourceParams:
+    def func(json_value: dict[str, Any]) -> LoaderoResourceParams:
         r = resource_params_class()
         r.from_dict(json_value)
 
         return r
 
     return func
 
@@ -254,29 +256,30 @@
         return json.dumps(self.to_dict_full(), indent=4)
 
 
 class LoaderoResource:
     """Base class for Loadero resources.
 
     All Loadero resources have
-        - params attribute that contains the resources data.
-        - __str__ method.
+        params attribute that contains the resources data.
+
+        __str__ method.
     """
 
     def __init__(self, params: LoaderoResourceParams):
         self.params = params
 
     def __str__(self):
         return self.params.__str__()
 
 
 class DuplicateResourceBodyParams(LoaderoResourceParams):
     """Duplicate resource body params."""
 
-    def __init__(self, name: str or None = None):
+    def __init__(self, name: str | None = None):
         super().__init__(
             attribute_map={
                 "name": "name",
             },
             body_attributes=[
                 "name",
             ],
@@ -346,15 +349,15 @@
         Returns:
             QueryParams: QueryParams with offset set.
         """
 
         self.__set_param("offset", offset)
         return self
 
-    def filter(self, key: FilterKey, *values: any) -> QueryParams:
+    def filter(self, key: FilterKey, *values: Any) -> QueryParams:
         """Set filter for read all operation.
 
         Args:
             key (ResourceFilters): Filter key.
 
             value (any): Filter value. Variadic argument.
 
@@ -380,34 +383,75 @@
         if isinstance(value, datetime):
             self.__add_param(str(key), int(value.timestamp()))
             return self
 
         self.__add_param(str(key), value)
         return self
 
-    def __set_param(self, key: str, value: any):
+    def __set_param(self, key: str, value: Any):
         if key not in self.__query_params:
             self.__query_params[key] = []
 
         self.__query_params[key] = [value]
 
-    def __add_param(self, key: str, value: any):
+    def __add_param(self, key: str, value: Any):
         if key not in self.__query_params:
             self.__query_params[key] = []
 
         self.__query_params[key].append(value)
 
-    def parse(self) -> List[Tuple[str, any]]:
+    def parse(self) -> List[Tuple[str, Any]]:
         """Parses QueryParams into a list of tuples representation that will be
             used for sending the request.
 
         Returns:
             list[tuple[str, any]]: List of tuples representation of QueryParams.
         """
 
         query_params = []
 
         for key, values in self.__query_params.items():
             for v in values:
                 query_params.append((key, v))
 
         return query_params
+
+
+class URL(Serializable):
+    """URL describes a single Loadero log file or artifact. Allows downloading
+    without manually supplying access token."""
+
+    def __init__(self, url: str = ""):
+        self.__url = url
+
+    def url(self) -> str:
+        """Returns URL string
+
+        Returns:
+            str: URL string
+        """
+
+        return self.__url
+
+    def download(self) -> str:
+        """Downloads the contents of a the URL, storing the result as a file in
+        current working directory
+
+        Returns
+            str: File name of the download.
+        """
+
+        name = self.url().rsplit("/", 1)[-1]
+        with open(name, "wb") as dest:
+            APIClient().get_raw(self.url(), dest)
+
+        return name
+
+    def from_dict(self, json_dict: str) -> URL:
+        self.__url = json_dict
+        return self
+
+    def to_dict(self) -> str:
+        return self.url()
+
+    def to_dict_full(self) -> str:
+        return self.to_dict()
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/result.py` & `loadero_python-1.2.0/loadero_python/resources/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Loadero result resource.
+
 Result resource is seperated into three parts
-    - ResultParams class describes result attributes
-    - ResultAPI group all API operations for result resource
-    - Result class combines ResultParams and ResultAPI
+    ResultParams class describes result attributes
+
+    ResultAPI group all API operations for result resource
+
+    Result class combines ResultParams and ResultAPI
 
 Single result object coresponds to single result in Loadero.
 """
 
 from __future__ import annotations
 from datetime import datetime
 from dateutil import parser
 
 from ..api_client import APIClient
 from .resource import (
     FilterKey,
     LoaderoResourceParams,
     LoaderoResource,
     QueryParams,
+    URL,
     from_dict_as_list,
     from_dict_as_new,
 )
 from .metric_path import MetricPath, MetricBasePath
 from .classificator import (
     MetricStatus,
     Operator,
@@ -72,25 +76,30 @@
                 "selenium": "_selenium",
                 "browser": "_browser",
                 "rru": "_rru",
                 "allure_report": "_allure_report",
             },
             custom_deserializers={
                 "created": parser.parse,
+                "webrtc": from_dict_as_new(URL),
+                "selenium": from_dict_as_new(URL),
+                "browser": from_dict_as_new(URL),
+                "rru": from_dict_as_new(URL),
+                "allure_report": from_dict_as_new(URL),
             },
         )
 
-        self._result_log_id = None
-        self._created = None
-        self._result_id = None
-        self._webrtc = None
-        self._selenium = None
-        self._browser = None
-        self._rru = None
-        self._allure_report = None
+        self._result_log_id: int
+        self._created: datetime
+        self._result_id: int
+        self._webrtc: URL
+        self._selenium: URL
+        self._browser: URL
+        self._rru: URL
+        self._allure_report: URL
 
     @property
     def result_log_id(self) -> int:
         """Result log id.
 
         Returns:
             int: Result log id.
@@ -115,55 +124,55 @@
         Returns:
             int: Result id.
         """
 
         return self._result_id
 
     @property
-    def webrtc(self) -> str:
+    def webrtc(self) -> URL:
         """WebRTC log URL.
 
         Returns:
-            str: WebRTC log URL.
+            URL: WebRTC log URL.
         """
 
         return self._webrtc
 
     @property
-    def selenium(self) -> str:
+    def selenium(self) -> URL:
         """Selenium log URL.
 
         Returns:
             str: Selenium log URL.
         """
 
         return self._selenium
 
     @property
-    def browser(self) -> str:
+    def browser(self) -> URL:
         """Browser log URL.
 
         Returns:
             str: Browser log URL.
         """
 
         return self._browser
 
     @property
-    def rru(self) -> str:
+    def rru(self) -> URL:
         """Result resource usage log URL.
 
         Returns:
             str: Result resource usage log URL.
         """
 
         return self._rru
 
     @property
-    def allure_report(self) -> str:
+    def allure_report(self) -> URL:
         """Allure report URL.
 
         Returns:
             str: Allure report URL.
         """
 
         return self._allure_report
@@ -311,35 +320,38 @@
 
     def __init__(self):
         super().__init__(
             attribute_map={
                 "error": "_error",
                 "paths": "_paths",
             },
+            custom_deserializers={
+                "paths": from_dict_as_list(URL),
+            },
         )
 
         self._error = None
         self._paths = None
 
     @property
-    def error(self) -> str:
+    def error(self) -> str | None:
         """Artifact error message.
 
         Returns:
             str: Artifact error message.
         """
 
         return self._error
 
     @property
-    def paths(self) -> list[str]:
+    def paths(self) -> list[URL] | None:
         """URLs of artifact files.
 
         Returns:
-            list[str]: URLs of artifact files.
+            list[URL]: URLs of artifact files.
         """
 
         return self._paths
 
 
 class ArtifactsInfoParams(LoaderoResourceParams):
     """ArtifactsInfoParams describes Loadero artifacts of a single test run."""
@@ -356,18 +368,18 @@
                 "audio": from_dict_as_new(ArtifactInfoParams),
                 "downloads": from_dict_as_new(ArtifactInfoParams),
                 "screenshots": from_dict_as_new(ArtifactInfoParams),
                 "video": from_dict_as_new(ArtifactInfoParams),
             },
         )
 
-        self._audio = None
-        self._downloads = None
-        self._screenshots = None
-        self._video = None
+        self._audio: ArtifactInfoParams
+        self._downloads: ArtifactInfoParams
+        self._screenshots: ArtifactInfoParams
+        self._video: ArtifactInfoParams
 
     @property
     def audio(self) -> ArtifactInfoParams:
         """Audio artifacts.
 
         Returns:
             ArtifactInfoParams: Audio artifacts.
@@ -1189,16 +1201,17 @@
         super().__init__(self.params)
 
     def read(self) -> Result:
         """Reads a existing result.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - result_id
-            - run_id
+
+        - result_id
+        - run_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/run.py` & `loadero_python-1.2.0/loadero_python/resources/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Loadero run resource.
 
-Run resources is seperated into three parts:
-    - RunParams class that describes runs attributes
+Run resources is seperated into three parts
+    RunParams class that describes runs attributes
 
-    - RunAPI class implements run resources API operations
+    RunAPI class implements run resources API operations
 
-    - Runs class that in combination with RunParams and RunAPI allows to manage
+    Runs class that in combination with RunParams and RunAPI allows to manage
     a single run resources instance.
 """
 
 from __future__ import annotations
 from time import sleep
 from datetime import datetime
 from dateutil import parser
@@ -434,15 +434,16 @@
         super().__init__(self.params)
 
     def create(self) -> Run:
         """Creates new run with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource.
 
             APIException: If API call fails.
 
@@ -455,15 +456,16 @@
         return self
 
     def read(self) -> Run:
         """Read an existing run resource.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_id
+
+        - run_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -477,15 +479,16 @@
 
     def stop(self) -> Run:
         """Stop an active run. To stop a run need only to specify the test_id
         and run_id in resource params.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_id
+
+        - run_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -500,15 +503,16 @@
     def poll(
         self, interval: float = 15.0, timeout: float = 12 * 60 * 60
     ) -> Run:
         """Polls run status until it is finished.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_id
+
+        - run_id
 
         Args:
             interval (float, optional): Poll interval in seconds.
             Defaults to 15.0.
 
             timeout (float, optional): Poll timeout in seconds. Defaults to
             12*60*60 (12h).
@@ -555,15 +559,16 @@
     def results(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Result], PaginationParams, dict[any, any]]:
         """Get all results of the run.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_id
+
+        - run_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             APIException: If API call fails.
 
@@ -578,28 +583,33 @@
         """
 
         if self.params.run_id is None:
             raise ValueError("Run.params.run_id must be a valid int")
 
         resp = ResultAPI.read_all(self.params.run_id, query_params=query_params)
 
+        results = convert_params_list(Result, resp.results)
+        for r in results:
+            r.params.run_id = self.params.run_id
+
         return (
-            convert_params_list(Result, resp.results),
+            results,
             resp.pagination,
             resp.filter,
         )
 
     def participants(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[RunParticipant], PaginationParams, dict[any, any]]:
         """Read all participants in run.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_id
+
+        - run_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Run.params.run_id must be a valid int.
 
@@ -632,19 +642,20 @@
 
     @staticmethod
     def create(params: RunParams) -> RunParams:
         """Creates and launches a new test run.
 
         Args:
             params (RunParams): Describes the run resource to be created. Only
-                the RunParams.test_id field is required.
+            the RunParams.test_id field is required.
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
-                resource.
+            resource.
+
             APIException: If API call fails.
 
         Returns:
             RunParams: Created run resource.
         """
 
         RunAPI.__validate_identifiers(params, False, False)
@@ -658,15 +669,16 @@
         """Read an existing run resource.
 
         Args:
             params (RunParams): Describes the run resource to read.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource.
+            resource.
+
             APIException: If API call fails.
 
         Returns:
             RunParams: Read run resource.
         """
 
         RunAPI.__validate_identifiers(params)
@@ -680,20 +692,22 @@
         test_id: int or None = None,
         query_params: QueryParams or None = None,
     ) -> PagedResponse:
         """Read all run resources.
 
         Args:
             test_id (int, optional): Parent test resource id. Defaults to None.
-                If omitted all runs in project will be read.
+            If omitted all runs in project will be read.
+
             query_params (QueryParams, optional): Describes query parameters.
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
-                resource.
+            resource.
+
             APIException: If API call fails.
 
         Returns:
             PagedResponse: Paged response of run resources.
         """
 
         qp = None
@@ -709,15 +723,16 @@
         """Stop an active test run.
 
         Args:
             params (RunParams): Describes the run resource to stop.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
-                resource.
+            resource.
+
             APIException: If API call fails.
         """
 
         RunAPI.__validate_identifiers(params, True, False)
 
         APIClient().post(
             RunAPI.route(test_id=params.test_id, run_id=params.run_id)
@@ -727,18 +742,19 @@
 
     @staticmethod
     def route(test_id: int or None = None, run_id: int or None = None) -> str:
         """Build run resource url route.
 
         Args:
             test_id (int, optional): Test resource id. Defaults to None. If
-                omitted route will point to all runs in project.
+            omitted route will point to all runs in project.
+
             run_id (int, optional): Run resource id. Defaults to None. If
-                omitted the route will point to all run resources that belong
-                to parent resource, either test or project.
+            omitted the route will point to all run resources that belong
+            to parent resource, either test or project.
 
         Returns:
             str: Route to run resource/s.
         """
 
         r = APIClient().project_route
 
@@ -756,22 +772,25 @@
     def __validate_identifiers(
         params: RunParams, single: bool = True, project_run: bool = True
     ) -> None:
         """Validate run resource identifiers.
 
         Args:
             params (RunParams): Run params.
+
             single (bool, optional): Indicates if the resource identifiers
-                should be validated as pointing to a single resource.
-                Defaults to True.
+            should be validated as pointing to a single resource.
+            Defaults to True.
+
             project_run (bool, optional): Indicates if the resource identifiers
-                should include a valid test id. Defaults to True.
+            should include a valid test id. Defaults to True.
 
         Raises:
             ValueError: RunParams.run_id must be a valid int.
+
             ValueError: RunParams.test_id must be a valid int.
         """
 
         if single and params.run_id is None:
             raise ValueError("RunParams.run_id must be a valid int")
 
         if not project_run and params.test_id is None:
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/run_participant.py` & `loadero_python-1.2.0/loadero_python/resources/run_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Loadero run participant resource.
 
 Run participant resources is seperated into three parts
-    - RunParticipantParams class describes run participant attributes
+    RunParticipantParams class describes run participant attributes
 
-    - RunParticipantAPI class groups all API operations related to run
+    RunParticipantAPI class groups all API operations related to run
     participant.
 
-    - RunParticipant class combined RunParticipantParams and RunParticipantAPI.
+    RunParticipant class combined RunParticipantParams and RunParticipantAPI.
 
 Single RunParticipant object coresponds to single run participant in Loadero.
 """
 
 
 from __future__ import annotations
 from datetime import datetime
@@ -311,16 +311,17 @@
         super().__init__(self.params)
 
     def read(self) -> RunParticipant:
         """Reads information about an existing run participant.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - run_participant_id
-            - run_id
+
+        - run_participant_id
+        - run_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
```

### Comparing `loadero_python-1.1.0/loadero_python/resources/test.py` & `loadero_python-1.2.0/loadero_python/resources/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Loadero test resource.
 
 Test resource is seperated into three parts
-    - TestParams class describes test attributes
+    TestParams class describes test attributes
 
-    - TestAPI class groups API operation with test resources.
+    TestAPI class groups API operation with test resources.
 
-    - Test class combines TestParams and TestAPI.
+    Test class combines TestParams and TestAPI.
 
 Single Test object coresponds to single test in Loadero.
 """
 
 from __future__ import annotations
+from typing import Any
 from datetime import datetime
 from dateutil import parser
 from ..api_client import APIClient
 from .resource import (
     FilterKey,
     QueryParams,
     Serializable,
@@ -114,15 +115,15 @@
 
         Returns:
             str: Script content.
         """
 
         return self.to_dict()
 
-    def from_dict(self, json_dict: dict[str, any]) -> Script:
+    def from_dict(self, _: dict[str, Any]) -> Script:
         """Loads script from a dictionary. Never used. Required for
         serialization.
 
         Args:
             json_dict (dict[str, any]): JSON parsed as dictionary.
 
         Returns:
@@ -465,19 +466,20 @@
         super().__init__(self.params)
 
     def create(self) -> Test:
         """Creates new test with given data.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - name
-            - start_interval
-            - participant_timeout
-            - mode
-            - increment_strategy
+
+        - name
+        - start_interval
+        - participant_timeout
+        - mode
+        - increment_strategy
 
         Raises:
             ValueError: If resource params do not sufficiently identify parent
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -489,15 +491,16 @@
         return self
 
     def read(self) -> Test:
         """Reads information about an existing test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -509,20 +512,21 @@
         return self
 
     def update(self) -> Test:
         """Updates test with given parameters.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
-            - name
-            - start_interval
-            - participant_timeout
-            - mode
-            - increment_strategy
+
+        - test_id
+        - name
+        - start_interval
+        - participant_timeout
+        - mode
+        - increment_strategy
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource or resource params required attributes are None.
 
             APIException: If API call fails.
 
@@ -534,15 +538,16 @@
         return self
 
     def delete(self) -> Test:
         """Deletes and existing test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -554,15 +559,16 @@
         return self
 
     def duplicate(self, name: str) -> Test:
         """Duplicates and existing test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Args:
             name (str): New name for the duplicate test.
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
@@ -578,15 +584,16 @@
         return dupl
 
     def launch(self) -> Run:
         """Launches test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Raises:
             ValueError: If resource params do not sufficiently identify
             resource.
 
             APIException: If API call fails.
 
@@ -601,15 +608,16 @@
     def groups(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Group], PaginationParams, dict[any, any]]:
         """Read all groups in test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Test.params.test_id must be a valid int.
 
@@ -637,15 +645,16 @@
     def participants(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Participant], PaginationParams, dict[any, any]]:
         """Read all participants in test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Test.params.test_id must be a valid int.
 
@@ -675,15 +684,16 @@
     def asserts(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Assert], PaginationParams, dict[any, any]]:
         """Read all asserts in test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Test.params.test_id must be a valid int.
 
@@ -713,15 +723,16 @@
     def runs(
         self, query_params: QueryParams or None = None
     ) -> tuple[list[Run], PaginationParams, dict[any, any]]:
         """Read all runs in test.
 
         Required attributes of params field that need to be populated, otherwise
         the method will raise an exception:
-            - test_id
+
+        - test_id
 
         Args:
             query_params (QueryParams, optional): Describes query parameters
 
         Raises:
             ValueError: Test.params.test_id must be a valid int.
```

### Comparing `loadero_python-1.1.0/loadero_python.egg-info/PKG-INFO` & `loadero_python-1.2.0/loadero_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadero-python
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python client for Loadero API
 Home-page: https://github.com/loadero/loadero-python
 Author: Loadero Team
 Author-email: support@loadero.com
 License: GPLv3
 Project-URL: Documentation, https://loadero.github.io/loadero-python/
 Project-URL: Source, https://github.com/loadero/loadero-python
@@ -72,21 +72,15 @@
 ```
 
 ## Usage
 
 ### API Access
 
 Before using the Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting support. More information about the
-API can be found in the
-[Loadero wiki](https://wiki.loadero.com/loadero-usage/api/).
-
-Before using Loadero-Python client an API access token needs to be acquired.
-Currently, this can be done by contacting
-[support](mailto:support@loadero.com?subject=I%20want%20to%20request%20project%20access%20token%20for%20API).
+This can be done in the projects settings page in Loadero web-app.
 More information about the API can be found in the
 [Loadero wiki](https://wiki.loadero.com/loadero-usage/api/)
 
 **Note** Access tokens are project specific and cannot be used across multiple
 projects. Make sure to specify the project ID in the request for an access
 token.
```

### Comparing `loadero_python-1.1.0/loadero_python.egg-info/SOURCES.txt` & `loadero_python-1.2.0/loadero_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loadero_python-1.1.0/setup.py` & `loadero_python-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 root_path = pathlib.Path(__file__).parent.resolve()
 long_description = (root_path / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="loadero_python",
-    version="1.1.0",
+    version="1.2.0",
     description="Python client for Loadero API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loadero/loadero-python",
     author="Loadero Team",
     author_email="support@loadero.com",
     license="GPLv3",
```

