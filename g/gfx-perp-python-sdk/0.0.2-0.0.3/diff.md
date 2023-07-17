# Comparing `tmp/gfx_perp_python_sdk-0.0.2.tar.gz` & `tmp/gfx_perp_python_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx_perp_python_sdk-0.0.2.tar", last modified: Mon Jul 17 16:02:45 2023, max compression
+gzip compressed data, was "gfx_perp_python_sdk-0.0.3.tar", last modified: Mon Jul 17 16:35:18 2023, max compression
```

## Comparing `gfx_perp_python_sdk-0.0.2.tar` & `gfx_perp_python_sdk-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.686726 gfx_perp_python_sdk-0.0.2/
--rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.2/LICENSE
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:02:45.686565 gfx_perp_python_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.2/README.md
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.685202 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)      325 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/requires.txt
--rw-r--r--   0 shashank   (501) staff       (20)       11 2023-07-17 16:02:45.000000 gfx_perp_python_sdk-0.0.2/gfx_perp_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:02:45.686033 gfx_perp_python_sdk-0.0.2/my_project/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.2/my_project/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.2/my_project/perp.py
--rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.2/my_project/product.py
--rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.2/my_project/trader.py
--rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-17 16:02:45.686767 gfx_perp_python_sdk-0.0.2/setup.cfg
--rw-r--r--   0 shashank   (501) staff       (20)      352 2023-07-17 16:01:48.000000 gfx_perp_python_sdk-0.0.2/setup.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.404509 gfx_perp_python_sdk-0.0.3/
+-rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.3/LICENSE
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:35:18.404385 gfx_perp_python_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.3/README.md
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.402668 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)      325 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       11 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.404085 gfx_perp_python_sdk-0.0.3/my_project/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.3/my_project/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.3/my_project/perp.py
+-rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.3/my_project/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.3/my_project/trader.py
+-rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-17 16:35:18.404545 gfx_perp_python_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 shashank   (501) staff       (20)      383 2023-07-17 16:33:38.000000 gfx_perp_python_sdk-0.0.3/setup.py
```

### Comparing `gfx_perp_python_sdk-0.0.2/LICENSE` & `gfx_perp_python_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx_perp_python_sdk-0.0.2/my_project/trader.py` & `gfx_perp_python_sdk-0.0.3/my_project/trader.py`

 * *Files identical despite different names*

