# Comparing `tmp/image_sky-0.3.0.tar.gz` & `tmp/image_sky-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\image_sky-0.3.0.tar", last modified: Mon Jul 17 08:29:03 2023, max compression
+gzip compressed data, was "dist\image_sky-0.4.0.tar", last modified: Mon Jul 17 09:05:21 2023, max compression
```

## Comparing `image_sky-0.3.0.tar` & `image_sky-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/
--rw-rw-rw-   0        0        0      288 2018-11-30 15:41:32.000000 image_sky-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      369 2023-07-17 08:29:03.000000 image_sky-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      623 2018-11-30 15:41:32.000000 image_sky-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/
--rw-rw-rw-   0        0        0     1223 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/__init__.py
--rw-rw-rw-   0        0        0    13624 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/ec2standalone.py
--rw-rw-rw-   0        0        0    14322 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/executor.py
--rw-rw-rw-   0        0        0     5124 2023-07-15 09:01:16.000000 image_sky-0.3.0/image_sky/fun_client.py
--rw-rw-rw-   0        0        0     9661 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/future.py
--rw-rw-rw-   0        0        0     4111 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/invokers.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/jobrunner/
--rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/jobrunner/__init__.py
--rw-rw-rw-   0        0        0     7565 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/jobrunner/jobrunner.py
--rw-rw-rw-   0        0        0     2032 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/local.py
--rw-rw-rw-   0        0        0     2587 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/queues.py
--rw-rw-rw-   0        0        0     1401 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/runtime.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/scripts/
--rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/scripts/__init__.py
--rw-rw-rw-   0        0        0    26647 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/scripts/pywrencli.py
--rw-rw-rw-   0        0        0     9676 2023-07-17 07:27:04.000000 image_sky-0.3.0/image_sky/scripts/setupscript.py
--rw-rw-rw-   0        0        0    14338 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/scripts/standalone.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/serialize/
--rw-rw-rw-   0        0        0     1649 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/serialize/cloudpickle/
--rw-rw-rw-   0        0        0     1666 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/serialize/cloudpickle/__init__.py
--rw-rw-rw-   0        0        0    36260 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/serialize/cloudpickle/cloudpickle.py
--rw-rw-rw-   0        0        0     9326 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/serialize/default_preinstalls.py
--rw-rw-rw-   0        0        0    14191 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/serialize/module_dependency.py
--rw-rw-rw-   0        0        0     4061 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/serialize/serialize.py
--rw-rw-rw-   0        0        0     2395 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/serialize/util.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky/storage/
--rw-rw-rw-   0        0        0     2823 2023-07-12 07:13:49.000000 image_sky-0.3.0/image_sky/storage/OssBackend.py
--rw-rw-rw-   0        0        0      764 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/storage/__init__.py
--rw-rw-rw-   0        0        0     1288 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/storage/exceptions.py
--rw-rw-rw-   0        0        0     3163 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/storage/s3_backend.py
--rw-rw-rw-   0        0        0     5522 2023-07-12 04:51:55.000000 image_sky-0.3.0/image_sky/storage/storage.py
--rw-rw-rw-   0        0        0     3630 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/storage/storage_utils.py
--rw-rw-rw-   0        0        0      322 2023-07-15 10:23:32.000000 image_sky-0.3.0/image_sky/test.py
--rw-rw-rw-   0        0        0      789 2023-07-17 08:28:52.000000 image_sky-0.3.0/image_sky/version.py
--rw-rw-rw-   0        0        0     7236 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/wait.py
--rw-rw-rw-   0        0        0     3945 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/wren.py
--rw-rw-rw-   0        0        0     6486 2023-07-15 10:23:31.000000 image_sky-0.3.0/image_sky/wrenconfig.py
--rw-rw-rw-   0        0        0    19811 2023-07-12 03:41:34.000000 image_sky-0.3.0/image_sky/wrenhandler.py
--rw-rw-rw-   0        0        0     1553 2018-11-30 15:41:32.000000 image_sky-0.3.0/image_sky/wrenlogging.py
--rw-rw-rw-   0        0        0     3496 2023-07-10 09:19:48.000000 image_sky-0.3.0/image_sky/wrenutil.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/
--rw-rw-rw-   0        0        0      369 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       74 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      185 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 08:29:03.000000 image_sky-0.3.0/image_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 08:29:03.000000 image_sky-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2579 2023-07-15 10:55:23.000000 image_sky-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/
+-rw-rw-rw-   0        0        0      288 2018-11-30 15:41:32.000000 image_sky-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      369 2023-07-17 09:05:21.000000 image_sky-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2018-11-30 15:41:32.000000 image_sky-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/
+-rw-rw-rw-   0        0        0     1223 2023-07-15 10:23:32.000000 image_sky-0.4.0/image_sky/__init__.py
+-rw-rw-rw-   0        0        0    13624 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/ec2standalone.py
+-rw-rw-rw-   0        0        0    14322 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/executor.py
+-rw-rw-rw-   0        0        0     5124 2023-07-15 09:01:16.000000 image_sky-0.4.0/image_sky/fun_client.py
+-rw-rw-rw-   0        0        0     9661 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/future.py
+-rw-rw-rw-   0        0        0     4111 2023-07-15 10:23:32.000000 image_sky-0.4.0/image_sky/invokers.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/jobrunner/
+-rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/jobrunner/__init__.py
+-rw-rw-rw-   0        0        0     7565 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/jobrunner/jobrunner.py
+-rw-rw-rw-   0        0        0     2032 2023-07-15 10:23:32.000000 image_sky-0.4.0/image_sky/local.py
+-rw-rw-rw-   0        0        0     2587 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/queues.py
+-rw-rw-rw-   0        0        0     1401 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/runtime.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/scripts/
+-rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/scripts/__init__.py
+-rw-rw-rw-   0        0        0    26647 2023-07-15 10:23:32.000000 image_sky-0.4.0/image_sky/scripts/pywrencli.py
+-rw-rw-rw-   0        0        0     9676 2023-07-17 08:51:05.000000 image_sky-0.4.0/image_sky/scripts/setupscript.py
+-rw-rw-rw-   0        0        0    14338 2023-07-15 10:23:32.000000 image_sky-0.4.0/image_sky/scripts/standalone.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/serialize/
+-rw-rw-rw-   0        0        0     1649 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/serialize/cloudpickle/
+-rw-rw-rw-   0        0        0     1666 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/serialize/cloudpickle/__init__.py
+-rw-rw-rw-   0        0        0    36260 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/serialize/cloudpickle/cloudpickle.py
+-rw-rw-rw-   0        0        0     9326 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/serialize/default_preinstalls.py
+-rw-rw-rw-   0        0        0    14191 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/serialize/module_dependency.py
+-rw-rw-rw-   0        0        0     4061 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/serialize/serialize.py
+-rw-rw-rw-   0        0        0     2395 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/serialize/util.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky/storage/
+-rw-rw-rw-   0        0        0     2823 2023-07-12 07:13:49.000000 image_sky-0.4.0/image_sky/storage/OssBackend.py
+-rw-rw-rw-   0        0        0      764 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/storage/__init__.py
+-rw-rw-rw-   0        0        0     1288 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/storage/exceptions.py
+-rw-rw-rw-   0        0        0     3163 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/storage/s3_backend.py
+-rw-rw-rw-   0        0        0     5522 2023-07-12 04:51:55.000000 image_sky-0.4.0/image_sky/storage/storage.py
+-rw-rw-rw-   0        0        0     3630 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/storage/storage_utils.py
+-rw-rw-rw-   0        0        0      789 2023-07-17 09:05:06.000000 image_sky-0.4.0/image_sky/version.py
+-rw-rw-rw-   0        0        0     7236 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/wait.py
+-rw-rw-rw-   0        0        0     3945 2023-07-15 10:23:31.000000 image_sky-0.4.0/image_sky/wren.py
+-rw-rw-rw-   0        0        0     6279 2023-07-17 09:02:16.000000 image_sky-0.4.0/image_sky/wrenconfig.py
+-rw-rw-rw-   0        0        0    19811 2023-07-12 03:41:34.000000 image_sky-0.4.0/image_sky/wrenhandler.py
+-rw-rw-rw-   0        0        0     1553 2018-11-30 15:41:32.000000 image_sky-0.4.0/image_sky/wrenlogging.py
+-rw-rw-rw-   0        0        0     3496 2023-07-10 09:19:48.000000 image_sky-0.4.0/image_sky/wrenutil.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       74 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      185 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 09:05:21.000000 image_sky-0.4.0/image_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:05:21.000000 image_sky-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2579 2023-07-15 10:55:23.000000 image_sky-0.4.0/setup.py
```

### Comparing `image_sky-0.3.0/README.md` & `image_sky-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/__init__.py` & `image_sky-0.4.0/image_sky/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/ec2standalone.py` & `image_sky-0.4.0/image_sky/ec2standalone.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/executor.py` & `image_sky-0.4.0/image_sky/executor.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/fun_client.py` & `image_sky-0.4.0/image_sky/fun_client.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/future.py` & `image_sky-0.4.0/image_sky/future.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/invokers.py` & `image_sky-0.4.0/image_sky/invokers.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/jobrunner/__init__.py` & `image_sky-0.4.0/image_sky/jobrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/jobrunner/jobrunner.py` & `image_sky-0.4.0/image_sky/jobrunner/jobrunner.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/local.py` & `image_sky-0.4.0/image_sky/local.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/queues.py` & `image_sky-0.4.0/image_sky/queues.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/runtime.py` & `image_sky-0.4.0/image_sky/runtime.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/scripts/__init__.py` & `image_sky-0.4.0/image_sky/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/scripts/pywrencli.py` & `image_sky-0.4.0/image_sky/scripts/pywrencli.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/scripts/setupscript.py` & `image_sky-0.4.0/image_sky/scripts/setupscript.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         if error_code == 404:
             exists = False
     except Exception as e:
         raise e
     return exists
 
 def create_unique_bucket_name():
-    bucket_name = "{}-image_sky-{}".format(get_username().lower(),
+    bucket_name = "{}-image-sky-{}".format(get_username().lower(),
                                         random.randint(0, 999))
     return bucket_name
 
 def check_valid_bucket_name(bucket_name):
     # Validates bucketname
     # Based on http://info.easydynamics.com/blog/aws-s3-bucket-name-validation-regex
     # https://docs.aws.amazon.com/AmazonS3/latest/dev/BucketRestrictions.html
```

### Comparing `image_sky-0.3.0/image_sky/scripts/standalone.py` & `image_sky-0.4.0/image_sky/scripts/standalone.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/__init__.py` & `image_sky-0.4.0/image_sky/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/cloudpickle/__init__.py` & `image_sky-0.4.0/image_sky/serialize/cloudpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/cloudpickle/cloudpickle.py` & `image_sky-0.4.0/image_sky/serialize/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/default_preinstalls.py` & `image_sky-0.4.0/image_sky/serialize/default_preinstalls.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/module_dependency.py` & `image_sky-0.4.0/image_sky/serialize/module_dependency.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/serialize.py` & `image_sky-0.4.0/image_sky/serialize/serialize.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/serialize/util.py` & `image_sky-0.4.0/image_sky/serialize/util.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/OssBackend.py` & `image_sky-0.4.0/image_sky/storage/OssBackend.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/__init__.py` & `image_sky-0.4.0/image_sky/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/exceptions.py` & `image_sky-0.4.0/image_sky/storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/s3_backend.py` & `image_sky-0.4.0/image_sky/storage/s3_backend.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/storage.py` & `image_sky-0.4.0/image_sky/storage/storage.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/storage/storage_utils.py` & `image_sky-0.4.0/image_sky/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/version.py` & `image_sky-0.4.0/image_sky/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 # limitations under the License.
 #
 
 from __future__ import print_function
 # we're following the version number guidelines
 # from https://www.python.org/dev/peps/pep-0386/
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 if __name__ == "__main__":
     print(__version__)
```

### Comparing `image_sky-0.3.0/image_sky/wait.py` & `image_sky-0.4.0/image_sky/wait.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/wren.py` & `image_sky-0.4.0/image_sky/wren.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/wrenconfig.py` & `image_sky-0.4.0/image_sky/wrenconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,24 @@
 ROLE = "arn:aws:iam::{}:role/{}".format(AWS_ACCOUNT_ID, AWS_ROLE)
 
 AWS_REGION_DEFAULT = 'cn-beijing'
 SERVICE_NAME = 'test'
 USER_ID = '1653787918608878'
 AWS_S3_BUCKET_DEFAULT = "image_sky.data"
 AWS_S3_PREFIX_DEFAULT = "image_sky.jobs"
-AWS_LAMBDA_ROLE_DEFAULT = 'pywren_exec_role_1'
-AWS_LAMBDA_FUNCTION_NAME_DEFAULT = 'pywren_1'
+AWS_LAMBDA_ROLE_DEFAULT = 'image_sky_exec_role_1'
+AWS_LAMBDA_FUNCTION_NAME_DEFAULT = 'image_sky_1'
 AWS_SQS_QUEUE_DEFAULT = 'image_sky-jobs-1'
 
 MAX_AGG_DATA_SIZE = 4e6
 
 DEFAULT_KEY_NAME = "PYWREN_DEFAULT_KEY"
 
-default_runtime = {'2.7' : "image_sky.runtimes/default_2.7.meta.json",
-                   '3.4' : "image_sky.runtimes/default_3.4.meta.json",
-                   '3.5' : "image_sky.runtimes/default_3.5.meta.json",
-                   '3.6' : "image_sky.runtime/pywren_runtime-3.6-default.meta.json",
-                   '3.7' : "image_sky.runtime/pywren_runtime-3.7-default.meta.json"}
+default_runtime = {'3.6' : "pywren.runtime/pywren_runtime-3.6-default.meta.json",
+                   '3.7' : "pywren.runtime/pywren_runtime-3.7-default.meta.json"}
 
 def load(config_filename):
     import yaml
     res = yaml.safe_load(open(config_filename, 'r'))
     # sanity check
     if res['s3']['bucket'] == 'BUCKET_NAME':
         raise Exception(
@@ -61,30 +58,30 @@
         res = patch_storage_config(res)
     if res['standalone']['ec2_ssh_key'] == DEFAULT_KEY_NAME:
         res['standalone']['ec2_ssh_key'] = None
 
     return res
 
 def get_default_home_filename():
-    default_home_filename = os.path.join(os.path.expanduser("~/.pywren_config_aliyun"))
+    default_home_filename = os.path.join(os.path.expanduser("~/.imageSky_config_aliyun"))
     return default_home_filename
 
 
 def get_default_config_filename():
     """
     First checks .pywren_config
     then checks PYWREN_CONFIG_FILE environment variable
     then ~/.pywren_config
     """
     if 'PYWREN_CONFIG_FILE' in os.environ:
         config_filename = os.environ['PYWREN_CONFIG_FILE']
         # FIXME log this
 
-    elif os.path.exists(".pywren_config_aliyun"):
-        config_filename = os.path.abspath('.pywren_config_aliyun')
+    elif os.path.exists(".imageSky_config_aliyun"):
+        config_filename = os.path.abspath('.imageSky_config_aliyun')
 
     else:
         config_filename = get_default_home_filename()
 
     return config_filename
 
 def patch_storage_config(config_data):
```

### Comparing `image_sky-0.3.0/image_sky/wrenhandler.py` & `image_sky-0.4.0/image_sky/wrenhandler.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/wrenlogging.py` & `image_sky-0.4.0/image_sky/wrenlogging.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky/wrenutil.py` & `image_sky-0.4.0/image_sky/wrenutil.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.3.0/image_sky.egg-info/SOURCES.txt` & `image_sky-0.4.0/image_sky.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 image_sky/executor.py
 image_sky/fun_client.py
 image_sky/future.py
 image_sky/invokers.py
 image_sky/local.py
 image_sky/queues.py
 image_sky/runtime.py
-image_sky/test.py
 image_sky/version.py
 image_sky/wait.py
 image_sky/wren.py
 image_sky/wrenconfig.py
 image_sky/wrenhandler.py
 image_sky/wrenlogging.py
 image_sky/wrenutil.py
```

### Comparing `image_sky-0.3.0/setup.py` & `image_sky-0.4.0/setup.py`

 * *Files identical despite different names*

