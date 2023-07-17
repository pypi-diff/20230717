# Comparing `tmp/saagieapi-2.6.1.tar.gz` & `tmp/saagieapi-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.6.1.tar", max compression
+gzip compressed data, was "saagieapi-2.6.2.tar", max compression
```

## Comparing `saagieapi-2.6.1.tar` & `saagieapi-2.6.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-06-28 09:33:57.612337 saagieapi-2.6.1/LICENSE
--rw-r--r--   0        0        0     4612 2023-06-28 09:33:57.612337 saagieapi-2.6.1/README.md
--rw-r--r--   0        0        0     1562 2023-06-28 09:34:27.021018 saagieapi-2.6.1/pyproject.toml
--rw-r--r--   0        0        0      583 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     7591 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    27280 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     4677 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       49 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/groups/__init__.py
--rw-r--r--   0        0        0    14568 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/groups/groups.py
--rw-r--r--   0        0        0       43 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     9510 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36521 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      222 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     8853 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     3572 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    30113 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/profiles/__init__.py
--rw-r--r--   0        0        0     4954 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/profiles/profiles.py
--rw-r--r--   0        0        0       55 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24404 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    19545 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/storages/storages.py
--rw-r--r--   0        0        0       46 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/users/__init__.py
--rw-r--r--   0        0        0    10981 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/users/users.py
--rw-r--r--   0        0        0        0 2023-06-28 09:33:57.616337 saagieapi-2.6.1/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-06-28 09:33:57.620337 saagieapi-2.6.1/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-06-28 09:33:57.620337 saagieapi-2.6.1/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-06-28 09:33:57.620337 saagieapi-2.6.1/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0     2336 2023-06-28 09:33:57.620337 saagieapi-2.6.1/saagieapi/utils/request_client.py
--rw-r--r--   0        0        0       54 2023-06-28 09:33:57.620337 saagieapi-2.6.1/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 saagieapi-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 15:09:43.512164 saagieapi-2.6.2/LICENSE
+-rw-r--r--   0        0        0     4612 2023-07-17 15:09:43.512164 saagieapi-2.6.2/README.md
+-rw-r--r--   0        0        0     1562 2023-07-17 15:10:19.487647 saagieapi-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0      583 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    33369 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0     7591 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     4677 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       49 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/groups/__init__.py
+-rw-r--r--   0        0        0    14568 2023-07-17 15:09:43.520164 saagieapi-2.6.2/saagieapi/groups/groups.py
+-rw-r--r--   0        0        0       43 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0     9510 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    36521 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      222 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     8853 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     3572 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    30113 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/profiles/__init__.py
+-rw-r--r--   0        0        0     4954 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/profiles/profiles.py
+-rw-r--r--   0        0        0       55 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24508 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    19545 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0       46 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/users/__init__.py
+-rw-r--r--   0        0        0    10981 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/users/users.py
+-rw-r--r--   0        0        0        0 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0     2336 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/request_client.py
+-rw-r--r--   0        0        0       54 2023-07-17 15:09:43.524164 saagieapi-2.6.2/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 saagieapi-2.6.2/PKG-INFO
```

### Comparing `saagieapi-2.6.1/LICENSE` & `saagieapi-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/README.md` & `saagieapi-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/pyproject.toml` & `saagieapi-2.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.6.1"
+version = "2.6.2"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
```

### Comparing `saagieapi-2.6.1/saagieapi/__init__.py` & `saagieapi-2.6.2/saagieapi/__init__.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/apps/apps.py` & `saagieapi-2.6.2/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/apps/gql_queries.py` & `saagieapi-2.6.2/saagieapi/apps/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.6.2/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.6.2/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/env_vars/env_vars.py` & `saagieapi-2.6.2/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.6.2/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/gql_queries.py` & `saagieapi-2.6.2/saagieapi/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/groups/groups.py` & `saagieapi-2.6.2/saagieapi/groups/groups.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/jobs/gql_queries.py` & `saagieapi-2.6.2/saagieapi/jobs/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/jobs/jobs.py` & `saagieapi-2.6.2/saagieapi/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.6.2/saagieapi/pipelines/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.6.2/saagieapi/pipelines/graph_pipeline.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/pipelines/pipelines.py` & `saagieapi-2.6.2/saagieapi/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/profiles/profiles.py` & `saagieapi-2.6.2/saagieapi/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/projects/gql_queries.py` & `saagieapi-2.6.2/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/projects/projects.py` & `saagieapi-2.6.2/saagieapi/projects/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,21 @@
 
         if group and role:
             saagie_role = Projects.__map_role(role)
             group_block = [{"name": group, "role": saagie_role}]
             params["authorizedGroups"] = group_block
             return params
 
-        raise RuntimeError(
-            "❌ Too few arguments, specify either a group and role, "
-            "or multiple groups and roles with groups_and_roles"
-        )
+        if (group and role is None) or (group is None and role):
+            raise RuntimeError(
+                "❌ Too few arguments, specify either a group and role, "
+                "or multiple groups and roles with groups_and_roles"
+            )
+
+        return params
 
     def list(self, pprint_result: Optional[bool] = None) -> Dict:
         """Get information for all projects (id, name, creator, description,
         jobCount and status)
         NB: You can only list projects you have rights on.
 
         Parameters
```

### Comparing `saagieapi-2.6.1/saagieapi/repositories/gql_queries.py` & `saagieapi-2.6.2/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/repositories/repositories.py` & `saagieapi-2.6.2/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/saagie_api.py` & `saagieapi-2.6.2/saagieapi/saagie_api.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/storages/gql_queries.py` & `saagieapi-2.6.2/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/storages/storages.py` & `saagieapi-2.6.2/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/users/users.py` & `saagieapi-2.6.2/saagieapi/users/users.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/utils/bearer_auth.py` & `saagieapi-2.6.2/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/utils/folder_functions.py` & `saagieapi-2.6.2/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/utils/gql_client.py` & `saagieapi-2.6.2/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/saagieapi/utils/request_client.py` & `saagieapi-2.6.2/saagieapi/utils/request_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.1/PKG-INFO` & `saagieapi-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.6.1
+Version: 2.6.2
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

