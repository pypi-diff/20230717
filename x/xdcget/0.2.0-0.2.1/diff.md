# Comparing `tmp/xdcget-0.2.0.tar.gz` & `tmp/xdcget-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcget-0.2.0.tar", last modified: Mon Jul 17 07:42:27 2023, max compression
+gzip compressed data, was "xdcget-0.2.1.tar", last modified: Mon Jul 17 08:02:06 2023, max compression
```

## Comparing `xdcget-0.2.0.tar` & `xdcget-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 07:42:27.878903 xdcget-0.2.0/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      282 2023-07-17 07:42:27.878903 xdcget-0.2.0/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2152 2023-07-13 14:35:59.000000 xdcget-0.2.0/README.md
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      541 2023-07-16 11:58:51.000000 xdcget-0.2.0/pyproject.toml
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-07-17 07:42:27.878903 xdcget-0.2.0/setup.cfg
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 07:42:27.878903 xdcget-0.2.0/src/
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 07:42:27.878903 xdcget-0.2.0/src/xdcget/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        2 2023-07-05 12:29:52.000000 xdcget-0.2.0/src/xdcget/__init__.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     6643 2023-07-13 14:35:59.000000 xdcget-0.2.0/src/xdcget/config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2311 2023-07-13 14:35:59.000000 xdcget-0.2.0/src/xdcget/main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)    11185 2023-07-14 13:04:30.000000 xdcget-0.2.0/src/xdcget/storage.py
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 07:42:27.878903 xdcget-0.2.0/src/xdcget.egg-info/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      282 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      377 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/SOURCES.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/dependency_links.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/entry_points.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       43 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/requires.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-07-17 07:42:27.000000 xdcget-0.2.0/src/xdcget.egg-info/top_level.txt
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 07:42:27.878903 xdcget-0.2.0/tests/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2438 2023-07-16 11:24:32.000000 xdcget-0.2.0/tests/test_config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     1521 2023-07-16 11:24:32.000000 xdcget-0.2.0/tests/test_main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2695 2023-07-16 11:24:32.000000 xdcget-0.2.0/tests/test_storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:02:06.353537 xdcget-0.2.1/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2704 2023-07-17 08:02:06.353537 xdcget-0.2.1/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2152 2023-07-13 14:35:59.000000 xdcget-0.2.1/README.md
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      755 2023-07-17 08:01:58.000000 xdcget-0.2.1/pyproject.toml
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-07-17 08:02:06.353537 xdcget-0.2.1/setup.cfg
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:02:06.353537 xdcget-0.2.1/src/
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:02:06.353537 xdcget-0.2.1/src/xdcget/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        2 2023-07-05 12:29:52.000000 xdcget-0.2.1/src/xdcget/__init__.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     6643 2023-07-13 14:35:59.000000 xdcget-0.2.1/src/xdcget/config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2311 2023-07-13 14:35:59.000000 xdcget-0.2.1/src/xdcget/main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)    11185 2023-07-14 13:04:30.000000 xdcget-0.2.1/src/xdcget/storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:02:06.353537 xdcget-0.2.1/src/xdcget.egg-info/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2704 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      377 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/entry_points.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       43 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/requires.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-07-17 08:02:06.000000 xdcget-0.2.1/src/xdcget.egg-info/top_level.txt
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:02:06.353537 xdcget-0.2.1/tests/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2438 2023-07-16 11:24:32.000000 xdcget-0.2.1/tests/test_config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     1521 2023-07-16 11:24:32.000000 xdcget-0.2.1/tests/test_main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2695 2023-07-16 11:24:32.000000 xdcget-0.2.1/tests/test_storage.py
```

### Comparing `xdcget-0.2.0/README.md` & `xdcget-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/pyproject.toml` & `xdcget-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 [project]
 name = "xdcget"
-version = "0.2.0"
+version = "0.2.1"
 #author = "holger and team" 
 #author_email = "holger@deltachat.de"
 description = "experimental tool for collecting latest releases of webxdc apps"
-#long_description = "file: README.rst"
 license = {text = "MPL-2.0"}
+requires-python = ">=3.10"
+readme = "README.md"
 
 scripts = {xdcget = "xdcget.main:main"}
 
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+    "Operating System :: POSIX",
+]
+
+
 dependencies = [
     "requests",
     "termcolor",
     "toml",
 ]
 
 [project.optional-dependencies]
```

### Comparing `xdcget-0.2.0/src/xdcget/config.py` & `xdcget-0.2.1/src/xdcget/config.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/src/xdcget/main.py` & `xdcget-0.2.1/src/xdcget/main.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/src/xdcget/storage.py` & `xdcget-0.2.1/src/xdcget/storage.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/tests/test_config.py` & `xdcget-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/tests/test_main.py` & `xdcget-0.2.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.0/tests/test_storage.py` & `xdcget-0.2.1/tests/test_storage.py`

 * *Files identical despite different names*

