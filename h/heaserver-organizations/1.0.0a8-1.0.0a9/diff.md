# Comparing `tmp/heaserver-organizations-1.0.0a8.tar.gz` & `tmp/heaserver-organizations-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heaserver-organizations-1.0.0a8.tar", last modified: Thu Feb 24 23:23:35 2022, max compression
+gzip compressed data, was "dist\heaserver-organizations-1.0.0a9.tar", last modified: Fri Feb 25 00:15:43 2022, max compression
```

## Comparing `heaserver-organizations-1.0.0a8.tar` & `heaserver-organizations-1.0.0a9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.102634 heaserver-organizations-1.0.0a8/
--rw-rw-rw-   0        0        0    11625 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0       39 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4649 2022-02-24 23:23:35.101635 heaserver-organizations-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3208 2022-02-24 21:21:03.000000 heaserver-organizations-1.0.0a8/README.md
--rw-rw-rw-   0        0        0       42 2022-02-24 23:23:35.102634 heaserver-organizations-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1967 2022-02-24 23:23:19.000000 heaserver-organizations-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.041647 heaserver-organizations-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.040639 heaserver-organizations-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.054633 heaserver-organizations-1.0.0a8/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    16230 2022-02-24 21:21:03.000000 heaserver-organizations-1.0.0a8/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.056640 heaserver-organizations-1.0.0a8/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0     6076 2022-02-18 21:43:20.000000 heaserver-organizations-1.0.0a8/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.093635 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     4649 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-02-24 23:23:34.000000 heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.042632 heaserver-organizations-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.042632 heaserver-organizations-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-02-24 23:23:35.098634 heaserver-organizations-1.0.0a8/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a8/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0      451 2021-10-14 22:23:35.000000 heaserver-organizations-1.0.0a8/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     4120 2022-01-25 16:19:05.000000 heaserver-organizations-1.0.0a8/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.968106 heaserver-organizations-1.0.0a9/
+-rw-rw-rw-   0        0        0    11625 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0       39 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4649 2022-02-25 00:15:43.967109 heaserver-organizations-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3208 2022-02-24 21:21:03.000000 heaserver-organizations-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0       42 2022-02-25 00:15:43.969107 heaserver-organizations-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1967 2022-02-25 00:15:16.000000 heaserver-organizations-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.875120 heaserver-organizations-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.873105 heaserver-organizations-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.898107 heaserver-organizations-1.0.0a9/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a9/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    16412 2022-02-25 00:10:28.000000 heaserver-organizations-1.0.0a9/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.900107 heaserver-organizations-1.0.0a9/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0     6390 2022-02-25 00:07:32.000000 heaserver-organizations-1.0.0a9/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.940109 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     4649 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-02-25 00:15:43.000000 heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.877107 heaserver-organizations-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.878105 heaserver-organizations-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2022-02-25 00:15:43.965108 heaserver-organizations-1.0.0a9/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2021-10-14 22:23:34.000000 heaserver-organizations-1.0.0a9/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0      451 2021-10-14 22:23:35.000000 heaserver-organizations-1.0.0a9/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     4120 2022-01-25 16:19:05.000000 heaserver-organizations-1.0.0a9/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver-organizations-1.0.0a8/LICENSE` & `heaserver-organizations-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.0a8/PKG-INFO` & `heaserver-organizations-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-organizations-1.0.0a8/README.md` & `heaserver-organizations-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.0a8/setup.py` & `heaserver-organizations-1.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.8',
```

### Comparing `heaserver-organizations-1.0.0a8/src/heaserver/organization/service.py` & `heaserver-organizations-1.0.0a9/src/heaserver/organization/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from heaserver.service.heaobjectsupport import type_to_resource_url
 from heaserver.service import response, client
 from heaobject.organization import Organization
 from heaobject.account import AWSAccount
 from heaobject.volume import AWSFileSystem, Volume
 from yarl import URL
 from asyncio import gather
+from typing import Optional, Dict
 import logging
 
 
 _logger = logging.getLogger(__name__)
 
 MONGODB_ORGANIZATION_COLLECTION = 'organizations'
 
@@ -99,15 +100,15 @@
 
     :param request: the HTTP request. Required.
     :return: the requested form, or Not Found if the requested organization was not found.
     """
     return await mongoservicelib.get(request, MONGODB_ORGANIZATION_COLLECTION)
 
 
-@routes.post('/organization/duplicator')
+@routes.post('/organizations/duplicator')
 async def post_organization_duplicator(request: web.Request) -> web.Response:
     """
     Posts the provided organization for duplication.
     :param request: the HTTP request.
     :return: a Response object with a status of Created and the object's URI in the
     """
     return await mongoservicelib.post(request, MONGODB_ORGANIZATION_COLLECTION, Organization)
@@ -410,14 +411,15 @@
         $ref: '#/components/responses/404'
     """
     return await mongoservicelib.opener(request, MONGODB_ORGANIZATION_COLLECTION)
 
 
 @routes.get('/organizations/{id}/awsaccounts')
 @routes.get('/organizations/{id}/awsaccounts/')
+@action('heaserver-organizations-aws-account-get-open-choices', rel='hea-opener-choices', path='/awsaccounts/{account_id}/opener')
 async def get_organization_aws_accounts(request: web.Request) -> web.Response:
     """
 
     :param request: the HTTP Request.
     :return: a Response object with a status code of 200.
     ---
     summary: An organization's AWS accounts.
@@ -430,29 +432,29 @@
         $ref: '#/components/responses/200'
     """
     org_dict = await request.app[HEA_DB].get(request, MONGODB_ORGANIZATION_COLLECTION, var_parts='id')
     if org_dict is None:
         return response.status_not_found()
     org = Organization()
     org.from_dict(org_dict)
-    headers = {SUB: request.headers.get(SUB)} if SUB in request.headers else None
+    headers = {SUB: request.headers.get(SUB, '')} if SUB in request.headers else None
 
     volume_url = await type_to_resource_url(request, Volume)
     if volume_url is None:
         raise ValueError('No Volume service registered')
     get_volumes_url = URL(volume_url) / 'byfilesystemtype' / AWSFileSystem.get_type_name()
 
     aws_account_url = await type_to_resource_url(request, AWSAccount, file_system_type_or_type_name=AWSFileSystem)
     if aws_account_url is None:
         raise ValueError('No AWSAccount service registered')
 
     async def get_one(volume_id):
         return await client.get(request.app, URL(aws_account_url) / volume_id / 'awsaccounts' / 'me', AWSAccount, headers=headers)
 
-    result = [a for a in await gather(*[get_one(v.id) async for v in client.get_all(request.app, get_volumes_url, Volume, headers=headers)]) if a.account_id in org.aws_account_ids]
+    result = [a.to_dict() for a in await gather(*[get_one(v.id) async for v in client.get_all(request.app, get_volumes_url, Volume, headers=headers)]) if a.account_id in org.aws_account_ids]
     return await response.get_all(request, result)
 
 
 def main() -> None:
     config = init_cmd_line(description='a service for managing organization information for research laboratories and other research groups',
                            default_port=8087)
     start(db=mongo.Mongo, wstl_builder_factory=builder_factory(__package__), config=config)
```

### Comparing `heaserver-organizations-1.0.0a8/src/heaserver/organization/wstl/all.json` & `heaserver-organizations-1.0.0a9/src/heaserver/organization/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'wstl'": "{'actions': {insert: [(5, OrderedDict([('name', "*

 * *           "'heaserver-organizations-aws-account-get-open-choices'), ('description', 'Open this "*

 * *           "AWS account'), ('type', 'safe'), ('action', 'read'), ('target', 'item read cj'), "*

 * *           "('prompt', 'Open')]))]}}"}*

```diff
@@ -158,12 +158,20 @@
             {
                 "action": "read",
                 "description": "Open AWS accounts",
                 "name": "heaserver-organizations-organization-open-aws-accounts",
                 "prompt": "Open",
                 "target": "item read cj",
                 "type": "safe"
+            },
+            {
+                "action": "read",
+                "description": "Open this AWS account",
+                "name": "heaserver-organizations-aws-account-get-open-choices",
+                "prompt": "Open",
+                "target": "item read cj",
+                "type": "safe"
             }
         ],
         "title": "HEA Server Organization"
     }
 }
```

### Comparing `heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-organizations-1.0.0a8/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver-organizations-1.0.0a9/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.0.0a8/tests/heaserver/organizationtest/testcase.py` & `heaserver-organizations-1.0.0a9/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

