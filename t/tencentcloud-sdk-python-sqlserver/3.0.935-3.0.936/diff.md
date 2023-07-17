# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.935.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.935.tar", last modified: Fri Jul 14 00:37:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.936.tar", last modified: Mon Jul 17 00:34:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.935.tar` & `tencentcloud-sdk-python-sqlserver-3.0.936.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   108720 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9722 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   571881 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-14 00:37:31.000000 tencentcloud-sdk-python-sqlserver-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   108687 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   572158 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 00:34:17.000000 tencentcloud-sdk-python-sqlserver-3.0.936/README.rst
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.936/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBackupFiles(self, request):
-        """本接口(DescribeBackupFiles)用于在非打包备份模式下单个库对应的备份文件
+        """本接口(DescribeBackupFiles)用于查询单库备份明细
 
         :param request: Request instance for DescribeBackupFiles.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupFilesRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupFilesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
 
     def __init__(self):
         r"""
         :param _UserName: 数据库用户名
         :type UserName: str
         :param _DBPrivileges: 账号权限变更信息
         :type DBPrivileges: list of DBPrivilegeModifyInfo
-        :param _IsAdmin: 是否为管理员账户,当值为true 等价于基础版AccountType=L0，高可用AccountType=L1，当值为false时，表示删除管理员权限，默认false
+        :param _IsAdmin: 表示是否为管理员账户，当值为true，表示是 管理员。若实例 是 单节点，则管理员所在的 账号类型为超级权限账号 ，即AccountType=L0；若实例 是 双节点，则管理员所在的 账号类型为高级权限账号，即AccountType=L1；当值为false，表示 不是管理员，则账号类型为普通账号，即AccountType=L3
         :type IsAdmin: bool
         :param _AccountType: 账号类型，IsAdmin字段的扩展字段。 L0-超级权限(基础版独有),L1-高级权限,L2-特殊权限,L3-普通权限，默认L3
         :type AccountType: str
         """
         self._UserName = None
         self._DBPrivileges = None
         self._IsAdmin = None
@@ -1684,15 +1684,15 @@
 
     def __init__(self):
         r"""
         :param _Strategy: 备份策略(0-实例备份 1-多库备份)
         :type Strategy: int
         :param _DBNames: 需要备份库名的列表(多库备份才填写)
         :type DBNames: list of str
-        :param _InstanceId: 实例ID，形如mssql-i1z41iwd
+        :param _InstanceId: 实例ID（必填），形如mssql-i1z41iwd
         :type InstanceId: str
         :param _BackupName: 备份名称，若不填则自动生成“实例ID_备份开始时间戳”
         :type BackupName: str
         """
         self._Strategy = None
         self._DBNames = None
         self._InstanceId = None
@@ -7096,15 +7096,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _InstanceId: 实例ID，形如mssql-njj2mtpl
         :type InstanceId: str
-        :param _GroupId: 聚合ID, 可通过接口DescribeBackups获取
+        :param _GroupId: 单库备份的聚合ID, 可通过接口DescribeBackups获取（不支持查询打包备份记录）
         :type GroupId: str
         :param _Limit: 分页返回，每页返回的数目，取值为1-100，默认值为20
         :type Limit: int
         :param _Offset: 分页返回，页编号，默认值为第0页
         :type Offset: int
         :param _DatabaseName: 按照备份的库名称筛选，不填则不筛选此项
         :type DatabaseName: str
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.936/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.936/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.935
+Version: 3.0.936
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.935/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.936/README.rst`

 * *Files identical despite different names*

