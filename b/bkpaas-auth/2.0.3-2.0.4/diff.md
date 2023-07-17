# Comparing `tmp/bkpaas-auth-2.0.3.tar.gz` & `tmp/bkpaas-auth-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkpaas-auth-2.0.3.tar", max compression
+gzip compressed data, was "dist/bkpaas-auth-2.0.4.tar", last modified: Mon Jul 17 07:15:54 2023, max compression
```

## Comparing `bkpaas-auth-2.0.3.tar` & `bkpaas-auth-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,31 @@
--rw-r--r--   0        0        0     5197 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/README.md
--rw-r--r--   0        0        0     1012 2023-04-14 03:10:40.138154 bkpaas-auth-2.0.3/bkpaas_auth/__init__.py
--rw-r--r--   0        0        0      191 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/apps.py
--rw-r--r--   0        0        0     8196 2023-04-14 03:10:40.138154 bkpaas-auth-2.0.3/bkpaas_auth/backends.py
--rw-r--r--   0        0        0     2526 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/conf.py
--rw-r--r--   0        0        0        0 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/__init__.py
--rw-r--r--   0        0        0      206 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/constants.py
--rw-r--r--   0        0        0     2302 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/encoder.py
--rw-r--r--   0        0        0      339 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/exceptions.py
--rw-r--r--   0        0        0     2167 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/http.py
--rw-r--r--   0        0        0     1173 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/plugins.py
--rw-r--r--   0        0        0     3134 2023-04-13 09:36:50.200528 bkpaas-auth-2.0.3/bkpaas_auth/core/services.py
--rw-r--r--   0        0        0     3820 2023-04-14 03:10:40.138154 bkpaas-auth-2.0.3/bkpaas_auth/core/token.py
--rw-r--r--   0        0        0     2493 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/user_info.py
--rw-r--r--   0        0        0      641 2022-11-07 11:27:06.280321 bkpaas-auth-2.0.3/bkpaas_auth/core/utils.py
--rw-r--r--   0        0        0     3548 2022-11-07 11:27:06.284320 bkpaas-auth-2.0.3/bkpaas_auth/middlewares.py
--rw-r--r--   0        0        0     3368 2022-11-07 11:27:06.284320 bkpaas-auth-2.0.3/bkpaas_auth/models.py
--rw-r--r--   0        0        0     1263 2022-11-07 11:27:06.284320 bkpaas-auth-2.0.3/bkpaas_auth/monkey.py
--rw-r--r--   0        0        0      939 2023-04-14 03:10:40.138154 bkpaas-auth-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     6058 2023-04-14 03:11:12.075268 bkpaas-auth-2.0.3/setup.py
--rw-r--r--   0        0        0     5927 2023-04-14 03:11:12.075910 bkpaas-auth-2.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/constants.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/http.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/user_info.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/services.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/core/token.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-17 04:21:57.000000 bkpaas-auth-2.0.4/bkpaas_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/conf.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/apps.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-07-17 04:18:55.000000 bkpaas-auth-2.0.4/bkpaas_auth/backends.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/models.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/monkey.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/bkpaas_auth/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 04:21:21.000000 bkpaas-auth-2.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-17 04:15:47.000000 bkpaas-auth-2.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      313 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/bkpaas_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-17 07:15:54.000000 bkpaas-auth-2.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-17 07:15:47.000000 bkpaas-auth-2.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bkpaas-auth-2.0.3/README.md` & `bkpaas-auth-2.0.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,180 @@
-# bkpaas-auth
+
+bkpaas-auth
+===========
 
 蓝鲸 PaaS 平台内部服务使用的用户鉴权模块。
 
-## 版本历史
+版本历史
+--------
+
+详见 ``CHANGES.md``\ 。
+
+开发指南
+--------
+
+发布包
+^^^^^^
 
-详见 `CHANGES.md`。
 
-## 开发指南
+* 在 ``bkpaas_auth/__init__.py``  文件中更新 ``__version__``
+* 在 ``setup.py`` 文件中更新 ``version``
+* 在 ``pyproject.toml`` 中更新 ``version``
+* 在 ``CHANGES.md`` 中添加对应的版本日志
+* 执行 ``poetry build`` 命令在 dist 目录下生成当前版本的包。然后执行 ``twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}`` 将其上传到 pypi 服务器上。
 
-### 发布包
+关于 setup.py
+^^^^^^^^^^^^^
 
-- 在 `bkpaas_auth/__init__.py`  文件中更新 `__version__`
-- 在 `setup.py` 文件中更新 `version`
-- 在 `pyproject.toml` 中更新 `version`
-- 在 `CHANGES.md` 中添加对应的版本日志
-- 执行 `poetry build` 命令在 dist 目录下生成当前版本的包。然后执行 `twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}` 将其上传到 pypi 服务器上。
+虽然在 `PEP 517 <https://python-poetry.org/docs/pyproject/#poetry-and-pep-517>`_ 规范里，Python 包不再需要 ``setup.py`` 文件。但真正少了 ``setup.py`` 文件后，会发现有些功能就没法正常使用，比如 pip 的可编辑安装模式、tox 等（\ `相关文档 <https://github.com/python-poetry/poetry/issues/761>`_\ ）。所以我们仍然需要它。
 
-### 关于 setup.py
+为了避免维护重复的 ``pyproject.toml`` 和 ``setup.py`` 文件，我们使用了 `dephell <https://github.com/dephell/dephell>`_ 工具来自动生成 ``setup.py`` 文件。
 
-虽然在 [PEP 517](https://python-poetry.org/docs/pyproject/#poetry-and-pep-517) 规范里，Python 包不再需要 `setup.py` 文件。但真正少了 `setup.py` 文件后，会发现有些功能就没法正常使用，比如 pip 的可编辑安装模式、tox 等（[相关文档](https://github.com/python-poetry/poetry/issues/761)）。所以我们仍然需要它。
 
-为了避免维护重复的 `pyproject.toml` 和 `setup.py` 文件，我们使用了 [dephell](https://github.com/dephell/dephell) 工具来自动生成 `setup.py` 文件。
+* 安装 dephell
+* 在根目录执行 ``dephell deps convert --from pyproject.toml --to setup.py``
 
-- 安装 dephell
-- 在根目录执行 `dephell deps convert --from pyproject.toml --to setup.py`
+使用指南
+--------
 
-## 使用指南
-1. 更新 settings：
-```python
-INSTALLED_APPS = [
+
+#. 更新 settings：
+   ```python
+   INSTALLED_APPS = [
     ...
     'bkpaas_auth',
     ...
-]
+   ]
 
 MIDDLEWARE = [
     ...
     'bkpaas_auth.middlewares.CookieLoginMiddleware',
     ...
 ]
 
 AUTHENTICATION_BACKENDS = [
-    # [推荐] 使用内置的虚拟用户类型，不依赖于数据库表.
-    'bkpaas_auth.backends.UniversalAuthBackend',
-    # 如果项目需要保留使用数据库表的方式来设计用户模型, 则需要使用 DjangoAuthUserCompatibleBackend
-    # 'bkpaas_auth.backends.DjangoAuthUserCompatibleBackend',
+
+.. code-block::
+
+   # [推荐] 使用内置的虚拟用户类型，不依赖于数据库表.
+   'bkpaas_auth.backends.UniversalAuthBackend',
+   # 如果项目需要保留使用数据库表的方式来设计用户模型, 则需要使用 DjangoAuthUserCompatibleBackend
+   # 'bkpaas_auth.backends.DjangoAuthUserCompatibleBackend',
+
 ]
 
-# 使用 bkpaas_auth 内置的基于内存的用户模型
-# 如果项目需要保留使用数据库表的方式来设计用户模型, 可阅读 「关于AUTH_USER_MODEL」的部分说明
+使用 bkpaas_auth 内置的基于内存的用户模型
+=========================================
+
+如果项目需要保留使用数据库表的方式来设计用户模型, 可阅读 「关于AUTH_USER_MODEL」的部分说明
+==========================================================================================
+
 AUTH_USER_MODEL = 'bkpaas_auth.User'
 
-# 用户登录态认证类型
+用户登录态认证类型
+==================
+
 BKAUTH_BACKEND_TYPE = "bk_token" # 可选值：bk_token/bk_ticket
-# 验证用户登录态的 API，如 蓝鲸统一登录校验登录态的 API
+
+验证用户登录态的 API，如 蓝鲸统一登录校验登录态的 API
+=====================================================
+
 BKAUTH_USER_COOKIE_VERIFY_URL = "http://bk-login-web/api/v3/is_login/"
 
-# [可选]`BKAUTH_DEFAULT_PROVIDER_TYPE` 的值用于 JWT 校验时获取默认的用户认证类型。
+[可选]\ ``BKAUTH_DEFAULT_PROVIDER_TYPE`` 的值用于 JWT 校验时获取默认的用户认证类型。
+======================================================================================
+
 BKAUTH_DEFAULT_PROVIDER_TYPE = 'RTX'  # 可选值：RTX/UIN/BK，详见 ProviderType
-```
 
-2. 在 app config 中进行 patch：
+.. code-block::
+
+
+   2. 在 app config 中进行 patch：
+
+   配置登录模块的 apps.py
+
+   ```python
+   from bkpaas_auth.backends import DjangoAuthUserCompatibleBackend
+   from bkpaas_auth.models import User
+   from django.apps import AppConfig
+
+
+   class MyAppConfig(AppConfig):
+       name = 'my_app'
 
-配置登录模块的 apps.py
+       def ready(self):
+           from bkpaas_auth.monkey import patch_middleware_get_user
 
-```python
-from bkpaas_auth.backends import DjangoAuthUserCompatibleBackend
-from bkpaas_auth.models import User
-from django.apps import AppConfig
+           patch_middleware_get_user()
 
+更新 ``__init__.py``\ ，配置 default_app_config
 
-class MyAppConfig(AppConfig):
-    name = 'my_app'
+.. code-block::
 
-    def ready(self):
-        from bkpaas_auth.monkey import patch_middleware_get_user
+   default_app_config = 'xxx.apps.MyAppConfig'
 
-        patch_middleware_get_user()
-```
 
-更新 `__init__.py`，配置 default_app_config
-```
-default_app_config = 'xxx.apps.MyAppConfig'
-```
+#. 配置日志（可选）
+   在 django settings 的 LOGGING 中，为 sdk 配置 logger，如
 
-3. 配置日志（可选）
-在 django settings 的 LOGGING 中，为 sdk 配置 logger，如
+.. code-block:: python
 
-```python
-LOGGING = {
-    "handlers": {
-        "root": {
-            ...
-        },
-    },
-    "loggers": {
-        "bkpaas_auth": {
-            "handlers": ["root"],
-            "level": "WARNING",
-            "propagate": True,
-        },
-    },
-}
-```
+   LOGGING = {
+       "handlers": {
+           "root": {
+               ...
+           },
+       },
+       "loggers": {
+           "bkpaas_auth": {
+               "handlers": ["root"],
+               "level": "WARNING",
+               "propagate": True,
+           },
+       },
+   }
 
-### 关于 AUTH_USER_MODEL
+关于 AUTH_USER_MODEL
+^^^^^^^^^^^^^^^^^^^^
 
-bkpaas-auth 内置的基于内存的不依赖于数据库表的用户模型, 如果需要复用原有的用户模型, 则需要使用 `DjangoAuthUserCompatibleBackend` 作为用户校验后端.
+bkpaas-auth 内置的基于内存的不依赖于数据库表的用户模型, 如果需要复用原有的用户模型, 则需要使用 ``DjangoAuthUserCompatibleBackend`` 作为用户校验后端.
 
-在默认情况下, `DjangoAuthUserCompatibleBackend` 会从 bkpaas-auth 获取到当前登录的用户信息, 并会根据用户信息尝试创建一个基于数据库的用户模型.
-如果你有以下诉求, 则应当继承 `DjangoAuthUserCompatibleBackend`, 自行实现具体的业务逻辑:
+在默认情况下, ``DjangoAuthUserCompatibleBackend`` 会从 bkpaas-auth 获取到当前登录的用户信息, 并会根据用户信息尝试创建一个基于数据库的用户模型.
+如果你有以下诉求, 则应当继承 ``DjangoAuthUserCompatibleBackend``\ , 自行实现具体的业务逻辑:
 
-1. 不希望自动创建基于数据库的用户模型:
-```python
 
+#. 不希望自动创建基于数据库的用户模型:
+   ```python
 
 class YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):
     create_unknown_user = False
-```
 
-2. 用户模型有与 django `auth.User` 不兼容的字段或其他需要初始化的字段:
-```python
+.. code-block::
 
-class YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):
-    def configure_user(self, db_user, bk_user: User):
-        """
-        Configure a user after creation and return the updated user.
-        """
-        ...
-        return db_user
-```
 
-#### 和 [apigw-manager](../apigw-manager) 集成
+   2. 用户模型有与 django `auth.User` 不兼容的字段或其他需要初始化的字段:
+   ```python
+
+   class YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):
+       def configure_user(self, db_user, bk_user: User):
+           """
+           Configure a user after creation and return the updated user.
+           """
+           ...
+           return db_user
+
+和 `apigw-manager <../apigw-manager>`_ 集成
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 该 SDK 可以和 apigw-manager 集成，完成网关 JWT 的校验，在 settings 中配置：
-```python
-INSTALLED_APPS += ["apigw_manager.apigw"]
-AUTHENTICATION_BACKENDS += ["bkpaas_auth.backends.APIGatewayAuthBackend"]
-MIDDLEWARE += [
-    "apigw_manager.apigw.authentication.ApiGatewayJWTGenericMiddleware",  # JWT 认证
-    "apigw_manager.apigw.authentication.ApiGatewayJWTAppMiddleware",  # JWT 透传的应用信息
-    "apigw_manager.apigw.authentication.ApiGatewayJWTUserMiddleware",  # JWT 透传的用户信息
-]
-```
 
-设置之后，通过 JWT 透传的用户态会验证后，会写入到 `request.user` 中。注意，配置了不认证用户的网关资源透传的请求，会生成一个有对应用户名的匿名用户对象（`is_authenticated` 为 `False`）。
+.. code-block:: python
+
+   INSTALLED_APPS += ["apigw_manager.apigw"]
+   AUTHENTICATION_BACKENDS += ["bkpaas_auth.backends.APIGatewayAuthBackend"]
+   MIDDLEWARE += [
+       "apigw_manager.apigw.authentication.ApiGatewayJWTGenericMiddleware",  # JWT 认证
+       "apigw_manager.apigw.authentication.ApiGatewayJWTAppMiddleware",  # JWT 透传的应用信息
+       "apigw_manager.apigw.authentication.ApiGatewayJWTUserMiddleware",  # JWT 透传的用户信息
+   ]
+
+设置之后，通过 JWT 透传的用户态会验证后，会写入到 ``request.user`` 中。注意，配置了不认证用户的网关资源透传的请求，会生成一个有对应用户名的匿名用户对象（\ ``is_authenticated`` 为 ``False``\ ）。
```

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/__init__.py` & `bkpaas-auth-2.0.4/bkpaas_auth/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 
 def get_user_by_user_id(user_id: str, username_only: bool = True):
     """Get a user object from given user_id"""
     from bkpaas_auth.core.constants import ProviderType
     from bkpaas_auth.core.encoder import user_id_encoder
     from bkpaas_auth.core.services import get_bk_user_info, get_rtx_user_info
```

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/backends.py` & `bkpaas-auth-2.0.4/bkpaas_auth/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         """
         default_admin_superusers = getattr(settings, 'DEFAULT_ADMIN_SUPERUSERS', [])
         if db_user.username in default_admin_superusers:
             db_user.is_active = True
             db_user.is_staff = True
             db_user.is_superuser = True
 
-        db_user.email = bk_user.email
+        db_user.email = bk_user.email or ""
         db_user.save(update_fields=["is_active", "is_staff", "is_superuser", "email"])
         return db_user
 
 
 class APIGatewayAuthBackend:
     """This backend is to be used in conjunction with the ``ApiGatewayJWTUserMiddleware``
     found in the middleware module of ``apigw_manager`` package.
```

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/conf.py` & `bkpaas-auth-2.0.4/bkpaas_auth/conf.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/encoder.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/encoder.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/http.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/http.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/plugins.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/plugins.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/services.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/services.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/token.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/token.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/user_info.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/user_info.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/core/utils.py` & `bkpaas-auth-2.0.4/bkpaas_auth/core/utils.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/middlewares.py` & `bkpaas-auth-2.0.4/bkpaas_auth/middlewares.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/models.py` & `bkpaas-auth-2.0.4/bkpaas_auth/models.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/bkpaas_auth/monkey.py` & `bkpaas-auth-2.0.4/bkpaas_auth/monkey.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.3/pyproject.toml` & `bkpaas-auth-2.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bkpaas-auth"
-version = "2.0.3"
+version = "2.0.4"
 description = "User authentication django app for blueking internal projects"
 license = "Apach License 2.0"
 readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.6,<4.0"
```

