# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.935.tar", last modified: Fri Jul 14 00:32:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.936.tar", last modified: Mon Jul 17 00:26:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82835 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)    20510 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   359337 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-14 00:32:39.000000 tencentcloud-sdk-python-iotexplorer-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82835 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)    20510 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360219 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-17 00:26:59.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-17 00:26:58.000000 tencentcloud-sdk-python-iotexplorer-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4495,25 +4495,33 @@
         :type UpgradeMode: str
         :param _ProductId: 产品ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProductId: str
         :param _OriginalVersion: 原始固件版本号，在UpgradeMode是originalVersion升级模式下会返回
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalVersion: str
+        :param _CreateUserId: 创建账号ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateUserId: int
+        :param _CreatorNickName: 创建账号ID昵称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreatorNickName: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TaskId = None
         self._Status = None
         self._CreateTime = None
         self._Type = None
         self._ProductName = None
         self._UpgradeMode = None
         self._ProductId = None
         self._OriginalVersion = None
+        self._CreateUserId = None
+        self._CreatorNickName = None
         self._RequestId = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
@@ -4573,14 +4581,30 @@
         return self._OriginalVersion
 
     @OriginalVersion.setter
     def OriginalVersion(self, OriginalVersion):
         self._OriginalVersion = OriginalVersion
 
     @property
+    def CreateUserId(self):
+        return self._CreateUserId
+
+    @CreateUserId.setter
+    def CreateUserId(self, CreateUserId):
+        self._CreateUserId = CreateUserId
+
+    @property
+    def CreatorNickName(self):
+        return self._CreatorNickName
+
+    @CreatorNickName.setter
+    def CreatorNickName(self, CreatorNickName):
+        self._CreatorNickName = CreatorNickName
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -4590,14 +4614,16 @@
         self._Status = params.get("Status")
         self._CreateTime = params.get("CreateTime")
         self._Type = params.get("Type")
         self._ProductName = params.get("ProductName")
         self._UpgradeMode = params.get("UpgradeMode")
         self._ProductId = params.get("ProductId")
         self._OriginalVersion = params.get("OriginalVersion")
+        self._CreateUserId = params.get("CreateUserId")
+        self._CreatorNickName = params.get("CreatorNickName")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeGatewayBindDevicesRequest(AbstractModel):
     """DescribeGatewayBindDevices请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.936/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.936/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.935/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.936/README.rst`

 * *Files identical despite different names*

