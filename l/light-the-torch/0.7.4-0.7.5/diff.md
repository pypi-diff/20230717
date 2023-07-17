# Comparing `tmp/light_the_torch-0.7.4.tar.gz` & `tmp/light_the_torch-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/light-the-torch/light-the-torch/dist/.tmp-gzw_gyf2/light_the_torch-0.7.4.tar", last modified: Tue May 16 07:57:29 2023, max compression
+gzip compressed data, was "/home/runner/work/light-the-torch/light-the-torch/dist/.tmp-dbvmvf6b/light_the_torch-0.7.5.tar", last modified: Mon Jul 17 08:23:32 2023, max compression
```

## Comparing `light_the_torch-0.7.4.tar` & `light_the_torch-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/light_the_torch/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/light_the_torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/local-project-stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/local-project-stubs/pep517-setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/local-project-stubs/pep517-setuptools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/local-project-stubs/pep517-setuptools/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-16 07:56:33.000000 light_the_torch-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:57:29.000000 light_the_torch-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/light_the_torch/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/light_the_torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/local-project-stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/local-project-stubs/pep517-setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/local-project-stubs/pep517-setuptools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/local-project-stubs/pep517-setuptools/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-17 08:22:53.000000 light_the_torch-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:23:32.000000 light_the_torch-0.7.5/setup.cfg
```

### Comparing `light_the_torch-0.7.4/CONTRIBUTING.md` & `light_the_torch-0.7.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/LICENSE` & `light_the_torch-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/PKG-INFO` & `light_the_torch-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light_the_torch
-Version: 0.7.4
+Version: 0.7.5
 Summary: Install PyTorch distributions with computation backend auto-detection
 Author-email: Philip Meier <github.pmeier@posteo.de>
 License: BSD-3-Clause
 Project-URL: Tracker, https://github.com/pmeier/light-the-torch/issues
 Project-URL: Source, https://github.com/pmeier/light-the-torch
 Keywords: pytorch,cuda,pip,install
 Classifier: Development Status :: 4 - Beta
```

### Comparing `light_the_torch-0.7.4/README.md` & `light_the_torch-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/light_the_torch/_cb.py` & `light_the_torch-0.7.5/light_the_torch/_cb.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/light_the_torch/_patch.py` & `light_the_torch-0.7.5/light_the_torch/_patch.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/light_the_torch/_utils.py` & `light_the_torch-0.7.5/light_the_torch/_utils.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/light_the_torch.egg-info/PKG-INFO` & `light_the_torch-0.7.5/light_the_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-the-torch
-Version: 0.7.4
+Version: 0.7.5
 Summary: Install PyTorch distributions with computation backend auto-detection
 Author-email: Philip Meier <github.pmeier@posteo.de>
 License: BSD-3-Clause
 Project-URL: Tracker, https://github.com/pmeier/light-the-torch/issues
 Project-URL: Source, https://github.com/pmeier/light-the-torch
 Keywords: pytorch,cuda,pip,install
 Classifier: Development Status :: 4 - Beta
```

### Comparing `light_the_torch-0.7.4/light_the_torch.egg-info/SOURCES.txt` & `light_the_torch-0.7.5/light_the_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.4/pyproject.toml` & `light_the_torch-0.7.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Installation/Setup",
     "Topic :: Utilities",
 ]
 requires-python = ">= 3.7"
 dependencies = [
-    "pip >=22.3, <23.2",
+    "pip >=22.3, <23.3",
     "importlib_metadata ; python_version < '3.8'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Tracker = "https://github.com/pmeier/light-the-torch/issues"
 Source = "https://github.com/pmeier/light-the-torch"
```

