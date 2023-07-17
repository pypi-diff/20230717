# Comparing `tmp/kaggle-1.6.0a3.tar.gz` & `tmp/kaggle-1.6.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaggle-1.6.0a3.tar", last modified: Thu Jul  6 16:58:38 2023, max compression
+gzip compressed data, was "kaggle-1.6.0a4.tar", last modified: Fri Jul  7 20:19:38 2023, max compression
```

## Comparing `kaggle-1.6.0a3.tar` & `kaggle-1.6.0a4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/
--rw-r--r--   0 root         (0) root         (0)    11541 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35600 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.605670 kaggle-1.6.0a3/kaggle/
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.609670 kaggle-1.6.0a3/kaggle/api/
--rw-r--r--   0 root         (0) root         (0)      742 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189890 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/kaggle_api.py
--rw-r--r--   0 root         (0) root         (0)   156655 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 root         (0) root         (0)    25458 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api_client.py
--rw-r--r--   0 root         (0) root         (0)    74101 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/cli.py
--rw-r--r--   0 root         (0) root         (0)     9163 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.613670 kaggle-1.6.0a3/kaggle/models/
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/api_blob_type.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/collaborator.py
--rw-r--r--   0 root         (0) root         (0)     5166 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/create_inbox_file_request.py
--rw-r--r--   0 root         (0) root         (0)     7424 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_column.py
--rw-r--r--   0 root         (0) root         (0)    12558 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9991 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)    10114 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     4342 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/error.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 root         (0) root         (0)    20199 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/kernel_push_request.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/license.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_instance_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_instance_update_request.py
--rw-r--r--   0 root         (0) root         (0)    12103 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_new_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    10055 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_new_request.py
--rw-r--r--   0 root         (0) root         (0)     9096 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_update_request.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/result.py
--rw-r--r--   0 root         (0) root         (0)     7844 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/start_blob_upload_request.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/start_blob_upload_response.py
--rw-r--r--   0 root         (0) root         (0)     5439 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/upload_file.py
--rw-r--r--   0 root         (0) root         (0)    13927 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/kaggle/test/
--rw-r--r--   0 root         (0) root         (0)      596 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/test/test_authenticate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.609670 kaggle-1.6.0a3/kaggle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1236 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1680 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/
+-rw-r--r--   0 root         (0) root         (0)    11541 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35600 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle/api/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189890 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/kaggle_api.py
+-rw-r--r--   0 root         (0) root         (0)   171676 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 root         (0) root         (0)    25458 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    75664 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9163 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/kaggle/models/
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/api_blob_type.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/collaborator.py
+-rw-r--r--   0 root         (0) root         (0)     5166 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/create_inbox_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     7424 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_column.py
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)    10114 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 root         (0) root         (0)    20199 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/license.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_instance_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_instance_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    12103 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_new_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    10055 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9096 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/model_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/result.py
+-rw-r--r--   0 root         (0) root         (0)     7844 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/start_blob_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/start_blob_upload_response.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-07-07 20:19:35.000000 kaggle-1.6.0a4/kaggle/models/upload_file.py
+-rw-r--r--   0 root         (0) root         (0)    13927 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.800876 kaggle-1.6.0a4/kaggle/test/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/kaggle/test/test_authenticate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:19:38.792875 kaggle-1.6.0a4/kaggle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-07 20:19:38.000000 kaggle-1.6.0a4/kaggle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-07 20:19:38.804876 kaggle-1.6.0a4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-07-07 20:19:36.000000 kaggle-1.6.0a4/setup.py
```

### Comparing `kaggle-1.6.0a3/LICENSE` & `kaggle-1.6.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/PKG-INFO` & `kaggle-1.6.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a3
+Version: 1.6.0a4
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a3/README.md` & `kaggle-1.6.0a4/README.md`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/__init__.py` & `kaggle-1.6.0a4/kaggle/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/api/__init__.py` & `kaggle-1.6.0a4/kaggle/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/api/kaggle_api.py` & `kaggle-1.6.0a4/kaggle/api/kaggle_api.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/api/kaggle_api_extended.py` & `kaggle-1.6.0a4/kaggle/api/kaggle_api_extended.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 from __future__ import print_function
 import csv
 from datetime import datetime
 import io
 import json
 import os
 from os.path import expanduser
+from random import random
 import sys
 import shutil
 import tarfile
+import time
 import zipfile
 import tempfile
 from ..api_client import ApiClient
 from kaggle.configuration import Configuration
 from .kaggle_api import KaggleApi
 from ..models.api_blob_type import ApiBlobType
 from ..models.collaborator import Collaborator
@@ -62,27 +64,30 @@
 from ..models.kaggle_models_extended import KernelPushResponse
 from ..models.kaggle_models_extended import LeaderboardEntry
 from ..models.kaggle_models_extended import ListFilesResult
 from ..models.kaggle_models_extended import Metadata
 from ..models.kaggle_models_extended import Model
 from ..models.kaggle_models_extended import ModelNewResponse
 from ..models.kaggle_models_extended import ModelDeleteResponse
+from ..models.kaggle_models_extended import ResumableUploadResult
 from ..models.kaggle_models_extended import Submission
 from ..models.kaggle_models_extended import SubmitResult
 from ..models.kernel_push_request import KernelPushRequest
 from ..models.license import License
 from ..models.model_new_request import ModelNewRequest
 from ..models.model_new_instance_request import ModelNewInstanceRequest
 from ..models.model_instance_new_version_request import ModelInstanceNewVersionRequest
 from ..models.model_update_request import ModelUpdateRequest
 from ..models.model_instance_update_request import ModelInstanceUpdateRequest
 from ..models.start_blob_upload_request import StartBlobUploadRequest
+from ..models.start_blob_upload_response import StartBlobUploadResponse
 from ..models.upload_file import UploadFile
 import requests
 from requests.adapters import HTTPAdapter
+import requests.packages.urllib3.exceptions as urllib3_exceptions
 from requests.packages.urllib3.util.retry import Retry
 from ..rest import ApiException
 import six
 from slugify import slugify
 from tqdm import tqdm
 import bleach
 import time
@@ -103,21 +108,175 @@
 
     def __enter__(self):
         self._temp_dir = tempfile.mkdtemp()
         _, dir_name = os.path.split(self._fullpath)
         self.path = shutil.make_archive(os.path.join(self._temp_dir, dir_name),
                                         self._format, self._fullpath)
         _, self.name = os.path.split(self.path)
+        return self
 
     def __exit__(self, *args):
         shutil.rmtree(self._temp_dir)
 
 
+class ResumableUploadContext(object):
+
+    def __init__(self, no_resume=False):
+        self.no_resume = no_resume
+        self._temp_dir = os.path.join(tempfile.gettempdir(), '.kaggle/uploads')
+        self._file_uploads = []
+
+    def __enter__(self):
+        if self.no_resume:
+            return
+        self._create_temp_dir()
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        if self.no_resume:
+            return
+        if exc_type is not None:
+            # Don't delete the upload file info when there is an error
+            # to give it a chance to retry/resume on the next invocation.
+            return
+        for file_upload in self._file_uploads:
+            file_upload.cleanup()
+
+    def get_upload_info_file_path(self, path):
+        return os.path.join(
+            self._temp_dir,
+            '%s.json' % path.replace(os.path.sep, '_').replace(':', '_'))
+
+    def new_resumable_file_upload(self, path, start_blob_upload_request):
+        file_upload = ResumableFileUpload(path, start_blob_upload_request,
+                                          self)
+        self._file_uploads.append(file_upload)
+        file_upload.load()
+        return file_upload
+
+    def _create_temp_dir(self):
+        try:
+            os.makedirs(self._temp_dir)
+        except FileExistsError:
+            pass
+
+
+class ResumableFileUpload(object):
+    # Reference: https://cloud.google.com/storage/docs/resumable-uploads
+    # A resumable upload must be completed within a week of being initiated
+    RESUMABLE_UPLOAD_EXPIRY_SECONDS = 6 * 24 * 3600
+
+    def __init__(self, path, start_blob_upload_request, context):
+        self.path = path
+        self.start_blob_upload_request = start_blob_upload_request
+        self.context = context
+        self.timestamp = int(time.time())
+        self.start_blob_upload_response = None
+        self.can_resume = False
+        self.upload_complete = False
+        if self.context.no_resume:
+            return
+        self._upload_info_file_path = self.context.get_upload_info_file_path(
+            path)
+
+    def get_token(self):
+        if self.upload_complete:
+            return self.start_blob_upload_response.token
+        return None
+
+    def load(self):
+        if self.context.no_resume:
+            return
+        self._load_previous_if_any()
+
+    def _load_previous_if_any(self):
+        if not os.path.exists(self._upload_info_file_path):
+            return False
+
+        try:
+            with io.open(self._upload_info_file_path, 'r') as f:
+                previous = ResumableFileUpload.from_dict(
+                    json.load(f), self.context)
+                if self._is_previous_valid(previous):
+                    self.start_blob_upload_response = previous.start_blob_upload_response
+                    self.timestamp = previous.timestamp
+                    self.can_resume = True
+        except Exception as e:
+            print('Error while trying to load upload info:', e)
+
+    def _is_previous_valid(self, previous):
+        return previous.path == self.path and \
+               previous.start_blob_upload_request == self.start_blob_upload_request and \
+               previous.timestamp > time.time() - ResumableFileUpload.RESUMABLE_UPLOAD_EXPIRY_SECONDS
+
+    def upload_initiated(self, start_blob_upload_response):
+        if self.context.no_resume:
+            return
+
+        self.start_blob_upload_response = start_blob_upload_response
+        with io.open(self._upload_info_file_path, 'w') as f:
+            json.dump(self.to_dict(), f, indent=True)
+
+    def upload_completed(self):
+        if self.context.no_resume:
+            return
+
+        self.upload_complete = True
+        self._save()
+
+    def _save(self):
+        with io.open(self._upload_info_file_path, 'w') as f:
+            json.dump(self.to_dict(), f, indent=True)
+
+    def cleanup(self):
+        if self.context.no_resume:
+            return
+
+        try:
+            os.remove(self._upload_info_file_path)
+        except OSError:
+            pass
+
+    def to_dict(self):
+        return {
+            'path':
+            self.path,
+            'start_blob_upload_request':
+            self.start_blob_upload_request.to_dict(),
+            'timestamp':
+            self.timestamp,
+            'start_blob_upload_response':
+            self.start_blob_upload_response.to_dict()
+            if self.start_blob_upload_response is not None else None,
+            'upload_complete':
+            self.upload_complete,
+        }
+
+    def from_dict(other, context):
+        new = ResumableFileUpload(
+            other['path'],
+            StartBlobUploadRequest(**other['start_blob_upload_request']),
+            context)
+        new.timestamp = other.get('timestamp')
+        start_blob_upload_response = other.get('start_blob_upload_response')
+        if start_blob_upload_response is not None:
+            new.start_blob_upload_response = StartBlobUploadResponse(
+                **start_blob_upload_response)
+            new.upload_complete = other.get('upload_complete') or False
+        return new
+
+    def to_str(self):
+        return str(self.to_dict())
+
+    def __repr__(self):
+        return self.to_str()
+
+
 class KaggleApi(KaggleApi):
-    __version__ = '1.6.0a3'
+    __version__ = '1.6.0a4'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
@@ -125,14 +284,15 @@
     HEADER_API_VERSION = 'X-Kaggle-ApiVersion'
     DATASET_METADATA_FILE = 'dataset-metadata.json'
     OLD_DATASET_METADATA_FILE = 'datapackage.json'
     KERNEL_METADATA_FILE = 'kernel-metadata.json'
     MODEL_METADATA_FILE = 'model-metadata.json'
     MODEL_INSTANCE_METADATA_FILE = 'model-instance-metadata.json'
     MAX_NUM_INBOX_FILES_TO_UPLOAD = 1000
+    MAX_UPLOAD_RESUME_ATTEMPTS = 10
 
     config_dir = os.environ.get('KAGGLE_CONFIG_DIR') or os.path.join(
         expanduser('~'), '.kaggle')
     if not os.path.exists(config_dir):
         os.makedirs(config_dir)
 
     config_file = 'kaggle.json'
@@ -176,14 +336,54 @@
     ]
 
     # Hack for https://github.com/Kaggle/kaggle-api/issues/22 / b/78194015
     if six.PY2:
         reload(sys)
         sys.setdefaultencoding('latin1')
 
+    def _is_retriable(self, e):
+        return issubclass(type(e), ConnectionError) or \
+            issubclass(type(e), urllib3_exceptions.ConnectionError) or \
+            issubclass(type(e), urllib3_exceptions.ConnectTimeoutError) or \
+            issubclass(type(e), urllib3_exceptions.ProtocolError) or \
+            issubclass(type(e), requests.exceptions.ConnectionError) or \
+            issubclass(type(e), requests.exceptions.ConnectTimeout)
+
+    def _calculate_backoff_delay(self, attempt, initial_delay_millis,
+                                 retry_multiplier, randomness_factor):
+        delay_ms = initial_delay_millis * (retry_multiplier**attempt)
+        random_wait_ms = int(random() - 0.5) * 2 * delay_ms * randomness_factor
+        total_delay = (delay_ms + random_wait_ms) / 1000.0
+        return total_delay
+
+    def with_retry(self,
+                   func,
+                   max_retries=10,
+                   initial_delay_millis=500,
+                   retry_multiplier=1.7,
+                   randomness_factor=0.5):
+
+        def retriable_func(*args):
+            for i in range(1, max_retries + 1):
+                try:
+                    return func(*args)
+                except Exception as e:
+                    if self._is_retriable(e) and i < max_retries:
+                        total_delay = self._calculate_backoff_delay(
+                            i, initial_delay_millis, retry_multiplier,
+                            randomness_factor)
+                        print(
+                            'Request failed: %s. Will retry in %2.1f seconds' %
+                            (e, total_delay))
+                        time.sleep(total_delay)
+                        continue
+                    raise
+
+        return retriable_func
+
     ## Authentication
 
     def authenticate(self):
         """authenticate the user with the Kaggle API. This method will generate
            a configuration, first checking the environment for credential
            variables, and falling back to looking for the .kaggle/kaggle.json
            configuration file.
@@ -563,18 +763,19 @@
                         file=file_name,
                         guid=url_result_list[-3],
                         content_length=url_result_list[-2],
                         last_modified_date_utc=url_result_list[-1]))
                 upload_result_token = upload_result['token']
             else:
                 # New submissions path!
-                success = self.upload_complete(file_name,
-                                               url_result['createUrl'], quiet)
-                if not success:
-                    # Actual error is printed during upload_complete.  Not
+                upload_status = self.upload_complete(file_name,
+                                                     url_result['createUrl'],
+                                                     quiet)
+                if upload_status != ResumableUploadResult.COMPLETE:
+                    # Actual error is printed during upload_complete. Not
                     # ideal but changing would not be backwards compatible
                     return "Could not submit to competition"
 
                 upload_result_token = url_result['token']
 
             submit_result = self.process_response(
                 self.competitions_submissions_submit_with_http_info(
@@ -1297,39 +1498,61 @@
         else:
             self.dataset_download_file(dataset,
                                        file_name,
                                        path=path,
                                        force=force,
                                        quiet=quiet)
 
-    def _upload_blob(self, path, quiet, blob_type):
+    def _upload_blob(self, path, quiet, blob_type, upload_context):
         """ upload a file
 
             Parameters
             ==========
             path: the complete path to upload
             quiet: suppress verbose output (default is False)
             blob_type (ApiBlobType): To which entity the file/blob refers
+            upload_context (ResumableUploadContext): Context for resumable uploads
         """
         file_name = os.path.basename(path)
         content_length = os.path.getsize(path)
         last_modified_epoch_seconds = int(os.path.getmtime(path))
 
-        request = StartBlobUploadRequest(
+        start_blob_upload_request = StartBlobUploadRequest(
             blob_type,
             file_name,
             content_length,
             last_modified_epoch_seconds=last_modified_epoch_seconds)
-        response = self.process_response(
-            self.upload_file_with_http_info(request))
-        success = self.upload_complete(path, response.create_url, quiet)
 
-        if success:
-            return response.token
-        return None
+        file_upload = upload_context.new_resumable_file_upload(
+            path, start_blob_upload_request)
+
+        for i in range(0, self.MAX_UPLOAD_RESUME_ATTEMPTS):
+            if file_upload.upload_complete:
+                return file_upload
+
+            if not file_upload.can_resume:
+                # Initiate upload on Kaggle backend to get the url and token.
+                start_blob_upload_response = self.process_response(
+                    self.with_retry(self.upload_file_with_http_info)(
+                        file_upload.start_blob_upload_request))
+                file_upload.upload_initiated(start_blob_upload_response)
+
+            upload_result = self.upload_complete(
+                path,
+                file_upload.start_blob_upload_response.create_url,
+                quiet,
+                resume=file_upload.can_resume)
+            if upload_result == ResumableUploadResult.INCOMPLETE:
+                continue  # Continue (i.e., retry/resume) only if the upload is incomplete.
+
+            if upload_result == ResumableUploadResult.COMPLETE:
+                file_upload.upload_completed()
+            break
+
+        return file_upload.get_token()
 
     def dataset_create_version(self,
                                folder,
                                version_notes,
                                quiet=False,
                                convert_to_csv=True,
                                delete_old_versions=False,
@@ -1373,38 +1596,41 @@
             version_notes=version_notes,
             subtitle=subtitle,
             description=description,
             files=[],
             convert_to_csv=convert_to_csv,
             category_ids=keywords,
             delete_old_versions=delete_old_versions)
-        self.upload_files(request, resources, folder, ApiBlobType.DATASET,
-                          quiet, dir_mode)
 
-        if id_no:
-            result = DatasetNewVersionResponse(
-                self.process_response(
-                    self.datasets_create_version_by_id_with_http_info(
-                        id_no, request)))
-        else:
-            if ref == self.config_values[
-                    self.CONFIG_NAME_USER] + '/INSERT_SLUG_HERE':
-                raise ValueError(
-                    'Default slug detected, please change values before '
-                    'uploading')
-            self.validate_dataset_string(ref)
-            ref_list = ref.split('/')
-            owner_slug = ref_list[0]
-            dataset_slug = ref_list[1]
-            result = DatasetNewVersionResponse(
-                self.process_response(
-                    self.datasets_create_version_with_http_info(
-                        owner_slug, dataset_slug, request)))
+        with ResumableUploadContext() as upload_context:
+            self.upload_files(request, resources, folder, ApiBlobType.DATASET,
+                              upload_context, quiet, dir_mode)
+
+            if id_no:
+                result = DatasetNewVersionResponse(
+                    self.process_response(
+                        self.with_retry(
+                            self.datasets_create_version_by_id_with_http_info)(
+                                id_no, request)))
+            else:
+                if ref == self.config_values[
+                        self.CONFIG_NAME_USER] + '/INSERT_SLUG_HERE':
+                    raise ValueError(
+                        'Default slug detected, please change values before '
+                        'uploading')
+                self.validate_dataset_string(ref)
+                ref_list = ref.split('/')
+                owner_slug = ref_list[0]
+                dataset_slug = ref_list[1]
+                result = DatasetNewVersionResponse(
+                    self.process_response(
+                        self.datasets_create_version_with_http_info(
+                            owner_slug, dataset_slug, request)))
 
-        return result
+            return result
 
     def dataset_create_version_cli(self,
                                    folder,
                                    version_notes,
                                    quiet=False,
                                    convert_to_csv=True,
                                    delete_old_versions=False,
@@ -1539,19 +1765,22 @@
                                     license_name=license_name,
                                     subtitle=subtitle,
                                     description=description,
                                     files=[],
                                     is_private=not public,
                                     convert_to_csv=convert_to_csv,
                                     category_ids=keywords)
-        self.upload_files(request, resources, folder, ApiBlobType.DATASET,
-                          quiet, dir_mode)
-        result = DatasetNewResponse(
-            self.process_response(
-                self.datasets_create_new_with_http_info(request)))
+
+        with ResumableUploadContext() as upload_context:
+            self.upload_files(request, resources, folder, ApiBlobType.DATASET,
+                              upload_context, quiet, dir_mode)
+            result = DatasetNewResponse(
+                self.process_response(
+                    self.with_retry(
+                        self.datasets_create_new_with_http_info)(request)))
 
         return result
 
     def dataset_create_new_cli(self,
                                folder=None,
                                public=False,
                                quiet=False,
@@ -2480,40 +2709,43 @@
 
         if result.hasId:
             print('Your model was created. Id={}. Url={}'.format(
                 result.id, result.url))
         else:
             print('Model creation error: ' + result.error)
 
-    def model_delete(self, model):
+    def model_delete(self, model, yes):
         """ call to delete a model from the API
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
+            yes: automatic confirmation
         """
         owner_slug, model_slug = self.split_model_string(model)
 
-        if not self.confirmation():
-            print('Deletion cancelled')
-            exit(0)
+        if not yes:
+            if not self.confirmation():
+                print('Deletion cancelled')
+                exit(0)
 
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_with_http_info(owner_slug, model_slug)))
         return res
 
-    def model_delete_cli(self, model):
+    def model_delete_cli(self, model, yes):
         """ wrapper for client for model_delete
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
+            yes: automatic confirmation
         """
-        result = self.model_delete(model)
+        result = self.model_delete(model, yes)
 
         if result.hasError:
             print('Model deletion error: ' + result.error)
         else:
             print('The model was deleted.')
 
     def model_update(self, folder):
@@ -2749,22 +2981,26 @@
                                           framework=framework,
                                           overview=overview,
                                           usage=usage,
                                           license_name=license_name,
                                           fine_tunable=fine_tunable,
                                           training_data=training_data,
                                           files=[])
-        self.upload_files(request, None, folder, ApiBlobType.MODEL, quiet,
-                          dir_mode)
-        result = ModelNewResponse(
-            self.process_response(
-                self.models_create_instance_with_http_info(
-                    owner_slug, model_slug, request)))
 
-        return result
+        with ResumableUploadContext() as upload_context:
+            self.upload_files(request, None, folder, ApiBlobType.MODEL,
+                              upload_context, quiet, dir_mode)
+            result = ModelNewResponse(
+                self.process_response(
+                    self.with_retry(
+                        self.models_create_instance_with_http_info)(owner_slug,
+                                                                    model_slug,
+                                                                    request)))
+
+            return result
 
     def model_instance_create_cli(self, folder, quiet=False, dir_mode='skip'):
         """ client wrapper for creating a new model instance
              Parameters
             ==========
             folder: the folder to get the metadata file from
             quiet: suppress verbose output (default is False)
@@ -2775,44 +3011,47 @@
 
         if result.hasId:
             print('Your model instance was created. Id={}. Url={}'.format(
                 result.id, result.url))
         else:
             print('Model instance creation error: ' + result.error)
 
-    def model_instance_delete(self, model_instance):
+    def model_instance_delete(self, model_instance, yes):
         """ call to delete a model instance from the API
              Parameters
             ==========
             model_instance: the string identified of the model instance
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
+            yes: automatic confirmation
         """
         if model_instance is None:
             raise ValueError('A model instance must be specified')
         owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
             model_instance)
 
-        if not self.confirmation():
-            print('Deletion cancelled')
-            exit(0)
+        if not yes:
+            if not self.confirmation():
+                print('Deletion cancelled')
+                exit(0)
 
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_instance_with_http_info(
                     owner_slug, model_slug, framework, instance_slug)))
         return res
 
-    def model_instance_delete_cli(self, model_instance):
+    def model_instance_delete_cli(self, model_instance, yes):
         """ wrapper for client for model_instance_delete
              Parameters
             ==========
             model_instance: the string identified of the model instance
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
+            yes: automatic confirmation
         """
-        result = self.model_instance_delete(model_instance)
+        result = self.model_instance_delete(model_instance, yes)
 
         if result.hasError:
             print('Model instance deletion error: ' + result.error)
         else:
             print('The model instance was deleted.')
 
     def model_instance_update(self, folder):
@@ -2924,23 +3163,26 @@
             dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
         """
         owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
             model_instance)
 
         request = ModelInstanceNewVersionRequest(version_notes=version_notes,
                                                  files=[])
-        self.upload_files(request, None, folder, ApiBlobType.MODEL, quiet,
-                          dir_mode)
-        result = ModelNewResponse(
-            self.process_response(
-                self.models_create_instance_version_with_http_info(
-                    owner_slug, model_slug, framework, instance_slug,
-                    request)))
 
-        return result
+        with ResumableUploadContext() as upload_context:
+            self.upload_files(request, None, folder, ApiBlobType.MODEL,
+                              upload_context, quiet, dir_mode)
+            result = ModelNewResponse(
+                self.process_response(
+                    self.with_retry(
+                        self.models_create_instance_version_with_http_info)(
+                            owner_slug, model_slug, framework, instance_slug,
+                            request)))
+
+            return result
 
     def model_instance_version_create_cli(self,
                                           model_instance,
                                           folder,
                                           version_notes='',
                                           quiet=False,
                                           dir_mode='skip'):
@@ -3049,83 +3291,100 @@
         """
         self.model_instance_version_download(model_instance_version,
                                              path=path,
                                              untar=untar,
                                              force=force,
                                              quiet=quiet)
 
-    def model_instance_version_delete(self, model_instance_version):
+    def model_instance_version_delete(self, model_instance_version, yes):
         """ call to delete a model instance version from the API
              Parameters
             ==========
             model_instance_version: the string identified of the model instance version
                 should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+            yes: automatic confirmation
         """
         if model_instance_version is None:
             raise ValueError('A model instance version must be specified')
 
         self.validate_model_instance_version_string(model_instance_version)
         urls = model_instance_version.split('/')
         owner_slug = urls[0]
         model_slug = urls[1]
         framework = urls[2]
         instance_slug = urls[3]
         version_number = urls[4]
 
-        if not self.confirmation():
-            print('Deletion cancelled')
-            exit(0)
+        if not yes:
+            if not self.confirmation():
+                print('Deletion cancelled')
+                exit(0)
 
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_instance_version_with_http_info(
                     owner_slug, model_slug, framework, instance_slug,
                     version_number)))
         return res
 
-    def model_instance_version_delete_cli(self, model_instance_version):
+    def model_instance_version_delete_cli(self, model_instance_version, yes):
         """ wrapper for client for model_instance_version_delete
              Parameters
             ==========
             model_instance_version: the string identified of the model instance version
                 should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+            yes: automatic confirmation
         """
-        result = self.model_instance_version_delete(model_instance_version)
+        result = self.model_instance_version_delete(model_instance_version,
+                                                    yes)
 
         if result.hasError:
             print('Model instance version deletion error: ' + result.error)
         else:
             print('The model instance version was deleted.')
 
-    def files_upload_cli(self, local_paths, inbox_path=None):
+    def files_upload_cli(self, local_paths, inbox_path, no_resume,
+                         no_compress):
         if len(local_paths) > self.MAX_NUM_INBOX_FILES_TO_UPLOAD:
-            print('Cannot upload more than',
-                  self.MAX_NUM_INBOX_FILES_TO_UPLOAD, 'files!')
+            print('Cannot upload more than %d files!' %
+                  self.MAX_NUM_INBOX_FILES_TO_UPLOAD)
             return
 
-        for local_path in local_paths:
-            self.file_upload_cli(local_path, inbox_path)
+        files_to_create = []
+        with ResumableUploadContext(no_resume) as upload_context:
+            for local_path in local_paths:
+                (upload_file,
+                 file_name) = self.file_upload_cli(local_path, inbox_path,
+                                                   no_compress, upload_context)
+                if upload_file is None:
+                    continue
+
+                create_inbox_file_request = CreateInboxFileRequest(
+                    virtual_directory=inbox_path,
+                    blob_file_token=upload_file.token)
+                files_to_create.append((create_inbox_file_request, file_name))
+
+            for (create_inbox_file_request, file_name) in files_to_create:
+                self.process_response(
+                    self.with_retry(
+                        self.create_inbox_file)(create_inbox_file_request))
+                print('Inbox file created:', file_name)
 
-    def file_upload_cli(self, local_path, inbox_path=None):
+    def file_upload_cli(self, local_path, inbox_path, no_compress,
+                        upload_context):
         full_path = os.path.abspath(local_path)
         parent_path = os.path.dirname(full_path)
         file_or_folder_name = os.path.basename(full_path)
+        dir_mode = 'tar' if no_compress else 'zip'
 
         upload_file = self._upload_file_or_folder(parent_path,
                                                   file_or_folder_name,
-                                                  ApiBlobType.INBOX, 'zip')
-        if upload_file is None:
-            return
-
-        inbox_path = inbox_path or ''
-        create_inbox_file_request = CreateInboxFileRequest(
-            virtual_directory=inbox_path, blob_file_token=upload_file.token)
-        self.process_response(
-            self.create_inbox_file(create_inbox_file_request))
-        print('Upload complete:', file_or_folder_name)
+                                                  ApiBlobType.INBOX,
+                                                  upload_context, dir_mode)
+        return (upload_file, file_or_folder_name)
 
     def print_obj(self, obj, indent=2):
         pretty = json.dumps(obj, indent=indent)
         print(pretty)
 
     def download_needed(self, response, outfile, quiet=True):
         """ determine if a download is needed based on timestamp. Return True
@@ -3294,81 +3553,87 @@
         return True
 
     def upload_files(self,
                      request,
                      resources,
                      folder,
                      blob_type,
+                     upload_context,
                      quiet=False,
                      dir_mode='skip'):
         """ upload files in a folder
              Parameters
             ==========
             request: the prepared request
             resources: the files to upload
             folder: the folder to upload from
             blob_type (ApiBlobType): To which entity the file/blob refers
+            upload_context (ResumableUploadContext): Context for resumable uploads
             quiet: suppress verbose output (default is False)
         """
         for file_name in os.listdir(folder):
             if (file_name in [
                     self.DATASET_METADATA_FILE, self.OLD_DATASET_METADATA_FILE,
                     self.KERNEL_METADATA_FILE, self.MODEL_METADATA_FILE,
                     self.MODEL_INSTANCE_METADATA_FILE
             ]):
                 continue
             upload_file = self._upload_file_or_folder(folder, file_name,
-                                                      blob_type, dir_mode,
+                                                      blob_type,
+                                                      upload_context, dir_mode,
                                                       quiet, resources)
             if upload_file is not None:
                 request.files.append(upload_file)
 
     def _upload_file_or_folder(self,
                                parent_path,
                                file_or_folder_name,
                                blob_type,
+                               upload_context,
                                dir_mode,
                                quiet=False,
                                resources=None):
         full_path = os.path.join(parent_path, file_or_folder_name)
         if os.path.isfile(full_path):
             return self._upload_file(file_or_folder_name, full_path, blob_type,
-                                     quiet, resources)
+                                     upload_context, quiet, resources)
 
         elif os.path.isdir(full_path):
             if dir_mode in ['zip', 'tar']:
-                archive = DirectoryArchive(full_path, dir_mode)
-                with archive:
+                with DirectoryArchive(full_path, dir_mode) as archive:
                     return self._upload_file(archive.name, archive.path,
-                                             blob_type, quiet, resources)
+                                             blob_type, upload_context, quiet,
+                                             resources)
             elif not quiet:
                 print("Skipping folder: " + file_or_folder_name +
                       "; use '--dir-mode' to upload folders")
         else:
             if not quiet:
                 print('Skipping: ' + file_or_folder_name)
         return None
 
-    def _upload_file(self, file_name, full_path, blob_type, quiet, resources):
+    def _upload_file(self, file_name, full_path, blob_type, upload_context,
+                     quiet, resources):
         """ Helper function to upload a single file
             Parameters
             ==========
             file_name: name of the file to upload
             full_path: path to the file to upload
             blob_type (ApiBlobType): To which entity the file/blob refers
+            upload_context (ResumableUploadContext): Context for resumable uploads
             quiet: suppress verbose output
             resources: optional file metadata
             :return: None - upload unsuccessful; instance of UploadFile - upload successful
         """
 
         if not quiet:
             print('Starting upload for file ' + file_name)
 
         content_length = os.path.getsize(full_path)
-        token = self._upload_blob(full_path, quiet, blob_type)
+        token = self._upload_blob(full_path, quiet, blob_type, upload_context)
         if token is None:
             if not quiet:
                 print('Upload unsuccessful: ' + file_name)
             return None
         if not quiet:
             print('Upload successful: ' + file_name + ' (' +
                   File.get_size(content_length) + ')')
@@ -3418,42 +3683,124 @@
                 processed_column.type = 'datetime'
             else:
                 # Possibly extended data type - not going to try to track those
                 # here. Will set the type and let the server handle it.
                 processed_column.type = original_type
         return processed_column
 
-    def upload_complete(self, path, url, quiet):
+    def upload_complete(self, path, url, quiet, resume=False):
         """ function to complete an upload to retrieve a path from a url
              Parameters
             ==========
             path: the path for the upload that is read in
             url: the url to send the POST to
             quiet: suppress verbose output (default is False)
         """
         file_size = os.path.getsize(path)
+        resumable_upload_result = ResumableUploadResult.Incomplete()
+
         try:
-            with tqdm(total=file_size,
+            if resume:
+                resumable_upload_result = self._resume_upload(
+                    url, file_size, quiet)
+                if resumable_upload_result.result != ResumableUploadResult.INCOMPLETE:
+                    return resumable_upload_result.result
+
+            start_at = resumable_upload_result.start_at
+            upload_size = file_size - start_at
+
+            with tqdm(total=upload_size,
                       unit='B',
                       unit_scale=True,
                       unit_divisor=1024,
                       disable=quiet) as progress_bar:
                 with io.open(path, 'rb', buffering=0) as fp:
-                    reader = TqdmBufferedReader(fp, progress_bar)
                     session = requests.Session()
+                    if start_at > 0:
+                        fp.seek(start_at)
+                        session.headers.update({
+                            'Content-Length':
+                            '%d' % upload_size,
+                            'Content-Range':
+                            'bytes %d-%d/%d' %
+                            (start_at, file_size - 1, file_size)
+                        })
+                    reader = TqdmBufferedReader(fp, progress_bar)
                     retries = Retry(total=10, backoff_factor=0.5)
                     adapter = HTTPAdapter(max_retries=retries)
                     session.mount('http://', adapter)
                     session.mount('https://', adapter)
                     response = session.put(url, data=reader)
+                    if self._is_upload_successful(response):
+                        return ResumableUploadResult.COMPLETE
+                    if response.status_code == 503:
+                        return ResumableUploadResult.INCOMPLETE
+                    # Server returned a non-resumable error so give up.
+                    return ResumableUploadResult.FAILED
         except Exception as error:
             print(error)
-            return False
+            # There is probably some weird bug in our code so try to resume the upload
+            # in case it works on the next try.
+            return ResumableUploadResult.INCOMPLETE
+
+    def _resume_upload(self, url, content_length, quiet):
+        # Documentation: https://developers.google.com/drive/api/guides/manage-uploads#resume-upload
+        session = requests.Session()
+        session.headers.update({
+            'Content-Length': '0',
+            'Content-Range': 'bytes */%d' % content_length,
+        })
+
+        response = session.put(url)
+
+        if self._is_upload_successful(response):
+            return ResumableUploadResult.Complete()
+        if response.status_code == 404:
+            # Upload expired so need to start from scratch.
+            if not query:
+                print('Upload of %s expired. Please try again.' % path)
+            return ResumableUploadResult.Failed()
+        if response.status_code == 308:  # Resume Incomplete
+            bytes_uploaded = self._get_bytes_already_uploaded(response, quiet)
+            if bytes_uploaded is None:
+                # There is an error with the Range header so need to start from scratch.
+                return ResumableUploadResult.Failed()
+            result = ResumableUploadResult.Incomplete(bytes_uploaded)
+            if not quiet:
+                print('Already uploaded %d bytes. Will resume upload at %d.' %
+                      (result.bytes_uploaded, result.start_at))
+            return result
+        else:
+            if not quiet:
+                print('Server returned %d. Please try again.' %
+                      response.status_code)
+            return ResumableUploadResult.Failed()
+
+    def _is_upload_successful(self, response):
         return response.status_code == 200 or response.status_code == 201
 
+    def _get_bytes_already_uploaded(self, response, quiet):
+        range_val = response.headers.get('Range')
+        if range_val is None:
+            return 0  # This means server hasn't received anything before.
+        items = range_val.split('-')  # Example: bytes=0-1000 => ['0', '1000']
+        if len(items) != 2:
+            if not quiet:
+                print('Invalid Range header format: %s. Will try again.' %
+                      range_val)
+            return None  # Shouldn't happen, something's wrong with Range header format.
+        bytes_uploaded_str = items[-1]  # Example: ['0', '1000'] => '1000'
+        try:
+            return int(bytes_uploaded_str)  # Example: '1000' => 1000
+        except ValueError:
+            if not quiet:
+                print('Invalid Range header format: %s. Will try again.' %
+                      range_val)
+            return None  # Shouldn't happen, something's wrong with Range header format.
+
     def validate_dataset_string(self, dataset):
         """ determine if a dataset string is valid, meaning it is in the format
             of {username}/{dataset-slug} or {username}/{dataset-slug}/{version-number}.
              Parameters
             ==========
             dataset: the dataset name to validate
         """
```

### Comparing `kaggle-1.6.0a3/kaggle/api_client.py` & `kaggle-1.6.0a4/kaggle/api_client.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/cli.py` & `kaggle-1.6.0a4/kaggle/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -953,14 +953,19 @@
     # Models delete
     parser_models_delete = subparsers_models.add_parser(
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_models_delete)
     parser_models_delete_optional = parser_models_delete._action_groups.pop()
     parser_models_delete_optional.add_argument('model', help=Help.param_model)
+    parser_models_delete_optional.add_argument('-y',
+                                               '--yes',
+                                               dest='yes',
+                                               action='store_true',
+                                               help=Help.param_yes)
     parser_models_delete._action_groups.append(parser_models_delete_optional)
     parser_models_delete.set_defaults(func=api.model_delete_cli)
 
     # Models update
     parser_models_update = subparsers_models.add_parser(
         'update',
         formatter_class=argparse.RawTextHelpFormatter,
@@ -1062,14 +1067,19 @@
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_delete)
     parser_model_instances_delete_optional = parser_model_instances_delete._action_groups.pop(
     )
     parser_model_instances_delete_optional.add_argument(
         'model_instance', help=Help.param_model_instance)
+    parser_model_instances_delete_optional.add_argument('-y',
+                                                        '--yes',
+                                                        dest='yes',
+                                                        action='store_true',
+                                                        help=Help.param_yes)
     parser_model_instances_delete._action_groups.append(
         parser_model_instances_delete_optional)
     parser_model_instances_delete.set_defaults(
         func=api.model_instance_delete_cli)
 
     # Models Instances update
     parser_model_instances_update = subparsers_model_instances.add_parser(
@@ -1180,14 +1190,16 @@
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instance_versions_delete)
     parser_model_instance_versions_delete_optional = parser_model_instance_versions_delete._action_groups.pop(
     )
     parser_model_instance_versions_delete_optional.add_argument(
         'model_instance_version', help=Help.param_model_instance_version)
+    parser_model_instance_versions_delete_optional.add_argument(
+        '-y', '--yes', dest='yes', action='store_true', help=Help.param_yes)
     parser_model_instance_versions_delete._action_groups.append(
         parser_model_instance_versions_delete_optional)
     parser_model_instance_versions_delete.set_defaults(
         func=api.model_instance_version_delete_cli)
 
 
 def parse_files(subparsers):
@@ -1210,20 +1222,35 @@
         aliases=['u'])
     parser_files_upload_optional = parser_files_upload._action_groups.pop()
     parser_files_upload_optional.add_argument(
         '-i',
         '--inbox-path',
         dest='inbox_path',
         required=False,
+        default='',
         help=Help.param_files_upload_inbox_path)
     parser_files_upload_optional.add_argument(
         'local_paths',
         metavar='local-path',
         nargs='+',
         help=Help.param_files_upload_local_paths)
+    parser_files_upload_optional.add_argument(
+        '--no-resume',
+        dest='no_resume',
+        action='store_true',
+        required=False,
+        default=False,
+        help=Help.param_files_upload_no_resume)
+    parser_files_upload_optional.add_argument(
+        '--no-compress',
+        dest='no_compress',
+        action='store_true',
+        required=False,
+        default=False,
+        help=Help.param_files_upload_no_compress)
     parser_files_upload._action_groups.append(parser_files_upload_optional)
     parser_files_upload.set_defaults(func=api.files_upload_cli)
 
 
 def parse_config(subparsers):
     parser_config = subparsers.add_parser(
         'config',
@@ -1391,14 +1418,17 @@
     param_page_token = 'Page token for results paging.'
     param_search = 'Term(s) to search for'
     param_mine = 'Display only my items'
     param_unzip = (
         'Unzip the downloaded file. Will delete the zip file when completed.')
     param_untar = (
         'Untar the downloaded file. Will delete the tar file when completed.')
+    param_yes = (
+        'Sets any confirmation values to "yes" automatically. Users will not be asked to confirm.'
+    )
 
     # Competitions params
     param_competition = (
         'Competition URL suffix (use "kaggle competitions list" '
         'to show options)\nIf empty, the default competition '
         'will be used (use "kaggle config set competition")"')
     param_competition_nonempty = (
@@ -1550,16 +1580,18 @@
     command_model_instance_versions_download = 'Download model instance version files'
     param_model_instance_version_notes = 'Version notes to record for the new model instance version'
 
     # Files params
     param_files_upload_inbox_path = 'Virtual path on the server where the uploaded files will be stored'
     param_files_upload_local_paths = (
         'List of local filesystem paths. Each path creates a separate file on the server. '
-        'Directories are uploaded as zip archives (e.g., a directory called "data" will be uploaded as "data.zip")'
-    )
+        'Directories are uploaded as zip archives by default (e.g., a directory called '
+        '"data" will be uploaded as "data.zip")')
+    param_files_upload_no_compress = 'Whether to compress directories (zip) or not (tar)'
+    param_files_upload_no_resume = 'Whether to skip resumable uploads.'
 
     # Config params
     param_config_name = ('Name of the configuration parameter\n(one of '
                          'competition, path, proxy)')
     param_config_value = (
         ('Value of the configuration parameter, valid values '
          'depending on name\n- competition: ') + param_competition_nonempty +
```

### Comparing `kaggle-1.6.0a3/kaggle/configuration.py` & `kaggle-1.6.0a4/kaggle/configuration.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/__init__.py` & `kaggle-1.6.0a4/kaggle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/api_blob_type.py` & `kaggle-1.6.0a4/kaggle/models/api_blob_type.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/collaborator.py` & `kaggle-1.6.0a4/kaggle/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/create_inbox_file_request.py` & `kaggle-1.6.0a4/kaggle/models/create_inbox_file_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/dataset_column.py` & `kaggle-1.6.0a4/kaggle/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/dataset_new_request.py` & `kaggle-1.6.0a4/kaggle/models/dataset_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/dataset_new_version_request.py` & `kaggle-1.6.0a4/kaggle/models/dataset_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/dataset_update_settings_request.py` & `kaggle-1.6.0a4/kaggle/models/dataset_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/error.py` & `kaggle-1.6.0a4/kaggle/models/error.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/kaggle_models_extended.py` & `kaggle-1.6.0a4/kaggle/models/kaggle_models_extended.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # coding=utf-8
 import os
+import time
 from datetime import datetime
 
 
 class Competition(object):
 
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
@@ -239,7 +240,37 @@
     for t in time_formats:
         try:
             result = datetime.strptime(string[:26], t).replace(microsecond=0)
             return result
         except:
             pass
     return string
+
+
+class ResumableUploadResult(object):
+    # Upload was complete, i.e., all bytes were received by the server.
+    COMPLETE = 1
+
+    # There was a non-transient error during the upload or the upload expired.
+    # The upload cannot be resumed so it should be restarted from scratch
+    # (i.e., call /api/v1/files/upload to initiate the upload and get the
+    # create/upload url and token).
+    FAILED = 2
+
+    # Upload was interrupted due to some (transient) failure but it can be
+    # safely resumed.
+    INCOMPLETE = 3
+
+    def __init__(self, result, bytes_uploaded=None):
+        self.result = result
+        self.bytes_uploaded = bytes_uploaded
+        self.start_at = 0 if bytes_uploaded is None else bytes_uploaded + 1
+
+    def Complete():
+        return ResumableUploadResult(ResumableUploadResult.COMPLETE)
+
+    def Failed():
+        return ResumableUploadResult(ResumableUploadResult.FAILED)
+
+    def Incomplete(bytes_uploaded=None):
+        return ResumableUploadResult(ResumableUploadResult.INCOMPLETE,
+                                     bytes_uploaded)
```

### Comparing `kaggle-1.6.0a3/kaggle/models/kernel_push_request.py` & `kaggle-1.6.0a4/kaggle/models/kernel_push_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/license.py` & `kaggle-1.6.0a4/kaggle/models/license.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/model_instance_new_version_request.py` & `kaggle-1.6.0a4/kaggle/models/model_instance_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/model_instance_update_request.py` & `kaggle-1.6.0a4/kaggle/models/model_instance_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/model_new_instance_request.py` & `kaggle-1.6.0a4/kaggle/models/model_new_instance_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/model_new_request.py` & `kaggle-1.6.0a4/kaggle/models/model_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/model_update_request.py` & `kaggle-1.6.0a4/kaggle/models/model_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/result.py` & `kaggle-1.6.0a4/kaggle/models/result.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/start_blob_upload_request.py` & `kaggle-1.6.0a4/kaggle/models/start_blob_upload_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/start_blob_upload_response.py` & `kaggle-1.6.0a4/kaggle/models/start_blob_upload_response.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/models/upload_file.py` & `kaggle-1.6.0a4/kaggle/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/rest.py` & `kaggle-1.6.0a4/kaggle/rest.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/test/__init__.py` & `kaggle-1.6.0a4/kaggle/test/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle/test/test_authenticate.py` & `kaggle-1.6.0a4/kaggle/test/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/kaggle.egg-info/PKG-INFO` & `kaggle-1.6.0a4/kaggle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a3
+Version: 1.6.0a4
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a3/kaggle.egg-info/SOURCES.txt` & `kaggle-1.6.0a4/kaggle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a3/setup.py` & `kaggle-1.6.0a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='kaggle',
-    version='1.6.0a3',
+    version='1.6.0a4',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
```

