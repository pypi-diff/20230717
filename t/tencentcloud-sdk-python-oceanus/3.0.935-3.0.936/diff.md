# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.935.tar", last modified: Fri Jul 14 00:35:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.936.tar", last modified: Mon Jul 17 00:32:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.935.tar` & `tencentcloud-sdk-python-oceanus-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24382 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)   206644 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-14 00:35:24.000000 tencentcloud-sdk-python-oceanus-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9664 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25309 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)   217602 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-17 00:32:06.000000 tencentcloud-sdk-python-oceanus-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 
 # AppId资源不匹配。
 INVALIDPARAMETER_APPIDRESOURCENOTMATCH = 'InvalidParameter.AppIdResourceNotMatch'
 
 # 非法的 MaxParallelism 参数。
 INVALIDPARAMETER_ILLEGALMAXPARALLELISM = 'InvalidParameter.IllegalMaxParallelism'
 
+# 非法的搜索字符串。
+INVALIDPARAMETER_ILLEGALSEARCHKEYWORD = 'InvalidParameter.IllegalSearchKeyword'
+
 # appid错误。
 INVALIDPARAMETER_INVALIDAPPID = 'InvalidParameter.InvalidAppId'
 
 # 无效集群id。
 INVALIDPARAMETER_INVALIDCLUSTERID = 'InvalidParameter.InvalidClusterId'
 
 # 名字不符合规范。
@@ -130,17 +133,23 @@
 
 # 群集Id报错。
 INVALIDPARAMETERVALUE_CLUSTERIDS = 'InvalidParameterValue.ClusterIds'
 
 # CU内存规格不匹配。
 INVALIDPARAMETERVALUE_CUMEM = 'InvalidParameterValue.CuMem'
 
+# 无效限制错误。
+INVALIDPARAMETERVALUE_INVALIDLIMIT = 'InvalidParameterValue.InvalidLimit'
+
 # 无效启动模式。
 INVALIDPARAMETERVALUE_INVALIDSTARTMODE = 'InvalidParameterValue.InvalidStartMode'
 
+# 无效时间错误。
+INVALIDPARAMETERVALUE_INVALIDTIME = 'InvalidParameterValue.InvalidTime'
+
 # 作业id的参数无效。
 INVALIDPARAMETERVALUE_JOBIDVALUEERROR = 'InvalidParameterValue.JobIdValueError'
 
 # Illegal JobName。
 INVALIDPARAMETERVALUE_JOBNAME = 'InvalidParameterValue.JobName'
 
 # 作业名称已存在。
@@ -205,14 +214,17 @@
 
 # 作业配置版本不存在。
 RESOURCENOTFOUND_JOBCONFIG = 'ResourceNotFound.JobConfig'
 
 # 找不到作业。
 RESOURCENOTFOUND_JOBID = 'ResourceNotFound.JobId'
 
+# 找不到日志。
+RESOURCENOTFOUND_LOGTOPIC = 'ResourceNotFound.LogTopic'
+
 # 程序包不存在。
 RESOURCENOTFOUND_RESOURCE = 'ResourceNotFound.Resource'
 
 # 程序包版本不存在。
 RESOURCENOTFOUND_RESOURCECONFIG = 'ResourceNotFound.ResourceConfig'
 
 # 资源不存在。
@@ -259,14 +271,17 @@
 
 # 未授权操作。
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
+# Cls Sql未启用。
+UNSUPPORTEDOPERATION_CLSSQLNOTENABLED = 'UnsupportedOperation.ClsSqlNotEnabled'
+
 # Checkpoint 时间间隔，错误。
 UNSUPPORTEDOPERATION_INVALIDCHECKPOINTINTERVALERROR = 'UnsupportedOperation.InvalidCheckpointIntervalError'
 
 # 权限拦截,没有进入权限。
 UNSUPPORTEDOPERATION_NOPERMISSIONACCESS = 'UnsupportedOperation.NoPermissionAccess'
 
 # 不支持的启动模式。
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeJobSubmissionLog(self, request):
+        """查询作业实例启动日志
+
+        :param request: Request instance for DescribeJobSubmissionLog.
+        :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobSubmissionLogRequest`
+        :rtype: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobSubmissionLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeJobSubmissionLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeJobSubmissionLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeJobs(self, request):
         """查询作业
 
         :param request: Request instance for DescribeJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobsRequest`
         :rtype: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobsResponse`
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud/oceanus/v20190422/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2996,14 +2996,242 @@
                 obj = Savepoint()
                 obj._deserialize(item)
                 self._RunningSavepoint.append(obj)
         self._RunningTotalNumber = params.get("RunningTotalNumber")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeJobSubmissionLogRequest(AbstractModel):
+    """DescribeJobSubmissionLog请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobId: 作业ID，例如：cql-6v1jkxrn
+        :type JobId: str
+        :param _StartTime: 起始时间，unix时间戳，毫秒级，例如：1611754219108
+        :type StartTime: int
+        :param _EndTime: 结束时间，unix时间戳，毫秒级，例如：1611754219108
+        :type EndTime: int
+        :param _RunningOrderId: 作业运行的实例ID, 例如：1,2,3。默认为0，表示未选中任何实例，搜索该时间段内最近的一个实例的日志
+        :type RunningOrderId: int
+        :param _Keyword: 日志搜索的关键词，默认为空
+        :type Keyword: str
+        :param _Cursor: 日志搜索的游标，可透传上次返回的值，默认为空
+        :type Cursor: str
+        :param _OrderType: 时间戳排序规则，asc - 升序，desc - 降序。默认为升序
+        :type OrderType: str
+        :param _Limit: 搜索的日志条数上限值，最大为100
+        :type Limit: int
+        """
+        self._JobId = None
+        self._StartTime = None
+        self._EndTime = None
+        self._RunningOrderId = None
+        self._Keyword = None
+        self._Cursor = None
+        self._OrderType = None
+        self._Limit = None
+
+    @property
+    def JobId(self):
+        return self._JobId
+
+    @JobId.setter
+    def JobId(self, JobId):
+        self._JobId = JobId
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def RunningOrderId(self):
+        return self._RunningOrderId
+
+    @RunningOrderId.setter
+    def RunningOrderId(self, RunningOrderId):
+        self._RunningOrderId = RunningOrderId
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def Cursor(self):
+        return self._Cursor
+
+    @Cursor.setter
+    def Cursor(self, Cursor):
+        self._Cursor = Cursor
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+
+    def _deserialize(self, params):
+        self._JobId = params.get("JobId")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._RunningOrderId = params.get("RunningOrderId")
+        self._Keyword = params.get("Keyword")
+        self._Cursor = params.get("Cursor")
+        self._OrderType = params.get("OrderType")
+        self._Limit = params.get("Limit")
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
+class DescribeJobSubmissionLogResponse(AbstractModel):
+    """DescribeJobSubmissionLog返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Cursor: 日志搜索的游标，需要搜索更多时透传这个值
+        :type Cursor: str
+        :param _ListOver: 是否返回了所有的日志记录
+        :type ListOver: bool
+        :param _JobRequestId: 作业启动的requestId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobRequestId: str
+        :param _JobInstanceList: 该时间段内符合关键字的所有的作业实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobInstanceList: list of JobInstanceForSubmissionLog
+        :param _LogList: 废弃，请使用LogContentList
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogList: list of str
+        :param _LogContentList: 日志列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogContentList: list of LogContent
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Cursor = None
+        self._ListOver = None
+        self._JobRequestId = None
+        self._JobInstanceList = None
+        self._LogList = None
+        self._LogContentList = None
+        self._RequestId = None
+
+    @property
+    def Cursor(self):
+        return self._Cursor
+
+    @Cursor.setter
+    def Cursor(self, Cursor):
+        self._Cursor = Cursor
+
+    @property
+    def ListOver(self):
+        return self._ListOver
+
+    @ListOver.setter
+    def ListOver(self, ListOver):
+        self._ListOver = ListOver
+
+    @property
+    def JobRequestId(self):
+        return self._JobRequestId
+
+    @JobRequestId.setter
+    def JobRequestId(self, JobRequestId):
+        self._JobRequestId = JobRequestId
+
+    @property
+    def JobInstanceList(self):
+        return self._JobInstanceList
+
+    @JobInstanceList.setter
+    def JobInstanceList(self, JobInstanceList):
+        self._JobInstanceList = JobInstanceList
+
+    @property
+    def LogList(self):
+        return self._LogList
+
+    @LogList.setter
+    def LogList(self, LogList):
+        self._LogList = LogList
+
+    @property
+    def LogContentList(self):
+        return self._LogContentList
+
+    @LogContentList.setter
+    def LogContentList(self, LogContentList):
+        self._LogContentList = LogContentList
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
+        self._Cursor = params.get("Cursor")
+        self._ListOver = params.get("ListOver")
+        self._JobRequestId = params.get("JobRequestId")
+        if params.get("JobInstanceList") is not None:
+            self._JobInstanceList = []
+            for item in params.get("JobInstanceList"):
+                obj = JobInstanceForSubmissionLog()
+                obj._deserialize(item)
+                self._JobInstanceList.append(obj)
+        self._LogList = params.get("LogList")
+        if params.get("LogContentList") is not None:
+            self._LogContentList = []
+            for item in params.get("LogContentList"):
+                obj = LogContent()
+                obj._deserialize(item)
+                self._LogContentList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeJobsRequest(AbstractModel):
     """DescribeJobs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4520,14 +4748,71 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class JobInstanceForSubmissionLog(AbstractModel):
+    """搜索启动日志时返回的作业实例
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RunningOrderId: 实例的Id, 按照启动的时间顺序，从1开始
+        :type RunningOrderId: int
+        :param _JobInstanceStartTime: 作业实例的启动时间
+        :type JobInstanceStartTime: str
+        :param _StartingMillis: 作业实例启动的时间（毫秒）
+        :type StartingMillis: int
+        """
+        self._RunningOrderId = None
+        self._JobInstanceStartTime = None
+        self._StartingMillis = None
+
+    @property
+    def RunningOrderId(self):
+        return self._RunningOrderId
+
+    @RunningOrderId.setter
+    def RunningOrderId(self, RunningOrderId):
+        self._RunningOrderId = RunningOrderId
+
+    @property
+    def JobInstanceStartTime(self):
+        return self._JobInstanceStartTime
+
+    @JobInstanceStartTime.setter
+    def JobInstanceStartTime(self, JobInstanceStartTime):
+        self._JobInstanceStartTime = JobInstanceStartTime
+
+    @property
+    def StartingMillis(self):
+        return self._StartingMillis
+
+    @StartingMillis.setter
+    def StartingMillis(self, StartingMillis):
+        self._StartingMillis = StartingMillis
+
+
+    def _deserialize(self, params):
+        self._RunningOrderId = params.get("RunningOrderId")
+        self._JobInstanceStartTime = params.get("JobInstanceStartTime")
+        self._StartingMillis = params.get("StartingMillis")
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
 class JobV1(AbstractModel):
     """Job详细信息
 
     """
 
     def __init__(self):
         r"""
@@ -4959,14 +5244,99 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LogContent(AbstractModel):
+    """日志查询的每行日志信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Log: 日志内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Log: str
+        :param _Time: 毫秒级时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Time: int
+        :param _PkgId: 日志组Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PkgId: str
+        :param _PkgLogId: 日志Id，在日志组范围里唯一
+        :type PkgLogId: int
+        :param _ContainerName: 日志所属的容器名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ContainerName: str
+        """
+        self._Log = None
+        self._Time = None
+        self._PkgId = None
+        self._PkgLogId = None
+        self._ContainerName = None
+
+    @property
+    def Log(self):
+        return self._Log
+
+    @Log.setter
+    def Log(self, Log):
+        self._Log = Log
+
+    @property
+    def Time(self):
+        return self._Time
+
+    @Time.setter
+    def Time(self, Time):
+        self._Time = Time
+
+    @property
+    def PkgId(self):
+        return self._PkgId
+
+    @PkgId.setter
+    def PkgId(self, PkgId):
+        self._PkgId = PkgId
+
+    @property
+    def PkgLogId(self):
+        return self._PkgLogId
+
+    @PkgLogId.setter
+    def PkgLogId(self, PkgLogId):
+        self._PkgLogId = PkgLogId
+
+    @property
+    def ContainerName(self):
+        return self._ContainerName
+
+    @ContainerName.setter
+    def ContainerName(self, ContainerName):
+        self._ContainerName = ContainerName
+
+
+    def _deserialize(self, params):
+        self._Log = params.get("Log")
+        self._Time = params.get("Time")
+        self._PkgId = params.get("PkgId")
+        self._PkgLogId = params.get("PkgLogId")
+        self._ContainerName = params.get("ContainerName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ModifyJobRequest(AbstractModel):
     """ModifyJob请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.936/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.936/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.935/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.936/README.rst`

 * *Files identical despite different names*

