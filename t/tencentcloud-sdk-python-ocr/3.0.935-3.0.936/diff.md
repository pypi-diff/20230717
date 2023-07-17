# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.935.tar", last modified: Fri Jul 14 00:35:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.936.tar", last modified: Mon Jul 17 00:32:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.935.tar` & `tencentcloud-sdk-python-ocr-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115238 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   816278 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115238 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   816287 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/setup.py` & `tencentcloud-sdk-python-ocr-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7171,15 +7171,15 @@
 11：增值税发票（卷票）
 12：购车发票
 13：过路过桥费发票
 15：非税发票
 16：全电发票
 17：医疗发票
         :type Type: int
-        :param _Polygon: 旋转后的图片四点坐标。
+        :param _Polygon: 该发票在原图片中的四点坐标。
         :type Polygon: :class:`tencentcloud.ocr.v20181119.models.Polygon`
         :param _Angle: 识别出的图片在混贴票据图片中的旋转角度。
         :type Angle: float
         :param _SingleInvoiceInfos: 识别到的内容。
         :type SingleInvoiceInfos: :class:`tencentcloud.ocr.v20181119.models.SingleInvoiceItem`
         :param _Page: 发票处于识别图片或PDF文件中的页教，默认从1开始。
         :type Page: int
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.935/README.rst` & `tencentcloud-sdk-python-ocr-3.0.936/README.rst`

 * *Files identical despite different names*

