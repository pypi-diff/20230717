# Comparing `tmp/Opensource License Compatibility from DoWell-0.2.0.tar.gz` & `tmp/Opensource License Compatibility from DoWell-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Opensource License Compatibility from DoWell-0.2.0.tar", last modified: Mon Jul 17 16:30:10 2023, max compression
+gzip compressed data, was "Opensource License Compatibility from DoWell-0.3.0.tar", last modified: Mon Jul 17 16:34:31 2023, max compression
```

## Comparing `Opensource License Compatibility from DoWell-0.2.0.tar` & `Opensource License Compatibility from DoWell-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.721293 Opensource License Compatibility from DoWell-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.707117 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/
--rw-rw-rw-   0        0        0    10657 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-07-17 16:30:10.000000 Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10657 2023-07-17 16:30:10.720298 Opensource License Compatibility from DoWell-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10152 2023-07-17 16:29:28.000000 Opensource License Compatibility from DoWell-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 16:30:10.712254 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/
--rw-rw-rw-   0        0        0       86 2023-07-17 16:16:50.000000 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/__init__.py
--rw-rw-rw-   0        0        0     5274 2023-07-17 16:16:38.000000 Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py
--rw-rw-rw-   0        0        0       42 2023-07-17 16:30:10.722345 Opensource License Compatibility from DoWell-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      786 2023-07-17 16:28:39.000000 Opensource License Compatibility from DoWell-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:34:31.879531 Opensource License Compatibility from DoWell-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-07-17 16:34:31.862725 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/
+-rw-rw-rw-   0        0        0    10657 2023-07-17 16:34:31.000000 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-17 16:34:31.000000 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:34:31.000000 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 16:34:31.000000 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-07-17 16:34:31.000000 Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10657 2023-07-17 16:34:31.877752 Opensource License Compatibility from DoWell-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10152 2023-07-17 16:34:27.000000 Opensource License Compatibility from DoWell-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 16:34:31.874999 Opensource License Compatibility from DoWell-0.3.0/doWellOpensourceLicenseCompatibility/
+-rw-rw-rw-   0        0        0       86 2023-07-17 16:16:50.000000 Opensource License Compatibility from DoWell-0.3.0/doWellOpensourceLicenseCompatibility/__init__.py
+-rw-rw-rw-   0        0        0     5715 2023-07-17 16:34:07.000000 Opensource License Compatibility from DoWell-0.3.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:34:31.879531 Opensource License Compatibility from DoWell-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      786 2023-07-17 16:34:23.000000 Opensource License Compatibility from DoWell-0.3.0/setup.py
```

### Comparing `Opensource License Compatibility from DoWell-0.2.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO` & `Opensource License Compatibility from DoWell-0.3.0/Opensource_License_Compatibility_from_DoWell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Opensource-License-Compatibility-from-DoWell
-Version: 0.2.0
+Version: 0.3.0
 Summary: Opensource License Compatibility from DoWell
 Author: DoWell UX Living Lab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
 # Dowell Opensource License Compatibility Library
 
-## Version 0.2.0
+## Version 0.3.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
```

### Comparing `Opensource License Compatibility from DoWell-0.2.0/PKG-INFO` & `Opensource License Compatibility from DoWell-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Opensource License Compatibility from DoWell
-Version: 0.2.0
+Version: 0.3.0
 Summary: Opensource License Compatibility from DoWell
 Author: DoWell UX Living Lab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
 # Dowell Opensource License Compatibility Library
 
-## Version 0.2.0
+## Version 0.3.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
```

### Comparing `Opensource License Compatibility from DoWell-0.2.0/README.md` & `Opensource License Compatibility from DoWell-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dowell Opensource License Compatibility Library
 
-## Version 0.2.0
+## Version 0.3.0
 
 ## Description
 
 The DoWell Legalzard Package provides a seamless interface to the Dowell Opensource License Compatibility Library powered
 by [DoWell UX Living Lab](https://uxlivinglab.com/en/).
 
 The Dowell Opensource License Compatibility Library provides access to a wide range of legal information and resources. It allows developers to retrieve
```

### Comparing `Opensource License Compatibility from DoWell-0.2.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py` & `Opensource License Compatibility from DoWell-0.3.0/doWellOpensourceLicenseCompatibility/doWellOpensourceLicenseCompatibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,101 @@
 import json
 
-LEGALZARD_API = 'https://100080.pythonanywhere.com/api/licenses/'
+LEGALZARD_API = 'https://100080.pythonanywhere.com/api/public/licenses/'
 import requests
+from requests.structures import CaseInsensitiveDict
 
 
 class doWellOpensourceLicenseCompatibility:
+    headers = CaseInsensitiveDict()
+
+    def __init__(self, api_key):
+        self.headers['API-KEY'] = api_key
+
     def _response(self, request):
-        if request.status_code == 200:
+        if request.status_code in [200, 201]:
             return request.json()
         return json.dumps({'Error': '{} {}'.format(request.status_code, request.content.decode('utf-8'))})
 
     def get_all(self):
         """
         Get all licenses submitted
         :return: An Object with retrieval status and an list of all licenses
 
         The response body
 
         :param: isSuccess: A boolean showing retrieval status
         :param data: A list of licenses.
 
         """
-        return self._response(requests.get(url=LEGALZARD_API))
+        return self._response(requests.get(url=LEGALZARD_API, headers=self.headers))
 
     def create(self, license: dict):
         """
         Create a license by adding all the fields required
         :param license: An object with the following license parameters as listed in the main documentation.
         :return: Retrieval Object with a single license information that was created
         The response body
 
         :param: isSuccess: A boolean showing retrieval status
         :param data: A list with a single license.
         """
-        return self._response(requests.post(url=LEGALZARD_API, data=json.dumps(license)))
+        return self._response(requests.post(url=LEGALZARD_API, json=json.dumps(license), headers=self.headers))
 
     def retrieve(self, event_id: str):
         """
         Retrieve license information using an ID
         :param event_id: A string ID of the license
         :return: Retrieval Object with a single license information that was created
         The response body
 
         :param: isSuccess: A boolean showing retrieval status
         :param data: A list with a single license.
         """
-        return self._response(requests.get(url='{}{}/'.format(LEGALZARD_API, event_id)))
+        return self._response(requests.get(url='{}{}/'.format(LEGALZARD_API, event_id), headers=self.headers))
 
     def update(self, event_id: str, license: dict):
         """
         This method updates the license information stored on the database
         :param event_id: This is the eventId parameter from the license information already stored
         :param license: An object with the following license parameters as listed in the main documentation.
         :return: New updated license information
 
         The response body
 
         :param: isSuccess: A boolean showing retrieval status
         :param data: A list with a single license.
         """
-        return self._response(requests.put(url='{}{}/'.format(LEGALZARD_API, event_id), data=json.dumps(license)))
+        return self._response(
+            requests.put(url='{}{}/'.format(LEGALZARD_API, event_id), json=json.dumps(license), headers=self.headers))
 
     def delete(self, event_id: str):
         """
         Use this method to delete a license
         :param event_id: This is the eventId parameter from the license information already stored
         :return: A success object with
 
         :param: event_id: The license that was deleted
         :param isSuccess: Status of the action
         """
-        return self._response(requests.delete(url='{}{}/'.format(LEGALZARD_API, event_id)))
+        return self._response(requests.delete(url='{}{}/'.format(LEGALZARD_API, event_id), headers=self.headers))
 
     def search(self, search_term: str):
         """
         Use this method to search for licenses containing some phrase
         :param search_term: This is the search phrase used to filter the licenses
         :return: Licenses matching the search parameters
         The response body
 
         :param: isSuccess: A boolean showing retrieval status
         :param data: A list with matching licenses.
         """
         return self._response(
-            requests.get(url=LEGALZARD_API, params={'action_type': 'search', 'search_term': search_term}))
+            requests.get(url=LEGALZARD_API, params={'action_type': 'search', 'search_term': search_term},
+                         headers=self.headers))
 
     def check_compatibility(self, comparison_data: dict):
         """
         This method allows you to check license compatibility of two licenses
         :param comparison_data: An object with the comparison fields
         :return: Comparison results
 
@@ -106,24 +114,25 @@
         :param license_2_event_id: License 2 event_id
         :param identifier: Comparison Id
         :param license_1: License object for license 1
         :param license_2: License object for license 2
 
         """
         comparison_data['action_type'] = 'check-compatibility'
-        return self._response(requests.post(url=LEGALZARD_API, data=json.dumps(comparison_data)))
+        return self._response(requests.post(url=LEGALZARD_API, json=json.dumps(comparison_data), headers=self.headers))
 
-    def get_compatibility_history(self, organization_id: str, user_id: str):
+    def get_compatibility_history(self, organization_id: str = None, user_id: str = None):
         """
         Get Compatibility Check History by a user.
         :param organization_id: Your Organization Id
         :param user_id: Your User Id
         :return: A Comparison History Object
 
         The Response body
 
         :param isSuccess: Request status
         :param data: a list of License comparison history objects
         """
         return self._response(
             requests.get(url=LEGALZARD_API, params={'collection_type': 'license-compatibility-history',
-                                                    'organization_id': organization_id, 'user_id': user_id}))
+                                                    'organization_id': organization_id, 'user_id': user_id},
+                         headers=self.headers))
```

### Comparing `Opensource License Compatibility from DoWell-0.2.0/setup.py` & `Opensource License Compatibility from DoWell-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="Opensource License Compatibility from DoWell",
-    version="0.2.0",
+    version="0.3.0",
     description="Opensource License Compatibility from DoWell",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='DoWell UX Living Lab',
     license="Apache License 2.0",
     packages=["doWellOpensourceLicenseCompatibility"],
     include_package_data=True,
```

