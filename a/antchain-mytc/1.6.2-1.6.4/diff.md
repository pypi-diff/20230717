# Comparing `tmp/antchain_mytc-1.6.2.tar.gz` & `tmp/antchain_mytc-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_mytc-1.6.2.tar", last modified: Fri Jun 30 09:39:13 2023, max compression
+gzip compressed data, was "dist/antchain_mytc-1.6.4.tar", last modified: Mon Jul 17 09:29:58 2023, max compression
```

## Comparing `antchain_mytc-1.6.2.tar` & `antchain_mytc-1.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86735 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/client.py
--rw-r--r--   0 root         (0) root         (0)   158210 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_mytc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/antchain_sdk_mytc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_sdk_mytc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89283 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_sdk_mytc/client.py
+-rw-r--r--   0 root         (0) root         (0)   161627 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/antchain_sdk_mytc/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 09:29:58.000000 antchain_mytc-1.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-07-17 09:29:57.000000 antchain_mytc-1.6.4/setup.py
```

### Comparing `antchain_mytc-1.6.2/LICENSE` & `antchain_mytc-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.2/PKG-INFO` & `antchain_mytc-1.6.4/antchain_mytc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_mytc
-Version: 1.6.2
+Name: antchain-mytc
+Version: 1.6.4
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.6.2/README-CN.md` & `antchain_mytc-1.6.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.2/README.md` & `antchain_mytc-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.2/antchain_mytc.egg-info/PKG-INFO` & `antchain_mytc-1.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-mytc
-Version: 1.6.2
+Name: antchain_mytc
+Version: 1.6.4
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.6.2/antchain_sdk_mytc/client.py` & `antchain_mytc-1.6.4/antchain_sdk_mytc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.2',
+                    'sdk_version': '1.6.4',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.2',
+                    'sdk_version': '1.6.4',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -276,42 +276,42 @@
         raise UnretryableException(_last_request, _last_exception)
 
     def recognize_anti_qrcodeac(
         self,
         request: mytc_models.RecognizeAntiQrcodeacRequest,
     ) -> mytc_models.RecognizeAntiQrcodeacResponse:
         """
-        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。
-        Summary: 二维码防伪识别
+        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。（废弃）
+        Summary: 二维码防伪识别(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.recognize_anti_qrcodeac_ex(request, headers, runtime)
 
     async def recognize_anti_qrcodeac_async(
         self,
         request: mytc_models.RecognizeAntiQrcodeacRequest,
     ) -> mytc_models.RecognizeAntiQrcodeacResponse:
         """
-        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。
-        Summary: 二维码防伪识别
+        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。（废弃）
+        Summary: 二维码防伪识别(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.recognize_anti_qrcodeac_ex_async(request, headers, runtime)
 
     def recognize_anti_qrcodeac_ex(
         self,
         request: mytc_models.RecognizeAntiQrcodeacRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.RecognizeAntiQrcodeacResponse:
         """
-        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。
-        Summary: 二维码防伪识别
+        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。（废弃）
+        Summary: 二维码防伪识别(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.anti.qrcodeac.recognize',
                 file_name=request.file_object_name
             )
@@ -335,16 +335,16 @@
     async def recognize_anti_qrcodeac_ex_async(
         self,
         request: mytc_models.RecognizeAntiQrcodeacRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.RecognizeAntiQrcodeacResponse:
         """
-        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。
-        Summary: 二维码防伪识别
+        Description: 主要用于二维码防伪识别，内部集成安创的二维码验真能力。（废弃）
+        Summary: 二维码防伪识别(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.anti.qrcodeac.recognize',
                 file_name=request.file_object_name
             )
@@ -456,42 +456,42 @@
         )
 
     def check_code_fakescreen(
         self,
         request: mytc_models.CheckCodeFakescreenRequest,
     ) -> mytc_models.CheckCodeFakescreenResponse:
         """
-        Description: 二维码防伪防屏拍图片验证
-        Summary: 二维码防伪防屏拍图片验证
+        Description: 二维码防伪防屏拍图片验证(废弃)
+        Summary: 二维码防伪防屏拍图片验证(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.check_code_fakescreen_ex(request, headers, runtime)
 
     async def check_code_fakescreen_async(
         self,
         request: mytc_models.CheckCodeFakescreenRequest,
     ) -> mytc_models.CheckCodeFakescreenResponse:
         """
-        Description: 二维码防伪防屏拍图片验证
-        Summary: 二维码防伪防屏拍图片验证
+        Description: 二维码防伪防屏拍图片验证(废弃)
+        Summary: 二维码防伪防屏拍图片验证(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.check_code_fakescreen_ex_async(request, headers, runtime)
 
     def check_code_fakescreen_ex(
         self,
         request: mytc_models.CheckCodeFakescreenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.CheckCodeFakescreenResponse:
         """
-        Description: 二维码防伪防屏拍图片验证
-        Summary: 二维码防伪防屏拍图片验证
+        Description: 二维码防伪防屏拍图片验证(废弃)
+        Summary: 二维码防伪防屏拍图片验证(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.code.fakescreen.check',
                 file_name=request.file_object_name
             )
@@ -515,16 +515,16 @@
     async def check_code_fakescreen_ex_async(
         self,
         request: mytc_models.CheckCodeFakescreenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.CheckCodeFakescreenResponse:
         """
-        Description: 二维码防伪防屏拍图片验证
-        Summary: 二维码防伪防屏拍图片验证
+        Description: 二维码防伪防屏拍图片验证(废弃)
+        Summary: 二维码防伪防屏拍图片验证(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.code.fakescreen.check',
                 file_name=request.file_object_name
             )
@@ -546,42 +546,42 @@
         )
 
     def upload_anti_file(
         self,
         request: mytc_models.UploadAntiFileRequest,
     ) -> mytc_models.UploadAntiFileResponse:
         """
-        Description: 防伪文件上传API
-        Summary: 防伪文件上传API
+        Description: 防伪文件上传API(废弃)
+        Summary: 防伪文件上传API(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.upload_anti_file_ex(request, headers, runtime)
 
     async def upload_anti_file_async(
         self,
         request: mytc_models.UploadAntiFileRequest,
     ) -> mytc_models.UploadAntiFileResponse:
         """
-        Description: 防伪文件上传API
-        Summary: 防伪文件上传API
+        Description: 防伪文件上传API(废弃)
+        Summary: 防伪文件上传API(废弃)
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.upload_anti_file_ex_async(request, headers, runtime)
 
     def upload_anti_file_ex(
         self,
         request: mytc_models.UploadAntiFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.UploadAntiFileResponse:
         """
-        Description: 防伪文件上传API
-        Summary: 防伪文件上传API
+        Description: 防伪文件上传API(废弃)
+        Summary: 防伪文件上传API(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.anti.file.upload',
                 file_name=request.file_object_name
             )
@@ -605,16 +605,16 @@
     async def upload_anti_file_ex_async(
         self,
         request: mytc_models.UploadAntiFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mytc_models.UploadAntiFileResponse:
         """
-        Description: 防伪文件上传API
-        Summary: 防伪文件上传API
+        Description: 防伪文件上传API(废弃)
+        Summary: 防伪文件上传API(废弃)
         """
         if not UtilClient.is_unset(request.file_object):
             upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
                 auth_token=request.auth_token,
                 api_code='antchain.mytc.anti.file.upload',
                 file_name=request.file_object_name
             )
@@ -687,14 +687,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             mytc_models.JudgeCodeFakescreenResponse(),
             await self.do_request_async('1.0', 'antchain.mytc.code.fakescreen.judge', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def auth_anti_account(
+        self,
+        request: mytc_models.AuthAntiAccountRequest,
+    ) -> mytc_models.AuthAntiAccountResponse:
+        """
+        Description: 二维码防伪校验授权，获取token后通过restful api可进行防伪验证操作。
+        Summary: 二维码防伪校验授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.auth_anti_account_ex(request, headers, runtime)
+
+    async def auth_anti_account_async(
+        self,
+        request: mytc_models.AuthAntiAccountRequest,
+    ) -> mytc_models.AuthAntiAccountResponse:
+        """
+        Description: 二维码防伪校验授权，获取token后通过restful api可进行防伪验证操作。
+        Summary: 二维码防伪校验授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.auth_anti_account_ex_async(request, headers, runtime)
+
+    def auth_anti_account_ex(
+        self,
+        request: mytc_models.AuthAntiAccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mytc_models.AuthAntiAccountResponse:
+        """
+        Description: 二维码防伪校验授权，获取token后通过restful api可进行防伪验证操作。
+        Summary: 二维码防伪校验授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mytc_models.AuthAntiAccountResponse(),
+            self.do_request('1.0', 'antchain.mytc.anti.account.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def auth_anti_account_ex_async(
+        self,
+        request: mytc_models.AuthAntiAccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mytc_models.AuthAntiAccountResponse:
+        """
+        Description: 二维码防伪校验授权，获取token后通过restful api可进行防伪验证操作。
+        Summary: 二维码防伪校验授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mytc_models.AuthAntiAccountResponse(),
+            await self.do_request_async('1.0', 'antchain.mytc.anti.account.auth', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def init_anti_imagesync(
         self,
         request: mytc_models.InitAntiImagesyncRequest,
     ) -> mytc_models.InitAntiImagesyncResponse:
         """
         Description: 防伪码平台防伪底图上传，初始化上传记录
         Summary: 防伪码平台防伪底图上传初始化
```

### Comparing `antchain_mytc-1.6.2/antchain_sdk_mytc/models.py` & `antchain_mytc-1.6.4/antchain_sdk_mytc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -956,29 +956,32 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         device_type: str = None,
         file_object: BinaryIO = None,
         file_object_name: str = None,
         file_id: str = None,
+        file_data: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 设备型号
         self.device_type = device_type
-        # 图片文件id，通过小程序拍照，上传的二维码图片信息。
+        # 图片文件id，通过小程序拍照，上传的二维码图片信息。和file_data二选一
         # 待上传文件
         self.file_object = file_object
         # 待上传文件名
         self.file_object_name = file_object_name
         self.file_id = file_id
+        # 文件流数据(iso-8859-1编码)，和file_id二选一
+        self.file_data = file_data
 
     def validate(self):
-        self.validate_required(self.file_id, 'file_id')
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -990,14 +993,16 @@
             result['device_type'] = self.device_type
         if self.file_object is not None:
             result['fileObject'] = self.file_object
         if self.file_object_name is not None:
             result['fileObjectName'] = self.file_object_name
         if self.file_id is not None:
             result['file_id'] = self.file_id
+        if self.file_data is not None:
+            result['file_data'] = self.file_data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -1006,14 +1011,16 @@
             self.device_type = m.get('device_type')
         if m.get('fileObject') is not None:
             self.file_object = m.get('fileObject')
         if m.get('fileObjectName') is not None:
             self.file_object_name = m.get('fileObjectName')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
+        if m.get('file_data') is not None:
+            self.file_data = m.get('file_data')
         return self
 
 
 class CheckCodeFakeResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -1447,14 +1454,111 @@
         if m.get('detect_code') is not None:
             self.detect_code = m.get('detect_code')
         if m.get('detect_message') is not None:
             self.detect_message = m.get('detect_message')
         return self
 
 
+class AuthAntiAccountRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        device_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户标识
+        self.user_id = user_id
+        # 手机设备型号
+        self.device_type = device_type
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.device_type is not None:
+            result['device_type'] = self.device_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('device_type') is not None:
+            self.device_type = m.get('device_type')
+        return self
+
+
+class AuthAntiAccountResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户授权唯一标识，在一定时间范围内有效
+        self.token = token
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.token is not None:
+            result['token'] = self.token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('token') is not None:
+            self.token = m.get('token')
+        return self
+
+
 class InitAntiImagesyncRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         code_type: str = None,
         batch_no: str = None,
```

### Comparing `antchain_mytc-1.6.2/setup.py` & `antchain_mytc-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_mytc.
 
-Created on 30/06/2023
+Created on 17/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_mytc"
 NAME = "antchain_mytc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain MYTC SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

