# Comparing `tmp/gfx-perp-python-sdk-0.0.1.tar.gz` & `tmp/gfx_perp_python_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx-perp-python-sdk-0.0.1.tar", last modified: Mon Jul 17 15:44:31 2023, max compression
+gzip compressed data, was "gfx_perp_python_sdk-0.0.2.tar", last modified: Mon Jul 17 16:02:45 2023, max compression
```

## Comparing `gfx-perp-python-sdk-0.0.1.tar` & `gfx_perp_python_sdk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 15:44:31.929228 gfx-perp-python-sdk-0.0.1/
--rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx-perp-python-sdk-0.0.1/LICENSE
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 15:44:31.929086 gfx-perp-python-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx-perp-python-sdk-0.0.1/README.md
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 15:44:31.927527 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 15:44:31.000000 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)      325 2023-07-17 15:44:31.000000 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-17 15:44:31.000000 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-17 15:44:31.000000 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/requires.txt
--rw-r--r--   0 shashank   (501) staff       (20)       11 2023-07-17 15:44:31.000000 gfx-perp-python-sdk-0.0.1/gfx_perp_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 15:44:31.928751 gfx-perp-python-sdk-0.0.1/my_project/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx-perp-python-sdk-0.0.1/my_project/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx-perp-python-sdk-0.0.1/my_project/perp.py
--rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx-perp-python-sdk-0.0.1/my_project/product.py
--rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx-perp-python-sdk-0.0.1/my_project/trader.py
--rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-17 15:44:31.929272 gfx-perp-python-sdk-0.0.1/setup.cfg
--rw-r--r--   0 shashank   (501) staff       (20)      352 2023-07-17 13:57:42.000000 gfx-perp-python-sdk-0.0.1/setup.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.686726 gfx_perp_python_sdk-0.0.2/
+-rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.2/LICENSE
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:02:45.686565 gfx_perp_python_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.2/README.md
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.685202 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)      325 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       11 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.686033 gfx_perp_python_sdk-0.0.2/my_project/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.2/my_project/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.2/my_project/perp.py
+-rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.2/my_project/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.2/my_project/trader.py
+-rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-17 16:02:45.686767 gfx_perp_python_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 shashank   (501) staff       (20)      352 2023-07-17 16:01:48.000000 gfx_perp_python_sdk-0.0.2/setup.py
```

### Comparing `gfx-perp-python-sdk-0.0.1/LICENSE` & `gfx_perp_python_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx-perp-python-sdk-0.0.1/my_project/trader.py` & `gfx_perp_python_sdk-0.0.2/my_project/trader.py`

 * *Files identical despite different names*

