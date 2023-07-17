# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.934.tar", last modified: Thu Jul 13 00:36:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.936.tar", last modified: Mon Jul 17 00:38:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.934.tar` & `tencentcloud-sdk-python-trtc-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    57241 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   287746 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:36:53.000000 tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    57241 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   287808 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:38:45.000000 tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/setup.py` & `tencentcloud-sdk-python-trtc-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6212,15 +6212,15 @@
         :param _StreamType: 录制的媒体流类型：
 0：录制音频+视频流（默认）;
 1：仅录制音频流；
 2：仅录制视频流，
         :type StreamType: int
         :param _SubscribeStreamUserIds: 指定订阅流白名单或者黑名单。
         :type SubscribeStreamUserIds: :class:`tencentcloud.trtc.v20190722.models.SubscribeStreamUserIds`
-        :param _OutputFormat: 输出文件的格式，上传到云点播时此参数无效，存储到云点播时请关注TencentVod内的MediaType参数。0：(默认)输出文件为hls格式。1：输出文件格式为hls+mp4。2：输出文件格式为hls+aac 。
+        :param _OutputFormat: 输出文件的格式，上传到云点播时此参数无效，存储到云点播时请关注TencentVod内的MediaType参数。0：(默认)输出文件为hls格式。1：输出文件格式为hls+mp4。2：输出文件格式为hls+aac 。3：输出文件格式为mp4。4：输出文件格式为aac。
         :type OutputFormat: int
         :param _AvMerge: 单流录制模式下，用户的音视频是否合并，0：单流音视频不合并（默认）。1：单流音视频合并成一个ts。混流录制此参数无需设置，默认音视频合并。
         :type AvMerge: int
         :param _MaxMediaFileDuration: 如果是aac或者mp4文件格式，超过长度限制后，系统会自动拆分视频文件。单位：分钟。默认为1440min（24h），取值范围为1-1440。【单文件限制最大为2G，满足文件大小 >2G 或录制时长度 > 24h任意一个条件，文件都会自动切分】
 Hls 格式录制此参数不生效。
         :type MaxMediaFileDuration: int
         :param _MediaId: 指定录制主辅流，0：主流+辅流（默认）；1:主流；2:辅流。
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.936/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.934'
+__version__ = '3.0.936'
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.936/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.934
+Version: 3.0.936
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/README.rst` & `tencentcloud-sdk-python-trtc-3.0.936/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.934/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.936/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.934
+Version: 3.0.936
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

