# Comparing `tmp/alibabacloud_dyvmsapi-intl20211015-1.0.0.tar.gz` & `tmp/alibabacloud_dyvmsapi-intl20211015-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dyvmsapi-intl20211015-1.0.0.tar", last modified: Wed Nov 30 10:09:39 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dyvmsapi-intl20211015-2.0.0.tar", last modified: Mon Jul 17 07:37:52 2023, max compression
```

## Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0.tar` & `alibabacloud_dyvmsapi-intl20211015-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170349 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/client.py
--rw-r--r--   0 root         (0) root         (0)   282483 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2662 2022-11-30 10:09:39.000000 alibabacloud_dyvmsapi-intl20211015-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   170477 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/client.py
+-rw-r--r--   0 root         (0) root         (0)   282817 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-07-17 07:37:52.000000 alibabacloud_dyvmsapi-intl20211015-2.0.0/setup.py
```

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/LICENSE` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/PKG-INFO` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dyvmsapi-intl20211015
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/README-CN.md` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/README.md` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/client.py` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         query = {}
         if not UtilClient.is_unset(request.called_number_shrink):
             query['CalledNumber'] = request.called_number_shrink
         if not UtilClient.is_unset(request.caller_id_number):
             query['CallerIdNumber'] = request.caller_id_number
         if not UtilClient.is_unset(request.country_id):
             query['CountryId'] = request.country_id
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_times):
             query['PlayTimes'] = request.play_times
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -112,14 +114,16 @@
         query = {}
         if not UtilClient.is_unset(request.called_number_shrink):
             query['CalledNumber'] = request.called_number_shrink
         if not UtilClient.is_unset(request.caller_id_number):
             query['CallerIdNumber'] = request.caller_id_number
         if not UtilClient.is_unset(request.country_id):
             query['CountryId'] = request.country_id
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_times):
             query['PlayTimes'] = request.play_times
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -180,14 +184,16 @@
         query = {}
         if not UtilClient.is_unset(request.called_number):
             query['CalledNumber'] = request.called_number
         if not UtilClient.is_unset(request.caller_id_number):
             query['CallerIdNumber'] = request.caller_id_number
         if not UtilClient.is_unset(request.country_id):
             query['CountryId'] = request.country_id
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_times):
             query['PlayTimes'] = request.play_times
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -228,14 +234,16 @@
         query = {}
         if not UtilClient.is_unset(request.called_number):
             query['CalledNumber'] = request.called_number
         if not UtilClient.is_unset(request.caller_id_number):
             query['CallerIdNumber'] = request.caller_id_number
         if not UtilClient.is_unset(request.country_id):
             query['CountryId'] = request.country_id
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_times):
             query['PlayTimes'] = request.play_times
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -2722,16 +2730,14 @@
     ) -> dyvmsapi_intl_20211015_models.QueryRecordingEnableResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QueryRecordingEnable',
             version='2021-10-15',
             protocol='HTTPS',
@@ -2754,16 +2760,14 @@
     ) -> dyvmsapi_intl_20211015_models.QueryRecordingEnableResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
-        if not UtilClient.is_unset(request.resource_owner_id):
-            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QueryRecordingEnable',
             version='2021-10-15',
             protocol='HTTPS',
```

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015/models.py` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class BackendCallGroupRequest(TeaModel):
     def __init__(
         self,
         called_number: List[str] = None,
         caller_id_number: str = None,
         country_id: str = None,
+        out_id: str = None,
         owner_id: int = None,
         play_times: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         send_type: int = None,
         speed: int = None,
         task_name: str = None,
@@ -21,14 +22,15 @@
         tts_code: str = None,
         voice_code: str = None,
         volume: int = None,
     ):
         self.called_number = called_number
         self.caller_id_number = caller_id_number
         self.country_id = country_id
+        self.out_id = out_id
         self.owner_id = owner_id
         self.play_times = play_times
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.send_type = send_type
         self.speed = speed
         self.task_name = task_name
@@ -48,14 +50,16 @@
         result = dict()
         if self.called_number is not None:
             result['CalledNumber'] = self.called_number
         if self.caller_id_number is not None:
             result['CallerIdNumber'] = self.caller_id_number
         if self.country_id is not None:
             result['CountryId'] = self.country_id
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_times is not None:
             result['PlayTimes'] = self.play_times
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
@@ -80,14 +84,16 @@
         m = m or dict()
         if m.get('CalledNumber') is not None:
             self.called_number = m.get('CalledNumber')
         if m.get('CallerIdNumber') is not None:
             self.caller_id_number = m.get('CallerIdNumber')
         if m.get('CountryId') is not None:
             self.country_id = m.get('CountryId')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlayTimes') is not None:
             self.play_times = m.get('PlayTimes')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
@@ -111,14 +117,15 @@
 
 class BackendCallGroupShrinkRequest(TeaModel):
     def __init__(
         self,
         called_number_shrink: str = None,
         caller_id_number: str = None,
         country_id: str = None,
+        out_id: str = None,
         owner_id: int = None,
         play_times: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         send_type: int = None,
         speed: int = None,
         task_name: str = None,
@@ -126,14 +133,15 @@
         tts_code: str = None,
         voice_code: str = None,
         volume: int = None,
     ):
         self.called_number_shrink = called_number_shrink
         self.caller_id_number = caller_id_number
         self.country_id = country_id
+        self.out_id = out_id
         self.owner_id = owner_id
         self.play_times = play_times
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.send_type = send_type
         self.speed = speed
         self.task_name = task_name
@@ -153,14 +161,16 @@
         result = dict()
         if self.called_number_shrink is not None:
             result['CalledNumber'] = self.called_number_shrink
         if self.caller_id_number is not None:
             result['CallerIdNumber'] = self.caller_id_number
         if self.country_id is not None:
             result['CountryId'] = self.country_id
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_times is not None:
             result['PlayTimes'] = self.play_times
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
@@ -185,14 +195,16 @@
         m = m or dict()
         if m.get('CalledNumber') is not None:
             self.called_number_shrink = m.get('CalledNumber')
         if m.get('CallerIdNumber') is not None:
             self.caller_id_number = m.get('CallerIdNumber')
         if m.get('CountryId') is not None:
             self.country_id = m.get('CountryId')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlayTimes') is not None:
             self.play_times = m.get('PlayTimes')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
@@ -305,26 +317,28 @@
 
 class BackendCallSignalRequest(TeaModel):
     def __init__(
         self,
         called_number: str = None,
         caller_id_number: str = None,
         country_id: str = None,
+        out_id: str = None,
         owner_id: int = None,
         play_times: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         speed: int = None,
         tts_code: str = None,
         tts_param: str = None,
         volume: int = None,
     ):
         self.called_number = called_number
         self.caller_id_number = caller_id_number
         self.country_id = country_id
+        self.out_id = out_id
         self.owner_id = owner_id
         self.play_times = play_times
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.speed = speed
         self.tts_code = tts_code
         self.tts_param = tts_param
@@ -341,14 +355,16 @@
         result = dict()
         if self.called_number is not None:
             result['CalledNumber'] = self.called_number
         if self.caller_id_number is not None:
             result['CallerIdNumber'] = self.caller_id_number
         if self.country_id is not None:
             result['CountryId'] = self.country_id
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_times is not None:
             result['PlayTimes'] = self.play_times
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
@@ -367,14 +383,16 @@
         m = m or dict()
         if m.get('CalledNumber') is not None:
             self.called_number = m.get('CalledNumber')
         if m.get('CallerIdNumber') is not None:
             self.caller_id_number = m.get('CallerIdNumber')
         if m.get('CountryId') is not None:
             self.country_id = m.get('CountryId')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlayTimes') is not None:
             self.play_times = m.get('PlayTimes')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
@@ -6103,45 +6121,39 @@
 
 
 class QueryRecordingEnableRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
         resource_owner_account: str = None,
-        resource_owner_id: int = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
-        self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
-        if self.resource_owner_id is not None:
-            result['ResourceOwnerId'] = self.resource_owner_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
-        if m.get('ResourceOwnerId') is not None:
-            self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class QueryRecordingEnableResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
```

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/PKG-INFO` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/alibabacloud_dyvmsapi_intl20211015.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dyvmsapi-intl20211015
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyvmsapi-intl20211015-1.0.0/setup.py` & `alibabacloud_dyvmsapi-intl20211015-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dyvmsapi-intl20211015.
 
-Created on 30/11/2022
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dyvmsapi_intl20211015"
 NAME = "alibabacloud_dyvmsapi-intl20211015" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

