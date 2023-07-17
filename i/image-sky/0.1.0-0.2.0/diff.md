# Comparing `tmp/image_sky-0.1.0.tar.gz` & `tmp/image_sky-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\image_sky-0.1.0.tar", last modified: Sat Jul 15 10:35:37 2023, max compression
+gzip compressed data, was "dist\image_sky-0.2.0.tar", last modified: Mon Jul 17 07:30:34 2023, max compression
```

## Comparing `image_sky-0.1.0.tar` & `image_sky-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/
--rw-rw-rw-   0        0        0      288 2018-11-30 15:41:32.000000 image_sky-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      380 2023-07-15 10:35:37.000000 image_sky-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      623 2018-11-30 15:41:32.000000 image_sky-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/
--rw-rw-rw-   0        0        0     1223 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/__init__.py
--rw-rw-rw-   0        0        0    13624 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/ec2standalone.py
--rw-rw-rw-   0        0        0    14322 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/executor.py
--rw-rw-rw-   0        0        0     5124 2023-07-15 09:01:16.000000 image_sky-0.1.0/image_sky/fun_client.py
--rw-rw-rw-   0        0        0     9661 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/future.py
--rw-rw-rw-   0        0        0     4111 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/invokers.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/jobrunner/
--rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/jobrunner/__init__.py
--rw-rw-rw-   0        0        0     7565 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/jobrunner/jobrunner.py
--rw-rw-rw-   0        0        0     2032 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/local.py
--rw-rw-rw-   0        0        0     2587 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/queues.py
--rw-rw-rw-   0        0        0     1401 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/runtime.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/scripts/
--rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/scripts/__init__.py
--rw-rw-rw-   0        0        0    26647 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/scripts/pywrencli.py
--rw-rw-rw-   0        0        0     9657 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/scripts/setupscript.py
--rw-rw-rw-   0        0        0    14338 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/scripts/standalone.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/serialize/
--rw-rw-rw-   0        0        0     1649 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/serialize/cloudpickle/
--rw-rw-rw-   0        0        0     1666 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/serialize/cloudpickle/__init__.py
--rw-rw-rw-   0        0        0    36260 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/serialize/cloudpickle/cloudpickle.py
--rw-rw-rw-   0        0        0     9326 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/serialize/default_preinstalls.py
--rw-rw-rw-   0        0        0    14191 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/serialize/module_dependency.py
--rw-rw-rw-   0        0        0     4061 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/serialize/serialize.py
--rw-rw-rw-   0        0        0     2395 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/serialize/util.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky/storage/
--rw-rw-rw-   0        0        0     2823 2023-07-12 07:13:49.000000 image_sky-0.1.0/image_sky/storage/OssBackend.py
--rw-rw-rw-   0        0        0      764 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/storage/__init__.py
--rw-rw-rw-   0        0        0     1288 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/storage/exceptions.py
--rw-rw-rw-   0        0        0     3163 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/storage/s3_backend.py
--rw-rw-rw-   0        0        0     5522 2023-07-12 04:51:55.000000 image_sky-0.1.0/image_sky/storage/storage.py
--rw-rw-rw-   0        0        0     3630 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/storage/storage_utils.py
--rw-rw-rw-   0        0        0      322 2023-07-15 10:23:32.000000 image_sky-0.1.0/image_sky/test.py
--rw-rw-rw-   0        0        0      789 2023-07-15 10:20:34.000000 image_sky-0.1.0/image_sky/version.py
--rw-rw-rw-   0        0        0     7236 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/wait.py
--rw-rw-rw-   0        0        0     3945 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/wren.py
--rw-rw-rw-   0        0        0     6486 2023-07-15 10:23:31.000000 image_sky-0.1.0/image_sky/wrenconfig.py
--rw-rw-rw-   0        0        0    19811 2023-07-12 03:41:34.000000 image_sky-0.1.0/image_sky/wrenhandler.py
--rw-rw-rw-   0        0        0     1553 2018-11-30 15:41:32.000000 image_sky-0.1.0/image_sky/wrenlogging.py
--rw-rw-rw-   0        0        0     3496 2023-07-10 09:19:48.000000 image_sky-0.1.0/image_sky/wrenutil.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/
--rw-rw-rw-   0        0        0      380 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       74 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      185 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 10:35:37.000000 image_sky-0.1.0/image_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 10:35:37.000000 image_sky-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2590 2023-07-15 10:23:32.000000 image_sky-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/
+-rw-rw-rw-   0        0        0      288 2018-11-30 15:41:32.000000 image_sky-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      369 2023-07-17 07:30:34.000000 image_sky-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2018-11-30 15:41:32.000000 image_sky-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/
+-rw-rw-rw-   0        0        0     1223 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/__init__.py
+-rw-rw-rw-   0        0        0    13624 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/ec2standalone.py
+-rw-rw-rw-   0        0        0    14322 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/executor.py
+-rw-rw-rw-   0        0        0     5124 2023-07-15 09:01:16.000000 image_sky-0.2.0/image_sky/fun_client.py
+-rw-rw-rw-   0        0        0     9661 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/future.py
+-rw-rw-rw-   0        0        0     4111 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/invokers.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/jobrunner/
+-rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/jobrunner/__init__.py
+-rw-rw-rw-   0        0        0     7565 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/jobrunner/jobrunner.py
+-rw-rw-rw-   0        0        0     2032 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/local.py
+-rw-rw-rw-   0        0        0     2587 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/queues.py
+-rw-rw-rw-   0        0        0     1401 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/runtime.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/scripts/
+-rw-rw-rw-   0        0        0      579 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/scripts/__init__.py
+-rw-rw-rw-   0        0        0    26647 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/scripts/pywrencli.py
+-rw-rw-rw-   0        0        0     9676 2023-07-17 07:27:04.000000 image_sky-0.2.0/image_sky/scripts/setupscript.py
+-rw-rw-rw-   0        0        0    14338 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/scripts/standalone.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/serialize/
+-rw-rw-rw-   0        0        0     1649 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/serialize/cloudpickle/
+-rw-rw-rw-   0        0        0     1666 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/serialize/cloudpickle/__init__.py
+-rw-rw-rw-   0        0        0    36260 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/serialize/cloudpickle/cloudpickle.py
+-rw-rw-rw-   0        0        0     9326 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/serialize/default_preinstalls.py
+-rw-rw-rw-   0        0        0    14191 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/serialize/module_dependency.py
+-rw-rw-rw-   0        0        0     4061 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/serialize/serialize.py
+-rw-rw-rw-   0        0        0     2395 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/serialize/util.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky/storage/
+-rw-rw-rw-   0        0        0     2823 2023-07-12 07:13:49.000000 image_sky-0.2.0/image_sky/storage/OssBackend.py
+-rw-rw-rw-   0        0        0      764 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/storage/__init__.py
+-rw-rw-rw-   0        0        0     1288 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/storage/exceptions.py
+-rw-rw-rw-   0        0        0     3163 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/storage/s3_backend.py
+-rw-rw-rw-   0        0        0     5522 2023-07-12 04:51:55.000000 image_sky-0.2.0/image_sky/storage/storage.py
+-rw-rw-rw-   0        0        0     3630 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/storage/storage_utils.py
+-rw-rw-rw-   0        0        0      322 2023-07-15 10:23:32.000000 image_sky-0.2.0/image_sky/test.py
+-rw-rw-rw-   0        0        0      789 2023-07-17 07:29:31.000000 image_sky-0.2.0/image_sky/version.py
+-rw-rw-rw-   0        0        0     7236 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/wait.py
+-rw-rw-rw-   0        0        0     3945 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/wren.py
+-rw-rw-rw-   0        0        0     6486 2023-07-15 10:23:31.000000 image_sky-0.2.0/image_sky/wrenconfig.py
+-rw-rw-rw-   0        0        0    19811 2023-07-12 03:41:34.000000 image_sky-0.2.0/image_sky/wrenhandler.py
+-rw-rw-rw-   0        0        0     1553 2018-11-30 15:41:32.000000 image_sky-0.2.0/image_sky/wrenlogging.py
+-rw-rw-rw-   0        0        0     3496 2023-07-10 09:19:48.000000 image_sky-0.2.0/image_sky/wrenutil.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-07-17 07:30:33.000000 image_sky-0.2.0/image_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-07-17 07:30:34.000000 image_sky-0.2.0/image_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       74 2023-07-17 07:30:33.000000 image_sky-0.2.0/image_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      185 2023-07-17 07:30:33.000000 image_sky-0.2.0/image_sky.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-07-17 07:30:33.000000 image_sky-0.2.0/image_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 07:30:33.000000 image_sky-0.2.0/image_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:30:34.000000 image_sky-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2579 2023-07-15 10:55:23.000000 image_sky-0.2.0/setup.py
```

### Comparing `image_sky-0.1.0/README.md` & `image_sky-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/__init__.py` & `image_sky-0.2.0/image_sky/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/ec2standalone.py` & `image_sky-0.2.0/image_sky/ec2standalone.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/executor.py` & `image_sky-0.2.0/image_sky/executor.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/fun_client.py` & `image_sky-0.2.0/image_sky/fun_client.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/future.py` & `image_sky-0.2.0/image_sky/future.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/invokers.py` & `image_sky-0.2.0/image_sky/invokers.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/jobrunner/__init__.py` & `image_sky-0.2.0/image_sky/jobrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/jobrunner/jobrunner.py` & `image_sky-0.2.0/image_sky/jobrunner/jobrunner.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/local.py` & `image_sky-0.2.0/image_sky/local.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/queues.py` & `image_sky-0.2.0/image_sky/queues.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/runtime.py` & `image_sky-0.2.0/image_sky/runtime.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/scripts/__init__.py` & `image_sky-0.2.0/image_sky/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/scripts/pywrencli.py` & `image_sky-0.2.0/image_sky/scripts/pywrencli.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/scripts/setupscript.py` & `image_sky-0.2.0/image_sky/scripts/setupscript.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,28 +134,28 @@
         """
         Debug suffix for defaults. For automated testing,
         automatically adds a suffix to each default
         """
         return "{}{}".format(key, suffix)
 
 
-    click.echo("This is the PyWren interactive setup script")
+    click.echo("This is the image_sky interactive setup script")
     #first we will try and make sure AWS is set up
 
     # account_id = ctx.invoke(pywrencli.get_aws_account_id, False)
     # click.echo("Your AWS configuration appears to be set up, and your account ID is {}".format(
     #     account_id))
 
-    click.echo("This interactive script will set up your initial PyWren configuration.")
-    click.echo("If this is the first time you are using PyWren then accepting the defaults " + \
+    click.echo("This interactive script will set up your initial image_sky configuration.")
+    click.echo("If this is the first time you are using image_sky then accepting the defaults " + \
                "should be fine.")
 
     # first, what is your default AWS region?
     aws_region = click_validate_prompt(
-        "What is your default aws region?",
+        "What is your default aliyun region?",
         default=image_sky.wrenconfig.AWS_REGION_DEFAULT,
         validate_func=check_aws_region_valid,
         #fail_msg="{} not a valid aws region. valid regions are " + " ".join(get_lambda_regions())
     )
     # # FIXME make sure this is a valid region
     #aws_region = "cn-beijing"
 
@@ -184,48 +184,48 @@
     config_filename = click_validate_prompt(
         "Location for config file: ",
         default=image_sky.wrenconfig.get_default_home_filename(),
         validate_func=check_overwrite_function)
     config_filename = os.path.expanduser(config_filename)
 
     s3_bucket = click_validate_prompt(
-        "PyWren requires an s3 bucket to store intermediate data. " + \
-            "What s3 bucket would you like to use?",
+        "image_sky requires an oss bucket to store intermediate data. " + \
+            "What oss bucket would you like to use?",
         default=create_unique_bucket_name(),
         validate_func=check_valid_bucket_name)
     create_bucket = False
     if not check_bucket_exists(s3_bucket, accessKeyID, accessKeySecret, endpoint):
         create_bucket = click.confirm(
             "Bucket does not currently exist, would you like to create it?", default=True)
 
-    click.echo("PyWren prefixes every object it puts in S3 with a particular prefix.")
+    click.echo("image_sky prefixes every object it puts in oss with a particular prefix.")
     bucket_pywren_prefix = click_validate_prompt(
-        "PyWren s3 prefix: ",
+        "image_sky oss prefix: ",
         default=image_sky.wrenconfig.AWS_S3_PREFIX_DEFAULT,
         validate_func=validate_s3_prefix)
 
     lambda_config_advanced = click.confirm(
-        "Would you like to configure advanced PyWren properties?", default=False)
+        "Would you like to configure advanced image_sky properties?", default=False)
     lambda_role = ds(image_sky.wrenconfig.AWS_LAMBDA_ROLE_DEFAULT)
     function_name = ds(image_sky.wrenconfig.AWS_LAMBDA_FUNCTION_NAME_DEFAULT)
 
     if lambda_config_advanced:
         lambda_role = click_validate_prompt(
-            "Each lambda function runs as a particular"
+            "Each fc function runs as a particular"
             "IAM role. What is the name of the role you"
-            "would like created for your lambda",
+            "would like created for your fc",
             default=lambda_role,
             validate_func=validate_lambda_role_name)
         function_name = click_validate_prompt(
-            "Each lambda function has a particular function name."
+            "Each fc function has a particular function name."
             "What is your function name?",
             default=function_name,
             validate_func=validate_lambda_function_name)
-    click.echo("PyWren standalone mode uses dedicated AWS instances to run PyWren tasks. " + \
-               "This is more flexible, but more expensive with fewer simultaneous workers.")
+    # click.echo("image_sky standalone mode uses dedicated AWS instances to run PyWren tasks. " + \
+    #            "This is more flexible, but more expensive with fewer simultaneous workers.")
     # use_standalone = click.confirm("Would you like to enable PyWren standalone mode?")
 
     click.echo("Creating config {}".format(config_filename))
     ctx.obj = {"config_filename" : config_filename}
     ctx.invoke(pywrencli.create_config,
                aws_region=aws_region,
                service_name=service_name,
@@ -243,15 +243,15 @@
         return
 
     if create_bucket:
         click.echo("Creating bucket {}.".format(s3_bucket))
         ctx.invoke(pywrencli.create_bucket)
     # click.echo("Creating role.")
     # ctx.invoke(pywrencli.create_role)
-    click.echo("Deploying lambda.")
+    click.echo("Deploying fc.")
     ctx.invoke(pywrencli.deploy_lambda)
 
     # if use_standalone:
     #     click.echo("Setting up standalone mode.")
     #     ctx.invoke(pywrencli.create_queue)
     #     ctx.invoke(pywrencli.create_ec2_ssh_key)
     #     ctx.invoke(pywrencli.create_instance_profile)
```

### Comparing `image_sky-0.1.0/image_sky/scripts/standalone.py` & `image_sky-0.2.0/image_sky/scripts/standalone.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/__init__.py` & `image_sky-0.2.0/image_sky/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/cloudpickle/__init__.py` & `image_sky-0.2.0/image_sky/serialize/cloudpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/cloudpickle/cloudpickle.py` & `image_sky-0.2.0/image_sky/serialize/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/default_preinstalls.py` & `image_sky-0.2.0/image_sky/serialize/default_preinstalls.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/module_dependency.py` & `image_sky-0.2.0/image_sky/serialize/module_dependency.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/serialize.py` & `image_sky-0.2.0/image_sky/serialize/serialize.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/serialize/util.py` & `image_sky-0.2.0/image_sky/serialize/util.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/OssBackend.py` & `image_sky-0.2.0/image_sky/storage/OssBackend.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/__init__.py` & `image_sky-0.2.0/image_sky/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/exceptions.py` & `image_sky-0.2.0/image_sky/storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/s3_backend.py` & `image_sky-0.2.0/image_sky/storage/s3_backend.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/storage.py` & `image_sky-0.2.0/image_sky/storage/storage.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/storage/storage_utils.py` & `image_sky-0.2.0/image_sky/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/version.py` & `image_sky-0.2.0/image_sky/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 # limitations under the License.
 #
 
 from __future__ import print_function
 # we're following the version number guidelines
 # from https://www.python.org/dev/peps/pep-0386/
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 if __name__ == "__main__":
     print(__version__)
```

### Comparing `image_sky-0.1.0/image_sky/wait.py` & `image_sky-0.2.0/image_sky/wait.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/wren.py` & `image_sky-0.2.0/image_sky/wren.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/wrenconfig.py` & `image_sky-0.2.0/image_sky/wrenconfig.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/wrenhandler.py` & `image_sky-0.2.0/image_sky/wrenhandler.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/wrenlogging.py` & `image_sky-0.2.0/image_sky/wrenlogging.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky/wrenutil.py` & `image_sky-0.2.0/image_sky/wrenutil.py`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/image_sky.egg-info/SOURCES.txt` & `image_sky-0.2.0/image_sky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_sky-0.1.0/setup.py` & `image_sky-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 # how to get version info into the project
 exec(open('image_sky/version.py').read())
 
 setup(
     name='image_sky',
     version=__version__,
     url='http://pywren.io',
-    author='Eric Jonas',
-    description='Run many jobs transparently on AWS Lambda and other cloud services',
-    long_description="PyWren lets you transparently run your python functions"
-    "on AWS cloud services, including AWS Lambda and AWS EC2.",
-    author_email='jonas@ericjonas.com',
+    author='zhudayong',
+    description='Run many jobs transparently on aliyun fc and other cloud services',
+    long_description="image_sky lets you transparently run your python functions"
+    "on aliyun cloud services, including aliyun fc .",
+    author_email='671850478@qq.com',
     packages=find_packages(),
     install_requires=[
         'Click', 'boto3', 'oss2', 'alibabacloud_tea_console', 'alibabacloud_fc_open20210406', 'PyYAML',
         'enum34', 'flaky', 'glob2',
         'watchtower', 'tblib' # it's nuts that we need both botos
     ],
     tests_requires=[
```

