# Comparing `tmp/salure_helpers_azure-1.0.1.tar.gz` & `tmp/salure_helpers_azure-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_azure-1.0.1.tar", last modified: Tue Jun 27 16:04:09 2023, max compression
+gzip compressed data, was "dist/salure_helpers_azure-1.2.1.tar", last modified: Mon Jul 17 15:25:58 2023, max compression
```

## Comparing `salure_helpers_azure-1.0.1.tar` & `salure_helpers_azure-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15697 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/active_directory.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/azure_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/blob_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15716 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/active_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/azure_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3662 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/salure_helpers/azure/blob_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/salure_helpers_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:25:58.000000 salure_helpers_azure-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-07-17 15:25:44.000000 salure_helpers_azure-1.2.1/setup.py
```

### Comparing `salure_helpers_azure-1.0.1/salure_helpers/azure/active_directory.py` & `salure_helpers_azure-1.2.1/salure_helpers/azure/active_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         return: response
         """
         url = f"https://graph.microsoft.com/v1.0/groups/{group_id}/members/$ref"
         data = {"@odata.id": f"https://graph.microsoft.com/v1.0/directoryObjects/{user_id}"}
         response = requests.post(url, headers=self.headers, data=json.dumps(data))
         return response
 
-    def remove_user_from_group(self):
+    def remove_user_from_group(self, user_id, group_id):
         """
         Remove a user from a group
         :param user_id: The Azure AD ID of the user
         :param group_id: The Azure AD ID of the group
         return: response
         """
         url = f"https://graph.microsoft.com/v1.0/groups/{group_id}/members/{user_id}/$ref"
```

### Comparing `salure_helpers_azure-1.0.1/salure_helpers/azure/azure_connection.py` & `salure_helpers_azure-1.2.1/salure_helpers/azure/azure_connection.py`

 * *Files identical despite different names*

