# Comparing `tmp/alibabacloud_green20220302_py2-1.0.5.tar.gz` & `tmp/alibabacloud_green20220302_py2-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.5.tar", last modified: Wed May 17 06:05:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.7.tar", last modified: Mon Jul 17 05:43:45 2023, max compression
```

## Comparing `alibabacloud_green20220302_py2-1.0.5.tar` & `alibabacloud_green20220302_py2-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9185 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    35779 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9927 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    41590 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/setup.py
```

### Comparing `alibabacloud_green20220302_py2-1.0.5/LICENSE` & `alibabacloud_green20220302_py2-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.5/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302_py2
-Version: 1.0.5
+Version: 1.0.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.5/README-CN.md` & `alibabacloud_green20220302_py2-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.5/README.md` & `alibabacloud_green20220302_py2-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,36 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_image_result_ext(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_image_result_ext_with_options(request, runtime)
 
+    def describe_upload_token_with_options(self, runtime):
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
+    def describe_upload_token(self):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_upload_token_with_options(runtime)
+
     def image_moderation_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service):
             body['Service'] = request.service
         if not UtilClient.is_unset(request.service_parameters):
             body['ServiceParameters'] = request.service_parameters
```

### Comparing `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,34 +91,39 @@
         m = m or dict()
         if m.get('FigureId') is not None:
             self.figure_id = m.get('FigureId')
         return self
 
 
 class DescribeImageResultExtResponseBodyDataTextInImage(TeaModel):
-    def __init__(self, ocr_datas=None):
+    def __init__(self, ocr_datas=None, risk_words=None):
         self.ocr_datas = ocr_datas  # type: list[str]
+        self.risk_words = risk_words  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeImageResultExtResponseBodyDataTextInImage, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.ocr_datas is not None:
             result['OcrDatas'] = self.ocr_datas
+        if self.risk_words is not None:
+            result['RiskWords'] = self.risk_words
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('OcrDatas') is not None:
             self.ocr_datas = m.get('OcrDatas')
+        if m.get('RiskWords') is not None:
+            self.risk_words = m.get('RiskWords')
         return self
 
 
 class DescribeImageResultExtResponseBodyData(TeaModel):
     def __init__(self, custom_image=None, public_figure=None, text_in_image=None):
         self.custom_image = custom_image  # type: list[DescribeImageResultExtResponseBodyDataCustomImage]
         self.public_figure = public_figure  # type: list[DescribeImageResultExtResponseBodyDataPublicFigure]
@@ -248,14 +253,154 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeImageResultExtResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeUploadTokenResponseBodyData(TeaModel):
+    def __init__(self, access_key_id=None, access_key_secret=None, bucket_name=None, expiration=None,
+                 file_name_prefix=None, oss_internal_end_point=None, oss_internet_end_point=None, security_token=None):
+        self.access_key_id = access_key_id  # type: str
+        self.access_key_secret = access_key_secret  # type: str
+        self.bucket_name = bucket_name  # type: str
+        self.expiration = expiration  # type: int
+        self.file_name_prefix = file_name_prefix  # type: str
+        self.oss_internal_end_point = oss_internal_end_point  # type: str
+        self.oss_internet_end_point = oss_internet_end_point  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeUploadTokenResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, data=None, msg=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: DescribeUploadTokenResponseBodyData
+        self.msg = msg  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(DescribeUploadTokenResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeUploadTokenResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeUploadTokenResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, service=None, service_parameters=None):
         self.service = service  # type: str
         self.service_parameters = service_parameters  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302-py2
-Version: 1.0.5
+Version: 1.0.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.5/setup.py` & `alibabacloud_green20220302_py2-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302_py2.
 
-Created on 17/05/2023
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

