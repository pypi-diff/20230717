# Comparing `tmp/affectivecloud-1.1.1.tar.gz` & `tmp/affectivecloud-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affectivecloud-1.1.1.tar", last modified: Mon May 15 02:03:28 2023, max compression
+gzip compressed data, was "affectivecloud-1.1.2.tar", last modified: Mon Jul 17 03:26:22 2023, max compression
```

## Comparing `affectivecloud-1.1.1.tar` & `affectivecloud-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.742218 affectivecloud-1.1.1/
--rw-r--r--   0 chenyitao   (501) staff       (20)     1056 2022-07-22 08:53:27.000000 affectivecloud-1.1.1/LICENSE
--rw-r--r--   0 chenyitao   (501) staff       (20)     2735 2023-05-15 02:03:28.742017 affectivecloud-1.1.1/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)     1716 2023-05-15 02:02:29.000000 affectivecloud-1.1.1/README.md
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.736064 affectivecloud-1.1.1/affectivecloud/
--rw-r--r--   0 chenyitao   (501) staff       (20)       51 2022-07-22 08:59:31.000000 affectivecloud-1.1.1/affectivecloud/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)       22 2022-07-26 10:21:02.000000 affectivecloud-1.1.1/affectivecloud/__version__.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.738180 affectivecloud-1.1.1/affectivecloud/algorithm/
--rw-r--r--   0 chenyitao   (501) staff       (20)      177 2022-07-22 08:36:20.000000 affectivecloud-1.1.1/affectivecloud/algorithm/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)      853 2022-07-25 08:05:08.000000 affectivecloud-1.1.1/affectivecloud/algorithm/affective_services.py
--rw-r--r--   0 chenyitao   (501) staff       (20)      183 2022-07-25 08:05:00.000000 affectivecloud-1.1.1/affectivecloud/algorithm/base_services.py
--rw-r--r--   0 chenyitao   (501) staff       (20)    12567 2022-07-25 08:47:13.000000 affectivecloud-1.1.1/affectivecloud/client.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.738772 affectivecloud-1.1.1/affectivecloud/protocols/
--rw-r--r--   0 chenyitao   (501) staff       (20)      603 2022-07-22 08:39:39.000000 affectivecloud-1.1.1/affectivecloud/protocols/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     2372 2022-07-25 08:30:56.000000 affectivecloud-1.1.1/affectivecloud/protocols/protocol.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.739927 affectivecloud-1.1.1/affectivecloud/protocols/requests/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 04:02:15.000000 affectivecloud-1.1.1/affectivecloud/protocols/requests/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     3443 2022-07-25 08:49:31.000000 affectivecloud-1.1.1/affectivecloud/protocols/requests/affective_service.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     4497 2022-07-25 08:50:49.000000 affectivecloud-1.1.1/affectivecloud/protocols/requests/base_service.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     3604 2022-07-25 08:51:39.000000 affectivecloud-1.1.1/affectivecloud/protocols/requests/session.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.741600 affectivecloud-1.1.1/affectivecloud/protocols/responses/
--rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 04:02:17.000000 affectivecloud-1.1.1/affectivecloud/protocols/responses/__init__.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     2183 2022-07-25 09:00:07.000000 affectivecloud-1.1.1/affectivecloud/protocols/responses/affective_service.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     1363 2022-07-25 09:01:43.000000 affectivecloud-1.1.1/affectivecloud/protocols/responses/base.py
--rw-r--r--   0 chenyitao   (501) staff       (20)     2175 2022-07-25 09:00:37.000000 affectivecloud-1.1.1/affectivecloud/protocols/responses/base_service.py
--rw-r--r--   0 chenyitao   (501) staff       (20)      707 2022-07-25 09:00:50.000000 affectivecloud-1.1.1/affectivecloud/protocols/responses/session.py
-drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-05-15 02:03:28.737394 affectivecloud-1.1.1/affectivecloud.egg-info/
--rw-r--r--   0 chenyitao   (501) staff       (20)     2735 2023-05-15 02:03:28.000000 affectivecloud-1.1.1/affectivecloud.egg-info/PKG-INFO
--rw-r--r--   0 chenyitao   (501) staff       (20)      973 2023-05-15 02:03:28.000000 affectivecloud-1.1.1/affectivecloud.egg-info/SOURCES.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)       84 2023-05-15 02:03:28.000000 affectivecloud-1.1.1/affectivecloud.egg-info/dependency_links.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-26 01:51:56.000000 affectivecloud-1.1.1/affectivecloud.egg-info/not-zip-safe
--rw-r--r--   0 chenyitao   (501) staff       (20)       16 2023-05-15 02:03:28.000000 affectivecloud-1.1.1/affectivecloud.egg-info/requires.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)       15 2023-05-15 02:03:28.000000 affectivecloud-1.1.1/affectivecloud.egg-info/top_level.txt
--rw-r--r--   0 chenyitao   (501) staff       (20)       38 2023-05-15 02:03:28.742407 affectivecloud-1.1.1/setup.cfg
--rw-r--r--   0 chenyitao   (501) staff       (20)     1644 2023-05-15 02:03:19.000000 affectivecloud-1.1.1/setup.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.317370 affectivecloud-1.1.2/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1056 2022-07-22 08:53:27.000000 affectivecloud-1.1.2/LICENSE
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2735 2023-07-17 03:26:22.317145 affectivecloud-1.1.2/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1716 2023-05-15 02:02:29.000000 affectivecloud-1.1.2/README.md
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.311177 affectivecloud-1.1.2/affectivecloud/
+-rw-r--r--   0 chenyitao   (501) staff       (20)       51 2022-07-22 08:59:31.000000 affectivecloud-1.1.2/affectivecloud/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)       22 2023-07-17 03:26:17.000000 affectivecloud-1.1.2/affectivecloud/__version__.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.313272 affectivecloud-1.1.2/affectivecloud/algorithm/
+-rw-r--r--   0 chenyitao   (501) staff       (20)      177 2022-07-22 08:36:20.000000 affectivecloud-1.1.2/affectivecloud/algorithm/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)      853 2022-07-25 08:05:08.000000 affectivecloud-1.1.2/affectivecloud/algorithm/affective_services.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)      183 2022-07-25 08:05:00.000000 affectivecloud-1.1.2/affectivecloud/algorithm/base_services.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)    12567 2022-07-25 08:47:13.000000 affectivecloud-1.1.2/affectivecloud/client.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.313868 affectivecloud-1.1.2/affectivecloud/protocols/
+-rw-r--r--   0 chenyitao   (501) staff       (20)      603 2022-07-22 08:39:39.000000 affectivecloud-1.1.2/affectivecloud/protocols/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2372 2022-07-25 08:30:56.000000 affectivecloud-1.1.2/affectivecloud/protocols/protocol.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.315089 affectivecloud-1.1.2/affectivecloud/protocols/requests/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 04:02:15.000000 affectivecloud-1.1.2/affectivecloud/protocols/requests/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     3443 2022-07-25 08:49:31.000000 affectivecloud-1.1.2/affectivecloud/protocols/requests/affective_service.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     4497 2022-07-25 08:50:49.000000 affectivecloud-1.1.2/affectivecloud/protocols/requests/base_service.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     3604 2022-07-25 08:51:39.000000 affectivecloud-1.1.2/affectivecloud/protocols/requests/session.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.316727 affectivecloud-1.1.2/affectivecloud/protocols/responses/
+-rw-r--r--   0 chenyitao   (501) staff       (20)        0 2022-07-14 04:02:17.000000 affectivecloud-1.1.2/affectivecloud/protocols/responses/__init__.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2183 2022-07-25 09:00:07.000000 affectivecloud-1.1.2/affectivecloud/protocols/responses/affective_service.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1363 2022-07-25 09:01:43.000000 affectivecloud-1.1.2/affectivecloud/protocols/responses/base.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2175 2022-07-25 09:00:37.000000 affectivecloud-1.1.2/affectivecloud/protocols/responses/base_service.py
+-rw-r--r--   0 chenyitao   (501) staff       (20)      707 2022-07-25 09:00:50.000000 affectivecloud-1.1.2/affectivecloud/protocols/responses/session.py
+drwxr-xr-x   0 chenyitao   (501) staff       (20)        0 2023-07-17 03:26:22.312409 affectivecloud-1.1.2/affectivecloud.egg-info/
+-rw-r--r--   0 chenyitao   (501) staff       (20)     2735 2023-07-17 03:26:22.000000 affectivecloud-1.1.2/affectivecloud.egg-info/PKG-INFO
+-rw-r--r--   0 chenyitao   (501) staff       (20)      973 2023-07-17 03:26:22.000000 affectivecloud-1.1.2/affectivecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)       84 2023-07-17 03:26:22.000000 affectivecloud-1.1.2/affectivecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)        1 2022-07-26 01:51:56.000000 affectivecloud-1.1.2/affectivecloud.egg-info/not-zip-safe
+-rw-r--r--   0 chenyitao   (501) staff       (20)       16 2023-07-17 03:26:22.000000 affectivecloud-1.1.2/affectivecloud.egg-info/requires.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)       15 2023-07-17 03:26:22.000000 affectivecloud-1.1.2/affectivecloud.egg-info/top_level.txt
+-rw-r--r--   0 chenyitao   (501) staff       (20)       38 2023-07-17 03:26:22.317440 affectivecloud-1.1.2/setup.cfg
+-rw-r--r--   0 chenyitao   (501) staff       (20)     1644 2023-07-17 03:25:54.000000 affectivecloud-1.1.2/setup.py
```

### Comparing `affectivecloud-1.1.1/LICENSE` & `affectivecloud-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/PKG-INFO` & `affectivecloud-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affectivecloud
-Version: 1.1.1
+Version: 1.1.2
 Summary: AffectiveCloud Python SDK
 Home-page: https://github.com/Entertech/Enter-Affectivecloud-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
 Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `affectivecloud-1.1.1/README.md` & `affectivecloud-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/algorithm/affective_services.py` & `affectivecloud-1.1.2/affectivecloud/algorithm/affective_services.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/client.py` & `affectivecloud-1.1.2/affectivecloud/client.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/__init__.py` & `affectivecloud-1.1.2/affectivecloud/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/protocol.py` & `affectivecloud-1.1.2/affectivecloud/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/requests/affective_service.py` & `affectivecloud-1.1.2/affectivecloud/protocols/requests/affective_service.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/requests/base_service.py` & `affectivecloud-1.1.2/affectivecloud/protocols/requests/base_service.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/requests/session.py` & `affectivecloud-1.1.2/affectivecloud/protocols/requests/session.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/responses/affective_service.py` & `affectivecloud-1.1.2/affectivecloud/protocols/responses/affective_service.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/responses/base.py` & `affectivecloud-1.1.2/affectivecloud/protocols/responses/base.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/responses/base_service.py` & `affectivecloud-1.1.2/affectivecloud/protocols/responses/base_service.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud/protocols/responses/session.py` & `affectivecloud-1.1.2/affectivecloud/protocols/responses/session.py`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/affectivecloud.egg-info/PKG-INFO` & `affectivecloud-1.1.2/affectivecloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affectivecloud
-Version: 1.1.1
+Version: 1.1.2
 Summary: AffectiveCloud Python SDK
 Home-page: https://github.com/Entertech/Enter-Affectivecloud-PC-SDK.git
 Author: Lockey
 Author-email: chenyitao@entertech.cn
 License: Entertech
 Platform: UNKNOWN
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `affectivecloud-1.1.1/affectivecloud.egg-info/SOURCES.txt` & `affectivecloud-1.1.2/affectivecloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `affectivecloud-1.1.1/setup.py` & `affectivecloud-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='affectivecloud',
-    version='1.1.1',
+    version='1.1.2',
     description='AffectiveCloud Python SDK',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Natural Language :: Chinese (Simplified)',
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
@@ -42,11 +42,11 @@
         ]
     ),
     include_package_data=False,
     install_requires=[
         'websockets==9.1',
     ],
     dependency_links=[
-        'git+https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git@v1.1.2#egg=enterble',
+        'git+https://github.com/Entertech/Enter-Biomodule-BLE-PC-SDK.git@v1.1.3#egg=enterble',
     ],
     zip_safe=False
 )
```

