# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.935.tar", last modified: Fri Jul 14 00:40:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.936.tar", last modified: Mon Jul 17 00:37:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.935.tar` & `tencentcloud-sdk-python-tione-3.0.936.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12673 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   527631 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144266 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-14 00:40:51.000000 tencentcloud-sdk-python-tione-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12673 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   531149 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144266 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-17 00:37:43.000000 tencentcloud-sdk-python-tione-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-tione-3.0.935/setup.py` & `tencentcloud-sdk-python-tione-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20211111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2267,14 +2267,18 @@
         :type ScheduledAction: :class:`tencentcloud.tione.v20211111.models.ScheduledAction`
         :param _VolumeMount: 挂载配置，目前只支持CFS
         :type VolumeMount: :class:`tencentcloud.tione.v20211111.models.VolumeMount`
         :param _ServiceLimit: 服务限速限流相关配置
         :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
         :param _CallbackUrl: 回调地址，用于回调创建服务状态信息，回调格式&内容详情见：[TI-ONE 接口回调说明](https://cloud.tencent.com/document/product/851/84292)
         :type CallbackUrl: str
+        :param _ModelTurboEnable: 是否开启模型的加速, 仅对StableDiffusion(动态加速)格式的模型有效。
+        :type ModelTurboEnable: bool
+        :param _ServiceCategory: 服务分类
+        :type ServiceCategory: str
         """
         self._ServiceGroupId = None
         self._ServiceGroupName = None
         self._ServiceDescription = None
         self._ChargeType = None
         self._ResourceGroupId = None
         self._ModelInfo = None
@@ -2295,14 +2299,16 @@
         self._HybridBillingPrepaidReplicas = None
         self._CreateSource = None
         self._ModelHotUpdateEnable = None
         self._ScheduledAction = None
         self._VolumeMount = None
         self._ServiceLimit = None
         self._CallbackUrl = None
+        self._ModelTurboEnable = None
+        self._ServiceCategory = None
 
     @property
     def ServiceGroupId(self):
         return self._ServiceGroupId
 
     @ServiceGroupId.setter
     def ServiceGroupId(self, ServiceGroupId):
@@ -2512,14 +2518,30 @@
     def CallbackUrl(self):
         return self._CallbackUrl
 
     @CallbackUrl.setter
     def CallbackUrl(self, CallbackUrl):
         self._CallbackUrl = CallbackUrl
 
+    @property
+    def ModelTurboEnable(self):
+        return self._ModelTurboEnable
+
+    @ModelTurboEnable.setter
+    def ModelTurboEnable(self, ModelTurboEnable):
+        self._ModelTurboEnable = ModelTurboEnable
+
+    @property
+    def ServiceCategory(self):
+        return self._ServiceCategory
+
+    @ServiceCategory.setter
+    def ServiceCategory(self, ServiceCategory):
+        self._ServiceCategory = ServiceCategory
+
 
     def _deserialize(self, params):
         self._ServiceGroupId = params.get("ServiceGroupId")
         self._ServiceGroupName = params.get("ServiceGroupName")
         self._ServiceDescription = params.get("ServiceDescription")
         self._ChargeType = params.get("ChargeType")
         self._ResourceGroupId = params.get("ResourceGroupId")
@@ -2572,14 +2594,16 @@
         if params.get("VolumeMount") is not None:
             self._VolumeMount = VolumeMount()
             self._VolumeMount._deserialize(params.get("VolumeMount"))
         if params.get("ServiceLimit") is not None:
             self._ServiceLimit = ServiceLimit()
             self._ServiceLimit._deserialize(params.get("ServiceLimit"))
         self._CallbackUrl = params.get("CallbackUrl")
+        self._ModelTurboEnable = params.get("ModelTurboEnable")
+        self._ServiceCategory = params.get("ServiceCategory")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7756,29 +7780,41 @@
 class DescribeModelServiceHotUpdatedResponse(AbstractModel):
     """DescribeModelServiceHotUpdated返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param _ModelTurboFlag: 模型加速标志位.Allowed 允许模型加速. Forbidden 禁止模型加速
+        :type ModelTurboFlag: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self._ModelTurboFlag = None
         self._RequestId = None
 
     @property
+    def ModelTurboFlag(self):
+        return self._ModelTurboFlag
+
+    @ModelTurboFlag.setter
+    def ModelTurboFlag(self, ModelTurboFlag):
+        self._ModelTurboFlag = ModelTurboFlag
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
+        self._ModelTurboFlag = params.get("ModelTurboFlag")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeModelServiceRequest(AbstractModel):
     """DescribeModelService请求参数结构体
 
     """
@@ -9741,23 +9777,27 @@
         :type MinBlockSizePt: str
         :param _MinBlockSizeTf: FROZEN_GRAPH、SAVED_MODEL格式在进行优化时切分子图的最小算子数目，一般无需进行改动，默认为10
 注意：此字段可能返回 null，表示取不到有效值。
         :type MinBlockSizeTf: str
         :param _PipelineArgs: Stable Diffusion 模型优化参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type PipelineArgs: str
+        :param _LoraScale: Stable Diffusion 模型优化参数，控制Lora模型的影响效果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LoraScale: str
         """
         self._MaxNNZ = None
         self._SlotNum = None
         self._CpuCachePercentage = None
         self._GpuCachePercentage = None
         self._EnableDistributed = None
         self._MinBlockSizePt = None
         self._MinBlockSizeTf = None
         self._PipelineArgs = None
+        self._LoraScale = None
 
     @property
     def MaxNNZ(self):
         return self._MaxNNZ
 
     @MaxNNZ.setter
     def MaxNNZ(self, MaxNNZ):
@@ -9815,24 +9855,33 @@
     def PipelineArgs(self):
         return self._PipelineArgs
 
     @PipelineArgs.setter
     def PipelineArgs(self, PipelineArgs):
         self._PipelineArgs = PipelineArgs
 
+    @property
+    def LoraScale(self):
+        return self._LoraScale
+
+    @LoraScale.setter
+    def LoraScale(self, LoraScale):
+        self._LoraScale = LoraScale
+
 
     def _deserialize(self, params):
         self._MaxNNZ = params.get("MaxNNZ")
         self._SlotNum = params.get("SlotNum")
         self._CpuCachePercentage = params.get("CpuCachePercentage")
         self._GpuCachePercentage = params.get("GpuCachePercentage")
         self._EnableDistributed = params.get("EnableDistributed")
         self._MinBlockSizePt = params.get("MinBlockSizePt")
         self._MinBlockSizeTf = params.get("MinBlockSizeTf")
         self._PipelineArgs = params.get("PipelineArgs")
+        self._LoraScale = params.get("LoraScale")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -11009,23 +11058,27 @@
         :type CosPathInfo: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         :param _AlgorithmFramework: 模型对应的算法框架，预留
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlgorithmFramework: str
         :param _ModelType: 默认为 NORMAL, 已加速模型: ACCELERATE, 自动学习模型 AUTO_ML
 注意：此字段可能返回 null，表示取不到有效值。
         :type ModelType: str
+        :param _ModelFormat: 模型格式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModelFormat: str
         """
         self._ModelVersionId = None
         self._ModelId = None
         self._ModelName = None
         self._ModelVersion = None
         self._ModelSource = None
         self._CosPathInfo = None
         self._AlgorithmFramework = None
         self._ModelType = None
+        self._ModelFormat = None
 
     @property
     def ModelVersionId(self):
         return self._ModelVersionId
 
     @ModelVersionId.setter
     def ModelVersionId(self, ModelVersionId):
@@ -11083,26 +11136,35 @@
     def ModelType(self):
         return self._ModelType
 
     @ModelType.setter
     def ModelType(self, ModelType):
         self._ModelType = ModelType
 
+    @property
+    def ModelFormat(self):
+        return self._ModelFormat
+
+    @ModelFormat.setter
+    def ModelFormat(self, ModelFormat):
+        self._ModelFormat = ModelFormat
+
 
     def _deserialize(self, params):
         self._ModelVersionId = params.get("ModelVersionId")
         self._ModelId = params.get("ModelId")
         self._ModelName = params.get("ModelName")
         self._ModelVersion = params.get("ModelVersion")
         self._ModelSource = params.get("ModelSource")
         if params.get("CosPathInfo") is not None:
             self._CosPathInfo = CosPathInfo()
             self._CosPathInfo._deserialize(params.get("CosPathInfo"))
         self._AlgorithmFramework = params.get("AlgorithmFramework")
         self._ModelType = params.get("ModelType")
+        self._ModelFormat = params.get("ModelFormat")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -11324,14 +11386,16 @@
         :type ModelHotUpdateEnable: bool
         :param _ScheduledAction: 定时停止配置
         :type ScheduledAction: :class:`tencentcloud.tione.v20211111.models.ScheduledAction`
         :param _ServiceLimit: 服务限速限流相关配置
         :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
         :param _VolumeMount: 挂载配置，目前只支持CFS
         :type VolumeMount: :class:`tencentcloud.tione.v20211111.models.VolumeMount`
+        :param _ModelTurboEnable: 是否开启模型的加速, 仅对StableDiffusion(动态加速)格式的模型有效。默认不开启
+        :type ModelTurboEnable: bool
         """
         self._ServiceId = None
         self._ModelInfo = None
         self._ImageInfo = None
         self._Env = None
         self._Resources = None
         self._InstanceType = None
@@ -11345,14 +11409,15 @@
         self._ScaleStrategy = None
         self._CronScaleJobs = None
         self._HybridBillingPrepaidReplicas = None
         self._ModelHotUpdateEnable = None
         self._ScheduledAction = None
         self._ServiceLimit = None
         self._VolumeMount = None
+        self._ModelTurboEnable = None
 
     @property
     def ServiceId(self):
         return self._ServiceId
 
     @ServiceId.setter
     def ServiceId(self, ServiceId):
@@ -11506,14 +11571,22 @@
     def VolumeMount(self):
         return self._VolumeMount
 
     @VolumeMount.setter
     def VolumeMount(self, VolumeMount):
         self._VolumeMount = VolumeMount
 
+    @property
+    def ModelTurboEnable(self):
+        return self._ModelTurboEnable
+
+    @ModelTurboEnable.setter
+    def ModelTurboEnable(self, ModelTurboEnable):
+        self._ModelTurboEnable = ModelTurboEnable
+
 
     def _deserialize(self, params):
         self._ServiceId = params.get("ServiceId")
         if params.get("ModelInfo") is not None:
             self._ModelInfo = ModelInfo()
             self._ModelInfo._deserialize(params.get("ModelInfo"))
         if params.get("ImageInfo") is not None:
@@ -11554,14 +11627,15 @@
             self._ScheduledAction._deserialize(params.get("ScheduledAction"))
         if params.get("ServiceLimit") is not None:
             self._ServiceLimit = ServiceLimit()
             self._ServiceLimit._deserialize(params.get("ServiceLimit"))
         if params.get("VolumeMount") is not None:
             self._VolumeMount = VolumeMount()
             self._VolumeMount._deserialize(params.get("VolumeMount"))
+        self._ModelTurboEnable = params.get("ModelTurboEnable")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -13163,14 +13237,17 @@
         :param _ServiceId: 服务id
         :type ServiceId: str
         :param _ServiceGroupName: 服务组名
         :type ServiceGroupName: str
         :param _ServiceDescription: 服务描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceDescription: str
+        :param _ServiceInfo: 服务的详细信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServiceInfo: :class:`tencentcloud.tione.v20211111.models.ServiceInfo`
         :param _ClusterId: 集群id
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClusterId: str
         :param _Region: 地域
 注意：此字段可能返回 null，表示取不到有效值。
         :type Region: str
         :param _Namespace: 命名空间
@@ -13178,14 +13255,23 @@
         :type Namespace: str
         :param _ChargeType: 付费类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChargeType: str
         :param _ResourceGroupId: 包年包月服务的资源组id，按量计费的服务为空
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupId: str
+        :param _ResourceGroupName: 包年包月服务对应的资源组名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceGroupName: str
+        :param _Tags: 服务的标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of Tag
+        :param _IngressName: 服务所在的 ingress 的 name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IngressName: str
         :param _CreatedBy: 创建者
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedBy: str
         :param _CreateTime: 创建时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
         :param _UpdateTime: 更新时间
@@ -13196,96 +13282,84 @@
         :type Uin: str
         :param _SubUin: 子账号
 注意：此字段可能返回 null，表示取不到有效值。
         :type SubUin: str
         :param _AppId: app_id
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppId: int
-        :param _Version: 版本号
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Version: str
-        :param _LatestVersion: 服务组下服务的最高版本号
-注意：此字段可能返回 null，表示取不到有效值。
-        :type LatestVersion: str
-        :param _ServiceInfo: 服务的详细信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ServiceInfo: :class:`tencentcloud.tione.v20211111.models.ServiceInfo`
         :param _BusinessStatus: 服务的业务状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type BusinessStatus: str
-        :param _CreateSource: 服务的创建来源
-AUTO_ML: 来自自动学习的一键发布
-DEFAULT: 其他来源
+        :param _ServiceLimit: 已废弃
 注意：此字段可能返回 null，表示取不到有效值。
-        :type CreateSource: str
-        :param _BillingInfo: 费用信息
+        :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
+        :param _ScheduledAction: 已废弃
 注意：此字段可能返回 null，表示取不到有效值。
-        :type BillingInfo: str
+        :type ScheduledAction: :class:`tencentcloud.tione.v20211111.models.ScheduledAction`
+        :param _CreateFailedReason: 服务创建失败的原因，创建成功后该字段为默认值 CREATE_SUCCEED
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateFailedReason: str
         :param _Status: 服务状态
 CREATING 创建中
 CREATE_FAILED 创建失败
 Normal	正常运行中
 Stopped  已停止
 Stopping 停止中
 Abnormal 异常
 Pending 启动中
 Waiting 就绪中
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: str
+        :param _BillingInfo: 费用信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BillingInfo: str
         :param _Weight: 模型权重
 注意：此字段可能返回 null，表示取不到有效值。
         :type Weight: int
-        :param _IngressName: 服务所在的 ingress 的 name
-注意：此字段可能返回 null，表示取不到有效值。
-        :type IngressName: str
-        :param _ServiceLimit: 服务限速限流相关配置
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
-        :param _ScheduledAction: 定时停止的配置
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ScheduledAction: :class:`tencentcloud.tione.v20211111.models.ScheduledAction`
-        :param _CreateFailedReason: 服务创建失败的原因，创建成功后该字段为默认值 CREATE_SUCCEED
+        :param _CreateSource: 服务的创建来源
+AUTO_ML: 来自自动学习的一键发布
+DEFAULT: 其他来源
 注意：此字段可能返回 null，表示取不到有效值。
-        :type CreateFailedReason: str
-        :param _ResourceGroupName: 包年包月服务对应的资源组名字
+        :type CreateSource: str
+        :param _Version: 版本号
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ResourceGroupName: str
-        :param _Tags: 服务的标签
+        :type Version: str
+        :param _LatestVersion: 服务组下服务的最高版本号
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Tags: list of Tag
+        :type LatestVersion: str
         """
         self._ServiceGroupId = None
         self._ServiceId = None
         self._ServiceGroupName = None
         self._ServiceDescription = None
+        self._ServiceInfo = None
         self._ClusterId = None
         self._Region = None
         self._Namespace = None
         self._ChargeType = None
         self._ResourceGroupId = None
+        self._ResourceGroupName = None
+        self._Tags = None
+        self._IngressName = None
         self._CreatedBy = None
         self._CreateTime = None
         self._UpdateTime = None
         self._Uin = None
         self._SubUin = None
         self._AppId = None
-        self._Version = None
-        self._LatestVersion = None
-        self._ServiceInfo = None
         self._BusinessStatus = None
-        self._CreateSource = None
-        self._BillingInfo = None
-        self._Status = None
-        self._Weight = None
-        self._IngressName = None
         self._ServiceLimit = None
         self._ScheduledAction = None
         self._CreateFailedReason = None
-        self._ResourceGroupName = None
-        self._Tags = None
+        self._Status = None
+        self._BillingInfo = None
+        self._Weight = None
+        self._CreateSource = None
+        self._Version = None
+        self._LatestVersion = None
 
     @property
     def ServiceGroupId(self):
         return self._ServiceGroupId
 
     @ServiceGroupId.setter
     def ServiceGroupId(self, ServiceGroupId):
@@ -13312,14 +13386,22 @@
         return self._ServiceDescription
 
     @ServiceDescription.setter
     def ServiceDescription(self, ServiceDescription):
         self._ServiceDescription = ServiceDescription
 
     @property
+    def ServiceInfo(self):
+        return self._ServiceInfo
+
+    @ServiceInfo.setter
+    def ServiceInfo(self, ServiceInfo):
+        self._ServiceInfo = ServiceInfo
+
+    @property
     def ClusterId(self):
         return self._ClusterId
 
     @ClusterId.setter
     def ClusterId(self, ClusterId):
         self._ClusterId = ClusterId
 
@@ -13352,14 +13434,38 @@
         return self._ResourceGroupId
 
     @ResourceGroupId.setter
     def ResourceGroupId(self, ResourceGroupId):
         self._ResourceGroupId = ResourceGroupId
 
     @property
+    def ResourceGroupName(self):
+        return self._ResourceGroupName
+
+    @ResourceGroupName.setter
+    def ResourceGroupName(self, ResourceGroupName):
+        self._ResourceGroupName = ResourceGroupName
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def IngressName(self):
+        return self._IngressName
+
+    @IngressName.setter
+    def IngressName(self, IngressName):
+        self._IngressName = IngressName
+
+    @property
     def CreatedBy(self):
         return self._CreatedBy
 
     @CreatedBy.setter
     def CreatedBy(self, CreatedBy):
         self._CreatedBy = CreatedBy
 
@@ -13400,167 +13506,135 @@
         return self._AppId
 
     @AppId.setter
     def AppId(self, AppId):
         self._AppId = AppId
 
     @property
-    def Version(self):
-        return self._Version
+    def BusinessStatus(self):
+        return self._BusinessStatus
 
-    @Version.setter
-    def Version(self, Version):
-        self._Version = Version
+    @BusinessStatus.setter
+    def BusinessStatus(self, BusinessStatus):
+        self._BusinessStatus = BusinessStatus
 
     @property
-    def LatestVersion(self):
-        return self._LatestVersion
+    def ServiceLimit(self):
+        return self._ServiceLimit
 
-    @LatestVersion.setter
-    def LatestVersion(self, LatestVersion):
-        self._LatestVersion = LatestVersion
+    @ServiceLimit.setter
+    def ServiceLimit(self, ServiceLimit):
+        self._ServiceLimit = ServiceLimit
 
     @property
-    def ServiceInfo(self):
-        return self._ServiceInfo
+    def ScheduledAction(self):
+        return self._ScheduledAction
 
-    @ServiceInfo.setter
-    def ServiceInfo(self, ServiceInfo):
-        self._ServiceInfo = ServiceInfo
+    @ScheduledAction.setter
+    def ScheduledAction(self, ScheduledAction):
+        self._ScheduledAction = ScheduledAction
 
     @property
-    def BusinessStatus(self):
-        return self._BusinessStatus
+    def CreateFailedReason(self):
+        return self._CreateFailedReason
 
-    @BusinessStatus.setter
-    def BusinessStatus(self, BusinessStatus):
-        self._BusinessStatus = BusinessStatus
+    @CreateFailedReason.setter
+    def CreateFailedReason(self, CreateFailedReason):
+        self._CreateFailedReason = CreateFailedReason
 
     @property
-    def CreateSource(self):
-        return self._CreateSource
+    def Status(self):
+        return self._Status
 
-    @CreateSource.setter
-    def CreateSource(self, CreateSource):
-        self._CreateSource = CreateSource
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
 
     @property
     def BillingInfo(self):
         return self._BillingInfo
 
     @BillingInfo.setter
     def BillingInfo(self, BillingInfo):
         self._BillingInfo = BillingInfo
 
     @property
-    def Status(self):
-        return self._Status
-
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
-
-    @property
     def Weight(self):
         return self._Weight
 
     @Weight.setter
     def Weight(self, Weight):
         self._Weight = Weight
 
     @property
-    def IngressName(self):
-        return self._IngressName
-
-    @IngressName.setter
-    def IngressName(self, IngressName):
-        self._IngressName = IngressName
-
-    @property
-    def ServiceLimit(self):
-        return self._ServiceLimit
-
-    @ServiceLimit.setter
-    def ServiceLimit(self, ServiceLimit):
-        self._ServiceLimit = ServiceLimit
-
-    @property
-    def ScheduledAction(self):
-        return self._ScheduledAction
-
-    @ScheduledAction.setter
-    def ScheduledAction(self, ScheduledAction):
-        self._ScheduledAction = ScheduledAction
-
-    @property
-    def CreateFailedReason(self):
-        return self._CreateFailedReason
+    def CreateSource(self):
+        return self._CreateSource
 
-    @CreateFailedReason.setter
-    def CreateFailedReason(self, CreateFailedReason):
-        self._CreateFailedReason = CreateFailedReason
+    @CreateSource.setter
+    def CreateSource(self, CreateSource):
+        self._CreateSource = CreateSource
 
     @property
-    def ResourceGroupName(self):
-        return self._ResourceGroupName
+    def Version(self):
+        return self._Version
 
-    @ResourceGroupName.setter
-    def ResourceGroupName(self, ResourceGroupName):
-        self._ResourceGroupName = ResourceGroupName
+    @Version.setter
+    def Version(self, Version):
+        self._Version = Version
 
     @property
-    def Tags(self):
-        return self._Tags
+    def LatestVersion(self):
+        return self._LatestVersion
 
-    @Tags.setter
-    def Tags(self, Tags):
-        self._Tags = Tags
+    @LatestVersion.setter
+    def LatestVersion(self, LatestVersion):
+        self._LatestVersion = LatestVersion
 
 
     def _deserialize(self, params):
         self._ServiceGroupId = params.get("ServiceGroupId")
         self._ServiceId = params.get("ServiceId")
         self._ServiceGroupName = params.get("ServiceGroupName")
         self._ServiceDescription = params.get("ServiceDescription")
+        if params.get("ServiceInfo") is not None:
+            self._ServiceInfo = ServiceInfo()
+            self._ServiceInfo._deserialize(params.get("ServiceInfo"))
         self._ClusterId = params.get("ClusterId")
         self._Region = params.get("Region")
         self._Namespace = params.get("Namespace")
         self._ChargeType = params.get("ChargeType")
         self._ResourceGroupId = params.get("ResourceGroupId")
+        self._ResourceGroupName = params.get("ResourceGroupName")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        self._IngressName = params.get("IngressName")
         self._CreatedBy = params.get("CreatedBy")
         self._CreateTime = params.get("CreateTime")
         self._UpdateTime = params.get("UpdateTime")
         self._Uin = params.get("Uin")
         self._SubUin = params.get("SubUin")
         self._AppId = params.get("AppId")
-        self._Version = params.get("Version")
-        self._LatestVersion = params.get("LatestVersion")
-        if params.get("ServiceInfo") is not None:
-            self._ServiceInfo = ServiceInfo()
-            self._ServiceInfo._deserialize(params.get("ServiceInfo"))
         self._BusinessStatus = params.get("BusinessStatus")
-        self._CreateSource = params.get("CreateSource")
-        self._BillingInfo = params.get("BillingInfo")
-        self._Status = params.get("Status")
-        self._Weight = params.get("Weight")
-        self._IngressName = params.get("IngressName")
         if params.get("ServiceLimit") is not None:
             self._ServiceLimit = ServiceLimit()
             self._ServiceLimit._deserialize(params.get("ServiceLimit"))
         if params.get("ScheduledAction") is not None:
             self._ScheduledAction = ScheduledAction()
             self._ScheduledAction._deserialize(params.get("ScheduledAction"))
         self._CreateFailedReason = params.get("CreateFailedReason")
-        self._ResourceGroupName = params.get("ResourceGroupName")
-        if params.get("Tags") is not None:
-            self._Tags = []
-            for item in params.get("Tags"):
-                obj = Tag()
-                obj._deserialize(item)
-                self._Tags.append(obj)
+        self._Status = params.get("Status")
+        self._BillingInfo = params.get("BillingInfo")
+        self._Weight = params.get("Weight")
+        self._CreateSource = params.get("CreateSource")
+        self._Version = params.get("Version")
+        self._LatestVersion = params.get("LatestVersion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -14079,36 +14153,39 @@
         :type HybridBillingPrepaidReplicas: int
         :param _OldHybridBillingPrepaidReplicas: 历史 HYBRID_PAID 时的实例数，用户恢复服务
 注意：此字段可能返回 null，表示取不到有效值。
         :type OldHybridBillingPrepaidReplicas: int
         :param _ModelHotUpdateEnable: 是否开启模型的热更新。默认不开启
 注意：此字段可能返回 null，表示取不到有效值。
         :type ModelHotUpdateEnable: bool
-        :param _Pods: Pod列表信息
+        :param _ScaleMode: 实例数量调节方式,默认为手动
+支持：自动 - "AUTO", 手动 - "MANUAL"
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Pods: :class:`tencentcloud.tione.v20211111.models.Pod`
-        :param _PodInfos: Pod列表信息
+        :type ScaleMode: str
+        :param _CronScaleJobs: 定时伸缩任务
 注意：此字段可能返回 null，表示取不到有效值。
-        :type PodInfos: list of Pod
+        :type CronScaleJobs: list of CronScaleJob
         :param _ScaleStrategy: 定时伸缩策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type ScaleStrategy: str
-        :param _CronScaleJobs: 定时伸缩任务
+        :param _ScheduledAction: 定时停止的配置
 注意：此字段可能返回 null，表示取不到有效值。
-        :type CronScaleJobs: list of CronScaleJob
-        :param _ScaleMode: 实例数量调节方式,默认为手动
-支持：自动 - "AUTO", 手动 - "MANUAL"
+        :type ScheduledAction: str
+        :param _Pods: Pod列表信息
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ScaleMode: str
+        :type Pods: :class:`tencentcloud.tione.v20211111.models.Pod`
+        :param _PodInfos: Pod列表信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PodInfos: list of Pod
         :param _ServiceLimit: 服务限速限流相关配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
-        :param _ScheduledAction: 定时停止的配置
+        :param _ModelTurboEnable: 是否开启模型的加速, 仅对StableDiffusion(动态加速)格式的模型有效。
 注意：此字段可能返回 null，表示取不到有效值。
-        :type ScheduledAction: str
+        :type ModelTurboEnable: bool
         """
         self._Replicas = None
         self._ImageInfo = None
         self._Env = None
         self._Resources = None
         self._InstanceType = None
         self._ModelInfo = None
@@ -14120,21 +14197,22 @@
         self._Weight = None
         self._PodList = None
         self._ResourceTotal = None
         self._OldReplicas = None
         self._HybridBillingPrepaidReplicas = None
         self._OldHybridBillingPrepaidReplicas = None
         self._ModelHotUpdateEnable = None
+        self._ScaleMode = None
+        self._CronScaleJobs = None
+        self._ScaleStrategy = None
+        self._ScheduledAction = None
         self._Pods = None
         self._PodInfos = None
-        self._ScaleStrategy = None
-        self._CronScaleJobs = None
-        self._ScaleMode = None
         self._ServiceLimit = None
-        self._ScheduledAction = None
+        self._ModelTurboEnable = None
 
     @property
     def Replicas(self):
         return self._Replicas
 
     @Replicas.setter
     def Replicas(self, Replicas):
@@ -14273,68 +14351,76 @@
         return self._ModelHotUpdateEnable
 
     @ModelHotUpdateEnable.setter
     def ModelHotUpdateEnable(self, ModelHotUpdateEnable):
         self._ModelHotUpdateEnable = ModelHotUpdateEnable
 
     @property
-    def Pods(self):
-        return self._Pods
+    def ScaleMode(self):
+        return self._ScaleMode
 
-    @Pods.setter
-    def Pods(self, Pods):
-        self._Pods = Pods
+    @ScaleMode.setter
+    def ScaleMode(self, ScaleMode):
+        self._ScaleMode = ScaleMode
 
     @property
-    def PodInfos(self):
-        return self._PodInfos
+    def CronScaleJobs(self):
+        return self._CronScaleJobs
 
-    @PodInfos.setter
-    def PodInfos(self, PodInfos):
-        self._PodInfos = PodInfos
+    @CronScaleJobs.setter
+    def CronScaleJobs(self, CronScaleJobs):
+        self._CronScaleJobs = CronScaleJobs
 
     @property
     def ScaleStrategy(self):
         return self._ScaleStrategy
 
     @ScaleStrategy.setter
     def ScaleStrategy(self, ScaleStrategy):
         self._ScaleStrategy = ScaleStrategy
 
     @property
-    def CronScaleJobs(self):
-        return self._CronScaleJobs
+    def ScheduledAction(self):
+        return self._ScheduledAction
 
-    @CronScaleJobs.setter
-    def CronScaleJobs(self, CronScaleJobs):
-        self._CronScaleJobs = CronScaleJobs
+    @ScheduledAction.setter
+    def ScheduledAction(self, ScheduledAction):
+        self._ScheduledAction = ScheduledAction
 
     @property
-    def ScaleMode(self):
-        return self._ScaleMode
+    def Pods(self):
+        return self._Pods
 
-    @ScaleMode.setter
-    def ScaleMode(self, ScaleMode):
-        self._ScaleMode = ScaleMode
+    @Pods.setter
+    def Pods(self, Pods):
+        self._Pods = Pods
+
+    @property
+    def PodInfos(self):
+        return self._PodInfos
+
+    @PodInfos.setter
+    def PodInfos(self, PodInfos):
+        self._PodInfos = PodInfos
 
     @property
     def ServiceLimit(self):
         return self._ServiceLimit
 
     @ServiceLimit.setter
     def ServiceLimit(self, ServiceLimit):
         self._ServiceLimit = ServiceLimit
 
     @property
-    def ScheduledAction(self):
-        return self._ScheduledAction
+    def ModelTurboEnable(self):
+        return self._ModelTurboEnable
 
-    @ScheduledAction.setter
-    def ScheduledAction(self, ScheduledAction):
-        self._ScheduledAction = ScheduledAction
+    @ModelTurboEnable.setter
+    def ModelTurboEnable(self, ModelTurboEnable):
+        self._ModelTurboEnable = ModelTurboEnable
 
 
     def _deserialize(self, params):
         self._Replicas = params.get("Replicas")
         if params.get("ImageInfo") is not None:
             self._ImageInfo = ImageInfo()
             self._ImageInfo._deserialize(params.get("ImageInfo"))
@@ -14367,35 +14453,36 @@
         if params.get("ResourceTotal") is not None:
             self._ResourceTotal = ResourceInfo()
             self._ResourceTotal._deserialize(params.get("ResourceTotal"))
         self._OldReplicas = params.get("OldReplicas")
         self._HybridBillingPrepaidReplicas = params.get("HybridBillingPrepaidReplicas")
         self._OldHybridBillingPrepaidReplicas = params.get("OldHybridBillingPrepaidReplicas")
         self._ModelHotUpdateEnable = params.get("ModelHotUpdateEnable")
+        self._ScaleMode = params.get("ScaleMode")
+        if params.get("CronScaleJobs") is not None:
+            self._CronScaleJobs = []
+            for item in params.get("CronScaleJobs"):
+                obj = CronScaleJob()
+                obj._deserialize(item)
+                self._CronScaleJobs.append(obj)
+        self._ScaleStrategy = params.get("ScaleStrategy")
+        self._ScheduledAction = params.get("ScheduledAction")
         if params.get("Pods") is not None:
             self._Pods = Pod()
             self._Pods._deserialize(params.get("Pods"))
         if params.get("PodInfos") is not None:
             self._PodInfos = []
             for item in params.get("PodInfos"):
                 obj = Pod()
                 obj._deserialize(item)
                 self._PodInfos.append(obj)
-        self._ScaleStrategy = params.get("ScaleStrategy")
-        if params.get("CronScaleJobs") is not None:
-            self._CronScaleJobs = []
-            for item in params.get("CronScaleJobs"):
-                obj = CronScaleJob()
-                obj._deserialize(item)
-                self._CronScaleJobs.append(obj)
-        self._ScaleMode = params.get("ScaleMode")
         if params.get("ServiceLimit") is not None:
             self._ServiceLimit = ServiceLimit()
             self._ServiceLimit._deserialize(params.get("ServiceLimit"))
-        self._ScheduledAction = params.get("ScheduledAction")
+        self._ModelTurboEnable = params.get("ModelTurboEnable")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -17169,23 +17256,27 @@
 Pending 启动中
 Stopping 停止中
         :type Status: str
         :param _StatefulSetCondition: 工作负载的状况信息
         :type StatefulSetCondition: list of StatefulSetCondition
         :param _Conditions: 工作负载历史的状况信息
         :type Conditions: list of StatefulSetCondition
+        :param _Reason: 状态异常时，展示原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Reason: str
         """
         self._Replicas = None
         self._UpdatedReplicas = None
         self._ReadyReplicas = None
         self._AvailableReplicas = None
         self._UnavailableReplicas = None
         self._Status = None
         self._StatefulSetCondition = None
         self._Conditions = None
+        self._Reason = None
 
     @property
     def Replicas(self):
         return self._Replicas
 
     @Replicas.setter
     def Replicas(self, Replicas):
@@ -17243,14 +17334,22 @@
     def Conditions(self):
         return self._Conditions
 
     @Conditions.setter
     def Conditions(self, Conditions):
         self._Conditions = Conditions
 
+    @property
+    def Reason(self):
+        return self._Reason
+
+    @Reason.setter
+    def Reason(self, Reason):
+        self._Reason = Reason
+
 
     def _deserialize(self, params):
         self._Replicas = params.get("Replicas")
         self._UpdatedReplicas = params.get("UpdatedReplicas")
         self._ReadyReplicas = params.get("ReadyReplicas")
         self._AvailableReplicas = params.get("AvailableReplicas")
         self._UnavailableReplicas = params.get("UnavailableReplicas")
@@ -17263,14 +17362,15 @@
                 self._StatefulSetCondition.append(obj)
         if params.get("Conditions") is not None:
             self._Conditions = []
             for item in params.get("Conditions"):
                 obj = StatefulSetCondition()
                 obj._deserialize(item)
                 self._Conditions.append(obj)
+        self._Reason = params.get("Reason")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.935/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.936/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.936/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.935/README.rst` & `tencentcloud-sdk-python-tione-3.0.936/README.rst`

 * *Files identical despite different names*

