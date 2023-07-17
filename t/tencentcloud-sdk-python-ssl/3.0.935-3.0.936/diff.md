# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.935.tar", last modified: Fri Jul 14 00:37:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.936.tar", last modified: Mon Jul 17 00:34:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.935.tar` & `tencentcloud-sdk-python-ssl-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9587 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   364656 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    49507 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:37:43.000000 tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9587 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   366108 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    49507 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:34:27.000000 tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/setup.py` & `tencentcloud-sdk-python-ssl-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3393,14 +3393,17 @@
         :type CertFingerprint: str
         :param _EncryptCertFingerprint: 加密证书 SHA1指纹 （国密证书特有）
 注意：此字段可能返回 null，表示取不到有效值。
         :type EncryptCertFingerprint: str
         :param _EncryptAlgorithm: 证书算法
 注意：此字段可能返回 null，表示取不到有效值。
         :type EncryptAlgorithm: str
+        :param _DvRevokeAuthDetail: DV证书吊销验证值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DvRevokeAuthDetail: list of DvAuths
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._OwnerUin = None
         self._ProjectId = None
         self._From = None
         self._CertificateType = None
@@ -3436,14 +3439,15 @@
         self._Tags = None
         self._RootCert = None
         self._EncryptCert = None
         self._EncryptPrivateKey = None
         self._CertFingerprint = None
         self._EncryptCertFingerprint = None
         self._EncryptAlgorithm = None
+        self._DvRevokeAuthDetail = None
         self._RequestId = None
 
     @property
     def OwnerUin(self):
         return self._OwnerUin
 
     @OwnerUin.setter
@@ -3759,14 +3763,22 @@
         return self._EncryptAlgorithm
 
     @EncryptAlgorithm.setter
     def EncryptAlgorithm(self, EncryptAlgorithm):
         self._EncryptAlgorithm = EncryptAlgorithm
 
     @property
+    def DvRevokeAuthDetail(self):
+        return self._DvRevokeAuthDetail
+
+    @DvRevokeAuthDetail.setter
+    def DvRevokeAuthDetail(self, DvRevokeAuthDetail):
+        self._DvRevokeAuthDetail = DvRevokeAuthDetail
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -3821,14 +3833,20 @@
             self._RootCert = RootCertificates()
             self._RootCert._deserialize(params.get("RootCert"))
         self._EncryptCert = params.get("EncryptCert")
         self._EncryptPrivateKey = params.get("EncryptPrivateKey")
         self._CertFingerprint = params.get("CertFingerprint")
         self._EncryptCertFingerprint = params.get("EncryptCertFingerprint")
         self._EncryptAlgorithm = params.get("EncryptAlgorithm")
+        if params.get("DvRevokeAuthDetail") is not None:
+            self._DvRevokeAuthDetail = []
+            for item in params.get("DvRevokeAuthDetail"):
+                obj = DvAuths()
+                obj._deserialize(item)
+                self._DvRevokeAuthDetail.append(obj)
         self._RequestId = params.get("RequestId")
 
 
 class DescribeCertificateOperateLogsRequest(AbstractModel):
     """DescribeCertificateOperateLogs请求参数结构体
 
     """
@@ -4105,14 +4123,17 @@
         :type CAEncryptAlgorithms: list of str
         :param _CACommonNames: CA证书的所有通用名称	
 注意：此字段可能返回 null，表示取不到有效值。
         :type CACommonNames: list of str
         :param _CAEndTimes: CA证书所有的到期时间	
 注意：此字段可能返回 null，表示取不到有效值。
         :type CAEndTimes: list of str
+        :param _DvRevokeAuthDetail: DV证书吊销验证值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DvRevokeAuthDetail: list of DvAuths
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._OwnerUin = None
         self._ProjectId = None
         self._From = None
         self._CertificateType = None
@@ -4143,14 +4164,15 @@
         self._RenewAble = None
         self._SubmittedData = None
         self._Deployable = None
         self._Tags = None
         self._CAEncryptAlgorithms = None
         self._CACommonNames = None
         self._CAEndTimes = None
+        self._DvRevokeAuthDetail = None
         self._RequestId = None
 
     @property
     def OwnerUin(self):
         return self._OwnerUin
 
     @OwnerUin.setter
@@ -4426,14 +4448,22 @@
         return self._CAEndTimes
 
     @CAEndTimes.setter
     def CAEndTimes(self, CAEndTimes):
         self._CAEndTimes = CAEndTimes
 
     @property
+    def DvRevokeAuthDetail(self):
+        return self._DvRevokeAuthDetail
+
+    @DvRevokeAuthDetail.setter
+    def DvRevokeAuthDetail(self, DvRevokeAuthDetail):
+        self._DvRevokeAuthDetail = DvRevokeAuthDetail
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -4481,14 +4511,20 @@
             for item in params.get("Tags"):
                 obj = Tags()
                 obj._deserialize(item)
                 self._Tags.append(obj)
         self._CAEncryptAlgorithms = params.get("CAEncryptAlgorithms")
         self._CACommonNames = params.get("CACommonNames")
         self._CAEndTimes = params.get("CAEndTimes")
+        if params.get("DvRevokeAuthDetail") is not None:
+            self._DvRevokeAuthDetail = []
+            for item in params.get("DvRevokeAuthDetail"):
+                obj = DvAuths()
+                obj._deserialize(item)
+                self._DvRevokeAuthDetail.append(obj)
         self._RequestId = params.get("RequestId")
 
 
 class DescribeCertificatesRequest(AbstractModel):
     """DescribeCertificates请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.936/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.936/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/README.rst` & `tencentcloud-sdk-python-ssl-3.0.936/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.935/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.936/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

