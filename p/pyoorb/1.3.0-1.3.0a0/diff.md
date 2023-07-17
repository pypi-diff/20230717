# Comparing `tmp/pyoorb-1.3.0.tar.gz` & `tmp/pyoorb-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoorb-1.3.0.tar", last modified: Mon Jul 17 07:56:28 2023, max compression
+gzip compressed data, was "pyoorb-1.3.0a0.tar", last modified: Fri Jul 14 14:30:08 2023, max compression
```

## Comparing `pyoorb-1.3.0.tar` & `pyoorb-1.3.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:56:28.384028 pyoorb-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-17 07:56:15.000000 pyoorb-1.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-17 07:56:28.384028 pyoorb-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-17 07:56:15.000000 pyoorb-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:56:28.384028 pyoorb-1.3.0/pyoorb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-17 07:56:28.000000 pyoorb-1.3.0/pyoorb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 07:56:28.000000 pyoorb-1.3.0/pyoorb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:56:28.000000 pyoorb-1.3.0/pyoorb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 07:56:28.000000 pyoorb-1.3.0/pyoorb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 07:56:28.000000 pyoorb-1.3.0/pyoorb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 07:56:15.000000 pyoorb-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:56:28.384028 pyoorb-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-17 07:56:15.000000 pyoorb-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:56:28.384028 pyoorb-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-17 07:56:15.000000 pyoorb-1.3.0/tests/test_compute_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-17 07:56:15.000000 pyoorb-1.3.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:30:08.148809 pyoorb-1.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-14 14:30:08.148809 pyoorb-1.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:30:08.144809 pyoorb-1.3.0a0/pyoorb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-14 14:30:08.000000 pyoorb-1.3.0a0/pyoorb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 14:30:08.000000 pyoorb-1.3.0a0/pyoorb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:30:08.000000 pyoorb-1.3.0a0/pyoorb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 14:30:08.000000 pyoorb-1.3.0a0/pyoorb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 14:30:08.000000 pyoorb-1.3.0a0/pyoorb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:30:08.148809 pyoorb-1.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:30:08.144809 pyoorb-1.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/tests/test_compute_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-14 14:29:55.000000 pyoorb-1.3.0a0/tests/test_version.py
```

### Comparing `pyoorb-1.3.0/COPYING` & `pyoorb-1.3.0a0/COPYING`

 * *Files identical despite different names*

### Comparing `pyoorb-1.3.0/PKG-INFO` & `pyoorb-1.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoorb
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: An open-source orbit-computation package for Solar System objects. 
 Home-page: https://github.com/oorb/oorb
 Download-URL: https://pypi.python.org/pypi/pyoorb
 Author: Mikael Granvik et al.
 Maintainer: oorb developers
 Maintainer-email: oorb@googlegroups.com
 License: GPL3
```

### Comparing `pyoorb-1.3.0/README.md` & `pyoorb-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pyoorb-1.3.0/pyoorb.egg-info/PKG-INFO` & `pyoorb-1.3.0a0/pyoorb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoorb
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: An open-source orbit-computation package for Solar System objects. 
 Home-page: https://github.com/oorb/oorb
 Download-URL: https://pypi.python.org/pypi/pyoorb
 Author: Mikael Granvik et al.
 Maintainer: oorb developers
 Maintainer-email: oorb@googlegroups.com
 License: GPL3
```

### Comparing `pyoorb-1.3.0/pyproject.toml` & `pyoorb-1.3.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyoorb-1.3.0/setup.py` & `pyoorb-1.3.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `pyoorb-1.3.0/tests/test_compute_version.py` & `pyoorb-1.3.0a0/tests/test_compute_version.py`

 * *Files identical despite different names*

### Comparing `pyoorb-1.3.0/tests/test_version.py` & `pyoorb-1.3.0a0/tests/test_version.py`

 * *Files identical despite different names*

