# Comparing `tmp/offlinerllib-0.0.8.tar.gz` & `tmp/offlinerllib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinerllib-0.0.8.tar", last modified: Tue Jun 27 12:35:35 2023, max compression
+gzip compressed data, was "offlinerllib-0.0.9.tar", last modified: Mon Jul 17 01:34:41 2023, max compression
```

## Comparing `offlinerllib-0.0.8.tar` & `offlinerllib-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.514042 offlinerllib-0.0.8/offlinerllib/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/d4rl_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/buffer/lap_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/env/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/d4rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/env/mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32225 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/module/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/net/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/module/td7_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/policy/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib/policy/model_free/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/awac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/edac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/inac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/iql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/sacn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td3bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/td7.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/xql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/offlinerllib/policy/model_free/xsac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/offlinerllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 12:35:35.000000 offlinerllib-0.0.8/offlinerllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:35:35.518042 offlinerllib-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-27 12:35:27.000000 offlinerllib-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.997387 offlinerllib-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-17 01:34:40.997387 offlinerllib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.989387 offlinerllib-0.0.9/offlinerllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.989387 offlinerllib-0.0.9/offlinerllib/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/buffer/d4rl_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/buffer/lap_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.989387 offlinerllib-0.0.9/offlinerllib/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/env/d4rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/env/mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.993387 offlinerllib-0.0.9/offlinerllib/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32225 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.993387 offlinerllib-0.0.9/offlinerllib/module/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/module/td7_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.993387 offlinerllib-0.0.9/offlinerllib/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.993387 offlinerllib-0.0.9/offlinerllib/policy/model_free/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/awac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/edac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/inac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/iql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/sacn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/td3bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/td7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/xql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/policy/model_free/xsac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.997387 offlinerllib-0.0.9/offlinerllib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/d4rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/offlinerllib/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:34:40.989387 offlinerllib-0.0.9/offlinerllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-17 01:34:40.000000 offlinerllib-0.0.9/offlinerllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-17 01:34:40.000000 offlinerllib-0.0.9/offlinerllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 01:34:40.000000 offlinerllib-0.0.9/offlinerllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 01:34:40.000000 offlinerllib-0.0.9/offlinerllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 01:34:40.000000 offlinerllib-0.0.9/offlinerllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 01:34:40.997387 offlinerllib-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-17 01:34:29.000000 offlinerllib-0.0.9/setup.py
```

### Comparing `offlinerllib-0.0.8/LICENSE` & `offlinerllib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/PKG-INFO` & `offlinerllib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.8/README.md` & `offlinerllib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/buffer/d4rl_buffer.py` & `offlinerllib-0.0.9/offlinerllib/buffer/d4rl_buffer.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/buffer/lap_buffer.py` & `offlinerllib-0.0.9/offlinerllib/buffer/lap_buffer.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/env/__init__.py` & `offlinerllib-0.0.9/offlinerllib/env/__init__.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/env/d4rl.py` & `offlinerllib-0.0.9/offlinerllib/env/d4rl.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/env/mixed.py` & `offlinerllib-0.0.9/offlinerllib/env/mixed.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/module/actor.py` & `offlinerllib-0.0.9/offlinerllib/module/actor.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/module/critic.py` & `offlinerllib-0.0.9/offlinerllib/module/critic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/module/net/basic.py` & `offlinerllib-0.0.9/offlinerllib/module/net/basic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/module/net/mlp.py` & `offlinerllib-0.0.9/offlinerllib/module/net/mlp.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/module/td7_net.py` & `offlinerllib-0.0.9/offlinerllib/module/td7_net.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/awac.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/awac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/dt.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/dt.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/edac.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/edac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/inac.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/inac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/iql.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/iql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/sac.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/sac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/sacn.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/sacn.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/td3.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/td3.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/td3bc.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/td3bc.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/td7.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/td7.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/xql.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/xql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib/policy/model_free/xsac.py` & `offlinerllib-0.0.9/offlinerllib/policy/model_free/xsac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.8/offlinerllib.egg-info/PKG-INFO` & `offlinerllib-0.0.9/offlinerllib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.8/offlinerllib.egg-info/SOURCES.txt` & `offlinerllib-0.0.9/offlinerllib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,16 @@
 offlinerllib/policy/model_free/iql.py
 offlinerllib/policy/model_free/sac.py
 offlinerllib/policy/model_free/sacn.py
 offlinerllib/policy/model_free/td3.py
 offlinerllib/policy/model_free/td3bc.py
 offlinerllib/policy/model_free/td7.py
 offlinerllib/policy/model_free/xql.py
-offlinerllib/policy/model_free/xsac.py
+offlinerllib/policy/model_free/xsac.py
+offlinerllib/utils/__init__.py
+offlinerllib/utils/d4rl.py
+offlinerllib/utils/distributions.py
+offlinerllib/utils/eval.py
+offlinerllib/utils/functional.py
+offlinerllib/utils/misc.py
+offlinerllib/utils/noise.py
+offlinerllib/utils/terminal.py
```

### Comparing `offlinerllib-0.0.8/setup.py` & `offlinerllib-0.0.9/setup.py`

 * *Files identical despite different names*

