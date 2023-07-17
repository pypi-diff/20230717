# Comparing `tmp/xdcget-0.2.2.tar.gz` & `tmp/xdcget-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcget-0.2.2.tar", last modified: Mon Jul 17 08:05:39 2023, max compression
+gzip compressed data, was "xdcget-0.2.3.tar", last modified: Mon Jul 17 08:18:30 2023, max compression
```

## Comparing `xdcget-0.2.2.tar` & `xdcget-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:05:39.269604 xdcget-0.2.2/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2704 2023-07-17 08:05:39.269604 xdcget-0.2.2/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2152 2023-07-13 14:35:59.000000 xdcget-0.2.2/README.md
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     1377 2023-07-17 08:05:20.000000 xdcget-0.2.2/pyproject.toml
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-07-17 08:05:39.269604 xdcget-0.2.2/setup.cfg
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:05:39.265604 xdcget-0.2.2/src/
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:05:39.265604 xdcget-0.2.2/src/xdcget/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        2 2023-07-05 12:29:52.000000 xdcget-0.2.2/src/xdcget/__init__.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     6643 2023-07-13 14:35:59.000000 xdcget-0.2.2/src/xdcget/config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2311 2023-07-13 14:35:59.000000 xdcget-0.2.2/src/xdcget/main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)    11185 2023-07-14 13:04:30.000000 xdcget-0.2.2/src/xdcget/storage.py
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:05:39.265604 xdcget-0.2.2/src/xdcget.egg-info/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2704 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      377 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/SOURCES.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/dependency_links.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/entry_points.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       43 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/requires.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-07-17 08:05:39.000000 xdcget-0.2.2/src/xdcget.egg-info/top_level.txt
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:05:39.265604 xdcget-0.2.2/tests/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2438 2023-07-16 11:24:32.000000 xdcget-0.2.2/tests/test_config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     1521 2023-07-16 11:24:32.000000 xdcget-0.2.2/tests/test_main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2695 2023-07-16 11:24:32.000000 xdcget-0.2.2/tests/test_storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3352 2023-07-17 08:18:30.439728 xdcget-0.2.3/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2800 2023-07-17 08:17:51.000000 xdcget-0.2.3/README.md
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     1310 2023-07-17 08:18:18.000000 xdcget-0.2.3/pyproject.toml
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-07-17 08:18:30.439728 xdcget-0.2.3/setup.cfg
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/xdcget/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        2 2023-07-05 12:29:52.000000 xdcget-0.2.3/src/xdcget/__init__.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     6643 2023-07-13 14:35:59.000000 xdcget-0.2.3/src/xdcget/config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2311 2023-07-13 14:35:59.000000 xdcget-0.2.3/src/xdcget/main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)    11185 2023-07-14 13:04:30.000000 xdcget-0.2.3/src/xdcget/storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/xdcget.egg-info/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3352 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      377 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/entry_points.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       43 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/requires.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/top_level.txt
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/tests/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2438 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     1521 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2695 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_storage.py
```

### Comparing `xdcget-0.2.2/PKG-INFO` & `xdcget-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdcget
-Version: 0.2.2
+Version: 0.2.3
 Summary: experimental tool for collecting latest releases of webxdc apps
 License: MPL-2.0
 Project-URL: homepage, https://codeberg.org/webxdc/xdcget
 Project-URL: issues, https://codeberg.org/webxdc/xdcget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -69,7 +69,25 @@
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
 and then insert it into the config file: 
 
     # the line you need to put into `xdcget.ini` 
     GITHUB_USER = <your-github-user-name> 
     GITHUB_TOKEN = <paste-your-github-access-token-here> 
+
+
+## Building and publishing xdcget releases (maintainer notes)
+
+This project uses a single `pyproject.toml` to define all python build/test metadata.
+See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+
+Quick notes on requirements for releasing: 
+
+- `pip install build twine` for building and uploading distribution files 
+
+- `python -m build` to build the distribution files
+
+- [create API-tokens on PyPI](https://pypi.org/manage/account/)
+  to be able to upload to PyPI repositories. 
+
+- `twine upload dist/*` to upload all built distribution files 
+
```

### Comparing `xdcget-0.2.2/README.md` & `xdcget-0.2.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -54,7 +54,25 @@
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
 and then insert it into the config file: 
 
     # the line you need to put into `xdcget.ini` 
     GITHUB_USER = <your-github-user-name> 
     GITHUB_TOKEN = <paste-your-github-access-token-here> 
+
+
+## Building and publishing xdcget releases (maintainer notes)
+
+This project uses a single `pyproject.toml` to define all python build/test metadata.
+See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+
+Quick notes on requirements for releasing: 
+
+- `pip install build twine` for building and uploading distribution files 
+
+- `python -m build` to build the distribution files
+
+- [create API-tokens on PyPI](https://pypi.org/manage/account/)
+  to be able to upload to PyPI repositories. 
+
+- `twine upload dist/*` to upload all built distribution files 
+
```

### Comparing `xdcget-0.2.2/pyproject.toml` & `xdcget-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 [project]
 name = "xdcget"
-version = "0.2.2"
-#author = "holger and team" 
-#author_email = "holger@deltachat.de"
+version = "0.2.3"
 description = "experimental tool for collecting latest releases of webxdc apps"
 license = {text = "MPL-2.0"}
 requires-python = ">=3.10"
 readme = "README.md"
 
 scripts = {xdcget = "xdcget.main:main"}
```

### Comparing `xdcget-0.2.2/src/xdcget/config.py` & `xdcget-0.2.3/src/xdcget/config.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.2/src/xdcget/main.py` & `xdcget-0.2.3/src/xdcget/main.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.2/src/xdcget/storage.py` & `xdcget-0.2.3/src/xdcget/storage.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.2/src/xdcget.egg-info/PKG-INFO` & `xdcget-0.2.3/src/xdcget.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdcget
-Version: 0.2.2
+Version: 0.2.3
 Summary: experimental tool for collecting latest releases of webxdc apps
 License: MPL-2.0
 Project-URL: homepage, https://codeberg.org/webxdc/xdcget
 Project-URL: issues, https://codeberg.org/webxdc/xdcget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -69,7 +69,25 @@
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
 and then insert it into the config file: 
 
     # the line you need to put into `xdcget.ini` 
     GITHUB_USER = <your-github-user-name> 
     GITHUB_TOKEN = <paste-your-github-access-token-here> 
+
+
+## Building and publishing xdcget releases (maintainer notes)
+
+This project uses a single `pyproject.toml` to define all python build/test metadata.
+See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+
+Quick notes on requirements for releasing: 
+
+- `pip install build twine` for building and uploading distribution files 
+
+- `python -m build` to build the distribution files
+
+- [create API-tokens on PyPI](https://pypi.org/manage/account/)
+  to be able to upload to PyPI repositories. 
+
+- `twine upload dist/*` to upload all built distribution files 
+
```

### Comparing `xdcget-0.2.2/tests/test_config.py` & `xdcget-0.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.2/tests/test_main.py` & `xdcget-0.2.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `xdcget-0.2.2/tests/test_storage.py` & `xdcget-0.2.3/tests/test_storage.py`

 * *Files identical despite different names*

