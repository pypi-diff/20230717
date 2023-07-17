# Comparing `tmp/basking-sdk-0.9.8.tar.gz` & `tmp/basking-sdk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basking-sdk-0.9.8.tar", last modified: Tue Aug  9 10:21:32 2022, max compression
+gzip compressed data, was "basking-sdk-0.9.9.tar", last modified: Wed Aug 10 10:34:10 2022, max compression
```

## Comparing `basking-sdk-0.9.8.tar` & `basking-sdk-0.9.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1064 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2461 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2037 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/basking_sdk.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2461 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/basking_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      483 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/basking_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/basking_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      638 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/basking_sdk.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        8 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/basking_sdk.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      600 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1871 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/setup.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1867 2022-08-09 10:21:32.000000 basking-sdk-0.9.8/setup_tmp.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/src/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-09 10:21:32.423314 basking-sdk-0.9.8/src/basking/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1698 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4213 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/api_usage_example.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7998 2022-08-09 09:24:44.000000 basking-sdk-0.9.8/src/basking/basking_sdk.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      296 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/constant.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    25477 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/graphql_query.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3584 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/insight.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10083 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/location.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    46802 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/occupancy.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12606 2022-08-09 09:19:48.000000 basking-sdk-0.9.8/src/basking/organization.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 10:34:10.711421 basking-sdk-0.9.9/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1064 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3828 2022-08-10 10:34:10.707421 basking-sdk-0.9.9/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2037 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 10:34:10.707421 basking-sdk-0.9.9/basking_sdk.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3828 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/basking_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      483 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/basking_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/basking_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      638 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/basking_sdk.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        8 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/basking_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      600 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2022-08-10 10:34:10.711421 basking-sdk-0.9.9/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1871 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/setup.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1867 2022-08-10 10:34:10.000000 basking-sdk-0.9.9/setup_tmp.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 10:34:10.707421 basking-sdk-0.9.9/src/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-08-10 10:34:10.707421 basking-sdk-0.9.9/src/basking/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1698 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4213 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/api_usage_example.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7998 2022-08-10 10:33:27.000000 basking-sdk-0.9.9/src/basking/basking_sdk.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      296 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/constant.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25477 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/graphql_query.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3584 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/insight.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10083 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/location.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    46802 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/occupancy.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12606 2022-08-09 10:41:14.000000 basking-sdk-0.9.9/src/basking/organization.py
```

### Comparing `basking-sdk-0.9.8/LICENSE` & `basking-sdk-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/PKG-INFO` & `basking-sdk-0.9.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: basking-sdk
-Version: 0.9.8
-Summary: Basking.io python SDK
-Home-page: https://basking.io
-Author: Basking Automation GmbH
-Author-email: info@basking.io
-License: UNKNOWN
-Project-URL: Bug Reports, https://basking.io/contact-us/
-Keywords: occupancy analytics data api bas basking basking.io
-Platform: UNKNOWN
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Basking.io SDK
 
 Integrate your data with the Basking API, customize the reports & experience,
 and join the community of developers building with workplace software apps together with Basking.
 
 Basking.io is a cloud based workplace occupancy platform.
 More Information about Basking can be found here: https://basking.io
@@ -69,9 +54,8 @@
 end_obj_tz_unaware=end_date_obj,
 pandify=True
 )
 df_daily.to_csv('./df_daily.csv')
 ```
 
 
-For more examples, see `basking.api_usage_example`, or [contact us](https://basking.io/contact-us/)
-
+For more examples, see `basking.api_usage_example`, or [contact us](https://basking.io/contact-us/)
```

### Comparing `basking-sdk-0.9.8/README.md` & `basking-sdk-0.9.9/src/basking/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,18 @@
+"""
 # Basking.io SDK
 
-Integrate your data with the Basking API, customize the reports & experience,
-and join the community of developers building with workplace software apps together with Basking.
+## Welcome to Basking.io Python SDK Documentation!
+Integrate your data with the Basking API, customize the reports & experience, and join the community of developers building with workplace software apps together with Basking.
+Basking.io is a cloud based workplace occupancy platform. More Information about Basking can be found here: https://basking.io
 
-Basking.io is a cloud based workplace occupancy platform.
-More Information about Basking can be found here: https://basking.io
+Basking uses a GraphQL API. The following Python SDK is a wrapper around the production API designed for our customers that require to access to data programmatically.
 
-Basking uses a GraphQL API. The following Python SDK is a wrapper around the production API
-designed for our customers that require to access to data programmatically.
-
-## Requirements
-
-* python >=3.7 (current tested version: 3.9)
-* pipenv
-* A [basking.io account](https://app.basking.io)
-
-## Getting started
-
-#### set the following environment variables:
-* `BASKING_USERNAME`: Your username (usually your email)
-* `BASKING_USER_PASSWORD`: Your password for Basking. 
-* _Optional_: `BASKING_AWS_REGION`: the aws region where your Basking.io instance is hosted. (Defaults to `eu-central-1`)
-* _Optional_: `BASKING_API_URL`: the url of the Basking API you would like to query. (Defaults to `api.basking.io`)
+## Getting Started
+More examples can be found in `basking.api_usage_examples`
 
 ```
 import logging
 from basking.basking_sdk import Basking
 
 # set the default logging
 logging.basicConfig()
@@ -42,20 +29,21 @@
 
 # get building meta data
 building_meta_data = basking_client.location.get_building(
 building_id=building_id
 )
 tz_str = building_meta_data['data']['getBuilding']['timeZone']
 
-
 # get building daily occupancy statistics
 df_daily = basking_client.occupancy.get_building_occupancy_stats_daily(
 building_id=building_id,
 start_obj_tz_unaware=start_date_obj,
 end_obj_tz_unaware=end_date_obj,
 pandify=True
 )
 df_daily.to_csv('./df_daily.csv')
 ```
+"""
 
-
-For more examples, see `basking.api_usage_example`, or [contact us](https://basking.io/contact-us/)
+from os import environ
+if not ('BASKING_USER_PASSWORD' in environ and 'BASKING_USERNAME' in environ):
+    raise EnvironmentError("Missing Basking.io credentials")
```

### Comparing `basking-sdk-0.9.8/basking_sdk.egg-info/requires.txt` & `basking-sdk-0.9.9/basking_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/pyproject.toml` & `basking-sdk-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/setup.py` & `basking-sdk-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/setup_tmp.py` & `basking-sdk-0.9.9/setup_tmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(path.join(path.abspath(path.dirname(__file__)), "README.md"), 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     # https://packaging.python.org/specifications/core-metadata/#name
     name="basking-sdk",  # Required
     # https://www.python.org/dev/peps/pep-0440/
-    version="0.9.8",
+    version="0.9.9",
     description="Basking.io python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://basking.io",
     author="Basking Automation GmbH",
     author_email="info@basking.io",
     keywords="occupancy analytics data api bas basking basking.io",
```

### Comparing `basking-sdk-0.9.8/src/basking/api_usage_example.py` & `basking-sdk-0.9.9/src/basking/api_usage_example.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/src/basking/basking_sdk.py` & `basking-sdk-0.9.9/src/basking/basking_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         """
         response = self._boto3_client.initiate_auth(
             AuthFlow='USER_PASSWORD_AUTH',
             AuthParameters={
                 'USERNAME': os.environ['BASKING_USERNAME'],
                 'PASSWORD': os.environ['BASKING_USER_PASSWORD']
             },
-            ClientId='3ehjj0o7hel3dpcmr8uu1ncckd'  
+            ClientId='7o5vqv7ukt9onolq1nvjt7m40e'  
         )
 
         return response
 
     def api_timeout_handler(self, api_data):
         """
         for handle api timeout error coming from graphql_query
```

### Comparing `basking-sdk-0.9.8/src/basking/graphql_query.py` & `basking-sdk-0.9.9/src/basking/graphql_query.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/src/basking/insight.py` & `basking-sdk-0.9.9/src/basking/insight.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/src/basking/location.py` & `basking-sdk-0.9.9/src/basking/location.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/src/basking/occupancy.py` & `basking-sdk-0.9.9/src/basking/occupancy.py`

 * *Files identical despite different names*

### Comparing `basking-sdk-0.9.8/src/basking/organization.py` & `basking-sdk-0.9.9/src/basking/organization.py`

 * *Files identical despite different names*

