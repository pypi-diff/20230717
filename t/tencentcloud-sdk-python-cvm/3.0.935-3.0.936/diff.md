# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.935.tar", last modified: Fri Jul 14 00:21:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.936.tar", last modified: Mon Jul 17 00:22:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.935.tar` & `tencentcloud-sdk-python-cvm-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43899 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   119300 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   623636 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:21:21.000000 tencentcloud-sdk-python-cvm-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43899 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   119300 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)   624148 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:22:18.000000 tencentcloud-sdk-python-cvm-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/setup.py` & `tencentcloud-sdk-python-cvm-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.936/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.936/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9412,14 +9412,17 @@
         :type CamRoleName: str
         :param _HpcClusterId: 高性能计算集群`ID`。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HpcClusterId: str
         :param _RdmaIpAddresses: 高性能计算集群`IP`列表。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RdmaIpAddresses: list of str
+        :param _DedicatedClusterId: 实例所在的专用集群`ID`。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DedicatedClusterId: str
         :param _IsolatedSource: 实例隔离类型。取值范围：<br><li>ARREAR：表示欠费隔离<br></li><li>EXPIRE：表示到期隔离<br></li><li>MANMADE：表示主动退还隔离<br></li><li>NOTISOLATED：表示未隔离<br></li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsolatedSource: str
         :param _GPUInfo: GPU信息。如果是gpu类型子机，该值会返回GPU信息，如果是其他类型子机则不返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type GPUInfo: :class:`tencentcloud.cvm.v20170312.models.GPUInfo`
         :param _LicenseType: 实例的操作系统许可类型，默认为TencentCloud
@@ -9463,14 +9466,15 @@
         self._LatestOperationState = None
         self._LatestOperationRequestId = None
         self._DisasterRecoverGroupId = None
         self._IPv6Addresses = None
         self._CamRoleName = None
         self._HpcClusterId = None
         self._RdmaIpAddresses = None
+        self._DedicatedClusterId = None
         self._IsolatedSource = None
         self._GPUInfo = None
         self._LicenseType = None
         self._DisableApiTermination = None
         self._DefaultLoginUser = None
         self._DefaultLoginPort = None
         self._LatestOperationErrorMsg = None
@@ -9736,14 +9740,22 @@
         return self._RdmaIpAddresses
 
     @RdmaIpAddresses.setter
     def RdmaIpAddresses(self, RdmaIpAddresses):
         self._RdmaIpAddresses = RdmaIpAddresses
 
     @property
+    def DedicatedClusterId(self):
+        return self._DedicatedClusterId
+
+    @DedicatedClusterId.setter
+    def DedicatedClusterId(self, DedicatedClusterId):
+        self._DedicatedClusterId = DedicatedClusterId
+
+    @property
     def IsolatedSource(self):
         return self._IsolatedSource
 
     @IsolatedSource.setter
     def IsolatedSource(self, IsolatedSource):
         self._IsolatedSource = IsolatedSource
 
@@ -9846,14 +9858,15 @@
         self._LatestOperationState = params.get("LatestOperationState")
         self._LatestOperationRequestId = params.get("LatestOperationRequestId")
         self._DisasterRecoverGroupId = params.get("DisasterRecoverGroupId")
         self._IPv6Addresses = params.get("IPv6Addresses")
         self._CamRoleName = params.get("CamRoleName")
         self._HpcClusterId = params.get("HpcClusterId")
         self._RdmaIpAddresses = params.get("RdmaIpAddresses")
+        self._DedicatedClusterId = params.get("DedicatedClusterId")
         self._IsolatedSource = params.get("IsolatedSource")
         if params.get("GPUInfo") is not None:
             self._GPUInfo = GPUInfo()
             self._GPUInfo._deserialize(params.get("GPUInfo"))
         self._LicenseType = params.get("LicenseType")
         self._DisableApiTermination = params.get("DisableApiTermination")
         self._DefaultLoginUser = params.get("DefaultLoginUser")
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.935/README.rst` & `tencentcloud-sdk-python-cvm-3.0.936/README.rst`

 * *Files identical despite different names*

