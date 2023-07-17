# Comparing `tmp/scratchrequest-0.5.0.tar.gz` & `tmp/scratchrequest-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchrequest-0.5.0.tar", last modified: Mon Jul 17 09:09:56 2023, max compression
+gzip compressed data, was "scratchrequest-0.5.1.tar", last modified: Mon Jul 17 16:32:18 2023, max compression
```

## Comparing `scratchrequest-0.5.0.tar` & `scratchrequest-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:09:56.865633 scratchrequest-0.5.0/
--rw-rw-rw-   0        0        0     1091 2023-07-06 16:37:14.000000 scratchrequest-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      724 2023-07-17 09:09:56.851637 scratchrequest-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        2 2023-07-06 16:23:32.000000 scratchrequest-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 09:09:56.715636 scratchrequest-0.5.0/scratchrequest/
--rw-rw-rw-   0        0        0      158 2023-07-03 18:02:47.000000 scratchrequest-0.5.0/scratchrequest/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-07-03 16:44:51.000000 scratchrequest-0.5.0/scratchrequest/_cloud.py
--rw-rw-rw-   0        0        0      322 2023-07-17 09:03:00.000000 scratchrequest-0.5.0/scratchrequest/_exceptions.py
--rw-rw-rw-   0        0        0     1899 2023-07-17 09:02:31.000000 scratchrequest-0.5.0/scratchrequest/_project.py
--rw-rw-rw-   0        0        0     3878 2023-07-16 19:16:17.000000 scratchrequest-0.5.0/scratchrequest/_session.py
--rw-rw-rw-   0        0        0     2974 2023-07-03 18:36:49.000000 scratchrequest-0.5.0/scratchrequest/_twcloud.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:09:56.840632 scratchrequest-0.5.0/scratchrequest.egg-info/
--rw-rw-rw-   0        0        0      724 2023-07-17 09:09:56.000000 scratchrequest-0.5.0/scratchrequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-07-17 09:09:56.000000 scratchrequest-0.5.0/scratchrequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:09:56.000000 scratchrequest-0.5.0/scratchrequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-17 09:09:56.000000 scratchrequest-0.5.0/scratchrequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-17 09:09:56.000000 scratchrequest-0.5.0/scratchrequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 09:09:56.866636 scratchrequest-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-17 09:07:05.000000 scratchrequest-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:32:18.705210 scratchrequest-0.5.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-06 16:37:14.000000 scratchrequest-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-07-17 16:32:18.702208 scratchrequest-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2023-07-06 16:23:32.000000 scratchrequest-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 16:32:18.635210 scratchrequest-0.5.1/scratchrequest/
+-rw-rw-rw-   0        0        0      158 2023-07-03 18:02:47.000000 scratchrequest-0.5.1/scratchrequest/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-07-03 16:44:51.000000 scratchrequest-0.5.1/scratchrequest/_cloud.py
+-rw-rw-rw-   0        0        0      322 2023-07-17 09:03:00.000000 scratchrequest-0.5.1/scratchrequest/_exceptions.py
+-rw-rw-rw-   0        0        0     1946 2023-07-17 10:39:16.000000 scratchrequest-0.5.1/scratchrequest/_project.py
+-rw-rw-rw-   0        0        0     3798 2023-07-17 10:39:49.000000 scratchrequest-0.5.1/scratchrequest/_session.py
+-rw-rw-rw-   0        0        0     2974 2023-07-03 18:36:49.000000 scratchrequest-0.5.1/scratchrequest/_twcloud.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:32:18.694210 scratchrequest-0.5.1/scratchrequest.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-07-17 16:32:18.000000 scratchrequest-0.5.1/scratchrequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-07-17 16:32:18.000000 scratchrequest-0.5.1/scratchrequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:32:18.000000 scratchrequest-0.5.1/scratchrequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-17 16:32:18.000000 scratchrequest-0.5.1/scratchrequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 16:32:18.000000 scratchrequest-0.5.1/scratchrequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:32:18.706210 scratchrequest-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-17 16:29:38.000000 scratchrequest-0.5.1/setup.py
```

### Comparing `scratchrequest-0.5.0/LICENSE` & `scratchrequest-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.5.0/PKG-INFO` & `scratchrequest-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchrequest
-Version: 0.5.0
+Version: 0.5.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/programordie2/scratchrequest
 Author: programORdie
 Author-email: 
 Keywords: scratch api,scratchrequest,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchrequest-0.5.0/scratchrequest/_cloud.py` & `scratchrequest-0.5.1/scratchrequest/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.5.0/scratchrequest/_project.py` & `scratchrequest-0.5.1/scratchrequest/_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import requests
 from ._exceptions import AuthError, UploadError, DownloadError, ProjectNotFound
 
 class CreateConnectProject:
-  def __init__(self, id: str, username: str=None, session_id: str=None, csrf: str=None, xtoken: str=None):
+  def __init__(self, id: str, session=None):
+    if session == None:
+      username = None
+    else:    
+      self.username = session.username
+      self.session_id = session.session_id
+      self.csrf_token = session.csrf_token
+      self.xtoken = session.xtoken
     self.id = id
-    self.username = username
-    self.session_id = session_id
-    self.csrf_token = csrf
-    self.xtoken = xtoken
     self._get_all_data()
 
   def _get_all_data(self):
     try:
       self._all_data = requests.get(f'https://api.scratch.mit.edu/projects/{self.id}/').json()
       self._all_data['id']
     except KeyError:
```

### Comparing `scratchrequest-0.5.0/scratchrequest/_session.py` & `scratchrequest-0.5.1/scratchrequest/_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,8 +84,8 @@
         '''
         return _cloud.CreateCloudConnection(project_id=project_id, session=self, **kwargs)
 
     def ConnectProject(self, id : int) -> _project.CreateConnectProject:
         '''
         Create a connection to a project.
         '''
-        return _project.CreateConnectProject(id=id, username=self.username, session_id=self.session_id, csrf=self.csrf_token, xtoken=self.xtoken)
+        return _project.CreateConnectProject(id=id, session=self)
```

### Comparing `scratchrequest-0.5.0/scratchrequest/_twcloud.py` & `scratchrequest-0.5.1/scratchrequest/_twcloud.py`

 * *Files identical despite different names*

### Comparing `scratchrequest-0.5.0/scratchrequest.egg-info/PKG-INFO` & `scratchrequest-0.5.1/scratchrequest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchrequest
-Version: 0.5.0
+Version: 0.5.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/programordie2/scratchrequest
 Author: programORdie
 Author-email: 
 Keywords: scratch api,scratchrequest,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchrequest-0.5.0/setup.py` & `scratchrequest-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchrequest",
     version=VERSION,
```

