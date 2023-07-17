# Comparing `tmp/tencentcloud-sdk-python-fmu-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-fmu-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.935.tar", last modified: Fri Jul 14 00:30:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.936.tar", last modified: Mon Jul 17 00:25:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-fmu-3.0.935.tar` & `tencentcloud-sdk-python-fmu-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)    10552 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/fmu_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45368 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:49.000000 tencentcloud-sdk-python-fmu-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:30:48.000000 tencentcloud-sdk-python-fmu-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)    10578 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/fmu_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    45807 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:25:16.000000 tencentcloud-sdk-python-fmu-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/setup.py` & `tencentcloud-sdk-python-fmu-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def BeautifyVideo(self, request):
-        """视频美颜
+        """视频美颜(此接口目前已下线)
 
         :param request: Request instance for BeautifyVideo.
         :type request: :class:`tencentcloud.fmu.v20191213.models.BeautifyVideoRequest`
         :rtype: :class:`tencentcloud.fmu.v20191213.models.BeautifyVideoResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-fmu-3.0.936/tencentcloud/fmu/v20191213/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,19 +1011,22 @@
     def __init__(self):
         r"""
         :param _JobStatus: 当前任务状态：排队中、处理中、处理失败或者处理完成
         :type JobStatus: str
         :param _BeautifyVideoOutput: 视频美颜输出的结果信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type BeautifyVideoOutput: :class:`tencentcloud.fmu.v20191213.models.BeautifyVideoOutput`
+        :param _JobStatusCode: 当前任务状态码：1：排队中、3: 处理中、5: 处理失败、7:处理完成
+        :type JobStatusCode: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._JobStatus = None
         self._BeautifyVideoOutput = None
+        self._JobStatusCode = None
         self._RequestId = None
 
     @property
     def JobStatus(self):
         return self._JobStatus
 
     @JobStatus.setter
@@ -1035,27 +1038,36 @@
         return self._BeautifyVideoOutput
 
     @BeautifyVideoOutput.setter
     def BeautifyVideoOutput(self, BeautifyVideoOutput):
         self._BeautifyVideoOutput = BeautifyVideoOutput
 
     @property
+    def JobStatusCode(self):
+        return self._JobStatusCode
+
+    @JobStatusCode.setter
+    def JobStatusCode(self, JobStatusCode):
+        self._JobStatusCode = JobStatusCode
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._JobStatus = params.get("JobStatus")
         if params.get("BeautifyVideoOutput") is not None:
             self._BeautifyVideoOutput = BeautifyVideoOutput()
             self._BeautifyVideoOutput._deserialize(params.get("BeautifyVideoOutput"))
+        self._JobStatusCode = params.get("JobStatusCode")
         self._RequestId = params.get("RequestId")
 
 
 class RGBAInfo(AbstractModel):
     """RGBA通道信息
 
     """
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.936/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.935/README.rst` & `tencentcloud-sdk-python-fmu-3.0.936/README.rst`

 * *Files identical despite different names*

