# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.935.tar", last modified: Fri Jul 14 00:30:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.936.tar", last modified: Mon Jul 17 00:24:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.935.tar` & `tencentcloud-sdk-python-emr-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30020 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    14329 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   455302 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:30:11.000000 tencentcloud-sdk-python-emr-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30020 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    14329 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455464 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:24:37.000000 tencentcloud-sdk-python-emr-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-emr-3.0.935/setup.py` & `tencentcloud-sdk-python-emr-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.935/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.936/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3843,15 +3843,15 @@
         :type DisplayStrategy: str
         :param _Offset: 页编号，默认值为0，表示第一页。
         :type Offset: int
         :param _Limit: 每页返回数量，默认值为10，最大值为100。
         :type Limit: int
         :param _OrderField: 排序字段。取值范围：<li>clusterId：表示按照实例ID排序。</li><li>addTime：表示按照实例创建时间排序。</li><li>status：表示按照实例的状态码排序。</li>
         :type OrderField: str
-        :param _Asc: 按照OrderField升序或者降序进行排序。取值范围：<li>0：表示降序。</li><li>1：表示升序。</li>默认值为0。
+        :param _Asc: 按照OrderField升序或者降序进行排序。取值范围：<li>0：表示降序。</li><li>1：表示升序。</li>默认值为0。
         :type Asc: int
         :param _Filters: 自定义查询
         :type Filters: list of Filters
         """
         self._DisplayStrategy = None
         self._Offset = None
         self._Limit = None
@@ -4000,24 +4000,24 @@
         :type InstanceIds: list of str
         :param _Offset: 页编号，默认值为0，表示第一页。
         :type Offset: int
         :param _Limit: 每页返回数量，默认值为10，最大值为100。
         :type Limit: int
         :param _ProjectId: 建议必填-1，表示拉取所有项目下的集群。
 不填默认值为0，表示拉取默认项目下的集群。
-实例所属项目ID。该参数可以通过调用 [DescribeProject](https://cloud.tencent.com/document/api/378/4400) 的返回值中的 projectId 字段来获取。
+实例所属项目ID。该参数可以通过调用 [DescribeProjects](https://cloud.tencent.com/document/product/651/78725) 的返回值中的 projectId 字段来获取。
         :type ProjectId: int
         :param _OrderField: 排序字段。取值范围：
 <li>clusterId：表示按照实例ID排序。</li>
 <li>addTime：表示按照实例创建时间排序。</li>
 <li>status：表示按照实例的状态码排序。</li>
         :type OrderField: str
         :param _Asc: 按照OrderField升序或者降序进行排序。取值范围：
 <li>0：表示降序。</li>
-<li>1：表示升序。</li>默认值为0。
+<li>1：表示升序。</li>默认值为0。
         :type Asc: int
         """
         self._DisplayStrategy = None
         self._InstanceIds = None
         self._Offset = None
         self._Limit = None
         self._ProjectId = None
@@ -6318,15 +6318,15 @@
         :type Placement: :class:`tencentcloud.emr.v20190103.models.Placement`
         :param _PayMode: 实例计费模式。此处只支持取值为1，表示包年包月。
         :type PayMode: int
         :param _TimeUnit: 实例续费的时间单位。取值范围：
 <li>m：表示月份。</li>
         :type TimeUnit: str
         :param _Currency: 货币种类。取值范围：
-<li>CNY：表示人民币。</li>
+<li>CNY：表示人民币。</li>
         :type Currency: str
         """
         self._TimeSpan = None
         self._InstanceId = None
         self._Placement = None
         self._PayMode = None
         self._TimeUnit = None
@@ -6410,15 +6410,15 @@
         :param _OriginalCost: 原价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCost: float
         :param _DiscountCost: 折扣价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiscountCost: float
         :param _TimeUnit: 实例续费的时间单位。取值范围：
-<li>m：表示月份。</li>
+<li>m：表示月份。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeUnit: str
         :param _TimeSpan: 实例续费的时长。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeSpan: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -6490,15 +6490,15 @@
 <li>m：表示月份。PayMode取值为1时，TimeUnit只能取值为m。</li>
         :type TimeUnit: str
         :param _TimeSpan: 购买实例的时长。结合TimeUnit一起使用。
 <li>TimeUnit为s时，该参数只能填写3600，表示按量计费实例。</li>
 <li>TimeUnit为m时，该参数填写的数字表示包年包月实例的购买时长，如1表示购买一个月</li>
         :type TimeSpan: int
         :param _Currency: 货币种类。取值范围：
-<li>CNY：表示人民币。</li>
+<li>CNY：表示人民币。</li>
         :type Currency: str
         :param _PayMode: 实例计费模式。取值范围：
 <li>0：表示按量计费。</li>
 <li>1：表示包年包月。</li>
         :type PayMode: int
         :param _SupportHA: 是否开启节点高可用。取值范围：
 <li>0：表示不开启节点高可用。</li>
@@ -6756,15 +6756,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCost: float
         :param _DiscountCost: 折扣价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiscountCost: float
         :param _TimeUnit: 购买实例的时间单位。取值范围：
 <li>s：表示秒。</li>
-<li>m：表示月份。</li>
+<li>m：表示月份。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeUnit: str
         :param _TimeSpan: 购买实例的时长。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeSpan: int
         :param _PriceList: 价格清单
 注意：此字段可能返回 null，表示取不到有效值。
@@ -6847,25 +6847,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param _TimeSpan: 实例续费的时长。需要结合TimeUnit一起使用。1表示续费一个月
         :type TimeSpan: int
-        :param _ResourceIds: 待续费节点的资源ID列表。资源ID形如：emr-vm-xxxxxxxx。有效的资源ID可通过登录[控制台](https://console.cloud.tencent.com/emr/static/hardware)查询。
+        :param _ResourceIds: 待续费节点的资源ID列表。资源ID形如：emr-vm-xxxxxxxx。有效的资源ID可通过登录[控制台](https://console.cloud.tencent.com/emr)查询。
         :type ResourceIds: list of str
         :param _Placement: 实例所在的位置。通过该参数可以指定实例所属可用区，所属项目等属性。
         :type Placement: :class:`tencentcloud.emr.v20190103.models.Placement`
         :param _PayMode: 实例计费模式。此处只支持取值为1，表示包年包月。
         :type PayMode: int
         :param _TimeUnit: 实例续费的时间单位。取值范围：
 <li>m：表示月份。</li>
         :type TimeUnit: str
         :param _Currency: 货币种类。取值范围：
-<li>CNY：表示人民币。</li>
+<li>CNY：表示人民币。</li>
         :type Currency: str
         :param _ModifyPayMode: 是否按量转包年包月。0：否，1：是。
         :type ModifyPayMode: int
         """
         self._TimeSpan = None
         self._ResourceIds = None
         self._Placement = None
@@ -6961,15 +6961,15 @@
         :param _OriginalCost: 原价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCost: float
         :param _DiscountCost: 折扣价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiscountCost: float
         :param _TimeUnit: 实例续费的时间单位。取值范围：
-<li>m：表示月份。</li>
+<li>m：表示月份。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeUnit: str
         :param _TimeSpan: 实例续费的时长。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeSpan: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -7053,15 +7053,15 @@
         :param _InstanceId: 实例ID。
         :type InstanceId: str
         :param _CoreCount: 扩容的Core节点数量。
         :type CoreCount: int
         :param _TaskCount: 扩容的Task节点数量。
         :type TaskCount: int
         :param _Currency: 货币种类。取值范围：
-<li>CNY：表示人民币。</li>
+<li>CNY：表示人民币。</li>
         :type Currency: str
         :param _RouterCount: 扩容的Router节点数量。
         :type RouterCount: int
         :param _MasterCount: 扩容的Master节点数量。
         :type MasterCount: int
         """
         self._TimeUnit = None
@@ -7188,15 +7188,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCost: str
         :param _DiscountCost: 折扣价，单位为元。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiscountCost: str
         :param _Unit: 扩容的时间单位。取值范围：
 <li>s：表示秒。</li>
-<li>m：表示月份。</li>
+<li>m：表示月份。</li>
 注意：此字段可能返回 null，表示取不到有效值。
         :type Unit: str
         :param _PriceSpec: 询价的节点规格。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PriceSpec: :class:`tencentcloud.emr.v20190103.models.PriceResource`
         :param _MultipleEmrPrice: 对应入参MultipleResources中多个规格的询价结果，其它出参返回的是第一个规格的询价结果
 注意：此字段可能返回 null，表示取不到有效值。
@@ -8231,18 +8231,21 @@
 
     def __init__(self):
         r"""
         :param _DiskType: 云盘类型
 <li>CLOUD_SSD：表示云SSD。</li>
 <li>CLOUD_PREMIUM：表示高效云盘。</li>
 <li>CLOUD_HSSD：表示增强型SSD云硬盘。</li>
+注意：此字段可能返回 null，表示取不到有效值。
         :type DiskType: str
         :param _Volume: 云盘大小
+注意：此字段可能返回 null，表示取不到有效值。
         :type Volume: int
         :param _Count: 该类型云盘个数
+注意：此字段可能返回 null，表示取不到有效值。
         :type Count: int
         """
         self._DiskType = None
         self._Volume = None
         self._Count = None
 
     @property
@@ -13566,15 +13569,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _InstanceId: 实例ID。
         :type InstanceId: str
-        :param _ResourceIds: 待销毁节点的资源ID列表。资源ID形如：emr-vm-xxxxxxxx。有效的资源ID可通过登录[控制台](https://console.cloud.tencent.com/emr/static/hardware)查询。
+        :param _ResourceIds: 待销毁节点的资源ID列表。资源ID形如：emr-vm-xxxxxxxx。有效的资源ID可通过登录[控制台](https://console.cloud.tencent.com/emr)查询。
         :type ResourceIds: list of str
         """
         self._InstanceId = None
         self._ResourceIds = None
 
     @property
     def InstanceId(self):
```

### Comparing `tencentcloud-sdk-python-emr-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.935/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.936/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.936/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.935/README.rst` & `tencentcloud-sdk-python-emr-3.0.936/README.rst`

 * *Files identical despite different names*

