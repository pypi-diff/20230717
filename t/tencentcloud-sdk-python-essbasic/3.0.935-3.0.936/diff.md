# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.935.tar", last modified: Fri Jul 14 00:30:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.936.tar", last modified: Mon Jul 17 00:24:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.935.tar` & `tencentcloud-sdk-python-essbasic-3.0.936.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53839 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   383862 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54861 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   386414 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ChannelCreateOrganizationModifyQrCode(self, request):
+        """生成渠道子客编辑企业信息二维码
+
+        :param request: Request instance for ChannelCreateOrganizationModifyQrCode.
+        :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateOrganizationModifyQrCodeRequest`
+        :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateOrganizationModifyQrCodeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ChannelCreateOrganizationModifyQrCode", params, headers=headers)
+            response = json.loads(body)
+            model = models.ChannelCreateOrganizationModifyQrCodeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ChannelCreatePrepareFlow(self, request):
         """创建预发起合同
         通过此接口指定：合同，签署人，填写控件信息，生成预创建合同链接，点击后跳转到web页面完成合同创建并发起
         可指定合同信息不可更改，签署人信息不可更改
         合同发起后，填写及签署流程与现有操作流程一致
         注意：目前仅支持模板发起
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2520,14 +2520,98 @@
             self._QrCode._deserialize(params.get("QrCode"))
         if params.get("SignUrls") is not None:
             self._SignUrls = SignUrl()
             self._SignUrls._deserialize(params.get("SignUrls"))
         self._RequestId = params.get("RequestId")
 
 
+class ChannelCreateOrganizationModifyQrCodeRequest(AbstractModel):
+    """ChannelCreateOrganizationModifyQrCode请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Agent: 应用相关信息。 此接口Agent.AppId 必填。
+        :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
+        """
+        self._Agent = None
+
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
+
+    def _deserialize(self, params):
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ChannelCreateOrganizationModifyQrCodeResponse(AbstractModel):
+    """ChannelCreateOrganizationModifyQrCode返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _QrCodeUrl: 二维码下载链接
+        :type QrCodeUrl: str
+        :param _ExpiredTime: 二维码失效时间 UNIX 时间戳 精确到秒
+        :type ExpiredTime: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._QrCodeUrl = None
+        self._ExpiredTime = None
+        self._RequestId = None
+
+    @property
+    def QrCodeUrl(self):
+        return self._QrCodeUrl
+
+    @QrCodeUrl.setter
+    def QrCodeUrl(self, QrCodeUrl):
+        self._QrCodeUrl = QrCodeUrl
+
+    @property
+    def ExpiredTime(self):
+        return self._ExpiredTime
+
+    @ExpiredTime.setter
+    def ExpiredTime(self, ExpiredTime):
+        self._ExpiredTime = ExpiredTime
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._QrCodeUrl = params.get("QrCodeUrl")
+        self._ExpiredTime = params.get("ExpiredTime")
+        self._RequestId = params.get("RequestId")
+
+
 class ChannelCreatePrepareFlowRequest(AbstractModel):
     """ChannelCreatePrepareFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7689,16 +7773,19 @@
         :type RecipientId: str
         :param _Deadline: 签署截止时间戳，默认一年
         :type Deadline: int
         :param _CallbackUrl: 签署完回调url，最大长度1000个字符
         :type CallbackUrl: str
         :param _SignComponents: 使用PDF文件直接发起合同时，签署人指定的签署控件
         :type SignComponents: list of Component
-        :param _ComponentLimitType: 个人签署方指定签署控件类型，目前支持：OCR_ESIGN -AI智慧手写签名
-HANDWRITE -手写签名
+        :param _ComponentLimitType: 	签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
+	HANDWRITE – 手写签名
+	OCR_ESIGN -- AI智能识别手写签名
+	ESIGN -- 个人印章类型
+	SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
         :type ComponentLimitType: list of str
         :param _PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
         :param _JumpUrl: 签署完前端跳转的url，此字段的用法场景请联系客户经理确认
         :type JumpUrl: str
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.essbasic.v20210526.models.ApproverOption`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.936/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.936/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

