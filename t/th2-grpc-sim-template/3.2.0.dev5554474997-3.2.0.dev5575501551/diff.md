# Comparing `tmp/th2_grpc_sim_template-3.2.0.dev5554474997.tar.gz` & `tmp/th2_grpc_sim_template-3.2.0.dev5575501551.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim_template-3.2.0.dev5554474997.tar", last modified: Fri Jul 14 13:13:24 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim_template-3.2.0.dev5575501551.tar", last modified: Mon Jul 17 12:19:26 2023, max compression
```

## Comparing `th2_grpc_sim_template-3.2.0.dev5554474997.tar` & `th2_grpc_sim_template-3.2.0.dev5575501551.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4600 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-14 13:12:26.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-14 13:13:03.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-14 13:13:24.000000 th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-17 12:18:20.000000 th2_grpc_sim_template-3.2.0.dev5575501551/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-17 12:18:21.000000 th2_grpc_sim_template-3.2.0.dev5575501551/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-07-17 12:18:20.000000 th2_grpc_sim_template-3.2.0.dev5575501551/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 12:19:25.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 12:19:25.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-17 12:18:20.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-07-17 12:19:25.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-07-17 12:19:25.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     6063 2023-07-17 12:19:25.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-17 12:19:03.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-17 12:19:26.000000 th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/PKG-INFO` & `th2_grpc_sim_template-3.2.0.dev5575501551/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim_template
-Version: 3.2.0.dev5554474997
+Version: 3.2.0.dev5575501551
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
```

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/README.md` & `th2_grpc_sim_template-3.2.0.dev5575501551/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/setup.py` & `th2_grpc_sim_template-3.2.0.dev5575501551/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,15 @@
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-sim-template',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
         'th2-grpc-sim~=5.1.0.dev',
-        'th2-grpc-common~=4.3.0.dev',
-        'grpcio-tools==1.56.0'
+        'th2-grpc-common~=4.3.0.dev'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template.proto` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.py` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2.pyi` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_pb2_grpc.py` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template/sim_template_service.py` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template/sim_template_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/PKG-INFO` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim-template
-Version: 3.2.0.dev5554474997
+Version: 3.2.0.dev5575501551
 Summary: th2_grpc_sim_template
 Home-page: https://github.com/th2-net/th2-grpc-sim-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim template library
```

### Comparing `th2_grpc_sim_template-3.2.0.dev5554474997/th2_grpc_sim_template.egg-info/SOURCES.txt` & `th2_grpc_sim_template-3.2.0.dev5575501551/th2_grpc_sim_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

