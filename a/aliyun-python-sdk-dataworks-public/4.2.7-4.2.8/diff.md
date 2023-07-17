# Comparing `tmp/aliyun-python-sdk-dataworks-public-4.2.7.tar.gz` & `tmp/aliyun-python-sdk-dataworks-public-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dataworks-public-4.2.7.tar", last modified: Fri Mar 31 09:29:27 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dataworks-public-4.2.8.tar", last modified: Mon Jun  5 03:10:36 2023, max compression
```

## Comparing `aliyun-python-sdk-dataworks-public-4.2.7.tar` & `aliyun-python-sdk-dataworks-public-4.2.8.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1602 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18964 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AbolishDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddMetaCollectionEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddProjectMemberToRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddToMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ApprovePermissionApplyOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ChangeResourceManagerResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckFileDeploymentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckMetaPartitionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckMetaTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDISyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDagComplementRequest.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDagTestRequest.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiAuthorityRequest.py
--rw-r--r--   0 root         (0) root         (0)     5036 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateExportMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateImportMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2878 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateManualDagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateMetaCollectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3634 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreatePermissionApplyOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateProjectMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityFollowerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityRelativeNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4902 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4314 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateRemindRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     6405 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableThemeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3708 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateUdfFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDISyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiAuthorityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1678 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFromMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteProjectMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityFollowerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRelativeNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteRemindRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableThemeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeployDISyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeployFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DesensitizeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/EstablishRelationTableToBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ExportDataSourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForCreatingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForUpdatingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineKeyPathRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDDLJobStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDISyncInstanceInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDISyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiTestRequest.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServicePublishedApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataSourceMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDeploymentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetExtensionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileTypeStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetIDEEventDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceConsumeTimeRankRequest.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceCountTrendRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceErrorRankRequest.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetManualDagInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaCollectionDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaColumnLineageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaDBInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaDBTableListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableBasicInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableChangeLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableColumnRequest.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableFullInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableIntroWikiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableLineageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableListByCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableOutputRequest.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTablePartitionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2442 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableProducingTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableThemeLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMigrationProcessRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMigrationSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeChildrenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeOnBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeParentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2422 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeTypeListInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOpRiskDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOpSensitiveDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOptionValueForProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetPermissionApplyOrderDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetProjectDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityFollowerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetRemindRequest.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetSensitiveDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetSuccessInstanceTrendRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetTopicInfluenceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetTopicRequest.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ImportDataSourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListAlertMessagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselineConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3118 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselineStatusesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListCalcEnginesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListConnectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDIProjectConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiAuthoritiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiTestRequest.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceAuthorizedApisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceFoldersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServicePublishedApisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataSourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3180 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDeploymentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListEnabledExtensionsForProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListExtensionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFileTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFileVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFoldersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInnerNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstanceAmountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstanceHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3784 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListManualDagInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionEntitiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaDBRequest.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMigrationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodeIORequest.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodeInputOrOutputRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesByBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesByOutputRequest.py
--rw-r--r--   0 root         (0) root         (0)     2728 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListPermissionApplyOrdersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProgramTypeCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectIdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectMembersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListRefDISyncTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListRemindsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2379 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListResourceGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListShiftPersonnelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListShiftSchedulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListSuccessInstanceAmountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTableLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTableThemeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTopicsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/MountDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/OfflineNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/PublishDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/QueryDISyncTaskConfigProcessResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/QueryPublicModelEngineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RemoveProjectMemberFromRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RestartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ResumeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RevokeColumnPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RevokeTablePermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunCycleDagNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunManualDagNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunSmokeTestRequest.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunTriggerNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2286 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SaveDataServiceApiTestResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ScanSensitiveDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SearchMetaTablesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SearchNodesByOutputRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SetDataSourceShareRequest.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SetSuccessInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StartDISyncInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StartMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StopDISyncInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StopInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SubmitDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SubmitFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SuspendInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TerminateDISyncInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3751 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TestDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TestNetworkConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TopTenElapsedTimeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TopTenErrorTimesInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UmountDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDIProjectConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDISyncTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     4092 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDataServiceApiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateIDEEventResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCollectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableIntroWikiRequest.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateNodeOwnerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateNodeRunModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateQualityFollowerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5232 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateQualityRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4662 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateRemindRequest.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableAddColumnRequest.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableLevelRequest.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableModelInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     6443 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableThemeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateUdfFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateWorkbenchEventResultRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-31 09:29:27.000000 aliyun-python-sdk-dataworks-public-4.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2517 2023-03-31 09:29:26.000000 aliyun-python-sdk-dataworks-public-4.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18964 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AbolishDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddMetaCollectionEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddProjectMemberToRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddToMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ApprovePermissionApplyOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ChangeResourceManagerResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckFileDeploymentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckMetaPartitionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckMetaTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDISyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDagComplementRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDagTestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiAuthorityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5036 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateExportMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7586 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateImportMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateManualDagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateMetaCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreatePermissionApplyOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateProjectMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityFollowerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityRelativeNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateRemindRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6405 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableThemeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateUdfFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDISyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiAuthorityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFromMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteProjectMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityFollowerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRelativeNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteRemindRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableThemeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeployDISyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeployFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DesensitizeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/EstablishRelationTableToBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ExportDataSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForCreatingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForUpdatingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineKeyPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDDLJobStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDISyncInstanceInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDISyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiTestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServicePublishedApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataSourceMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDeploymentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetExtensionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileTypeStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetIDEEventDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceConsumeTimeRankRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceCountTrendRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceErrorRankRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetManualDagInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaCollectionDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaColumnLineageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaDBInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaDBTableListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableBasicInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableChangeLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableColumnRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableFullInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableIntroWikiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableLineageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableListByCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableOutputRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTablePartitionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableProducingTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableThemeLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMigrationProcessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMigrationSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeChildrenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeOnBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeParentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeTypeListInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOpRiskDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOpSensitiveDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOptionValueForProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetPermissionApplyOrderDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetProjectDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityFollowerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetRemindRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetSensitiveDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetSuccessInstanceTrendRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetTopicInfluenceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetTopicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ImportDataSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListAlertMessagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselineConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselineStatusesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListCalcEnginesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListConnectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDIProjectConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiAuthoritiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiTestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceAuthorizedApisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceFoldersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServicePublishedApisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDeploymentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListEnabledExtensionsForProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListExtensionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFileTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFileVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFoldersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInnerNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstanceAmountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstanceHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3784 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListManualDagInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionEntitiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaDBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMigrationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodeIORequest.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodeInputOrOutputRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesByBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesByOutputRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListPermissionApplyOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProgramTypeCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectIdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectMembersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListRefDISyncTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListRemindsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListResourceGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListShiftPersonnelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListShiftSchedulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListSuccessInstanceAmountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTableLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTableThemeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTopicsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/MountDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/OfflineNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/PublishDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/QueryDISyncTaskConfigProcessResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/QueryPublicModelEngineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RemoveProjectMemberFromRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RestartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ResumeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RevokeColumnPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RevokeTablePermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunCycleDagNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunManualDagNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunSmokeTestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunTriggerNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SaveDataServiceApiTestResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ScanSensitiveDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SearchMetaTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SearchNodesByOutputRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SetDataSourceShareRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SetSuccessInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StartDISyncInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StartMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StopDISyncInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StopInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SubmitDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SubmitFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SuspendInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TerminateDISyncInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TestDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TestNetworkConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TopTenElapsedTimeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TopTenErrorTimesInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UmountDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDIProjectConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDISyncTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDataServiceApiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7542 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateIDEEventResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableIntroWikiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateNodeOwnerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateNodeRunModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateQualityFollowerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateQualityRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateRemindRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableAddColumnRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableLevelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableModelInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6443 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableThemeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateUdfFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateWorkbenchEventResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-05 03:10:36.000000 aliyun-python-sdk-dataworks-public-4.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-06-05 03:10:35.000000 aliyun-python-sdk-dataworks-public-4.2.8/setup.py
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/LICENSE` & `aliyun-python-sdk-dataworks-public-4.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/PKG-INFO` & `aliyun-python-sdk-dataworks-public-4.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dataworks-public
-Version: 4.2.7
+Version: 4.2.8
 Summary: The dataworks-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dataworks-public
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/README.rst` & `aliyun-python-sdk-dataworks-public-4.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/PKG-INFO` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dataworks-public
-Version: 4.2.7
+Version: 4.2.8
 Summary: The dataworks-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dataworks-public
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyun_python_sdk_dataworks_public.egg-info/SOURCES.txt` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyun_python_sdk_dataworks_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/endpoint.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AbolishDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AbolishDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddMetaCollectionEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddMetaCollectionEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddProjectMemberToRoleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddProjectMemberToRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/AddToMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/AddToMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ApprovePermissionApplyOrderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ApprovePermissionApplyOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ChangeResourceManagerResourceGroupRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ChangeResourceManagerResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckFileDeploymentRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckFileDeploymentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckMetaPartitionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckMetaPartitionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CheckMetaTableRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CheckMetaTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateConnectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDISyncTaskRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDISyncTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDagComplementRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDagComplementRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDagTestRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDagTestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiAuthorityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiAuthorityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceGroupRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataServiceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateDataSourceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateExportMigrationRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateExportMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateFileRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
 	def set_AutoRerunTimes(self, AutoRerunTimes):  # Integer
 		self.add_body_params('AutoRerunTimes', AutoRerunTimes)
 	def get_CronExpress(self): # String
 		return self.get_body_params().get('CronExpress')
 
 	def set_CronExpress(self, CronExpress):  # String
 		self.add_body_params('CronExpress', CronExpress)
+	def get_IgnoreParentSkipRunningProperty(self): # Boolean
+		return self.get_body_params().get('IgnoreParentSkipRunningProperty')
+
+	def set_IgnoreParentSkipRunningProperty(self, IgnoreParentSkipRunningProperty):  # Boolean
+		self.add_body_params('IgnoreParentSkipRunningProperty', IgnoreParentSkipRunningProperty)
 	def get_EndEffectDate(self): # Long
 		return self.get_body_params().get('EndEffectDate')
 
 	def set_EndEffectDate(self, EndEffectDate):  # Long
 		self.add_body_params('EndEffectDate', EndEffectDate)
 	def get_FileName(self): # String
 		return self.get_body_params().get('FileName')
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateImportMigrationRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateImportMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateManualDagRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateManualDagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateMetaCollectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateMetaCollectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreatePermissionApplyOrderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreatePermissionApplyOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateProjectMemberRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateProjectMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityFollowerRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityFollowerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityRelativeNodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityRelativeNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateQualityRuleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateQualityRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateRemindRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateRemindRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableLevelRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateTableThemeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateTableThemeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/CreateUdfFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/CreateUdfFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteConnectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDISyncTaskRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDISyncTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiAuthorityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiAuthorityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteDataSourceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteFromMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteFromMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteMetaCollectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteProjectMemberRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteProjectMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityFollowerRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityFollowerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRelativeNodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRelativeNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRuleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteQualityRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteRemindRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteRemindRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableLevelRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeleteTableThemeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeleteTableThemeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeployDISyncTaskRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeployDISyncTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DeployFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DeployFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/DesensitizeDataRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/DesensitizeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/EstablishRelationTableToBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/EstablishRelationTableToBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ExportDataSourcesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ExportDataSourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForCreatingRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForCreatingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForUpdatingRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GenerateDISyncTaskConfigForUpdatingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineConfigRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineKeyPathRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineKeyPathRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBaselineStatusRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBaselineStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDDLJobStatusRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDDLJobStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDISyncInstanceInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDISyncInstanceInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDISyncTaskRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDISyncTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDagRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiTestRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApiTestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApplicationRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServiceGroupRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServiceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataServicePublishedApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataServicePublishedApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDataSourceMetaRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDataSourceMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetDeploymentRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetDeploymentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetExtensionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetExtensionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileTypeStatisticRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileTypeStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFileVersionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFileVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetIDEEventDetailRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetIDEEventDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceConsumeTimeRankRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceConsumeTimeRankRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceCountTrendRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceCountTrendRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceErrorRankRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceErrorRankRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceLogRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusCountRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusStatisticRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetInstanceStatusStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetManualDagInstancesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetManualDagInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaCollectionDetailRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaCollectionDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaColumnLineageRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaColumnLineageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaDBInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaDBInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaDBTableListRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaDBTableListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableBasicInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableBasicInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableChangeLogRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableChangeLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableColumnRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableColumnRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableFullInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableFullInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableIntroWikiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableIntroWikiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableLineageRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableLineageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableListByCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableListByCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableOutputRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableOutputRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTablePartitionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTablePartitionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableProducingTasksRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableProducingTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMetaTableThemeLevelRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMetaTableThemeLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMigrationProcessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMigrationProcessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetMigrationSummaryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetMigrationSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeChildrenRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeChildrenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeCodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeOnBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeOnBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeParentsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeParentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetNodeTypeListInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetNodeTypeListInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOpRiskDataRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOpRiskDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOpSensitiveDataRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOpSensitiveDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetOptionValueForProjectRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetOptionValueForProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetPermissionApplyOrderDetailRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetPermissionApplyOrderDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetProjectDetailRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetProjectDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetProjectRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityFollowerRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityFollowerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetQualityRuleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetQualityRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetRemindRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetRemindRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetSensitiveDataRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetSensitiveDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetSuccessInstanceTrendRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetSuccessInstanceTrendRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetTopicInfluenceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetTopicInfluenceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/GetTopicRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/GetTopicRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ImportDataSourcesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ImportDataSourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListAlertMessagesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListAlertMessagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselineConfigsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselineConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselineStatusesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselineStatusesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBaselinesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBaselinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListCalcEnginesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListCalcEnginesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListConnectionsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListConnectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDIProjectConfigRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDIProjectConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDagsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiAuthoritiesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiAuthoritiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiTestRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApiTestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApisRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApplicationsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceApplicationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceAuthorizedApisRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceAuthorizedApisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceFoldersRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceFoldersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServiceGroupsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServiceGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataServicePublishedApisRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataServicePublishedApisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDataSourcesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDataSourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListDeploymentsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListDeploymentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListEnabledExtensionsForProjectRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListEnabledExtensionsForProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListExtensionsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListExtensionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFileTypeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFileTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFileVersionsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFileVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFilesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListFoldersRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListFoldersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInnerNodesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInnerNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstanceAmountRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstanceAmountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstanceHistoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstanceHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListInstancesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListManualDagInstancesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListManualDagInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionEntitiesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionEntitiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaCollectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMetaDBRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMetaDBRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListMigrationsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListMigrationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodeIORequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodeIORequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodeInputOrOutputRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodeInputOrOutputRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesByBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesByBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesByOutputRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesByOutputRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListNodesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListPermissionApplyOrdersRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListPermissionApplyOrdersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProgramTypeCountRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProgramTypeCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectIdsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectIdsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectMembersRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectMembersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectRolesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListProjectsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByEntityRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByRuleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityResultsByRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListQualityRulesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListQualityRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListRefDISyncTasksRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListRefDISyncTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListRemindsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListRemindsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListResourceGroupsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListResourceGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListShiftPersonnelsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListShiftPersonnelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListShiftSchedulesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListShiftSchedulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListSuccessInstanceAmountRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListSuccessInstanceAmountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTableLevelRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTableLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTableThemeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTableThemeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ListTopicsRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ListTopicsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/MountDirectoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/MountDirectoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/OfflineNodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/OfflineNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/PublishDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/PublishDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/QueryDISyncTaskConfigProcessResultRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/QueryDISyncTaskConfigProcessResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/QueryPublicModelEngineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/QueryPublicModelEngineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RemoveProjectMemberFromRoleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RemoveProjectMemberFromRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RestartInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RestartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ResumeInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ResumeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RevokeColumnPermissionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RevokeColumnPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RevokeTablePermissionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RevokeTablePermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunCycleDagNodesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunCycleDagNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunManualDagNodesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunManualDagNodesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,24 @@
 	def set_ProjectEnv(self, ProjectEnv):  # String
 		self.add_body_params('ProjectEnv', ProjectEnv)
 	def get_ProjectName(self): # String
 		return self.get_body_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_body_params('ProjectName', ProjectName)
+	def get_StartBizDate(self): # String
+		return self.get_body_params().get('StartBizDate')
+
+	def set_StartBizDate(self, StartBizDate):  # String
+		self.add_body_params('StartBizDate', StartBizDate)
+	def get_EndBizDate(self): # String
+		return self.get_body_params().get('EndBizDate')
+
+	def set_EndBizDate(self, EndBizDate):  # String
+		self.add_body_params('EndBizDate', EndBizDate)
 	def get_DagParameters(self): # String
 		return self.get_body_params().get('DagParameters')
 
 	def set_DagParameters(self, DagParameters):  # String
 		self.add_body_params('DagParameters', DagParameters)
 	def get_IncludeNodeIds(self): # String
 		return self.get_body_params().get('IncludeNodeIds')
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunSmokeTestRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunSmokeTestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/RunTriggerNodeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/RunTriggerNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SaveDataServiceApiTestResultRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SaveDataServiceApiTestResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/ScanSensitiveDataRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/ScanSensitiveDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SearchMetaTablesRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SearchMetaTablesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SearchNodesByOutputRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SearchNodesByOutputRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SetDataSourceShareRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SetDataSourceShareRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SetSuccessInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SetSuccessInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StartDISyncInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StartDISyncInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StartMigrationRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StartMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StopDISyncInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StopDISyncInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/StopInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/StopInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SubmitDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SubmitDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SubmitFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SubmitFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/SuspendInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/SuspendInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TerminateDISyncInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TerminateDISyncInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TestDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TestDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TestNetworkConnectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TestNetworkConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TopTenElapsedTimeInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TopTenElapsedTimeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/TopTenErrorTimesInstanceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/TopTenErrorTimesInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UmountDirectoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UmountDirectoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateBaselineRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateBusinessRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateConnectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDIProjectConfigRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDIProjectConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDISyncTaskRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDISyncTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDataServiceApiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDataServiceApiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateDataSourceRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateFileRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
 	def set_AutoRerunTimes(self, AutoRerunTimes):  # Integer
 		self.add_body_params('AutoRerunTimes', AutoRerunTimes)
 	def get_CronExpress(self): # String
 		return self.get_body_params().get('CronExpress')
 
 	def set_CronExpress(self, CronExpress):  # String
 		self.add_body_params('CronExpress', CronExpress)
+	def get_IgnoreParentSkipRunningProperty(self): # Boolean
+		return self.get_body_params().get('IgnoreParentSkipRunningProperty')
+
+	def set_IgnoreParentSkipRunningProperty(self, IgnoreParentSkipRunningProperty):  # Boolean
+		self.add_body_params('IgnoreParentSkipRunningProperty', IgnoreParentSkipRunningProperty)
 	def get_EndEffectDate(self): # Long
 		return self.get_body_params().get('EndEffectDate')
 
 	def set_EndEffectDate(self, EndEffectDate):  # Long
 		self.add_body_params('EndEffectDate', EndEffectDate)
 	def get_FileName(self): # String
 		return self.get_body_params().get('FileName')
```

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateFolderRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateFolderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateIDEEventResultRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateIDEEventResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCategoryRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCollectionRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaCollectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableIntroWikiRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableIntroWikiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateMetaTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateNodeOwnerRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateNodeOwnerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateNodeRunModeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateNodeRunModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateQualityFollowerRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateQualityFollowerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateQualityRuleRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateQualityRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateRemindRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateRemindRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableAddColumnRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableAddColumnRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableLevelRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableLevelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableModelInfoRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableModelInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateTableThemeRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateTableThemeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateUdfFileRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateUdfFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/aliyunsdkdataworks_public/request/v20200518/UpdateWorkbenchEventResultRequest.py` & `aliyun-python-sdk-dataworks-public-4.2.8/aliyunsdkdataworks_public/request/v20200518/UpdateWorkbenchEventResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dataworks-public-4.2.7/setup.py` & `aliyun-python-sdk-dataworks-public-4.2.8/setup.py`

 * *Files identical despite different names*

