# Comparing `tmp/tencentcloud-sdk-python-ie-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-ie-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ie-3.0.935.tar", last modified: Fri Jul 14 00:32:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ie-3.0.936.tar", last modified: Mon Jul 17 00:26:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ie-3.0.935.tar` & `tencentcloud-sdk-python-ie-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10985 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/ie_client.py
--rw-r--r--   0 root         (0) root         (0)   233379 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-14 00:32:04.000000 tencentcloud-sdk-python-ie-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10985 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/ie_client.py
+-rw-r--r--   0 root         (0) root         (0)   233379 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-17 00:26:29.000000 tencentcloud-sdk-python-ie-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-ie-3.0.935/tencentcloud_sdk_python_ie.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ie-3.0.936/tencentcloud_sdk_python_ie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ie
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ie SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ie-3.0.935/setup.py` & `tencentcloud-sdk-python-ie-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ie-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/errorcodes.py` & `tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/ie_client.py` & `tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/ie_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.935/tencentcloud/ie/v20200304/models.py` & `tencentcloud-sdk-python-ie-3.0.936/tencentcloud/ie/v20200304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-ie-3.0.936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ie
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Ie SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ie-3.0.935/README.rst` & `tencentcloud-sdk-python-ie-3.0.936/README.rst`

 * *Files identical despite different names*

