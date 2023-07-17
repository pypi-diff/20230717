# Comparing `tmp/iconsdk-2.4.5.tar.gz` & `tmp/iconsdk-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iconsdk-2.4.5.tar", last modified: Thu Apr 27 03:33:25 2023, max compression
+gzip compressed data, was "dist/iconsdk-2.5.0.tar", last modified: Mon Jul 17 06:59:23 2023, max compression
```

## Comparing `iconsdk-2.4.5.tar` & `iconsdk-2.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-27 03:33:25.000000 iconsdk-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-27 03:33:16.000000 iconsdk-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/builder/call_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/builder/transaction_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/icon_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/libs/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/libs/in_memory_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/libs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/libs/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/providers/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/signed_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/convert_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/hexadecimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/utils/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/typing/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-27 03:33:16.000000 iconsdk-2.4.5/iconsdk/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-27 03:33:24.000000 iconsdk-2.4.5/iconsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-27 03:33:25.000000 iconsdk-2.4.5/iconsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:33:24.000000 iconsdk-2.4.5/iconsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 03:33:24.000000 iconsdk-2.4.5/iconsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 03:33:24.000000 iconsdk-2.4.5/iconsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 03:33:25.000000 iconsdk-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-27 03:33:16.000000 iconsdk-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-07-17 06:59:23.000000 iconsdk-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33508 2023-07-17 06:59:14.000000 iconsdk-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/builder/call_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/builder/transaction_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22579 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/icon_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/libs/in_memory_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/libs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/libs/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/providers/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/signed_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/convert_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/hexadecimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/utils/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/typing/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-17 06:59:14.000000 iconsdk-2.5.0/iconsdk/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-07-17 06:59:22.000000 iconsdk-2.5.0/iconsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 06:59:23.000000 iconsdk-2.5.0/iconsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:59:22.000000 iconsdk-2.5.0/iconsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 06:59:22.000000 iconsdk-2.5.0/iconsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 06:59:22.000000 iconsdk-2.5.0/iconsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 06:59:23.000000 iconsdk-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-17 06:59:14.000000 iconsdk-2.5.0/setup.py
```

### Comparing `iconsdk-2.4.5/PKG-INFO` & `iconsdk-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.5
+Version: 2.5.0
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
@@ -813,15 +813,15 @@
         # Generates an instance of transaction for deploying SCORE.
         transaction = DeployTransactionBuilder()\
             .from_(wallet.get_address())\
             .to("cx00...02")\
             .step_limit(1000000)\
             .nid(3)\
             .nonce(100)\
-            .content_type("application/zip")\
+            .content_type("application/java")\
             .content(b'D8\xe9...\xfc')\
             .params(params)\
             .build()
         
         # Generates an instance of transaction for calling method in SCORE.
         transaction = CallTransactionBuilder()\
             .from_(wallet.get_address())\
@@ -939,15 +939,15 @@
         # Generates an instance of transaction for deploying SCORE.
         transaction = DeployTransactionBuilder()\
             .from_(wallet.get_address())\
             .to("cx00...02")\
             .step_limit(1000000)\
             .nid(3)\
             .nonce(100)\
-            .content_type("application/zip")\
+            .content_type("application/java")\
             .content(b'D8\xe9...\xfc')\
             .params(params)\
             .build()
         ```
```

### Comparing `iconsdk-2.4.5/README.md` & `iconsdk-2.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -805,15 +805,15 @@
 # Generates an instance of transaction for deploying SCORE.
 transaction = DeployTransactionBuilder()\
     .from_(wallet.get_address())\
     .to("cx00...02")\
     .step_limit(1000000)\
     .nid(3)\
     .nonce(100)\
-    .content_type("application/zip")\
+    .content_type("application/java")\
     .content(b'D8\xe9...\xfc')\
     .params(params)\
     .build()
 
 # Generates an instance of transaction for calling method in SCORE.
 transaction = CallTransactionBuilder()\
     .from_(wallet.get_address())\
@@ -931,15 +931,15 @@
 # Generates an instance of transaction for deploying SCORE.
 transaction = DeployTransactionBuilder()\
     .from_(wallet.get_address())\
     .to("cx00...02")\
     .step_limit(1000000)\
     .nid(3)\
     .nonce(100)\
-    .content_type("application/zip")\
+    .content_type("application/java")\
     .content(b'D8\xe9...\xfc')\
     .params(params)\
     .build()
 ```
```

### Comparing `iconsdk-2.4.5/iconsdk/__init__.py` & `iconsdk-2.5.0/iconsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/builder/__init__.py` & `iconsdk-2.5.0/iconsdk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/builder/call_builder.py` & `iconsdk-2.5.0/iconsdk/builder/call_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/builder/transaction_builder.py` & `iconsdk-2.5.0/iconsdk/builder/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/exception.py` & `iconsdk-2.5.0/iconsdk/exception.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/icon_service.py` & `iconsdk-2.5.0/iconsdk/icon_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -526,8 +526,18 @@
         Monitor events specified in the spec
 
         :param spec: Monitor specification
         :param keep_alive: interval to send keep-alive while it reads a message
         in fraction of seconds
         :return: Monitoring handle
         """
-        return self.__provider.make_monitor(spec, keep_alive)
+        return self.__provider.make_monitor(spec, keep_alive)
+
+    def get_network_info(self) -> dict:
+        """
+        Returns basic network information
+        Delegates to icx_getNetworkInfo RPC method.
+        https://github.com/icon-project/goloop/blob/master/doc/jsonrpc_v3.md#icx_getNetworkInfo
+
+        :return: Basic network information
+        """
+        return self.__provider.make_request('icx_getNetworkInfo')
```

### Comparing `iconsdk-2.4.5/iconsdk/libs/__init__.py` & `iconsdk-2.5.0/iconsdk/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/libs/in_memory_zip.py` & `iconsdk-2.5.0/iconsdk/libs/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/libs/serializer.py` & `iconsdk-2.5.0/iconsdk/libs/serializer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/libs/signer.py` & `iconsdk-2.5.0/iconsdk/libs/signer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/monitor.py` & `iconsdk-2.5.0/iconsdk/monitor.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/providers/__init__.py` & `iconsdk-2.5.0/iconsdk/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/providers/http_provider.py` & `iconsdk-2.5.0/iconsdk/providers/http_provider.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/providers/provider.py` & `iconsdk-2.5.0/iconsdk/providers/provider.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/signed_transaction.py` & `iconsdk-2.5.0/iconsdk/signed_transaction.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/__init__.py` & `iconsdk-2.5.0/iconsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/convert_type.py` & `iconsdk-2.5.0/iconsdk/utils/convert_type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/converter.py` & `iconsdk-2.5.0/iconsdk/utils/converter.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/hexadecimal.py` & `iconsdk-2.5.0/iconsdk/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/templates.py` & `iconsdk-2.5.0/iconsdk/utils/templates.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/type.py` & `iconsdk-2.5.0/iconsdk/utils/type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/typing/__init__.py` & `iconsdk-2.5.0/iconsdk/utils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/typing/conversion.py` & `iconsdk-2.5.0/iconsdk/utils/typing/conversion.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/utils/validation.py` & `iconsdk-2.5.0/iconsdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/wallet/__init__.py` & `iconsdk-2.5.0/iconsdk/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk/wallet/wallet.py` & `iconsdk-2.5.0/iconsdk/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/iconsdk.egg-info/PKG-INFO` & `iconsdk-2.5.0/iconsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.5
+Version: 2.5.0
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
@@ -813,15 +813,15 @@
         # Generates an instance of transaction for deploying SCORE.
         transaction = DeployTransactionBuilder()\
             .from_(wallet.get_address())\
             .to("cx00...02")\
             .step_limit(1000000)\
             .nid(3)\
             .nonce(100)\
-            .content_type("application/zip")\
+            .content_type("application/java")\
             .content(b'D8\xe9...\xfc')\
             .params(params)\
             .build()
         
         # Generates an instance of transaction for calling method in SCORE.
         transaction = CallTransactionBuilder()\
             .from_(wallet.get_address())\
@@ -939,15 +939,15 @@
         # Generates an instance of transaction for deploying SCORE.
         transaction = DeployTransactionBuilder()\
             .from_(wallet.get_address())\
             .to("cx00...02")\
             .step_limit(1000000)\
             .nid(3)\
             .nonce(100)\
-            .content_type("application/zip")\
+            .content_type("application/java")\
             .content(b'D8\xe9...\xfc')\
             .params(params)\
             .build()
         ```
```

### Comparing `iconsdk-2.4.5/iconsdk.egg-info/SOURCES.txt` & `iconsdk-2.5.0/iconsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.5/setup.py` & `iconsdk-2.5.0/setup.py`

 * *Files identical despite different names*

