# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.935.tar", last modified: Fri Jul 14 00:30:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.936.tar", last modified: Mon Jul 17 00:24:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.935.tar` & `tencentcloud-sdk-python-ess-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    61652 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   428668 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:24.000000 tencentcloud-sdk-python-ess-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:30:23.000000 tencentcloud-sdk-python-ess-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    61830 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   430546 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/setup.py` & `tencentcloud-sdk-python-ess-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.935'
+__version__ = '3.0.936'
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,21 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateChannelSubOrganizationModifyQrCode(self, request):
-        """生成子客编辑企业信息二维码
+        """根据产品要求，调整接口目录
+
+        新接口：ChannelCreateOrganizationModifyQrCode
+
+        老接口目前无线上流量，测试用例已下线处理
+
+        生成子客编辑企业信息二维码
 
         :param request: Request instance for CreateChannelSubOrganizationModifyQrCode.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateChannelSubOrganizationModifyQrCodeRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateChannelSubOrganizationModifyQrCodeResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.935/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9605,14 +9605,24 @@
         :type JumpUrl: str
         :param _SignId: 签署ID
 - 发起流程时系统自动补充
 - 创建签署链接时，可以通过查询详情接口获得签署人的SignId，然后可传入此值为该签署人创建签署链接，无需再传姓名、手机号、证件号等其他信息
         :type SignId: str
         :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要。为个人签署方时则由发起方企业审核。
         :type ApproverNeedSignReview: bool
+        :param _SignComponents: 签署人签署控件
+        :type SignComponents: list of Component
+        :param _Components: 签署人填写控件
+        :type Components: list of Component
+        :param _ComponentLimitType: 签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
+	HANDWRITE – 手写签名
+	OCR_ESIGN -- AI智能识别手写签名
+	ESIGN -- 个人印章类型
+	SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
+        :type ComponentLimitType: list of str
         """
         self._ApproverType = None
         self._OrganizationName = None
         self._ApproverName = None
         self._ApproverMobile = None
         self._ApproverIdCardType = None
         self._ApproverIdCardNumber = None
@@ -9626,14 +9636,17 @@
         self._ApproverSource = None
         self._CustomApproverTag = None
         self._RegisterInfo = None
         self._ApproverOption = None
         self._JumpUrl = None
         self._SignId = None
         self._ApproverNeedSignReview = None
+        self._SignComponents = None
+        self._Components = None
+        self._ComponentLimitType = None
 
     @property
     def ApproverType(self):
         return self._ApproverType
 
     @ApproverType.setter
     def ApproverType(self, ApproverType):
@@ -9791,14 +9804,38 @@
     def ApproverNeedSignReview(self):
         return self._ApproverNeedSignReview
 
     @ApproverNeedSignReview.setter
     def ApproverNeedSignReview(self, ApproverNeedSignReview):
         self._ApproverNeedSignReview = ApproverNeedSignReview
 
+    @property
+    def SignComponents(self):
+        return self._SignComponents
+
+    @SignComponents.setter
+    def SignComponents(self, SignComponents):
+        self._SignComponents = SignComponents
+
+    @property
+    def Components(self):
+        return self._Components
+
+    @Components.setter
+    def Components(self, Components):
+        self._Components = Components
+
+    @property
+    def ComponentLimitType(self):
+        return self._ComponentLimitType
+
+    @ComponentLimitType.setter
+    def ComponentLimitType(self, ComponentLimitType):
+        self._ComponentLimitType = ComponentLimitType
+
 
     def _deserialize(self, params):
         self._ApproverType = params.get("ApproverType")
         self._OrganizationName = params.get("OrganizationName")
         self._ApproverName = params.get("ApproverName")
         self._ApproverMobile = params.get("ApproverMobile")
         self._ApproverIdCardType = params.get("ApproverIdCardType")
@@ -9817,14 +9854,27 @@
             self._RegisterInfo._deserialize(params.get("RegisterInfo"))
         if params.get("ApproverOption") is not None:
             self._ApproverOption = ApproverOption()
             self._ApproverOption._deserialize(params.get("ApproverOption"))
         self._JumpUrl = params.get("JumpUrl")
         self._SignId = params.get("SignId")
         self._ApproverNeedSignReview = params.get("ApproverNeedSignReview")
+        if params.get("SignComponents") is not None:
+            self._SignComponents = []
+            for item in params.get("SignComponents"):
+                obj = Component()
+                obj._deserialize(item)
+                self._SignComponents.append(obj)
+        if params.get("Components") is not None:
+            self._Components = []
+            for item in params.get("Components"):
+                obj = Component()
+                obj._deserialize(item)
+                self._Components.append(obj)
+        self._ComponentLimitType = params.get("ComponentLimitType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.936/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.935/README.rst` & `tencentcloud-sdk-python-ess-3.0.936/README.rst`

 * *Files identical despite different names*

