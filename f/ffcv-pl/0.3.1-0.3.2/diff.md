# Comparing `tmp/ffcv_pl-0.3.1.tar.gz` & `tmp/ffcv_pl-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffcv_pl-0.3.1.tar", last modified: Thu Jul 13 11:35:36 2023, max compression
+gzip compressed data, was "ffcv_pl-0.3.2.tar", last modified: Mon Jul 17 10:19:30 2023, max compression
```

## Comparing `ffcv_pl-0.3.1.tar` & `ffcv_pl-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.741825 ffcv_pl-0.3.1/ffcv_pl/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.3.1/ffcv_pl/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     4497 2023-07-13 09:22:10.000000 ffcv_pl-0.3.1/ffcv_pl/data_loading.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/augmentations.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2597 2023-07-13 09:21:21.000000 ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/utils.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2520 2023-07-13 09:56:55.000000 ffcv_pl-0.3.1/ffcv_pl/generate_dataset.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/ffcv_pl.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      329 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-13 10:18:03.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-07-13 11:35:36.000000 ffcv_pl-0.3.1/ffcv_pl.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-07-13 11:35:36.745825 ffcv_pl-0.3.1/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      483 2023-07-13 11:35:07.000000 ffcv_pl-0.3.1/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-17 10:19:30.946774 ffcv_pl-0.3.2/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      519 2023-07-17 10:19:30.946774 ffcv_pl-0.3.2/PKG-INFO
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-17 10:19:30.942774 ffcv_pl-0.3.2/ffcv_pl/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.3.2/ffcv_pl/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     7637 2023-07-17 09:56:26.000000 ffcv_pl-0.3.2/ffcv_pl/data_loading.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-17 10:19:30.946774 ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/augmentations.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2613 2023-07-17 08:42:53.000000 ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/utils.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     4566 2023-07-17 09:44:04.000000 ffcv_pl-0.3.2/ffcv_pl/generate_dataset.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-17 10:19:30.942774 ffcv_pl-0.3.2/ffcv_pl.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      519 2023-07-17 10:19:30.000000 ffcv_pl-0.3.2/ffcv_pl.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      329 2023-07-17 10:19:30.000000 ffcv_pl-0.3.2/ffcv_pl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-17 10:19:30.000000 ffcv_pl-0.3.2/ffcv_pl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-17 10:19:30.000000 ffcv_pl-0.3.2/ffcv_pl.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-07-17 10:19:30.000000 ffcv_pl-0.3.2/ffcv_pl.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-07-17 10:19:30.946774 ffcv_pl-0.3.2/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      725 2023-07-17 10:10:22.000000 ffcv_pl-0.3.2/setup.py
```

### Comparing `ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/augmentations.py` & `ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.3.1/ffcv_pl/ffcv_utils/utils.py` & `ffcv_pl-0.3.2/ffcv_pl/ffcv_utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                TorchTensorField: "tensor"}
     return mapping[f]
 
 
 def obj_to_field(obj: Any) -> Field:
 
     if isinstance(obj, Image):
-        return RGBImageField()
+        return RGBImageField(write_mode="jpg")
 
     elif isinstance(obj, int):
         return IntField()
 
     elif isinstance(obj, float):
         return FloatField()
```

