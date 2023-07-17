# Comparing `tmp/openwholeslide-0.0.12.tar.gz` & `tmp/openwholeslide-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwholeslide-0.0.12.tar", max compression
+gzip compressed data, was "openwholeslide-0.0.14.tar", max compression
```

## Comparing `openwholeslide-0.0.12.tar` & `openwholeslide-0.0.14.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1092 2023-07-13 13:41:02.334199 openwholeslide-0.0.12/LICENSE
--rw-r--r--   0        0        0     1082 2023-07-17 12:11:16.736887 openwholeslide-0.0.12/README.md
--rw-r--r--   0        0        0      595 2023-07-17 12:14:54.765928 openwholeslide-0.0.12/pyproject.toml
--rw-r--r--   0        0        0      291 2023-07-13 14:59:46.056144 openwholeslide-0.0.12/src/openwholeslide/__init__.py
--rw-r--r--   0        0        0    13015 2023-07-13 13:52:32.513541 openwholeslide-0.0.12/src/openwholeslide/_slide.py
--rw-r--r--   0        0        0     4217 2023-07-12 13:40:21.409104 openwholeslide-0.0.12/src/openwholeslide/vectors.py
--rw-r--r--   0        0        0    12643 2023-07-12 13:53:46.784996 openwholeslide-0.0.12/src/openwholeslide/wsi.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 openwholeslide-0.0.12/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2023-07-13 13:41:02.334199 openwholeslide-0.0.14/LICENSE
+-rw-r--r--   0        0        0     1082 2023-07-17 12:11:16.736887 openwholeslide-0.0.14/README.md
+-rw-r--r--   0        0        0      739 2023-07-17 13:07:49.541482 openwholeslide-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-13 14:59:46.056144 openwholeslide-0.0.14/src/openwholeslide/__init__.py
+-rw-r--r--   0        0        0    13015 2023-07-13 13:52:32.513541 openwholeslide-0.0.14/src/openwholeslide/_slide.py
+-rw-r--r--   0        0        0     4217 2023-07-12 13:40:21.409104 openwholeslide-0.0.14/src/openwholeslide/vectors.py
+-rw-r--r--   0        0        0    12643 2023-07-12 13:53:46.784996 openwholeslide-0.0.14/src/openwholeslide/wsi.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 openwholeslide-0.0.14/PKG-INFO
```

### Comparing `openwholeslide-0.0.12/LICENSE` & `openwholeslide-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `openwholeslide-0.0.12/README.md` & `openwholeslide-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `openwholeslide-0.0.12/pyproject.toml` & `openwholeslide-0.0.14/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "openwholeslide"
-version = "0.0.12"
+version = "0.0.14"
 description = "Wrapper around tifffile library to have the same API as OpenSlide."
 authors = ["Arthur Elskens and Adrien Foucart"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10.6"
 numpy = ">=1.23.5"
 tifffile = ">=2023.1.23.1"
 Pillow = ">=9.4.0"
 scikit-image = ">=0.19.3"
 SimpleITK = ">=2.2.1"
 imagecodecs = ">=2023.7.10"
 
-[tool.poetry.dev-dependencies]
+[project.urls]
+"Source" = "https://gitlab.com/prother-wal_ulb_lis_mnu/openwholeslide.git"
+"Bug Tracker" = "https://gitlab.com/prother-wal_ulb_lis_mnu/openwholeslide/-/issues"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openwholeslide-0.0.12/src/openwholeslide/_slide.py` & `openwholeslide-0.0.14/src/openwholeslide/_slide.py`

 * *Files identical despite different names*

### Comparing `openwholeslide-0.0.12/src/openwholeslide/vectors.py` & `openwholeslide-0.0.14/src/openwholeslide/vectors.py`

 * *Files identical despite different names*

### Comparing `openwholeslide-0.0.12/src/openwholeslide/wsi.py` & `openwholeslide-0.0.14/src/openwholeslide/wsi.py`

 * *Files identical despite different names*

### Comparing `openwholeslide-0.0.12/PKG-INFO` & `openwholeslide-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwholeslide
-Version: 0.0.12
+Version: 0.0.14
 Summary: Wrapper around tifffile library to have the same API as OpenSlide.
 License: MIT
 Author: Arthur Elskens and Adrien Foucart
 Requires-Python: >=3.10.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

