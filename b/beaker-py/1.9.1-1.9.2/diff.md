# Comparing `tmp/beaker-py-1.9.1.tar.gz` & `tmp/beaker-py-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beaker-py-1.9.1.tar", last modified: Thu Sep 15 20:49:41 2022, max compression
+gzip compressed data, was "dist/beaker-py-1.9.2.tar", last modified: Wed Sep 21 19:55:20 2022, max compression
```

## Comparing `beaker-py-1.9.1.tar` & `beaker-py-1.9.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:49:41.000000 beaker-py-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-09-15 20:49:27.000000 beaker-py-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-15 20:49:27.000000 beaker-py-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-09-15 20:49:41.000000 beaker-py-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-09-15 20:49:27.000000 beaker-py-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker/
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)    15259 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker/data_model/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)    21308 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/experiment_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/job.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/node.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/data_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7099 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker/services/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/account.py
--rw-r--r--   0 runner    (1001) docker     (121)    14293 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    34115 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    36269 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)    10105 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/group.py
--rw-r--r--   0 runner    (1001) docker     (121)    13309 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    22452 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/job.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     6239 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/organization.py
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)     8379 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/service_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27178 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/services/workspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-15 20:49:27.000000 beaker-py-1.9.1/beaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-15 20:49:41.000000 beaker-py-1.9.1/beaker_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-15 20:49:27.000000 beaker-py-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 20:49:41.000000 beaker-py-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-15 20:49:27.000000 beaker-py-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:55:20.000000 beaker-py-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-09-21 19:55:07.000000 beaker-py-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-21 19:55:07.000000 beaker-py-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-09-21 19:55:20.000000 beaker-py-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-09-21 19:55:07.000000 beaker-py-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker/
+-rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15259 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker/data_model/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21308 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/experiment_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/data_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7099 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker/services/
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/account.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14293 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34337 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36269 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10105 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13309 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22452 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6239 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/organization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8379 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/service_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30307 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/services/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-21 19:55:07.000000 beaker-py-1.9.2/beaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-21 19:55:20.000000 beaker-py-1.9.2/beaker_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-21 19:55:07.000000 beaker-py-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:55:20.000000 beaker-py-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-21 19:55:07.000000 beaker-py-1.9.2/setup.py
```

### Comparing `beaker-py-1.9.1/LICENSE` & `beaker-py-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/PKG-INFO` & `beaker-py-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-py
-Version: 1.9.1
+Version: 1.9.2
 Home-page: https://github.com/allenai/beaker-py
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beaker-py Version: 1.9.1 Home-page: https://
+Metadata-Version: 2.1 Name: beaker-py Version: 1.9.2 Home-page: https://
 github.com/allenai/beaker-py Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Classifier:
 Intended Audience :: Science/Research Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `beaker-py-1.9.1/README.md` & `beaker-py-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/__init__.py` & `beaker-py-1.9.2/beaker/__init__.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/client.py` & `beaker-py-1.9.2/beaker/client.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/config.py` & `beaker-py-1.9.2/beaker/config.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/base.py` & `beaker-py-1.9.2/beaker/data_model/base.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/cluster.py` & `beaker-py-1.9.2/beaker/data_model/cluster.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/dataset.py` & `beaker-py-1.9.2/beaker/data_model/dataset.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/experiment.py` & `beaker-py-1.9.2/beaker/data_model/experiment.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/experiment_spec.py` & `beaker-py-1.9.2/beaker/data_model/experiment_spec.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/group.py` & `beaker-py-1.9.2/beaker/data_model/group.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/image.py` & `beaker-py-1.9.2/beaker/data_model/image.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/job.py` & `beaker-py-1.9.2/beaker/data_model/job.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/node.py` & `beaker-py-1.9.2/beaker/data_model/node.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/organization.py` & `beaker-py-1.9.2/beaker/data_model/organization.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/data_model/workspace.py` & `beaker-py-1.9.2/beaker/data_model/workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "WorkspacePage",
     "WorkspaceSpec",
     "WorkspaceTransferSpec",
     "Permission",
     "WorkspacePermissions",
     "WorkspacePatch",
     "WorkspacePermissionsPatch",
+    "WorkspaceClearResult",
 ]
 
 
 class WorkspaceSize(BaseModel):
     datasets: int
     experiments: int
     groups: int
@@ -87,7 +88,15 @@
     description: Optional[str] = None
     archive: Optional[bool] = None
 
 
 class WorkspacePermissionsPatch(BaseModel):
     public: Optional[bool] = None
     authorizations: Optional[Dict[str, Permission]] = None
+
+
+class WorkspaceClearResult(BaseModel):
+    groups_deleted: int = 0
+    experiments_deleted: int = 0
+    images_deleted: int = 0
+    datasets_deleted: int = 0
+    secrets_deleted: int = 0
```

### Comparing `beaker-py-1.9.1/beaker/exceptions.py` & `beaker-py-1.9.2/beaker/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 __all__ = [
     "BeakerError",
     "ValidationError",
     "HTTPError",
     "RequestException",
+    "NotFoundError",
     "AccountNotFound",
     "OrganizationNotFound",
     "OrganizationNotSet",
     "ConfigurationError",
     "ImageNotFound",
     "ImageConflict",
     "WorkspaceNotFound",
@@ -61,19 +62,25 @@
     """
     Base class for all Beaker errors other than :exc:`HTTPError`, which is re-exported
     from :exc:`requests.exceptions.HTTPError`, and :exc:`ValidationError`, which is
     re-exported from `pydantic <https://pydantic-docs.helpmanual.io/>`_.
     """
 
 
-class AccountNotFound(BeakerError):
+class NotFoundError(BeakerError):
+    """
+    Base class for all "not found" error types.
+    """
+
+
+class AccountNotFound(NotFoundError):
     pass
 
 
-class OrganizationNotFound(BeakerError):
+class OrganizationNotFound(NotFoundError):
     """
     Raised when a specified organization doesn't exist.
     """
 
 
 class OrganizationNotSet(BeakerError):
     """
@@ -84,25 +91,25 @@
 
 class ConfigurationError(BeakerError):
     """
     Raised when the :class:`~beaker.Config` fails to instantiate.
     """
 
 
-class ImageNotFound(BeakerError):
+class ImageNotFound(NotFoundError):
     pass
 
 
 class ImageConflict(BeakerError):
     """
     Raised when attempting to create/rename an image if an image by that name already exists.
     """
 
 
-class WorkspaceNotFound(BeakerError):
+class WorkspaceNotFound(NotFoundError):
     pass
 
 
 class WorkspaceWriteError(BeakerError):
     """
     Raised when attempting to modify or add to a workspace that's been archived.
     """
@@ -110,25 +117,25 @@
 
 class WorkspaceConflict(BeakerError):
     """
     Raised when attempting to create/rename a workspace if a workspace by that name already exists.
     """
 
 
-class ClusterNotFound(BeakerError):
+class ClusterNotFound(NotFoundError):
     pass
 
 
 class ClusterConflict(BeakerError):
     """
     Raised when attempting to create a cluster if a cluster by that name already exists.
     """
 
 
-class ExperimentNotFound(BeakerError):
+class ExperimentNotFound(NotFoundError):
     pass
 
 
 class ExperimentConflict(BeakerError):
     """
     Raised when attempting to create/rename an experiment if an experiment by that name already exists.
     """
@@ -136,35 +143,35 @@
 
 class DatasetConflict(BeakerError):
     """
     Raised when attempting to create/rename a dataset if a dataset by that name already exists.
     """
 
 
-class DatasetNotFound(BeakerError):
+class DatasetNotFound(NotFoundError):
     pass
 
 
 class UnexpectedEOFError(BeakerError):
     """
     Raised when creating a dataset when an empty source file is encountered.
     """
 
 
-class JobNotFound(BeakerError):
+class JobNotFound(NotFoundError):
     pass
 
 
 class WorkspaceNotSet(BeakerError):
     """
     Raised when workspace argument is not provided and there is no default workspace set.
     """
 
 
-class NodeNotFound(BeakerError):
+class NodeNotFound(NotFoundError):
     pass
 
 
 class DatasetWriteError(BeakerError):
     """
     Raised when a write operation on a dataset fails because the dataset has already been committed.
     """
@@ -173,25 +180,25 @@
 class DatasetReadError(BeakerError):
     """
     Raised when a read operation on a dataset fails because the dataset hasn't been committed yet,
     or the :data:`~beaker.data_model.Dataset.storage` hasn't been set for some other reason.
     """
 
 
-class SecretNotFound(BeakerError):
+class SecretNotFound(NotFoundError):
     pass
 
 
 class GroupConflict(BeakerError):
     """
     Raised when attempting to create/rename a group if a group by that name already exists.
     """
 
 
-class GroupNotFound(BeakerError):
+class GroupNotFound(NotFoundError):
     pass
 
 
 class DuplicateJobError(BeakerError):
     """
     Raised when duplicate jobs are passed into a method that expects unique jobs.
     """
@@ -199,15 +206,15 @@
 
 class DuplicateExperimentError(BeakerError):
     """
     Raised when duplicate experiments are passed into a method that expects unique experiments.
     """
 
 
-class TaskNotFound(BeakerError):
+class TaskNotFound(NotFoundError):
     pass
 
 
 class ChecksumFailedError(BeakerError):
     """
     Raised when a downloaded file from a Beaker dataset is corrupted.
     """
```

### Comparing `beaker-py-1.9.1/beaker/progress.py` & `beaker-py-1.9.2/beaker/progress.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/account.py` & `beaker-py-1.9.2/beaker/services/account.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/cluster.py` & `beaker-py-1.9.2/beaker/services/cluster.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/dataset.py` & `beaker-py-1.9.2/beaker/services/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,22 +160,29 @@
 
         :raises DatasetNotFound: If the dataset can't be found.
         :raises BeakerError: Any other :class:`~beaker.exceptions.BeakerError` type that can occur.
         :raises RequestException: Any other exception that can occur when contacting the
             Beaker server.
         """
         dataset_id = self.resolve_dataset(dataset).id
-        return Dataset.from_json(
-            self.request(
-                f"datasets/{self.url_quote(dataset_id)}",
-                method="PATCH",
-                data=DatasetPatch(commit=True),
-                exceptions_for_status={404: DatasetNotFound(self._not_found_err_msg(dataset))},
-            ).json()
-        )
+
+        @retriable()
+        def commit() -> Dataset:
+            # It's okay to retry this because committing a dataset multiple
+            # times does nothing.
+            return Dataset.from_json(
+                self.request(
+                    f"datasets/{self.url_quote(dataset_id)}",
+                    method="PATCH",
+                    data=DatasetPatch(commit=True),
+                    exceptions_for_status={404: DatasetNotFound(self._not_found_err_msg(dataset))},
+                ).json()
+            )
+
+        return commit()
 
     def fetch(
         self,
         dataset: Union[str, Dataset],
         target: Optional[PathOrStr] = None,
         force: bool = False,
         max_workers: Optional[int] = None,
```

### Comparing `beaker-py-1.9.1/beaker/services/experiment.py` & `beaker-py-1.9.2/beaker/services/experiment.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/group.py` & `beaker-py-1.9.2/beaker/services/group.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/image.py` & `beaker-py-1.9.2/beaker/services/image.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/job.py` & `beaker-py-1.9.2/beaker/services/job.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/node.py` & `beaker-py-1.9.2/beaker/services/node.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/organization.py` & `beaker-py-1.9.2/beaker/services/organization.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/secret.py` & `beaker-py-1.9.2/beaker/services/secret.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/service_client.py` & `beaker-py-1.9.2/beaker/services/service_client.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker/services/workspace.py` & `beaker-py-1.9.2/beaker/services/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from typing import Dict, List, Optional, Union
 
 from ..data_model import *
 from ..exceptions import *
 from .service_client import ServiceClient
 
 
@@ -613,12 +614,84 @@
         :raises WorkspaceNotFound: If the workspace doesn't exist.
         :raises WorkspaceNotSet: If neither ``workspace`` nor
             :data:`Beaker.config.default_workspace <beaker.Config.default_workspace>` are set.
         """
         workspace_name = self.resolve_workspace(workspace, read_only_ok=True).full_name
         return f"{self.config.agent_address}/ws/{workspace_name}"
 
+    def clear(
+        self,
+        workspace: Optional[Union[str, Workspace]] = None,
+        groups: bool = True,
+        experiments: bool = True,
+        images: bool = True,
+        datasets: bool = True,
+        secrets: bool = True,
+    ):
+        """
+        Remove groups, experiments, images, datasets, and secrets from a workspace.
+
+        :param workspace: The Beaker workspace name, or object. If not specified,
+            :data:`Beaker.config.default_workspace <beaker.Config.default_workspace>` is used.
+        :param groups: Whether to delete groups.
+        :param experiments: Whether to delete experiments.
+        :param images: Whether to delete images.
+        :param datasets: Whether to delete datasets.
+        :param secrets: Whether to delete secrets.
+
+        :raises WorkspaceNotFound: If the workspace doesn't exist.
+        :raises WorkspaceNotSet: If neither ``workspace`` nor
+            :data:`Beaker.config.default_workspace <beaker.Config.default_workspace>` are set.
+        :raises BeakerError: Any other :class:`~beaker.exceptions.BeakerError` type that can occur.
+        :raises RequestException: Any other exception that can occur when contacting the
+            Beaker server.
+        """
+        import concurrent.futures
+
+        deletion_counts: Dict[str, int] = defaultdict(int)
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            deletion_futures = []
+
+            if groups:
+                for group in self.groups(workspace):
+                    future = executor.submit(self.beaker.group.delete, group)
+                    deletion_futures.append(future)
+                    deletion_counts["groups_deleted"] += 1
+
+            if experiments:
+                for experiment in self.experiments(workspace):
+                    future = executor.submit(self.beaker.experiment.delete, experiment)
+                    deletion_futures.append(future)
+                    deletion_counts["experiments_deleted"] += 1
+
+            if images:
+                for image in self.images(workspace):
+                    future = executor.submit(self.beaker.image.delete, image)
+                    deletion_futures.append(future)
+                    deletion_counts["images_deleted"] += 1
+
+            if datasets:
+                for dataset in self.datasets(workspace):
+                    future = executor.submit(self.beaker.dataset.delete, dataset)
+                    deletion_futures.append(future)
+                    deletion_counts["datasets_deleted"] += 1
+
+            if secrets:
+                for secret in self.secrets(workspace):
+                    future = executor.submit(self.beaker.secret.delete, secret, workspace)
+                    deletion_futures.append(future)
+                    deletion_counts["secrets_deleted"] += 1
+
+            done, _ = concurrent.futures.wait(deletion_futures)
+            for future in done:
+                try:
+                    future.result()
+                except NotFoundError:
+                    pass
+
+        return WorkspaceClearResult(**deletion_counts)
+
     def _not_found_err_msg(self, workspace: str) -> str:
         return (
             f"'{workspace}': Make sure you're using the workspace ID or *full* name "
             f"(with the organization prefix, e.g. 'org/workspace_name')."
         )
```

### Comparing `beaker-py-1.9.1/beaker/util.py` & `beaker-py-1.9.2/beaker/util.py`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/beaker_py.egg-info/PKG-INFO` & `beaker-py-1.9.2/beaker_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-py
-Version: 1.9.1
+Version: 1.9.2
 Home-page: https://github.com/allenai/beaker-py
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beaker-py Version: 1.9.1 Home-page: https://
+Metadata-Version: 2.1 Name: beaker-py Version: 1.9.2 Home-page: https://
 github.com/allenai/beaker-py Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Classifier:
 Intended Audience :: Science/Research Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `beaker-py-1.9.1/beaker_py.egg-info/SOURCES.txt` & `beaker-py-1.9.2/beaker_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beaker-py-1.9.1/setup.py` & `beaker-py-1.9.2/setup.py`

 * *Files identical despite different names*

