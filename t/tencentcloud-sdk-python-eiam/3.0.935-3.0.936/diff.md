# Comparing `tmp/tencentcloud-sdk-python-eiam-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-eiam-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.935.tar", last modified: Fri Jul 14 00:30:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.936.tar", last modified: Mon Jul 17 00:24:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eiam-3.0.935.tar` & `tencentcloud-sdk-python-eiam-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/
--rw-r--r--   0 root         (0) root         (0)    38932 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/eiam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   218794 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-14 00:30:00.000000 tencentcloud-sdk-python-eiam-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/
+-rw-r--r--   0 root         (0) root         (0)    38932 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/eiam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   218794 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 00:24:28.000000 tencentcloud-sdk-python-eiam-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.936/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/setup.py` & `tencentcloud-sdk-python-eiam-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/eiam_client.py` & `tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/eiam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/errorcodes.py` & `tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/tencentcloud/eiam/v20210420/models.py` & `tencentcloud-sdk-python-eiam-3.0.936/tencentcloud/eiam/v20210420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.936/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.935/README.rst` & `tencentcloud-sdk-python-eiam-3.0.936/README.rst`

 * *Files identical despite different names*

