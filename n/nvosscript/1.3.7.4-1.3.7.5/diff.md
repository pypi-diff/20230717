# Comparing `tmp/nvosscript-1.3.7.4.tar.gz` & `tmp/nvosscript-1.3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.7.4.tar", last modified: Fri Jul 14 09:05:26 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.5.tar", last modified: Mon Jul 17 08:14:14 2023, max compression
```

## Comparing `nvosscript-1.3.7.4.tar` & `nvosscript-1.3.7.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.148304 nvosscript-1.3.7.4/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.4/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 09:05:26.148050 nvosscript-1.3.7.4/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.4/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.137767 nvosscript-1.3.7.4/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.4/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.4/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.4/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.4/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.141550 nvosscript-1.3.7.4/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-14 09:05:26.148355 nvosscript-1.3.7.4/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-14 09:04:49.000000 nvosscript-1.3.7.4/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.144357 nvosscript-1.3.7.4/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.4/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.4/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1024 2023-07-14 09:04:44.000000 nvosscript-1.3.7.4/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     2529 2023-07-14 06:45:43.000000 nvosscript-1.3.7.4/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.146919 nvosscript-1.3.7.4/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.4/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.4/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-14 09:04:53.000000 nvosscript-1.3.7.4/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.4/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.147492 nvosscript-1.3.7.4/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.4/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.902410 nvosscript-1.3.7.5/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.5/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-17 08:14:14.902037 nvosscript-1.3.7.5/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.5/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.877526 nvosscript-1.3.7.5/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.5/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.5/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.5/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.5/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.886992 nvosscript-1.3.7.5/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-17 08:14:14.902466 nvosscript-1.3.7.5/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-17 08:13:24.000000 nvosscript-1.3.7.5/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.890119 nvosscript-1.3.7.5/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.5/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.5/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      748 2023-07-17 07:08:02.000000 nvosscript-1.3.7.5/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3083 2023-07-17 08:12:44.000000 nvosscript-1.3.7.5/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.900531 nvosscript-1.3.7.5/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.5/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.5/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-17 08:13:33.000000 nvosscript-1.3.7.5/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.5/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.901351 nvosscript-1.3.7.5/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.5/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.7.4/LICENSE` & `nvosscript-1.3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/nvos/file.py` & `nvosscript-1.3.7.5/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/nvos/remote.py` & `nvosscript-1.3.7.5/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/nvos/run.py` & `nvosscript-1.3.7.5/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/setup.py` & `nvosscript-1.3.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.7.04',
+    version='1.3.7.05',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.7.4/skyeye/loghandler.py` & `nvosscript-1.3.7.5/skyeye/loghandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,18 @@
         print("please upload correct path")
         return
     logger.info(f" start filter_effective_log {path}")
     logger_list = []
     if not os.path.exists(path) or os.path.isdir(path):
         print(f"{path} not exists or this path is directory,please upload a logger file ")
         return
-
     with open(path, 'r') as f:
         for line in f:
             matchObj = re.search("\d\|\d+\|\d+\|.*", line, re.M | re.I)
             if matchObj:
                 logger_list.append(line)
-            if len(logger_list) == 1000:
-                logger.info(f"filter logger info data is {logger_list}")
-                remote.upload_file(logger_list, os.path.basename(path))
-                logger_list.clear()
 
-    logger.info(f"filter logger info data is {logger_list}")
-    remote.upload_file(logger_list, os.path.basename(path))
+    remote.upload_file_process(logger_list, os.path.basename(path))
```

### Comparing `nvosscript-1.3.7.4/skyeye/remote.py` & `nvosscript-1.3.7.5/skyeye/remote.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import os
 import logging
 import json
+from tqdm import tqdm
 from start import utils,login
 
 
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
     "prod": "https://sky-eye-trace.nioint.com",
@@ -20,34 +21,55 @@
     "dev": "https://soa-tools-dev.nioint.com/#/nvosTool/spaceList",
     "local": "http://127.0.0.1:12800"
 }
 
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 
-def upload_file(data_list,file_name):
+global_var = 0
+
+exist_error = False
+
+def upload_file_process(data_list,fileName):
+    global global_var
+    global exist_error
+    total = int((len(data_list) / 1000) + 1)
+    with tqdm(desc="uploading", total= total) as progress:
+        for index in range(0, total):
+            temp_list = data_list[index * 1000: (index + 1) * 1000]
+            upload_file(temp_list,fileName,index)
+            progress.update(1)
+
+
+
+
+def upload_file(data_list,file_name,index):
+    global global_var
+    global exist_error
     get_current_env()
     url = daemon_network + "/v3/vehicleLogs"
     header = {
         "content-type": "application/x-www-form-urlencoded"
     }
 
     params = {
         "logDataList": data_list,
         "username": login.get_user_id(),
-        "fileName": file_name
+        "fileName": file_name,
+        "index": index
     }
     logger.info(f'request url:{url} params:{params}')
     r = requests.post(url, headers=header, data=params)
     logger.info(f"response status_code: {r.status_code} text: {r.text} ")
     if r.status_code == 200:
         result = r.text
         if result == "SUCCESS":
-            print("upload success")
+            global_var = global_var + 1
         else:
+            exist_error = True
             print("upload fail ,Please try again later.")
     return {}
 
 
 
 def get_current_env():
     global daemon_network
```

### Comparing `nvosscript-1.3.7.4/start/login.py` & `nvosscript-1.3.7.5/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/start/main.py` & `nvosscript-1.3.7.5/start/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.7.04")
+        print("1.3.7.05")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.7.4/start/utils.py` & `nvosscript-1.3.7.5/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.4/win/win_auto_script.py` & `nvosscript-1.3.7.5/win/win_auto_script.py`

 * *Files identical despite different names*

