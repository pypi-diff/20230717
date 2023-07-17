# Comparing `tmp/opsapp-0.0.24.tar.gz` & `tmp/opsapp-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\opsapp-0.0.24.tar", last modified: Mon Jul 17 08:46:12 2023, max compression
+gzip compressed data, was "dist\opsapp-0.0.25.tar", last modified: Mon Jul 17 09:03:55 2023, max compression
```

## Comparing `opsapp-0.0.24.tar` & `opsapp-0.0.25.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:12.000000 opsapp-0.0.24/
--rw-rw-rw-   0        0        0      254 2023-07-17 08:46:11.000000 opsapp-0.0.24/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/demo/
--rw-rw-rw-   0        0        0        0 2022-06-19 05:18:54.000000 opsapp-0.0.24/demo/__init__.py
--rw-rw-rw-   0        0        0     2212 2022-06-19 05:20:01.000000 opsapp-0.0.24/demo/app.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/
--rw-rw-rw-   0        0        0      115 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/
--rw-rw-rw-   0        0        0       40 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/
--rw-rw-rw-   0        0        0       25 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/aip/
--rw-rw-rw-   0        0        0      409 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/aip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/events/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/events/__init__.py
--rw-rw-rw-   0        0        0      708 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/events/events.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/logging/
--rw-rw-rw-   0        0        0      465 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/logging/__init__.py
--rw-rw-rw-   0        0        0     2569 2022-06-18 13:09:26.000000 opsapp-0.0.24/opsapp/app/core/logging/logging.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/middleware/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/middleware/__init__.py
--rw-rw-rw-   0        0        0      927 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/middleware/middleware.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/openapi/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/openapi/__init__.py
--rw-rw-rw-   0        0        0    14915 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/openapi/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/redis/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/redis/__init__.py
--rw-rw-rw-   0        0        0      582 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/redis/redis.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/response/
--rw-rw-rw-   0        0        0      776 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/response/BaseResponse.py
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/response/__init__.py
--rw-rw-rw-   0        0        0      889 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/response/http_error.py
--rw-rw-rw-   0        0        0      622 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/response/validation_error.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/router/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/router/__init__.py
--rw-rw-rw-   0        0        0      544 2023-07-17 08:31:54.000000 opsapp-0.0.24/opsapp/app/core/router/router.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/utils/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/utils/__init__.py
--rw-rw-rw-   0        0        0     1443 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/core/websocket/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/websocket/__init__.py
--rw-rw-rw-   0        0        0      490 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/core/websocket/websocket.py
--rw-rw-rw-   0        0        0     3888 2023-07-17 08:44:21.000000 opsapp-0.0.24/opsapp/app/main.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/models/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/models/__init__.py
--rw-rw-rw-   0        0        0       83 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/models/db.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/settings/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/settings/__init__.py
--rw-rw-rw-   0        0        0     2022 2023-07-17 08:45:02.000000 opsapp-0.0.24/opsapp/app/settings/config.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/app/swagger/
--rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/__init__.py
--rw-rw-rw-   0        0        0   930543 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/redoc.standalone.js
--rw-rw-rw-   0        0        0   930543 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/redoc.standalone.js.map
--rw-rw-rw-   0        0        0  1061872 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/swagger-ui-bundle.js
--rw-rw-rw-   0        0        0  1061872 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/swagger-ui-bundle.js.map
--rw-rw-rw-   0        0        0   143212 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/swagger-ui.css
--rw-rw-rw-   0        0        0   143212 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/app/swagger/swagger-ui.css.map
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/base/
--rw-rw-rw-   0        0        0       45 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/__init__.py
--rw-rw-rw-   0        0        0     1463 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/hook.py
--rw-rw-rw-   0        0        0     1995 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/logger.py
--rw-rw-rw-   0        0        0     9760 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/misc.py
--rw-rw-rw-   0        0        0     3110 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/path.py
--rw-rw-rw-   0        0        0     7269 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/progressbar.py
--rw-rw-rw-   0        0        0     5985 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/registry.py
--rw-rw-rw-   0        0        0     3011 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/base/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp/utils/
--rw-rw-rw-   0        0        0      291 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/utils/__init__.py
--rw-rw-rw-   0        0        0      399 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/utils/base64utils.py
--rw-rw-rw-   0        0        0     2768 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/utils/colors.py
--rw-rw-rw-   0        0        0     6132 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/utils/utils.py
--rw-rw-rw-   0        0        0     4329 2022-06-03 14:39:02.000000 opsapp-0.0.24/opsapp/utils/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/
--rw-rw-rw-   0        0        0      254 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1727 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 08:46:11.000000 opsapp-0.0.24/opsapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 08:46:12.000000 opsapp-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     1108 2022-12-01 14:48:28.000000 opsapp-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/
+-rw-rw-rw-   0        0        0      254 2023-07-17 09:03:55.000000 opsapp-0.0.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/demo/
+-rw-rw-rw-   0        0        0        0 2022-06-19 05:18:54.000000 opsapp-0.0.25/demo/__init__.py
+-rw-rw-rw-   0        0        0     2212 2022-06-19 05:20:01.000000 opsapp-0.0.25/demo/app.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/
+-rw-rw-rw-   0        0        0      115 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/
+-rw-rw-rw-   0        0        0       40 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/
+-rw-rw-rw-   0        0        0       25 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/aip/
+-rw-rw-rw-   0        0        0      409 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/aip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/events/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/events/__init__.py
+-rw-rw-rw-   0        0        0      708 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/events/events.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/logging/
+-rw-rw-rw-   0        0        0      465 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/logging/__init__.py
+-rw-rw-rw-   0        0        0     2569 2022-06-18 13:09:26.000000 opsapp-0.0.25/opsapp/app/core/logging/logging.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/middleware/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/middleware/__init__.py
+-rw-rw-rw-   0        0        0      927 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/middleware/middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/openapi/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/openapi/__init__.py
+-rw-rw-rw-   0        0        0    14915 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/openapi/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/redis/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/redis/__init__.py
+-rw-rw-rw-   0        0        0      582 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/redis/redis.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/response/
+-rw-rw-rw-   0        0        0      776 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/response/BaseResponse.py
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/response/__init__.py
+-rw-rw-rw-   0        0        0      889 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/response/http_error.py
+-rw-rw-rw-   0        0        0      622 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/response/validation_error.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/router/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/router/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-07-17 08:31:54.000000 opsapp-0.0.25/opsapp/app/core/router/router.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     1443 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/core/websocket/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/websocket/__init__.py
+-rw-rw-rw-   0        0        0      490 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/core/websocket/websocket.py
+-rw-rw-rw-   0        0        0     3883 2023-07-17 09:03:28.000000 opsapp-0.0.25/opsapp/app/main.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/models/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/models/__init__.py
+-rw-rw-rw-   0        0        0       83 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/models/db.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/settings/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/settings/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-07-17 09:00:48.000000 opsapp-0.0.25/opsapp/app/settings/config.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/app/swagger/
+-rw-rw-rw-   0        0        0        0 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/__init__.py
+-rw-rw-rw-   0        0        0   930543 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/redoc.standalone.js
+-rw-rw-rw-   0        0        0   930543 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/redoc.standalone.js.map
+-rw-rw-rw-   0        0        0  1061872 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/swagger-ui-bundle.js
+-rw-rw-rw-   0        0        0  1061872 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/swagger-ui-bundle.js.map
+-rw-rw-rw-   0        0        0   143212 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/swagger-ui.css
+-rw-rw-rw-   0        0        0   143212 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/app/swagger/swagger-ui.css.map
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/base/
+-rw-rw-rw-   0        0        0       45 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/__init__.py
+-rw-rw-rw-   0        0        0     1463 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/hook.py
+-rw-rw-rw-   0        0        0     1995 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/logger.py
+-rw-rw-rw-   0        0        0     9760 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/misc.py
+-rw-rw-rw-   0        0        0     3110 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/path.py
+-rw-rw-rw-   0        0        0     7269 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/progressbar.py
+-rw-rw-rw-   0        0        0     5985 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/registry.py
+-rw-rw-rw-   0        0        0     3011 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/base/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp/utils/
+-rw-rw-rw-   0        0        0      291 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      399 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/utils/base64utils.py
+-rw-rw-rw-   0        0        0     2768 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/utils/colors.py
+-rw-rw-rw-   0        0        0     6132 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/utils/utils.py
+-rw-rw-rw-   0        0        0     4329 2022-06-03 14:39:02.000000 opsapp-0.0.25/opsapp/utils/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp.egg-info/
+-rw-rw-rw-   0        0        0      254 2023-07-17 09:03:54.000000 opsapp-0.0.25/opsapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1727 2023-07-17 09:03:55.000000 opsapp-0.0.25/opsapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:03:54.000000 opsapp-0.0.25/opsapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 09:03:54.000000 opsapp-0.0.25/opsapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 09:03:54.000000 opsapp-0.0.25/opsapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:03:55.000000 opsapp-0.0.25/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2022-12-01 14:48:28.000000 opsapp-0.0.25/setup.py
```

### Comparing `opsapp-0.0.24/demo/app.py` & `opsapp-0.0.25/demo/app.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/events/events.py` & `opsapp-0.0.25/opsapp/app/core/events/events.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/logging/logging.py` & `opsapp-0.0.25/opsapp/app/core/logging/logging.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/middleware/middleware.py` & `opsapp-0.0.25/opsapp/app/core/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/openapi/converter.py` & `opsapp-0.0.25/opsapp/app/core/openapi/converter.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/redis/redis.py` & `opsapp-0.0.25/opsapp/app/core/redis/redis.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/response/BaseResponse.py` & `opsapp-0.0.25/opsapp/app/core/response/BaseResponse.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/response/http_error.py` & `opsapp-0.0.25/opsapp/app/core/response/http_error.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/response/validation_error.py` & `opsapp-0.0.25/opsapp/app/core/response/validation_error.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/router/router.py` & `opsapp-0.0.25/opsapp/app/core/router/router.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/core/utils/utils.py` & `opsapp-0.0.25/opsapp/app/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/main.py` & `opsapp-0.0.25/opsapp/app/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,41 @@
 )
 import json,yaml    
 from .core.openapi.converter import Converter   
 
 # 初始化应用
 application = FastAPI(title=config.PROJECT_NAME, version=config.VERSION, description=config.DESCRIPTION,docs_url=None, redoc_url=None)
 
-@application.get("/docs", include_in_schema=False)
+@application.get(f"/{config.DOCS}", include_in_schema=False)
 async def custom_swagger_ui_html():
-    if config.DOCS:
+    if config.DOCS == "True":
         return get_swagger_ui_html(
             openapi_url=application.openapi_url,
             title=application.title + " - Swagger UI",
             oauth2_redirect_url=application.swagger_ui_oauth2_redirect_url,
             swagger_js_url=f"/{config.SWAGGER}/swagger-ui-bundle.js",
             swagger_css_url=f"/{config.SWAGGER}/swagger-ui.css",
         )
-    return ""
 
 
 @application.get(application.swagger_ui_oauth2_redirect_url, include_in_schema=False)
 async def swagger_ui_redirect():
-    if config.DOCS:
+    if config.DOCS == "True":
         return get_swagger_ui_oauth2_redirect_html()
-    return ""
         
 
 
 @application.get("/redoc", include_in_schema=False)
 async def redoc_html():
-    if config.DOCS:
+    if config.DOCS == "True":
         return get_redoc_html(
             openapi_url=application.openapi_url,
             title=application.title + " - ReDoc",
             redoc_js_url=f"/{config.SWAGGER}/redoc.standalone.js",
         ) 
-    return ""
         
 # 注入
 def get_application() -> FastAPI:
     # Log
     application.state.log = LoggerFactory('log').logger
     # 添加事件
     application.add_event_handler("startup", create_start_app_handler(application))
```

### Comparing `opsapp-0.0.24/opsapp/app/settings/config.py` & `opsapp-0.0.25/opsapp/app/settings/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from ..models.db import outModels
 # -----------------------系统调试------------------------------------
 DEBUG = os.getenv('DEBUG', False)
 INTERCEPT = True
 
 # -----------------------项目信息------------------------------------
 API_PREFIX = "/aip"
-VERSION = "0.0.24"
+VERSION = "0.0.25"
 PROJECT_NAME = "API_UNIFORM_INTERFACE"
 DESCRIPTION = 'A simple uniform interface'
 MDDOC_URL = '/mddoc'
 OPENAPI_JSON = ''
-DOCS = True
+DOCS = "True"
 
 # -----------------------数据库配置-----------------------------------
 MYSQL_USER = os.getenv('MYSQL_USER', 'root')
 MYSQL_PASSWORD = os.getenv('MYSQL_PASSWORD', '123')
 MYSQL_HOST = os.getenv('MYSQL_HOST', 'localhost')
 MYSQL_PORT = os.getenv('MYSQL_PORT', 3306)
 MYSQL_DB = os.getenv('MYSQL_DB', 'saas')
```

### Comparing `opsapp-0.0.24/opsapp/app/swagger/redoc.standalone.js` & `opsapp-0.0.25/opsapp/app/swagger/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/swagger/redoc.standalone.js.map` & `opsapp-0.0.25/opsapp/app/swagger/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/swagger/swagger-ui-bundle.js` & `opsapp-0.0.25/opsapp/app/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/swagger/swagger-ui-bundle.js.map` & `opsapp-0.0.25/opsapp/app/swagger/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/swagger/swagger-ui.css` & `opsapp-0.0.25/opsapp/app/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/app/swagger/swagger-ui.css.map` & `opsapp-0.0.25/opsapp/app/swagger/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/hook.py` & `opsapp-0.0.25/opsapp/base/hook.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/logger.py` & `opsapp-0.0.25/opsapp/base/logger.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/misc.py` & `opsapp-0.0.25/opsapp/base/misc.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/path.py` & `opsapp-0.0.25/opsapp/base/path.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/progressbar.py` & `opsapp-0.0.25/opsapp/base/progressbar.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/registry.py` & `opsapp-0.0.25/opsapp/base/registry.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/base/timer.py` & `opsapp-0.0.25/opsapp/base/timer.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/utils/colors.py` & `opsapp-0.0.25/opsapp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/utils/utils.py` & `opsapp-0.0.25/opsapp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp/utils/visualization.py` & `opsapp-0.0.25/opsapp/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/opsapp.egg-info/SOURCES.txt` & `opsapp-0.0.25/opsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsapp-0.0.24/setup.py` & `opsapp-0.0.25/setup.py`

 * *Files identical despite different names*

