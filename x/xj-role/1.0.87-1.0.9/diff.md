# Comparing `tmp/xj_role-1.0.87.tar.gz` & `tmp/xj_role-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_role-1.0.87.tar", last modified: Mon Jul 17 07:06:34 2023, max compression
+gzip compressed data, was "dist\xj_role-1.0.9.tar", last modified: Thu Sep 15 05:32:40 2022, max compression
```

## Comparing `xj_role-1.0.87.tar` & `xj_role-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/
--rw-rw-rw-   0        0        0      354 2023-07-17 07:06:34.000000 xj_role-1.0.87/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_role-1.0.87/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 07:06:34.000000 xj_role-1.0.87/setup.cfg
--rw-rw-rw-   0        0        0     1956 2023-07-17 06:57:17.000000 xj_role-1.0.87/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/
--rw-rw-rw-   0        0        0        0 2023-06-28 10:29:35.000000 xj_role-1.0.87/xj_role/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-07-05 02:52:04.000000 xj_role-1.0.87/xj_role/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.87/xj_role/apis/__init__.py
--rw-rw-rw-   0        0        0     7001 2023-07-17 02:56:30.000000 xj_role-1.0.87/xj_role/apis/group_api.py
--rw-rw-rw-   0        0        0     3879 2023-07-06 06:27:04.000000 xj_role-1.0.87/xj_role/apis/permission_api.py
--rw-rw-rw-   0        0        0     4513 2023-07-06 06:26:38.000000 xj_role-1.0.87/xj_role/apis/role_api.py
--rw-rw-rw-   0        0        0     3638 2023-07-12 11:01:13.000000 xj_role-1.0.87/xj_role/apis/role_menu_apis.py
--rw-rw-rw-   0        0        0     2162 2023-06-30 01:35:19.000000 xj_role-1.0.87/xj_role/apis/role_system_apis.py
--rw-rw-rw-   0        0        0      202 2022-09-06 06:05:16.000000 xj_role-1.0.87/xj_role/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/library/
--rw-rw-rw-   0        0        0      149 2023-06-15 03:18:24.000000 xj_role-1.0.87/xj_role/library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/library/api_interrupter/
--rw-rw-rw-   0        0        0      158 2023-07-05 02:30:03.000000 xj_role-1.0.87/xj_role/library/api_interrupter/__init__.py
--rw-rw-rw-   0        0        0     4491 2023-07-17 06:52:05.000000 xj_role-1.0.87/xj_role/library/api_interrupter/api_interrupter.py
--rw-rw-rw-   0        0        0      973 2023-07-06 06:13:34.000000 xj_role-1.0.87/xj_role/library/api_interrupter/api_interrupter_middleware.py
--rw-rw-rw-   0        0        0     4659 2023-06-29 06:33:09.000000 xj_role-1.0.87/xj_role/library/get_system_apis.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/library/permission_execute/
--rw-rw-rw-   0        0        0      238 2023-06-28 10:26:56.000000 xj_role-1.0.87/xj_role/library/permission_execute/__init__.py
--rw-rw-rw-   0        0        0      292 2023-06-28 08:42:31.000000 xj_role-1.0.87/xj_role/library/permission_execute/permission_base.py
--rw-rw-rw-   0        0        0      280 2023-06-28 10:21:54.000000 xj_role-1.0.87/xj_role/library/permission_execute/permission_executor.py
--rw-rw-rw-   0        0        0     9953 2023-07-17 02:49:32.000000 xj_role-1.0.87/xj_role/models.py
--rw-rw-rw-   0        0        0     1091 2023-04-18 01:47:55.000000 xj_role-1.0.87/xj_role/service_register.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.87/xj_role/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/services/abstract/
--rw-rw-rw-   0        0        0      168 2022-11-15 00:46:06.000000 xj_role-1.0.87/xj_role/services/abstract/__init__.py
--rw-rw-rw-   0        0        0      767 2023-06-15 03:13:45.000000 xj_role-1.0.87/xj_role/services/abstract/observer_subject.py
--rw-rw-rw-   0        0        0     6264 2022-10-27 09:43:36.000000 xj_role-1.0.87/xj_role/services/auto_permission_service.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/services/observer/
--rw-rw-rw-   0        0        0      321 2023-05-11 03:10:56.000000 xj_role-1.0.87/xj_role/services/observer/__init__.py
--rw-rw-rw-   0        0        0    17658 2023-07-07 01:42:39.000000 xj_role-1.0.87/xj_role/services/permission_service.py
--rw-rw-rw-   0        0        0     6454 2023-07-05 08:13:19.000000 xj_role-1.0.87/xj_role/services/role_apis_services.py
--rw-rw-rw-   0        0        0    10593 2023-07-12 11:01:55.000000 xj_role-1.0.87/xj_role/services/role_nemus_services.py
--rw-rw-rw-   0        0        0    22658 2023-07-11 08:28:47.000000 xj_role-1.0.87/xj_role/services/role_service.py
--rw-rw-rw-   0        0        0    12667 2022-10-08 03:39:06.000000 xj_role-1.0.87/xj_role/services/user_group_service [backup].py
--rw-rw-rw-   0        0        0    22845 2023-07-17 03:01:26.000000 xj_role-1.0.87/xj_role/services/user_group_service.py
--rw-rw-rw-   0        0        0     3634 2023-06-30 01:15:41.000000 xj_role-1.0.87/xj_role/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.87/xj_role/utils/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-04 07:07:56.000000 xj_role-1.0.87/xj_role/utils/api_interrupter_wrapper.py
--rw-rw-rw-   0        0        0     1082 2023-06-29 09:26:10.000000 xj_role-1.0.87/xj_role/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     4618 2023-07-05 03:21:30.000000 xj_role-1.0.87/xj_role/utils/custom_response.py
--rw-rw-rw-   0        0        0    39226 2023-07-17 06:47:39.000000 xj_role-1.0.87/xj_role/utils/custom_tool.py
--rw-rw-rw-   0        0        0      958 2022-10-25 06:03:08.000000 xj_role-1.0.87/xj_role/utils/j_dict.py
--rw-rw-rw-   0        0        0    10114 2023-07-03 06:01:14.000000 xj_role-1.0.87/xj_role/utils/j_recur.py
--rw-rw-rw-   0        0        0      660 2022-11-29 06:32:59.000000 xj_role-1.0.87/xj_role/utils/join_list.py
--rw-rw-rw-   0        0        0     2691 2023-07-05 01:26:58.000000 xj_role-1.0.87/xj_role/utils/omnipotence_wrapper.py
--rw-rw-rw-   0        0        0     5867 2023-07-17 01:50:28.000000 xj_role-1.0.87/xj_role/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_role-1.0.87/xj_role/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role.egg-info/
--rw-rw-rw-   0        0        0      354 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-17 07:06:34.000000 xj_role-1.0.87/xj_role.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/
+-rw-rw-rw-   0        0        0      581 2022-09-15 05:32:40.000000 xj_role-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_role-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-15 05:32:40.000000 xj_role-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2119 2022-09-15 05:32:08.000000 xj_role-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/__init__.py
+-rw-rw-rw-   0        0        0     1916 2022-09-07 02:09:37.000000 xj_role-1.0.9/xj_role/admin.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/apis/__init__.py
+-rw-rw-rw-   0        0        0     3133 2022-09-09 01:10:05.000000 xj_role-1.0.9/xj_role/apis/group_api.py
+-rw-rw-rw-   0        0        0     2506 2022-09-07 02:01:28.000000 xj_role-1.0.9/xj_role/apis/permission_api.py
+-rw-rw-rw-   0        0        0      756 2022-09-08 09:00:53.000000 xj_role-1.0.9/xj_role/apis/role_api.py
+-rw-rw-rw-   0        0        0      202 2022-09-06 06:05:16.000000 xj_role-1.0.9/xj_role/apps.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/migrations/
+-rw-rw-rw-   0        0        0      546 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1684 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0002_baseinfo.py
+-rw-rw-rw-   0        0        0     1373 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0003_auto_20210511_1250.py
+-rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1450.py
+-rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1707.py
+-rw-rw-rw-   0        0        0     1469 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0005_auth.py
+-rw-rw-rw-   0        0        0      287 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0005_merge_0004_auto_20220101_1450_0004_auto_20220101_1707.py
+-rw-rw-rw-   0        0        0      658 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0006_auto_20220205_1300.py
+-rw-rw-rw-   0        0        0      322 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0007_merge_20220205_1325.py
+-rw-rw-rw-   0        0        0     1071 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0008_auto_20220206_2238.py
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6808 2022-09-07 02:09:37.000000 xj_role-1.0.9/xj_role/models.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/services/__init__.py
+-rw-rw-rw-   0        0        0     7475 2022-09-13 07:53:08.000000 xj_role-1.0.9/xj_role/services/group_service.py
+-rw-rw-rw-   0        0        0     6099 2022-09-15 05:24:28.000000 xj_role-1.0.9/xj_role/services/permission_service.py
+-rw-rw-rw-   0        0        0     3619 2022-09-13 01:51:54.000000 xj_role-1.0.9/xj_role/services/role_service.py
+-rw-rw-rw-   0        0        0     1340 2022-09-09 05:49:03.000000 xj_role-1.0.9/xj_role/urls.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/custom_response.py
+-rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/j_dict.py
+-rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/join_list.py
+-rw-rw-rw-   0        0        0     7024 2022-09-02 08:00:24.000000 xj_role-1.0.9/xj_role/utils/model_handle.py
+-rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/validator.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/
+-rw-rw-rw-   0        0        0      581 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1168 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/top_level.txt
```

### Comparing `xj_role-1.0.87/setup.py` & `xj_role-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,32 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_role',  # 模块名称
-    version='1.0.87',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='权限模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     # author='sieyoo',
     # author_email='sieyoo@163.com',
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
     license="apache 3.0",
 
-    install_requires=[]
+    install_requires=[
+    #     'requests',
+    #     'django>=3.2.0,<3.3.0',
+    #     'mysqlclient',
+    #     'djangorestframework',
+    #     'PyJWT',
+    #     'redis',
+    ]
 )
 """
 name : 打包后包的文件名
 version : 版本号
 author : 作者
 author_email : 作者的邮箱
 py_modules : 要打包的.py文件
```

### Comparing `xj_role-1.0.87/xj_role/services/user_group_service [backup].py` & `xj_role-1.0.9/xj_role/services/group_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,78 +4,63 @@
 @author: 孙楷炎
 @Email: sky4834@163.com
 @synopsis: 用户组（部门服务）
 @created_time: 2022/9/5 11:33
 """
 
 from django.core.paginator import Paginator
-from django.db.models import F
-from django.forms.models import model_to_dict
-from django.db.models import Q
+
 from xj_role.services.role_service import RoleService
-from xj_user.models import BaseInfo
 from xj_user.services.user_service import UserService
-from xj_user.services.user_detail_info_service import DetailInfoService
-from ..models import UserToGroup, RoleUserGroup, UserToRole
+from ..models import UserToGroup, RoleUserGroup
 from ..utils.model_handle import format_params_handle, parse_json
 
 
 # 用户组 树状数据返回
 class GroupTreeService(object):
     @staticmethod
-    # 这个代码的复杂度不高吗？递归是个for循环，循环里是个递归，继续for，每个树枝都会循环一次列表
-    def get_tree(data_list, parent_group):
+    def getTree(data_list, parent_group):
         tree = []
         for item in data_list:
             if str(item['parent_group_id']) == str(parent_group):
+                id(item)
                 item['name'] = item['group_name']
                 item['is_group'] = True
-                children = GroupTreeService.get_tree(data_list, item['id'])
+                children = GroupTreeService.getTree(data_list, item['id'])
                 if children:
                     item['children'] = children
                 tree.append(item)
-
         return tree
 
     @staticmethod
-    def get_trees(data_list, parent_group):
+    def getTrees(data_list, parent_group):
         tree = []
-        # 如果他不是树根 则搜索具体树枝生成的树
         if parent_group != 0:
             base_node = RoleUserGroup.objects.filter(id=parent_group).to_json()
             for item in data_list:
                 if str(item['parent_group_id']) == str(parent_group):
-                    item['name'] = item['group_name']
-                    item['children'] = GroupTreeService.get_tree(data_list, item['id'])
+                    item['children'] = GroupTreeService.getTree(data_list, item['id'])
                     tree.append(item)
             base_node[0]['children'] = tree
             return base_node[0]
-        # 如果是树根
         else:
             # 默认不需要搜索
             for item in data_list:
-                if str(item.get('parent_group_id', None)) != str(parent_group):
+                if not str(item['parent_group_id']) == str(parent_group):
                     continue
-                child = GroupTreeService.get_tree(data_list, item['id'])
+                child = GroupTreeService.getTree(data_list, item['id'])
                 if child:
-                    item['name'] = item['group_name']
                     item['children'] = child
                     tree.append(item)
-                else:
-                    item['name'] = item['group_name']
-                    item['children'] = []
-                    tree.append(item)
         return tree
 
     @staticmethod
-    def get_user_group_tree(group_id=0):
-        """获取用户所在组树"""
-        data_list = list(RoleUserGroup.objects.filter().values())
-        print("> group_tree:", group_id, data_list)
-        group_tree = GroupTreeService.get_trees(data_list, group_id)
+    def group_tree(group_id=0):
+        data_list = RoleUserGroup.objects.filter().to_json()
+        group_tree = GroupTreeService.getTrees(data_list, group_id)
         return group_tree, None
 
 
 # 用户组CURD服务
 class GroupService(object):
     @staticmethod
     def get_user_from_group(group_id):
@@ -87,15 +72,15 @@
             user_list = [i['user_id'] for i in user_list]
         return user_list, None
 
     @staticmethod
     def group_tree_role(params):
         # 分组角色树
         group_id = params.get("group_id", 0)
-        tree_data, err = GroupTreeService.get_user_group_tree(group_id)
+        tree_data, err = GroupTreeService.group_tree(group_id)
         if err:
             return None, err
         role_list, err = RoleService.get_role_list({}, None)
         role_dict = {}
         for role in role_list:
             index = str(role['user_group_id'])
             if index not in role_dict.keys():
@@ -115,24 +100,23 @@
 
         return parse_tree(parse_json(tree_data), 0), None
 
     @staticmethod
     def group_tree_user(params):
         # 分组用户树
         group_id = params.get("group_id", 0)
-        tree_data, err = GroupTreeService.get_user_group_tree(group_id)
+        tree_data, err = GroupTreeService.group_tree(group_id)
         if err:
             return None, err
         user_group_obj = UserToGroup.objects
         if group_id:
             user_group_set = user_group_obj.filter(user_group_id=group_id)
         else:
             user_group_set = user_group_obj.all()
-        user_group_dict = {str(item["user_id"]): str(item['user_group_id']) for item in
-                           list(user_group_set.values())} if user_group_set else {}
+        user_group_dict = {str(item["user_id"]): str(item['user_group_id']) for item in list(user_group_set.values())} if user_group_set else {}
         user_list, err = UserService.user_list({"id__in": user_group_dict.keys()}, None)
         group_user_dict = {}
         for user in user_list:
             index = user_group_dict.get(str(user['id']), None)
             if not index:
                 continue
             if index not in group_user_dict.keys():
@@ -149,92 +133,14 @@
                 if str(item['id']) in group_user_dict.keys():
                     item['children'].extend(group_user_dict[str(item['id'])])
             return tree
 
         return parse_tree(parse_json(tree_data), 0), None
 
     @staticmethod
-    def group_user_list(group_id, page, size):
-
-        user_set = UserToGroup.objects.filter(user_group=group_id).annotate(
-            user_group_value=F("user_group__group_name"))
-        user_set = user_set.values(
-            "user_id",
-            "user_group",
-        )
-        params = {
-            "page": page,
-            "size": size
-        }
-        # TODO 这样的逻辑 返回的用户组列表 无法显示全部 。解决方案一：在详情的时候处理用户所在的组 方案二：通过聚合表 拿到用户的组
-        # user_dict = {}
-        # for it in user_set:
-        #     if str(it['user_id']) not in user_dict:
-        #         user_dict[str(it['user_id'])] = []
-        #     user_dict[str(it['user_id'])].append(it['user_group'])
-        user_id_list = [it['user_id'] for it in user_set]
-        user_serv, err = UserService.user_list(params, allow_user_list=user_id_list)
-        if err:
-            return None, err
-        # for it in user_list:
-        #     if str(it['user_id']) in user_dict:
-        #         it['user_group_list'] = user_dict[str(it['user_id'])]
-        return user_serv, None
-
-    @staticmethod
-    def group_user_detail(user_id):
-        user_serv, err = DetailInfoService.get_detail(user_id)
-        user_group_serv = UserToGroup.objects.filter(user_id=user_id).values("user_id", 'user_group_id')
-        user_group_dict = {item['user_group_id'] for item in user_group_serv}
-        user_role_serv = UserToRole.objects.filter(user_id=user_id).values("user_id", 'role_id')
-        user_role_dict = {item['role_id'] for item in user_role_serv}
-        user_serv['user_group_list'] = list(user_group_dict)
-        user_serv['user_role_list'] = list(user_role_dict)
-        if err:
-            return None, err
-        return user_serv, None
-
-    @staticmethod
-    def group_user_add(params):
-        # 用户角色部门绑定
-        user_role_list = params.get('user_role_list', None)
-        user_group_list = params.get('user_group_list', None)
-        user_serv, err = UserService.user_add(params)
-        if err:
-            return None, err
-        if user_group_list:
-            GroupService.bind_user_group(user_serv['user_id'], user_group_list)
-
-        if user_role_list:
-            RoleService.bind_user_role(user_serv['user_id'], user_role_list)
-        return user_serv, None
-
-    @staticmethod
-    def group_user_edit(params):
-        # 用户角色部门绑定
-        user_role_list = params.get('user_role_list', None)
-        user_group_list = params.get('user_group_list', None)
-        user_serv, err = UserService.user_edit(params)
-        if err:
-            return None, err
-        if user_group_list:
-            GroupService.bind_user_group(user_serv['user_id'], user_group_list)
-
-        if user_role_list:
-            RoleService.bind_user_role(user_serv['user_id'], user_role_list)
-        return user_serv, None
-
-    @staticmethod
-    def group_user_delete(params):
-        user_serv, err = UserService.user_delete(params)
-        if err:
-            return None, err
-        return None, None
-
-    @staticmethod
     def user_bind_group(user_id, group_id):
         # 用户绑定部门
         if not user_id or not group_id:
             return None, "参数错误，user_id, group_id 必传"
         try:
             UserToGroup.objects.get_or_create(
                 {"user_id": user_id, "group_id": group_id},
@@ -242,76 +148,48 @@
                 group_id=group_id,
             )
             return None, None
         except Exception as e:
             return None, str(e)
 
     @staticmethod
-    def bind_user_group(user_id, group_list):
-        list = group_list.split(',')
-        UserToGroup.objects.filter(user_id=user_id).delete()
-        try:
-            for i in list:
-                data = {
-                    "user_id": user_id,
-                    "user_group_id": i
-                }
-                UserToGroup.objects.create(**data)
-            return None, None
-        except Exception as e:
-            return None, str(e)
-
-    @staticmethod
     def group_list(params):
         params = format_params_handle(
             param_dict=params,
             filter_filed_list=["page", "size", "group", "group_name", "parent_group_id"],
             alias_dict={"group_name": "group_name__contains"}
         )
         page = params.pop("page", 1)
         size = params.pop("size", 20)
-        group_set = RoleUserGroup.objects.filter(**params)
-        count = group_set.count()
-        group_list = group_set.values()
-        finish_set = list(Paginator(group_list, size).page(page))
-        return {"page": int(page), "size": int(size), "count": int(count), "list": finish_set}, None
+        group_set = RoleUserGroup.objects.filter(**params).values()
+        finish_set = list(Paginator(group_set, size).page(page))
+        return {"page": int(page), "size": int(size), "list": finish_set}, None
 
     @staticmethod
     def add_group(params):
-        params = format_params_handle(param_dict=params,
-                                      filter_filed_list=["group", "group_name", "parent_group_id", "description"])
+        params = format_params_handle(param_dict=params, filter_filed_list=["group", "group_name", "parent_group_id", "description"])
         if not params:
             return None, "参数不能为空"
-        res = RoleUserGroup.objects.filter(group=params.get("group")).exists()
-        if res:
-            return None, "组标签，必须唯一"
         instance = RoleUserGroup.objects.create(**params)
-        return None, None
+        return {"id": instance.id}, None
 
     @staticmethod
     def edit_group(params):
-        params = format_params_handle(param_dict=params,
-                                      filter_filed_list=["id", "group", "group_name", "parent_group_id", "description"])
+        params = format_params_handle(param_dict=params, filter_filed_list=["id", "group", "group_name", "parent_group_id", "description"])
         id = params.pop("id", None)
         if not id:
             return None, "ID 不可以为空"
         if not params:
             return None, "没有可以修改的字段"
-        res = RoleUserGroup.objects.filter(Q(group=params.get("group")), ~Q(id=id)).exists()
-        if res:
-            return None, "组标签，必须唯一"
         instance = RoleUserGroup.objects.filter(id=id)
         if params:
             instance.update(**params)
         return None, None
 
     @staticmethod
     def del_group(id):
         if not id:
             return None, "ID 不可以为空"
-        user_role_set = UserToGroup.objects.filter(user_group_id=id).exists()
-        if user_role_set:
-            return None, "该组织有绑定关系,无法删除"
         instance = RoleUserGroup.objects.filter(id=id)
         if instance:
             instance.delete()
         return None, None
```

### Comparing `xj_role-1.0.87/xj_role/utils/custom_authorization.py` & `xj_role-1.0.9/xj_role/utils/custom_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 # import jwt
 # from django.conf import settings
 from rest_framework import authentication
 # from apps.xj_user.models import BaseInfo
 from rest_framework import exceptions
-from xj_user.services.user_service import UserService
+from ..services.user_service import UserService
 
 
 class CustomAuthentication(authentication.BaseAuthentication):
     """用户认证"""
 
     def authenticate(self, request):
         # 验证是否已经登录，函数名必须为：authenticate
```

### Comparing `xj_role-1.0.87/xj_role/utils/validator.py` & `xj_role-1.0.9/xj_role/utils/validator.py`

 * *Files identical despite different names*

