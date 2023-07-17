# Comparing `tmp/tasq_cli-1.0.8.tar.gz` & `tmp/tasq_cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasq_cli-1.0.8.tar", last modified: Mon Nov 23 13:11:56 2020, max compression
+gzip compressed data, was "tasq_cli-1.0.9.tar", last modified: Mon Nov 30 10:02:09 2020, max compression
```

## Comparing `tasq_cli-1.0.8.tar` & `tasq_cli-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      683 2020-11-23 13:00:58.112191 tasq_cli-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       25 2020-10-26 13:33:47.403952 tasq_cli-1.0.8/tasq_cli/__init__.py
--rw-r--r--   0        0        0       26 2020-10-26 13:33:58.380981 tasq_cli-1.0.8/tasq_cli/__main__.py
--rw-r--r--   0        0        0     2235 2020-11-04 07:22:21.868253 tasq_cli-1.0.8/tasq_cli/db.py
--rw-r--r--   0        0        0        0 2020-10-26 13:31:01.792020 tasq_cli-1.0.8/tasq_cli/entrypoint.py
--rw-r--r--   0        0        0     3160 2020-11-04 07:27:55.295226 tasq_cli-1.0.8/tasq_cli/main.py
--rw-r--r--   0        0        0     1559 2020-11-23 13:02:17.678115 tasq_cli-1.0.8/tasq_cli/settings.py
--rw-r--r--   0        0        0     8263 2020-11-23 13:06:29.702500 tasq_cli-1.0.8/tasq_cli/upload.py
--rw-r--r--   0        0        0     1267 2020-09-18 12:46:18.998445 tasq_cli-1.0.8/tasq_cli/utils.py
--rw-r--r--   0        0        0     1116 2020-11-23 13:11:56.811917 tasq_cli-1.0.8/setup.py
--rw-r--r--   0        0        0     1056 2020-11-23 13:11:56.812583 tasq_cli-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      683 2020-11-30 10:01:01.896972 tasq_cli-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       25 2020-10-26 13:33:47.403952 tasq_cli-1.0.9/tasq_cli/__init__.py
+-rw-r--r--   0        0        0       26 2020-10-26 13:33:58.380981 tasq_cli-1.0.9/tasq_cli/__main__.py
+-rw-r--r--   0        0        0     2235 2020-11-04 07:22:21.868253 tasq_cli-1.0.9/tasq_cli/db.py
+-rw-r--r--   0        0        0        0 2020-10-26 13:31:01.792020 tasq_cli-1.0.9/tasq_cli/entrypoint.py
+-rw-r--r--   0        0        0     3160 2020-11-04 07:27:55.295226 tasq_cli-1.0.9/tasq_cli/main.py
+-rw-r--r--   0        0        0     1559 2020-11-30 10:01:10.790505 tasq_cli-1.0.9/tasq_cli/settings.py
+-rw-r--r--   0        0        0     8265 2020-11-30 10:00:49.686688 tasq_cli-1.0.9/tasq_cli/upload.py
+-rw-r--r--   0        0        0     1267 2020-09-18 12:46:18.998445 tasq_cli-1.0.9/tasq_cli/utils.py
+-rw-r--r--   0        0        0     1116 2020-11-30 10:02:09.494312 tasq_cli-1.0.9/setup.py
+-rw-r--r--   0        0        0     1056 2020-11-30 10:02:09.495044 tasq_cli-1.0.9/PKG-INFO
```

### Comparing `tasq_cli-1.0.8/pyproject.toml` & `tasq_cli-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tasq_cli"
-version = "1.0.8"
+version = "1.0.9"
 description = "The command line tool for tasq.ai."
 authors = ["tasq.ai <info@tasq.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 altgraph = "^0.17"
 boto3 = "^1.16.4"
```

### Comparing `tasq_cli-1.0.8/tasq_cli/db.py` & `tasq_cli-1.0.9/tasq_cli/db.py`

 * *Files identical despite different names*

### Comparing `tasq_cli-1.0.8/tasq_cli/main.py` & `tasq_cli-1.0.9/tasq_cli/main.py`

 * *Files identical despite different names*

### Comparing `tasq_cli-1.0.8/tasq_cli/settings.py` & `tasq_cli-1.0.9/tasq_cli/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 from tasq_cli.utils import get_config_directory, get_config_file_path, get_credentials
 
 KB = 1024
 MB = KB * 1024
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 # ---
 # Logging
 # ---
 
 def setup_logger():
     logger = logging.getLogger('Tasq CLI')
```

### Comparing `tasq_cli-1.0.8/tasq_cli/upload.py` & `tasq_cli-1.0.9/tasq_cli/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                     Body=image_wrapper,
                     Bucket=settings.BUCKET,
                     Key=object_name,
                     ContentMD5=content_md5,
                     # TODO this is questionable
                     # we might not want to make these
                     # public in the long term
-                    ACL='public-read'
+                    # ACL='public-read'
                     # NOTE
                     # consider that sync might work faster than put_object
                 )
                 if response['ResponseMetadata']['HTTPStatusCode'] == 200 and response['ETag'] == f'"{md5_hash}"':
                     tag_response = client.put_object_tagging(
                         Bucket=settings.BUCKET,
                         Key=object_name,
```

### Comparing `tasq_cli-1.0.8/tasq_cli/utils.py` & `tasq_cli-1.0.9/tasq_cli/utils.py`

 * *Files identical despite different names*

### Comparing `tasq_cli-1.0.8/setup.py` & `tasq_cli-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'urllib3>=1.25.11,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['tasq = tasq_cli.main:main']}
 
 setup_kwargs = {
     'name': 'tasq-cli',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'The command line tool for tasq.ai.',
     'long_description': None,
     'author': 'tasq.ai',
     'author_email': 'info@tasq.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tasq_cli-1.0.8/PKG-INFO` & `tasq_cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasq-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: The command line tool for tasq.ai.
 Author: tasq.ai
 Author-email: info@tasq.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

