# Comparing `tmp/stock-open-api-0.0.1.tar.gz` & `tmp/stock-open-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.1.tar", last modified: Mon Jul 17 03:24:50 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.2.tar", last modified: Mon Jul 17 10:09:47 2023, max compression
```

## Comparing `stock-open-api-0.0.1.tar` & `stock-open-api-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,35 @@
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/
--rwxr-xr-x   0 hina       (501) staff       (20)      414 2023-07-17 03:13:13.000000 stock-open-api-0.0.1/MANIFEST.in
--rw-r--r--   0 hina       (501) staff       (20)     1573 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)       76 2023-07-17 03:11:19.000000 stock-open-api-0.0.1/README.md
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/requirements/
--rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 03:10:06.000000 stock-open-api-0.0.1/requirements/production.txt
--rw-r--r--   0 hina       (501) staff       (20)       38 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/setup.cfg
--rwxr-xr-x   0 hina       (501) staff       (20)     3171 2023-07-17 03:24:15.000000 stock-open-api-0.0.1/setup.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_api/
--rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 02:58:35.000000 stock-open-api-0.0.1/stock_api/__init__.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_api/eastmoney/
--rw-r--r--   0 hina       (501) staff       (20)      136 2023-07-17 03:07:42.000000 stock-open-api-0.0.1/stock_api/eastmoney/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      201 2023-07-17 03:03:14.000000 stock-open-api-0.0.1/stock_api/eastmoney/hk_stocks.py
--rw-r--r--   0 hina       (501) staff       (20)       99 2023-07-17 03:06:20.000000 stock-open-api-0.0.1/stock_api/version.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/
--rw-r--r--   0 hina       (501) staff       (20)     1573 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)      388 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 hina       (501) staff       (20)       16 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 03:24:50.000000 stock-open-api-0.0.1/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/
+-rwxr-xr-x   0 hina       (501) staff       (20)      414 2023-07-17 03:13:13.000000 stock-open-api-0.0.2/MANIFEST.in
+-rw-r--r--   0 hina       (501) staff       (20)     4951 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/PKG-INFO
+-rw-r--r--   0 hina       (501) staff       (20)     2833 2023-07-17 09:05:44.000000 stock-open-api-0.0.2/README.md
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/requirements/
+-rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 03:10:06.000000 stock-open-api-0.0.2/requirements/production.txt
+-rw-r--r--   0 hina       (501) staff       (20)       38 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/setup.cfg
+-rwxr-xr-x   0 hina       (501) staff       (20)     3181 2023-07-17 10:08:42.000000 stock-open-api-0.0.2/setup.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/
+-rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 02:58:35.000000 stock-open-api-0.0.2/stock_open_api/__init__.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/
+-rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 06:54:43.000000 stock-open-api-0.0.2/stock_open_api/api/__init__.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/
+-rw-r--r--   0 hina       (501) staff       (20)      136 2023-07-17 03:07:42.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 hina       (501) staff       (20)     6384 2023-07-17 07:46:00.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 hina       (501) staff       (20)     3495 2023-07-17 07:04:03.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock_config.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/sse/
+-rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 07:14:57.000000 stock-open-api-0.0.2/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 hina       (501) staff       (20)     2972 2023-07-17 07:43:31.000000 stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 hina       (501) staff       (20)     1471 2023-07-17 07:18:17.000000 stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock_config.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/items/
+-rw-r--r--   0 hina       (501) staff       (20)      102 2023-07-17 06:55:24.000000 stock-open-api-0.0.2/stock_open_api/items/__init__.py
+-rw-r--r--   0 hina       (501) staff       (20)      333 2023-07-17 07:00:59.000000 stock-open-api-0.0.2/stock_open_api/items/list_item.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/utils/
+-rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 03:33:51.000000 stock-open-api-0.0.2/stock_open_api/utils/__init__.py
+-rw-r--r--   0 hina       (501) staff       (20)      263 2023-07-17 03:39:39.000000 stock-open-api-0.0.2/stock_open_api/utils/time_util.py
+-rw-r--r--   0 hina       (501) staff       (20)      209 2023-07-17 03:42:26.000000 stock-open-api-0.0.2/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 hina       (501) staff       (20)       95 2023-07-17 09:55:34.000000 stock-open-api-0.0.2/stock_open_api/version.py
+drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/
+-rw-r--r--   0 hina       (501) staff       (20)     4951 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 hina       (501) staff       (20)      772 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 hina       (501) staff       (20)       21 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 07:07:04.000000 stock-open-api-0.0.2/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.1/setup.py` & `stock-open-api-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 && python setup.py sdist bdist_wheel  \
 && twine check dist/* \
 && twine upload dist/*
 
 
 ## 下载测试
 安装测试
-pip3 install -U stock-api -i https://pypi.org/simple
+pip3 install -U stock-open-api -i https://pypi.org/simple
 
 打包的用的setup必须引入
 
 参考：
 https://packaging.python.org/guides/making-a-pypi-friendly-readme/
 
 """
@@ -70,15 +70,15 @@
     version=VERSION,
     description="a api collection for stock",
 
     keywords='stock,api',
     author='Peng Shiyu',
     author_email='pengshiyuyx@gmail.com',
     license='MIT',
-    url="https://github.com/mouday/stock-api",
+    url="https://github.com/mouday/stock-open-api",
 
     long_description=long_description,
     long_description_content_type='text/markdown',
     platforms=['any'],
     # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

