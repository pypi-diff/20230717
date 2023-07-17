# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.935.tar", last modified: Fri Jul 14 00:45:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.936.tar", last modified: Mon Jul 17 00:39:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.935.tar` & `tencentcloud-sdk-python-tts-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23658 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:45:09.000000 tencentcloud-sdk-python-tts-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23658 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:08.000000 tencentcloud-sdk-python-tts-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-tts-3.0.935/setup.py` & `tencentcloud-sdk-python-tts-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 # CallbackUrl非法或不可访问。
 INVALIDPARAMETERVALUE_CALLBACKURL = 'InvalidParameterValue.CallbackUrl'
 
 # Codec非法，请参考Codec参数说明。
 INVALIDPARAMETERVALUE_CODEC = 'InvalidParameterValue.Codec'
 
-# ssml的say-as标签属性为cardinal、currency、address时，数字部分非有效常数，仅允许包含数字、“,”、“.”和空格。
+# ssml的say-as标签属性为cardinal、currency、address时，数字部分非有效参数，仅允许包含数字、“,”、“.”和空格。
 INVALIDPARAMETERVALUE_ERRORCARDINALFORMAT = 'InvalidParameterValue.ErrorCardinalFormat'
 
 # 请求文本含有非法字符，或请求文本没有有效字符。
 INVALIDPARAMETERVALUE_INVALIDTEXT = 'InvalidParameterValue.InvalidText'
 
 # 缺少参数。
 INVALIDPARAMETERVALUE_MISSPARAMETERS = 'InvalidParameterValue.MissParameters'
```

### Comparing `tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.935/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.936/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.935/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.936/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.935/README.rst` & `tencentcloud-sdk-python-tts-3.0.936/README.rst`

 * *Files identical despite different names*

