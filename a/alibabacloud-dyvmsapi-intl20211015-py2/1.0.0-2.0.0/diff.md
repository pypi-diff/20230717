# Comparing `tmp/alibabacloud_dyvmsapi-intl20211015_py2-1.0.0.tar.gz` & `tmp/alibabacloud_dyvmsapi-intl20211015_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dyvmsapi-intl20211015_py2-1.0.0.tar", last modified: Wed Nov 30 10:09:21 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dyvmsapi-intl20211015_py2-2.0.0.tar", last modified: Mon Jul 17 07:37:19 2023, max compression
```

## Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0.tar` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2532 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1063 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1146 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71979 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/client.py
--rw-r--r--   0 root         (0) root         (0)   283295 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2532 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2955 2022-11-30 10:09:21.000000 alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72043 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/client.py
+-rw-r--r--   0 root         (0) root         (0)   283641 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-07-17 07:37:19.000000 alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/LICENSE` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/PKG-INFO` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dyvmsapi-intl20211015_py2
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/README-CN.md` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/README.md` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/client.py` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,16 @@
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
@@ -93,14 +95,16 @@
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
@@ -1167,16 +1171,14 @@
     def query_recording_enable_with_options(self, request, runtime):
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

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015/models.py` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class BackendCallGroupRequest(TeaModel):
-    def __init__(self, called_number=None, caller_id_number=None, country_id=None, owner_id=None, play_times=None,
-                 resource_owner_account=None, resource_owner_id=None, send_type=None, speed=None, task_name=None, timing_start=None,
-                 tts_code=None, voice_code=None, volume=None):
+    def __init__(self, called_number=None, caller_id_number=None, country_id=None, out_id=None, owner_id=None,
+                 play_times=None, resource_owner_account=None, resource_owner_id=None, send_type=None, speed=None,
+                 task_name=None, timing_start=None, tts_code=None, voice_code=None, volume=None):
         self.called_number = called_number  # type: list[str]
         self.caller_id_number = caller_id_number  # type: str
         self.country_id = country_id  # type: str
+        self.out_id = out_id  # type: str
         self.owner_id = owner_id  # type: long
         self.play_times = play_times  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.send_type = send_type  # type: long
         self.speed = speed  # type: long
         self.task_name = task_name  # type: str
@@ -33,14 +34,16 @@
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
@@ -65,14 +68,16 @@
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
@@ -91,20 +96,21 @@
             self.voice_code = m.get('VoiceCode')
         if m.get('Volume') is not None:
             self.volume = m.get('Volume')
         return self
 
 
 class BackendCallGroupShrinkRequest(TeaModel):
-    def __init__(self, called_number_shrink=None, caller_id_number=None, country_id=None, owner_id=None,
-                 play_times=None, resource_owner_account=None, resource_owner_id=None, send_type=None, speed=None,
-                 task_name=None, timing_start=None, tts_code=None, voice_code=None, volume=None):
+    def __init__(self, called_number_shrink=None, caller_id_number=None, country_id=None, out_id=None,
+                 owner_id=None, play_times=None, resource_owner_account=None, resource_owner_id=None, send_type=None,
+                 speed=None, task_name=None, timing_start=None, tts_code=None, voice_code=None, volume=None):
         self.called_number_shrink = called_number_shrink  # type: str
         self.caller_id_number = caller_id_number  # type: str
         self.country_id = country_id  # type: str
+        self.out_id = out_id  # type: str
         self.owner_id = owner_id  # type: long
         self.play_times = play_times  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.send_type = send_type  # type: long
         self.speed = speed  # type: long
         self.task_name = task_name  # type: str
@@ -124,14 +130,16 @@
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
@@ -156,14 +164,16 @@
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
@@ -260,19 +270,21 @@
         if m.get('body') is not None:
             temp_model = BackendCallGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BackendCallSignalRequest(TeaModel):
-    def __init__(self, called_number=None, caller_id_number=None, country_id=None, owner_id=None, play_times=None,
-                 resource_owner_account=None, resource_owner_id=None, speed=None, tts_code=None, tts_param=None, volume=None):
+    def __init__(self, called_number=None, caller_id_number=None, country_id=None, out_id=None, owner_id=None,
+                 play_times=None, resource_owner_account=None, resource_owner_id=None, speed=None, tts_code=None,
+                 tts_param=None, volume=None):
         self.called_number = called_number  # type: str
         self.caller_id_number = caller_id_number  # type: str
         self.country_id = country_id  # type: str
+        self.out_id = out_id  # type: str
         self.owner_id = owner_id  # type: long
         self.play_times = play_times  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.speed = speed  # type: long
         self.tts_code = tts_code  # type: str
         self.tts_param = tts_param  # type: str
@@ -289,14 +301,16 @@
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
@@ -315,14 +329,16 @@
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
@@ -5329,44 +5345,39 @@
         if m.get('body') is not None:
             temp_model = QueryHomeStatResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordingEnableRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None):
+    def __init__(self, owner_id=None, resource_owner_account=None):
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
-        self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(QueryRecordingEnableRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
-        if m.get('ResourceOwnerId') is not None:
-            self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class QueryRecordingEnableResponseBody(TeaModel):
     def __init__(self, code=None, enable=None, message=None, request_id=None):
         self.code = code  # type: str
         self.enable = enable  # type: bool
```

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/PKG-INFO` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/alibabacloud_dyvmsapi_intl20211015_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dyvmsapi-intl20211015-py2
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dyvmsapi-intl20211015_py2-1.0.0/setup.py` & `alibabacloud_dyvmsapi-intl20211015_py2-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dyvmsapi-intl20211015_py2.
 
-Created on 30/11/2022
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dyvmsapi_intl20211015"
 NAME = "alibabacloud_dyvmsapi-intl20211015_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dyvmsapi-intl (20211015) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

