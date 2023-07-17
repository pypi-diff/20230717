# Comparing `tmp/mindsight_people_control_api-0.1.8.tar.gz` & `tmp/mindsight_people_control_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsight_people_control_api-0.1.8.tar", max compression
+gzip compressed data, was "mindsight_people_control_api-0.1.9.tar", max compression
```

## Comparing `mindsight_people_control_api-0.1.8.tar` & `mindsight_people_control_api-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/LICENSE
--rw-r--r--   0        0        0     1342 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/README.md
--rw-r--r--   0        0        0      428 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/__init__.py
--rw-r--r--   0        0        0     5225 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/base_requests.py
--rw-r--r--   0        0        0      392 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/exceptions.py
--rw-r--r--   0        0        0     1869 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/models.py
--rw-r--r--   0        0        0      865 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/__init__.py
--rw-r--r--   0        0        0     4566 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/area_records.py
--rw-r--r--   0        0        0     7415 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/areas.py
--rw-r--r--   0        0        0     5513 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_areas.py
--rw-r--r--   0        0        0     5591 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_managers.py
--rw-r--r--   0        0        0     5623 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_positions.py
--rw-r--r--   0        0        0     4896 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_records.py
--rw-r--r--   0        0        0    12367 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employees.py
--rw-r--r--   0        0        0     4721 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/parent_areas.py
--rw-r--r--   0        0        0     2057 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/position_records.py
--rw-r--r--   0        0        0     7060 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/positions.py
--rw-r--r--   0        0        0     7654 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/users.py
--rw-r--r--   0        0        0      895 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/settings.py
--rw-r--r--   0        0        0        0 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/utils/__init__.py
--rw-r--r--   0        0        0      308 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/mindsight_people_control_api/utils/aux_functions.py
--rw-r--r--   0        0        0      747 2023-06-28 21:02:05.682726 mindsight_people_control_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1355 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/README.md
+-rw-r--r--   0        0        0      428 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/__init__.py
+-rw-r--r--   0        0        0     5225 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/base_requests.py
+-rw-r--r--   0        0        0      392 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/exceptions.py
+-rw-r--r--   0        0        0     1869 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/models.py
+-rw-r--r--   0        0        0      865 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/area_records.py
+-rw-r--r--   0        0        0     7415 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/areas.py
+-rw-r--r--   0        0        0     5513 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_areas.py
+-rw-r--r--   0        0        0     5591 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_managers.py
+-rw-r--r--   0        0        0     5623 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_positions.py
+-rw-r--r--   0        0        0     4896 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_records.py
+-rw-r--r--   0        0        0    12367 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employees.py
+-rw-r--r--   0        0        0     4721 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/parent_areas.py
+-rw-r--r--   0        0        0     2057 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/position_records.py
+-rw-r--r--   0        0        0     7060 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/positions.py
+-rw-r--r--   0        0        0     7654 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/users.py
+-rw-r--r--   0        0        0      896 2023-06-29 17:09:18.716174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/settings.py
+-rw-r--r--   0        0        0        0 2023-06-29 17:09:18.720174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/utils/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-29 17:09:18.720174 mindsight_people_control_api-0.1.9/mindsight_people_control_api/utils/aux_functions.py
+-rw-r--r--   0        0        0      747 2023-06-29 17:09:18.720174 mindsight_people_control_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.9/PKG-INFO
```

### Comparing `mindsight_people_control_api-0.1.8/LICENSE` & `mindsight_people_control_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/README.md` & `mindsight_people_control_api-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 ```
 
 # Configuration
 ## Environment variables
 To use mindsight-people-control-api, you need to set two environment variables:
 ```dotenv
 # ---DOTENV EXAMPLE---
-MINDSIGHT_API_TOKEN= # Token to authenticate
-MINDSIGHT_API_BASE_URL=https://controle.mindsight.com.br/api # Base path of your api instance
+MINDSIGHT_CP_API_TOKEN= # Token to authenticate
+MINDSIGHT_CP_API_URL=https://controle.mindsight.com.br/api # Base path of your api instance
 ```
 # Usage Example
-You can use mindsight-people-control-api create, update and delete registers on all system tables.
+You can use mindsight-people-control-api in order to create, update and delete registers on all system tables.
 
 ## List registers
 You can use get methods to list registers of system table. See the following example:
 ```python
 import mindsight_people_control_api
```

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/base_requests.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/base_requests.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/helpers/models.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/helpers/models.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/__init__.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/area_records.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/area_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/areas.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_areas.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_managers.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_managers.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_positions.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employee_records.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employee_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/employees.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/employees.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/parent_areas.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/parent_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/position_records.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/position_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/positions.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/scripts/users.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/scripts/users.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.8/mindsight_people_control_api/settings.py` & `mindsight_people_control_api-0.1.9/mindsight_people_control_api/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module define project configurations variables"""
 
 from decouple import config
 
 # API Constants
-API_TOKEN = config("MINDSIGHT_API_TOKEN")
-API_BASE_URL = config("MINDSIGHT_API_BASE_URL")
+API_TOKEN = config("MINDSIGHT_CP_API_TOKEN")
+API_BASE_URL = config("MINDSIGHT_CP_API_URL")
 API_VERSION = "v1"
 
 # Request config
 PAGE_SIZE: int = 1000
 TIMEOUT: int = 600  # Default set to 600 seconds (10 minutes)
 
 # Date formats
```

### Comparing `mindsight_people_control_api-0.1.8/pyproject.toml` & `mindsight_people_control_api-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mindsight-people-control-api"
-version = "0.1.8"
+version = "0.1.9"
 description = "Mindsight People Control API to create, update and delete records"
 authors = ["stone_people_analytics <systems-techpeople@stone.com.br>"]
 maintainers = [
     "diogo56 <diogo.amorim2001@gmail.com>",
     "guilherme_lsilva <manager.guilherme.silva@gmail.com>",
     "root-who <joaopaulo_gonzaga@outlook.com>",
 ]
```

### Comparing `mindsight_people_control_api-0.1.8/PKG-INFO` & `mindsight_people_control_api-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsight-people-control-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Mindsight People Control API to create, update and delete records
 Home-page: https://github.com/people-analytics-tech/mindsight-people-control-api
 License: MIT
 Author: stone_people_analytics
 Author-email: systems-techpeople@stone.com.br
 Maintainer: diogo56
 Maintainer-email: diogo.amorim2001@gmail.com
@@ -29,19 +29,19 @@
 ```
 
 # Configuration
 ## Environment variables
 To use mindsight-people-control-api, you need to set two environment variables:
 ```dotenv
 # ---DOTENV EXAMPLE---
-MINDSIGHT_API_TOKEN= # Token to authenticate
-MINDSIGHT_API_BASE_URL=https://controle.mindsight.com.br/api # Base path of your api instance
+MINDSIGHT_CP_API_TOKEN= # Token to authenticate
+MINDSIGHT_CP_API_URL=https://controle.mindsight.com.br/api # Base path of your api instance
 ```
 # Usage Example
-You can use mindsight-people-control-api create, update and delete registers on all system tables.
+You can use mindsight-people-control-api in order to create, update and delete registers on all system tables.
 
 ## List registers
 You can use get methods to list registers of system table. See the following example:
 ```python
 import mindsight_people_control_api
```

