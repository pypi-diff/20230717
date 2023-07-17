# Comparing `tmp/alibabacloud_green20220302-1.0.6.tar.gz` & `tmp/alibabacloud_green20220302-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-1.0.6.tar", last modified: Tue Jun 20 06:11:40 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-1.0.7.tar", last modified: Mon Jul 17 05:44:43 2023, max compression
```

## Comparing `alibabacloud_green20220302-1.0.6.tar` & `alibabacloud_green20220302-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      264 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19695 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    35811 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-06-20 06:11:40.000000 alibabacloud_green20220302-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21541 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    41338 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-07-17 05:44:43.000000 alibabacloud_green20220302-1.0.7/setup.py
```

### Comparing `alibabacloud_green20220302-1.0.6/LICENSE` & `alibabacloud_green20220302-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.6/PKG-INFO` & `alibabacloud_green20220302-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.6/README-CN.md` & `alibabacloud_green20220302-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.6/README.md` & `alibabacloud_green20220302-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,64 @@
     async def describe_image_result_ext_async(
         self,
         request: green_20220302_models.DescribeImageResultExtRequest,
     ) -> green_20220302_models.DescribeImageResultExtResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_image_result_ext_with_options_async(request, runtime)
 
+    def describe_upload_token_with_options(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> green_20220302_models.DescribeUploadTokenResponse:
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='DescribeUploadToken',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.DescribeUploadTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_upload_token_with_options_async(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> green_20220302_models.DescribeUploadTokenResponse:
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='DescribeUploadToken',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.DescribeUploadTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_upload_token(self) -> green_20220302_models.DescribeUploadTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_upload_token_with_options(runtime)
+
+    async def describe_upload_token_async(self) -> green_20220302_models.DescribeUploadTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_upload_token_with_options_async(runtime)
+
     def image_moderation_with_options(
         self,
         request: green_20220302_models.ImageModerationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> green_20220302_models.ImageModerationResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-1.0.7/alibabacloud_green20220302/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,174 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeImageResultExtResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeUploadTokenResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        access_key_id: str = None,
+        access_key_secret: str = None,
+        bucket_name: str = None,
+        expiration: int = None,
+        file_name_prefix: str = None,
+        oss_internal_end_point: str = None,
+        oss_internet_end_point: str = None,
+        security_token: str = None,
+    ):
+        self.access_key_id = access_key_id
+        self.access_key_secret = access_key_secret
+        self.bucket_name = bucket_name
+        self.expiration = expiration
+        self.file_name_prefix = file_name_prefix
+        self.oss_internal_end_point = oss_internal_end_point
+        self.oss_internet_end_point = oss_internet_end_point
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key_id is not None:
+            result['AccessKeyId'] = self.access_key_id
+        if self.access_key_secret is not None:
+            result['AccessKeySecret'] = self.access_key_secret
+        if self.bucket_name is not None:
+            result['BucketName'] = self.bucket_name
+        if self.expiration is not None:
+            result['Expiration'] = self.expiration
+        if self.file_name_prefix is not None:
+            result['FileNamePrefix'] = self.file_name_prefix
+        if self.oss_internal_end_point is not None:
+            result['OssInternalEndPoint'] = self.oss_internal_end_point
+        if self.oss_internet_end_point is not None:
+            result['OssInternetEndPoint'] = self.oss_internet_end_point
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessKeyId') is not None:
+            self.access_key_id = m.get('AccessKeyId')
+        if m.get('AccessKeySecret') is not None:
+            self.access_key_secret = m.get('AccessKeySecret')
+        if m.get('BucketName') is not None:
+            self.bucket_name = m.get('BucketName')
+        if m.get('Expiration') is not None:
+            self.expiration = m.get('Expiration')
+        if m.get('FileNamePrefix') is not None:
+            self.file_name_prefix = m.get('FileNamePrefix')
+        if m.get('OssInternalEndPoint') is not None:
+            self.oss_internal_end_point = m.get('OssInternalEndPoint')
+        if m.get('OssInternetEndPoint') is not None:
+            self.oss_internet_end_point = m.get('OssInternetEndPoint')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeUploadTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: DescribeUploadTokenResponseBodyData = None,
+        msg: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.msg = msg
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.msg is not None:
+            result['Msg'] = self.msg
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeUploadTokenResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Msg') is not None:
+            self.msg = m.get('Msg')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeUploadTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeUploadTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeUploadTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ImageModerationRequest(TeaModel):
     def __init__(
         self,
         service: str = None,
         service_parameters: str = None,
     ):
         self.service = service
```

### Comparing `alibabacloud_green20220302-1.0.6/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-1.0.7/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.6/setup.py` & `alibabacloud_green20220302-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 20/06/2023
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

