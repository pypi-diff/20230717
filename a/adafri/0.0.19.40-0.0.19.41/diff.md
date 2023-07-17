# Comparing `tmp/adafri-0.0.19.40.tar.gz` & `tmp/adafri-0.0.19.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.40.tar", last modified: Mon Jul 17 02:01:45 2023, max compression
+gzip compressed data, was "adafri-0.0.19.41.tar", last modified: Mon Jul 17 02:31:06 2023, max compression
```

## Comparing `adafri-0.0.19.40.tar` & `adafri-0.0.19.41.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.131446 adafri-0.0.19.40/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:01:45.131109 adafri-0.0.19.40/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.107945 adafri-0.0.19.40/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-17 02:01:40.000000 adafri-0.0.19.40/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.111851 adafri-0.0.19.40/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.40/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.40/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.40/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.112655 adafri-0.0.19.40/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.40/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.113442 adafri-0.0.19.40/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.40/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.115931 adafri-0.0.19.40/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.40/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.40/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.40/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.116834 adafri-0.0.19.40/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.40/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.117992 adafri-0.0.19.40/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.40/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.40/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.118704 adafri-0.0.19.40/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.40/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.119052 adafri-0.0.19.40/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.124126 adafri-0.0.19.40/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6614 2023-07-17 02:01:30.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    14240 2023-07-17 01:30:03.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.125923 adafri-0.0.19.40/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)      885 2023-07-17 01:56:00.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.40/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.127369 adafri-0.0.19.40/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.40/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.40/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.127952 adafri-0.0.19.40/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.40/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.130236 adafri-0.0.19.40/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.40/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.40/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.40/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:01:45.109961 adafri-0.0.19.40/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:01:45.000000 adafri-0.0.19.40/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-17 02:01:45.000000 adafri-0.0.19.40/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-17 02:01:45.000000 adafri-0.0.19.40/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-17 02:01:45.000000 adafri-0.0.19.40/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-17 02:01:45.131586 adafri-0.0.19.40/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.40/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.441291 adafri-0.0.19.41/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:31:06.440829 adafri-0.0.19.41/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.411383 adafri-0.0.19.41/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-17 02:31:00.000000 adafri-0.0.19.41/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.416637 adafri-0.0.19.41/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.41/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.41/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.41/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.417627 adafri-0.0.19.41/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.41/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.418607 adafri-0.0.19.41/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.41/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.421558 adafri-0.0.19.41/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.41/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.41/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.41/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.423000 adafri-0.0.19.41/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.41/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.424692 adafri-0.0.19.41/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.41/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.41/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.425629 adafri-0.0.19.41/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.41/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.426137 adafri-0.0.19.41/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.431935 adafri-0.0.19.41/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    14193 2023-07-17 02:30:19.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.434107 adafri-0.0.19.41/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)      867 2023-07-17 02:30:46.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.41/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.435814 adafri-0.0.19.41/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.41/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.41/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.436456 adafri-0.0.19.41/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.41/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.439660 adafri-0.0.19.41/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.41/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.41/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.41/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:31:06.414013 adafri-0.0.19.41/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:31:06.000000 adafri-0.0.19.41/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-17 02:31:06.000000 adafri-0.0.19.41/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-17 02:31:06.000000 adafri-0.0.19.41/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-17 02:31:06.000000 adafri-0.0.19.41/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-17 02:31:06.441452 adafri-0.0.19.41/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.41/setup.py
```

### Comparing `adafri-0.0.19.40/adafri/utils/response.py` & `adafri-0.0.19.41/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/utils/utils.py` & `adafri-0.0.19.41/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/account/models/account.py` & `adafri-0.0.19.41/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.41/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.41/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,14 @@
     def check_endpoint_auth_method(self, method, endpoint):
         if endpoint == 'token':
             # if client table has ``token_endpoint_auth_method``
             return self.token_endpoint_auth_method == method
         return True
     
     def check_grant_type(self, grant_type):
-        print('check_grant_type', grant_type)
-        print('client grant_types', self.grant_types)
         return grant_type in self.grant_types
     
     def get_allowed_scope(self, scope):
         if not scope:
             return ''
         allowed = set(scope_to_list(self.scope))
         return list_to_scope([s for s in scope.split() if s in allowed])
```

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Authorization code {self.id} deleted"}, None);
         except:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
 
     
 
 class AuthorizationCodeGrant(grants.AuthorizationCodeGrant):
-    # RESPONSE_TYPES = set({"code"})
     TOKEN_ENDPOINT_AUTH_METHODS = [
         'client_secret_basic',
         'client_secret_post',
         'none'
     ]
     def save_authorization_code(self, code, request):
         code_challenge = request.data.get('code_challenge')
@@ -247,19 +246,19 @@
         "nonce": nonce,
     }
     auth_code = OAuthGrant.create(**grant)
     return auth_code.data
 
 class OpenIDAuthorizationCodeGrant(grants.AuthorizationCodeGrant):
     # RESPONSE_TYPES = set({"code"})
-    # TOKEN_ENDPOINT_AUTH_METHODS = [
-    #     'client_secret_basic',
-    #     'client_secret_post',
-    #     'none'
-    # ]
+    TOKEN_ENDPOINT_AUTH_METHODS = [
+        'client_secret_basic',
+        'client_secret_post',
+        'none'
+    ]
     def save_authorization_code(self, code, request):
         code_challenge = request.data.get('code_challenge')
         code_challenge_method = request.data.get('code_challenge_method')
         redirect_uri = request.redirect_uri;
         nonce = request.data.get('nonce')
         if request.args.get("redirect_uri") is not None:
             redirect_uri = request.args.get("redirect_uri");
```

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 require_oidc_oauth = ResourceProtector()
 
 def config_oidc_oauth(app):
     oidc_authorization_server.query_client = OAuthClient().get_by_client_id
     oidc_authorization_server.save_token = OAuthToken().save
     oidc_authorization_server.init_app(app)
     oidc_authorization_server.register_grant(AuthCodeGrant, [
-        OpenIDCode(require_nonce=True),
+        OpenIDCode(),
     ])
     oidc_authorization_server.register_grant(OpenIDImplicitGrant)
     oidc_authorization_server.register_grant(OpenIDHybridGrant)
     require_oidc_oauth.register_token_validator(TokenValidator())
```

### Comparing `adafri-0.0.19.40/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.19.41/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.41/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/user/models/user.py` & `adafri-0.0.19.41/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.41/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.41/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.40/setup.py` & `adafri-0.0.19.41/setup.py`

 * *Files identical despite different names*

