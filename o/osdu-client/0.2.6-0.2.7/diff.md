# Comparing `tmp/osdu_client-0.2.6.tar.gz` & `tmp/osdu_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdu_client-0.2.6.tar", last modified: Mon Jun  5 19:11:44 2023, max compression
+gzip compressed data, was "osdu_client-0.2.7.tar", last modified: Mon Jul 17 14:31:16 2023, max compression
```

## Comparing `osdu_client-0.2.6.tar` & `osdu_client-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 19:11:40.000000 osdu_client-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 19:11:44.885796 osdu_client-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 19:11:40.000000 osdu_client-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-05 19:11:44.885796 osdu_client-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 19:11:40.000000 osdu_client-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.881795 osdu_client-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/entitlements_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/legal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/sdms_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-05 19:11:40.000000 osdu_client-0.2.6/src/osdu_client/services/storage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:11:44.885796 osdu_client-0.2.6/src/osdu_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 19:11:44.000000 osdu_client-0.2.6/src/osdu_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:16.219316 osdu_client-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 14:31:10.000000 osdu_client-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-17 14:31:16.219316 osdu_client-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-17 14:31:10.000000 osdu_client-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 14:31:16.223316 osdu_client-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 14:31:10.000000 osdu_client-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:16.219316 osdu_client-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:16.219316 osdu_client-0.2.7/src/osdu_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:16.219316 osdu_client-0.2.7/src/osdu_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/entitlements_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/legal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/sdms_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-17 14:31:10.000000 osdu_client-0.2.7/src/osdu_client/services/storage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:31:16.219316 osdu_client-0.2.7/src/osdu_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-17 14:31:16.000000 osdu_client-0.2.7/src/osdu_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:31:16.000000 osdu_client-0.2.7/src/osdu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:31:16.000000 osdu_client-0.2.7/src/osdu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 14:31:16.000000 osdu_client-0.2.7/src/osdu_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:31:16.000000 osdu_client-0.2.7/src/osdu_client.egg-info/top_level.txt
```

### Comparing `osdu_client-0.2.6/LICENSE` & `osdu_client-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.6/PKG-INFO` & `osdu_client-0.2.7/src/osdu_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: osdu_client
-Version: 0.2.6
+Name: osdu-client
+Version: 0.2.7
 Summary: OSDU API Client
 Home-page: https://github.com/micmurawski/osdu-client/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -29,29 +29,29 @@
 
 # Example
 OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
 
 
 
 ```python
-from typing import AnyStr, Dict
+from typing import Dict
 
 from osdu_client import OSDUAPI
 from osdu_client.auth import AuthBackendInterface
 
 
 class AuthBackend(AuthBackendInterface):
     def __init__(self, headers, base_url) -> None:
         self._headers = headers
         self._base_url = base_url
 
     def get_headers(self) -> Dict:
         return self._headers
 
-    def get_base_url(self) -> AnyStr:
+    def get_base_url(self) -> str:
         return self._osdu_base_url
 
     def get_sd_connection_params(self, log_level: int = None) -> Dict:
         return {}
 
 
 auth_backend = AuthBackend(
```

### Comparing `osdu_client-0.2.6/README.md` & `osdu_client-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
 # Example
 OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
 
 
 
 ```python
-from typing import AnyStr, Dict
+from typing import Dict
 
 from osdu_client import OSDUAPI
 from osdu_client.auth import AuthBackendInterface
 
 
 class AuthBackend(AuthBackendInterface):
     def __init__(self, headers, base_url) -> None:
         self._headers = headers
         self._base_url = base_url
 
     def get_headers(self) -> Dict:
         return self._headers
 
-    def get_base_url(self) -> AnyStr:
+    def get_base_url(self) -> str:
         return self._osdu_base_url
 
     def get_sd_connection_params(self, log_level: int = None) -> Dict:
         return {}
 
 
 auth_backend = AuthBackend(
```

### Comparing `osdu_client-0.2.6/setup.py` & `osdu_client-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def get_dependencies():
     with open("requirements.txt", encoding="utf-8") as fh:
         return fh.read().splitlines()
 
 
 setup(
     name='osdu_client',
-    version='0.2.6',
+    version='0.2.7',
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="OSDU API Client",
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/osdu-client/",
     package_dir={"": "src"},
```

### Comparing `osdu_client-0.2.6/src/osdu_client/client.py` & `osdu_client-0.2.7/src/osdu_client/client.py`

 * *Files identical despite different names*

### Comparing `osdu_client-0.2.6/src/osdu_client/services/dataset_api.py` & `osdu_client-0.2.7/src/osdu_client/services/dataset_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import AnyStr, Dict, List
+from typing import Dict, List
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
@@ -11,50 +11,74 @@
     pass
 
 
 class DatasetAPIClient(BaseOSDUAPIClient):
     service_path = "api/dataset/v1"
 
     def get_storage_instructions(
-        self, *, kind_sub_type: AnyStr
+        self, *, kind_sub_type: str
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
-            "getStorageInstructions",
+            "storageInstructions",
         )
         params = {"kindSubType": kind_sub_type}
-        response = requests.get(
+        response = requests.post(
             url=url, headers=self.osdu_auth_backend.headers, params=params
         )
 
         if not response.ok:
             raise DatasetAPIError(
                 status_code=response.status_code,
                 message=response.text
             )
 
         return response.json()
 
-    def get_retrieval_instructions(
+    def get_batch_retrieval_instructions(
         self,
         *,
-        dataset_registry_ids: List[AnyStr]
+        dataset_registry_ids: List[str]
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
-            "getRetrievalInstructions",
+            "retrievalInstructions",
         )
         response = requests.post(
             url=url,
             headers=self.osdu_auth_backend.headers,
             json={"datasetRegistryIds": dataset_registry_ids},
         )
 
         if not response.ok:
             raise DatasetAPIError(
                 status_code=response.status_code,
                 message=response.text
             )
+
+        return response.json()
+
+    def get_retrieval_instructions(
+        self,
+        *,
+        id: str
+    ) -> Dict:
+        url = os.path.join(
+            self.osdu_auth_backend.base_url,
+            self.service_path,
+            "retrievalInstructions",
+        )
+        response = requests.get(
+            url=url,
+            headers=self.osdu_auth_backend.headers,
+            params={"id": id},
+        )
+
+        if not response.ok:
+            raise DatasetAPIError(
+                status_code=response.status_code,
+                message=response.text
+            )
 
         return response.json()
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/entitlements_api.py` & `osdu_client-0.2.7/src/osdu_client/services/entitlements_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import AnyStr, Dict
+from typing import Dict
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
@@ -44,15 +44,15 @@
         if not response.ok:
             raise EntitlementsAPIException(
                 status_code=response.status_code, message=response.text
             )
 
         return response.json()
 
-    def add_member(self, *, email: AnyStr, group_name: AnyStr, role: AnyStr) -> Dict:
+    def add_member(self, *, email: str, group_name: str, role: str) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"groups/{group_name}/members",
         )
         response = requests.post(
             url=url,
@@ -66,18 +66,18 @@
             )
 
         return response.json()
 
     def create_group(
         self,
         *,
-        name: AnyStr,
-        description: AnyStr,
-        email: AnyStr,
-        data_partition_id: AnyStr = None,
+        name: str,
+        description: str,
+        email: str,
+        data_partition_id: str = None,
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "groups",
         )
         data = {"name": name, "description": description, "email": email}
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/legal_api.py` & `osdu_client-0.2.7/src/osdu_client/services/legal_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, List
+from typing import List
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
@@ -28,15 +28,15 @@
         )
         params = {"valid": valid}
         headers = self.osdu_auth_backend.headers
         if osdu_account_id:
             headers["OSDU-Account-Id"] = osdu_account_id
         if osdu_on_behalf_of:
             headers["OSDU-On-Behalf-Of"] = osdu_on_behalf_of
-        response = requests.get(url=url, headers=headers)
+        response = requests.get(url=url, headers=headers, params=params)
 
         if not response.ok:
             raise LegalAPIException(
                 status_code=response.status_code, message=response.text
             )
 
         return response.json()
@@ -92,15 +92,14 @@
                 originator=originator,
                 dataType=data_type,
                 securityClassification=security_classification,
                 personalData=personal_data,
                 exportClassification=export_classification,
             )
         )
-        #raise Exception(expiration_date, contract_id)
         if expiration_date:
             request_body['properties']['expirationDate'] = expiration_date
         if extension_properties:
             request_body['properties']['extensionProperties'] = extension_properties
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
@@ -169,18 +168,14 @@
         osdu_account_id: str = None,
         osdu_on_behalf_of: str = None,
     ) -> dict:
 
         request_body = dict(
             names=names,
         )
-        if expiration_date:
-            request_body['expirationDate'] = expiration_date
-        if extension_properties:
-            request_body['extensionProperties'] = extension_properties
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "legaltags:batchRetrieve"
         )
         headers = self.osdu_auth_backend.headers
@@ -204,18 +199,14 @@
         osdu_account_id: str = None,
         osdu_on_behalf_of: str = None,
     ) -> dict:
 
         request_body = dict(
             names=names,
         )
-        if expiration_date:
-            request_body['expirationDate'] = expiration_date
-        if extension_properties:
-            request_body['extensionProperties'] = extension_properties
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "legaltags:validate"
         )
         headers = self.osdu_auth_backend.headers
@@ -228,33 +219,7 @@
 
         if not response.ok:
             raise LegalAPIException(
                 status_code=response.status_code, message=response.text
             )
 
         return response.json()
-
-    def validate_legal_tags(
-        self, *,
-        osdu_account_id: str = None,
-        osdu_on_behalf_of: str = None,
-    ) -> dict:
-
-        url = os.path.join(
-            self.osdu_auth_backend.base_url,
-            self.service_path,
-            "legaltags:properties"
-        )
-        headers = self.osdu_auth_backend.headers
-        if osdu_account_id:
-            headers["OSDU-Account-Id"] = osdu_account_id
-        if osdu_on_behalf_of:
-            headers["OSDU-On-Behalf-Of"] = osdu_on_behalf_of
-
-        response = requests.get(url=url, headers=headers)
-
-        if not response.ok:
-            raise LegalAPIException(
-                status_code=response.status_code, message=response.text
-            )
-
-        return response.json()
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/schema_api.py` & `osdu_client-0.2.7/src/osdu_client/services/schema_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
-from typing import AnyStr, Dict
+from typing import Dict
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
 class SchemaAPIError(OSDUAPIError):
     pass
 
 
 class SchemaAPIClient(BaseOSDUAPIClient):
     service_path = "api/schema-service/v1/schema"
 
-    def get_schema(self, *, id: AnyStr, ) -> Dict:
+    def get_schema(self, *, id: str) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             f"{self.service_path}/{id}",
         )
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
 
         if not response.ok:
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/sdms_api.py` & `osdu_client-0.2.7/src/osdu_client/services/sdms_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from json import JSONDecodeError
-from typing import AnyStr, Dict, List, Optional
+from typing import Dict, List, Optional
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
 class SDMSAPIError(OSDUAPIError):
     pass
 
 
 class SDMSTokenAPI:
     def create_impersonation_token(
-        self, *, user_token: AnyStr, resources: List[Dict], metadata: Dict
+        self, *, user_token: str, resources: List[Dict], metadata: Dict
     ) -> Dict:
         headers = self.osdu_auth_backend.headers
         headers["user-token"] = user_token
         url = os.path.join(
             self.osdu_auth_backend.base_url, self.service_path, "impersonation-token"
         )
         request_body = {"resources": resources, "metadata": metadata}
@@ -27,15 +27,15 @@
         )
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def refresh_impersonation_token(
-        self, *, impersonation_token: AnyStr, impersonation_token_context: AnyStr
+        self, *, impersonation_token: str, impersonation_token_context: str
     ) -> Dict:
         headers = self.osdu_auth_backend.headers
         headers["impersonation-token"] = impersonation_token
         headers["impersonation-token-context"] = impersonation_token_context
         url = os.path.join(
             self.osdu_auth_backend.base_url, self.service_path, "impersonation-token"
         )
@@ -43,60 +43,60 @@
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
 
 class SDMSAppsAPI:
-    def register_app(self, *, email: AnyStr, sdpath: AnyStr) -> Dict:
+    def register_app(self, *, email: str, sdpath: str) -> Dict:
         params = {"email": email, "sdpath": sdpath}
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "app",
         )
         response = requests.post(
             url=url, headers=self.osdu_auth_backend.headers, params=params
         )
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
-    def retrive_registered_apps(self, *, sdpath: AnyStr) -> Dict:
+    def retrive_registered_apps(self, *, sdpath: str) -> Dict:
         params = {"sdpath": sdpath}
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "app",
         )
         response = requests.get(
             url=url, headers=self.osdu_auth_backend.headers, params=params
         )
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return {"apps": response.json()}
 
-    def set_trusted_app(self, *, email: AnyStr, sdpath: AnyStr) -> Dict:
+    def set_trusted_app(self, *, email: str, sdpath: str) -> Dict:
         params = {"email": email, "sdpath": sdpath}
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "app/trusted",
         )
         response = requests.post(
             url=url, headers=self.osdu_auth_backend.headers, params=params
         )
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
-    def retrive_trusted_apps(self, *, sdpath: AnyStr) -> Dict:
+    def retrive_trusted_apps(self, *, sdpath: str) -> Dict:
         params = {"sdpath": sdpath}
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             "app/trusted",
         )
         response = requests.get(
@@ -108,18 +108,18 @@
         return {"apps": response.json()}
 
 
 class SDMSDatasetAPI:
     def retrieve_dataset(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        path: Optional[AnyStr] = "/",
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        path: Optional[str] = "/",
         fetch_meta: bool = False,
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}/dataset/{dataset_id}",
         )
@@ -133,18 +133,18 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def retrieve_dataset_permission(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        path: Optional[AnyStr] = "/",
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        path: Optional[str] = "/",
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}/dataset/{dataset_id}/permission",
         )
         # fill path & meta params
@@ -157,18 +157,18 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def delete_dataset(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        path: Optional[AnyStr] = "/",
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        path: Optional[str] = "/",
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}/dataset/{dataset_id}",
         )
         # fill path & meta params
@@ -179,15 +179,15 @@
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def list_subprojects_datasets(
-        self, *, tenant_id: AnyStr, subproject_id: AnyStr
+        self, *, tenant_id: str, subproject_id: str
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}",
         )
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
@@ -196,29 +196,28 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def register_dataset(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        legal_tags: List[AnyStr],
-        gtags: List[AnyStr],
-        other_relevant_data_countries: List[AnyStr],
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        legal_tags: List[str],
+        gtags: List[str],
+        other_relevant_data_countries: List[str],
         data: Dict,
-        type: AnyStr,
+        type: str,
         slm: Dict = {},
-        path: AnyStr = None,
-        kind: AnyStr = None,
-        id: AnyStr = None,
-        parents: List[AnyStr] = [],
+        path: str = None,
+        kind: str = None,
+        id: str = None,
+        parents: List[str] = [],
     ) -> Dict:
-        #tenant_id, *_ = kind.split(":")
 
         request_body = {
             "type": type,
             "gtags": gtags,
             "seismicmeta": {
                 "ancestry": {"parents": parents},
                 "kind": kind,
@@ -252,22 +251,22 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def patch_datasets_metadata(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
         metadata: Dict = {},
         filemetadata: Dict = {},
         seismicmeta: Dict = None,
-        path: AnyStr = None,
-        close: AnyStr = None,
+        path: str = None,
+        close: str = None,
     ) -> Dict:
         request_body = {
             "metadata": metadata,
             "filemetadata": filemetadata,
         }
         if seismicmeta:
             request_body["seismicmeta"] = seismicmeta
@@ -290,20 +289,20 @@
             )
 
         return response.json()
 
     def lock_dataset(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        path: AnyStr = None,
-        openmode: AnyStr = "write",
-        wid: AnyStr = None,
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        path: str = None,
+        openmode: str = "write",
+        wid: str = None,
     ) -> Dict:
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}/dataset/{dataset_id}/lock",
         )
@@ -316,19 +315,19 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def unlock_dataset(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        path: AnyStr,
-        openmode: AnyStr,
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        path: str,
+        openmode: str,
     ) -> Dict:
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"dataset/tenant/{tenant_id}/subproject/{subproject_id}/dataset/{dataset_id}/unlock",
         )
@@ -343,18 +342,18 @@
         return response.json()
 
 
 class SDMSUtilityAPI:
     def generate_gcs_access_token(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        dataset_id: AnyStr,
-        dataset_path: AnyStr = "/",
+        tenant_id: str,
+        subproject_id: str,
+        dataset_id: str,
+        dataset_path: str = "/",
         readonly=False,
     ) -> Dict:
 
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             "api/seismic-store/v3/utility/gcs-access-token",
         )
@@ -391,20 +390,20 @@
         return response.json()
 
 
 class SDMSubprojectAPI:
     def create_new_subproject(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        admin: AnyStr,
-        storage_class: AnyStr = None,
-        storage_location: AnyStr = None,
-        legal_tags: AnyStr = None,
+        tenant_id: str,
+        subproject_id: str,
+        admin: str,
+        storage_class: str = None,
+        storage_location: str = None,
+        legal_tags: str = None,
         acls: Dict = None,
     ) -> Dict:
         request_body = {
             "admin": admin,
             "storage_class": storage_class or "REGIONAL",
             "storage_location": (storage_location).upper(),
         }
@@ -429,30 +428,30 @@
         )
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
-    def get_sdms_subprojects(self, *, tenant_id: AnyStr) -> Dict:
+    def get_sdms_subprojects(self, *, tenant_id: str) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"subproject/tenant/{tenant_id}",
         )
 
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return {"subprojects": response.json()}
 
     def get_sdms_subproject(
-        self, *, tenant_id: AnyStr, subproject_id: AnyStr, translate_user_info=True
+        self, *, tenant_id: str, subproject_id: str, translate_user_info=True
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"subproject/tenant/{tenant_id}",
             f"subproject/{subproject_id}",
         )
@@ -464,15 +463,15 @@
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def delete_sdms_subproject(
-        self, *, tenant_id: AnyStr, subproject_id: AnyStr
+        self, *, tenant_id: str, subproject_id: str
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             self.service_path,
             f"subproject/tenant/{tenant_id}",
             f"subproject/{subproject_id}",
         )
@@ -482,20 +481,20 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
     def patch_sdms_subproject_metadata(
         self,
         *,
-        tenant_id: AnyStr,
-        subproject_id: AnyStr,
-        ltag: AnyStr = None,
+        tenant_id: str,
+        subproject_id: str,
+        ltag: str = None,
         acls: Dict = None,
-        access_policy: AnyStr = None,
-        recursive: AnyStr = None,
+        access_policy: str = None,
+        recursive: str = None,
     ) -> Dict:
         requests_body = {}
         if acls:
             requests_body["acls"] = acls
         if access_policy:
             requests_body["access_policy"] = access_policy
 
@@ -520,30 +519,30 @@
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
 
 class SDMSTenantAPI:
     def register_sdms_tenant(
-        self, *, tenant_id: AnyStr, gcpid: AnyStr, esd: AnyStr, default_acl: AnyStr
+        self, *, tenant_id: str, gcpid: str, esd: str, default_acl: str
     ) -> Dict:
         requests_body = {"gcpid": gcpid, "esd": esd, "default_acl": default_acl}
         url = os.path.join(
             self.osdu_auth_backend.base_url, self.service_path, f"tenant/{tenant_id}"
         )
         response = requests.post(
             url=url, json=requests_body, headers=self.osdu_auth_backend.headers
         )
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
 
         return response.json()
 
-    def get_sdms_tenant(self, *, tenant_id: AnyStr) -> Dict:
+    def get_sdms_tenant(self, *, tenant_id: str) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url, self.service_path, f"tenant/{tenant_id}"
         )
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
 
         if not response.ok:
             raise SDMSAPIError(status_code=response.status_code, message=response.text)
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/search_api.py` & `osdu_client-0.2.7/src/osdu_client/services/search_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import AnyStr, Dict, List
+from typing import Dict, List
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
@@ -12,18 +12,18 @@
 
 
 class SearchAPIClient(BaseOSDUAPIClient):
 
     def search_query(
         self,
         *,
-        kind: AnyStr,
-        query: AnyStr = None,
+        kind: str,
+        query: str = None,
         spatial_filter: Dict = None,
-        returned_fields: List[AnyStr] = None,
+        returned_fields: List[str] = None,
         limit: int = 20,
         offset: int = 0,
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             "api/search/v2/query",
         )
@@ -53,19 +53,19 @@
             )
 
         return response.json()
 
     def search_query_with_cursor(
         self,
         *,
-        kind: AnyStr,
-        query: AnyStr = None,
+        kind: str,
+        query: str = None,
         spatial_filter: Dict = None,
-        returned_fields: List[AnyStr] = None,
-        cursor: AnyStr = None,
+        returned_fields: List[str] = None,
+        cursor: str = None,
         limit: int = 20,
         offset: int = 0,
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             "api/search/v2/query_with_cursor",
         )
```

### Comparing `osdu_client-0.2.6/src/osdu_client/services/storage_api.py` & `osdu_client-0.2.7/src/osdu_client/services/storage_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import AnyStr, Dict, List
+from typing import Dict, List
 
 import requests
 
 from .base_api import BaseOSDUAPIClient
 from .exceptions import OSDUAPIError
 
 
@@ -31,15 +31,15 @@
             )
 
         return response.json()
 
     def get_record(
         self,
         *,
-        id: AnyStr,
+        id: str,
 
 
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             f"api/storage/v2/records/{id}",
         )
@@ -52,15 +52,15 @@
             )
 
         return response.json()
 
     def delete_record(
         self,
         *,
-        id: AnyStr
+        id: str
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             f"api/storage/v2/records/{id}",
         )
         response = requests.delete(url=url, headers=self.osdu_auth_backend.headers)
 
@@ -69,15 +69,15 @@
                 status_code=response.status_code,
                 message=response.text
             )
 
     def get_record_versions(
         self,
         *,
-        id: AnyStr,
+        id: str,
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             f"api/storage/v2/records/versions/{id}",
         )
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
 
@@ -88,15 +88,15 @@
             )
 
         return response.json()
 
     def get_specific_record(
         self,
         *,
-        versioned_id: AnyStr
+        versioned_id: str
     ) -> Dict:
         _id, version = versioned_id.rsplit(":", 1)
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             f"api/storage/v2/records/{_id}/{version}",
         )
         response = requests.get(url=url, headers=self.osdu_auth_backend.headers)
@@ -108,15 +108,15 @@
             )
 
         return response.json()
 
     def query_records(
         self,
         *,
-        records: List[AnyStr]
+        records: List[str]
     ) -> Dict:
         url = os.path.join(
             self.osdu_auth_backend.base_url,
             "api/storage/v2/query/records",
         )
         response = requests.post(
             url=url,
```

### Comparing `osdu_client-0.2.6/src/osdu_client.egg-info/PKG-INFO` & `osdu_client-0.2.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: osdu-client
-Version: 0.2.6
+Name: osdu_client
+Version: 0.2.7
 Summary: OSDU API Client
 Home-page: https://github.com/micmurawski/osdu-client/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -29,29 +29,29 @@
 
 # Example
 OSDU API client can be adjusted to specific OSDU deployment by defining auth backend according to `AuthBackendInterface` methods.
 
 
 
 ```python
-from typing import AnyStr, Dict
+from typing import Dict
 
 from osdu_client import OSDUAPI
 from osdu_client.auth import AuthBackendInterface
 
 
 class AuthBackend(AuthBackendInterface):
     def __init__(self, headers, base_url) -> None:
         self._headers = headers
         self._base_url = base_url
 
     def get_headers(self) -> Dict:
         return self._headers
 
-    def get_base_url(self) -> AnyStr:
+    def get_base_url(self) -> str:
         return self._osdu_base_url
 
     def get_sd_connection_params(self, log_level: int = None) -> Dict:
         return {}
 
 
 auth_backend = AuthBackend(
```

### Comparing `osdu_client-0.2.6/src/osdu_client.egg-info/SOURCES.txt` & `osdu_client-0.2.7/src/osdu_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

