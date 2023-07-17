# Comparing `tmp/adbutils-1.2.8.tar.gz` & `tmp/adbutils-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adbutils-1.2.8.tar", last modified: Wed Mar  8 12:03:53 2023, max compression
+gzip compressed data, was "dist/adbutils-1.2.9.tar", last modified: Fri Mar 10 02:25:51 2023, max compression
```

## Comparing `adbutils-1.2.8.tar` & `adbutils-1.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (116)      125 2023-03-08 12:03:44.000000 adbutils-1.2.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-08 12:03:44.000000 adbutils-1.2.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)      942 2023-03-08 12:03:44.000000 adbutils-1.2.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-03-08 12:03:53.000000 adbutils-1.2.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)      371 2023-03-08 12:03:53.000000 adbutils-1.2.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-08 12:03:44.000000 adbutils-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-08 12:03:53.000000 adbutils-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14215 2023-03-08 12:03:44.000000 adbutils-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils/
--rw-r--r--   0 runner    (1001) docker     (116)     3333 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11931 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12159 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (116)    46766 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (116)     1705 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (116)     6713 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      272 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (116)       49 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      940 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    12871 2023-03-08 12:03:44.000000 adbutils-1.2.8/adbutils/pidcat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      805 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)       84 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-03-08 12:03:53.000000 adbutils-1.2.8/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/assets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/assets/images/
--rw-r--r--   0 runner    (1001) docker     (116)   127305 2023-03-08 12:03:44.000000 adbutils-1.2.8/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (116)     6098 2023-03-08 12:03:44.000000 adbutils-1.2.8/build_wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      609 2023-03-08 12:03:44.000000 adbutils-1.2.8/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (116)       83 2023-03-08 12:03:44.000000 adbutils-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      646 2023-03-08 12:03:53.000000 adbutils-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      418 2023-03-08 12:03:44.000000 adbutils-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-08 12:03:53.000000 adbutils-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      320 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)      749 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (116)      575 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (116)     5258 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (116)      952 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (116)      299 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (116)      276 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (116)      706 2023-03-08 12:03:44.000000 adbutils-1.2.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2023-03-10 02:25:42.000000 adbutils-1.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-10 02:25:42.000000 adbutils-1.2.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2023-03-10 02:25:42.000000 adbutils-1.2.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2023-03-10 02:25:51.000000 adbutils-1.2.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)      300 2023-03-10 02:25:51.000000 adbutils-1.2.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-10 02:25:42.000000 adbutils-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-10 02:25:51.000000 adbutils-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    14215 2023-03-10 02:25:42.000000 adbutils-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (116)     3333 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11931 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12159 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    46766 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1718 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6713 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      940 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12871 2023-03-10 02:25:42.000000 adbutils-1.2.9/adbutils/pidcat.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      805 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2023-03-10 02:25:51.000000 adbutils-1.2.9/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/assets/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (116)   127305 2023-03-10 02:25:42.000000 adbutils-1.2.9/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6098 2023-03-10 02:25:42.000000 adbutils-1.2.9/build_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      609 2023-03-10 02:25:42.000000 adbutils-1.2.9/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (116)       83 2023-03-10 02:25:42.000000 adbutils-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      646 2023-03-10 02:25:51.000000 adbutils-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      418 2023-03-10 02:25:42.000000 adbutils-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 02:25:51.000000 adbutils-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      320 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (116)      575 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5258 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (116)      952 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (116)      299 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)      276 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (116)      706 2023-03-10 02:25:42.000000 adbutils-1.2.9/tests/test_utils.py
```

### Comparing `adbutils-1.2.8/.github/workflows/publish-to-pypi.yml` & `adbutils-1.2.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/.travis.yml` & `adbutils-1.2.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/LICENSE` & `adbutils-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/PKG-INFO` & `adbutils-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 1.2.8
+Version: 1.2.9
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-1.2.8/README.md` & `adbutils-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/__init__.py` & `adbutils-1.2.9/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/__main__.py` & `adbutils-1.2.9/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/_adb.py` & `adbutils-1.2.9/adbutils/_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/_device.py` & `adbutils-1.2.9/adbutils/_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/_proto.py` & `adbutils-1.2.9/adbutils/_proto.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     DEV = "dev"
     LOCAL = "local"
     LOCAL_RESERVED = "localreserved"
     LOCAL_FILESYSTEM = "localfilesystem"
     LOCAL_ABSTRACT = "localabstract"  # same as UNIX
 
 
-@dataclass
+@dataclass(frozen=True)
 class DeviceEvent:
     present: bool
     serial: str
     status: str
 
 
 @dataclass
```

### Comparing `adbutils-1.2.8/adbutils/_utils.py` & `adbutils-1.2.9/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/errors.py` & `adbutils-1.2.9/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils/pidcat.py` & `adbutils-1.2.9/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/adbutils.egg-info/PKG-INFO` & `adbutils-1.2.9/adbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 1.2.8
+Version: 1.2.9
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-1.2.8/adbutils.egg-info/SOURCES.txt` & `adbutils-1.2.9/adbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/assets/images/pidcat.png` & `adbutils-1.2.9/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/build_wheel.py` & `adbutils-1.2.9/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/examples/reset-offline.py` & `adbutils-1.2.9/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/setup.cfg` & `adbutils-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/tests/test_adb.py` & `adbutils-1.2.9/tests/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/tests/test_deprecated.py` & `adbutils-1.2.9/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/tests/test_device.py` & `adbutils-1.2.9/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/tests/test_forward_reverse.py` & `adbutils-1.2.9/tests/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-1.2.8/tests/test_utils.py` & `adbutils-1.2.9/tests/test_utils.py`

 * *Files identical despite different names*

