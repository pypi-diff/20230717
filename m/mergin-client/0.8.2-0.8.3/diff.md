# Comparing `tmp/mergin-client-0.8.2.tar.gz` & `tmp/mergin-client-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergin-client-0.8.2.tar", last modified: Wed Mar  8 16:09:17 2023, max compression
+gzip compressed data, was "mergin-client-0.8.3.tar", last modified: Mon Jul 17 11:24:04 2023, max compression
```

## Comparing `mergin-client-0.8.2.tar` & `mergin-client-0.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:17.256916 mergin-client-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-08 16:09:07.000000 mergin-client-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-08 16:09:17.256916 mergin-client-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-03-08 16:09:07.000000 mergin-client-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:17.256916 mergin-client-0.8.2/mergin/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   275794 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/cert.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)    21311 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    39922 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32367 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/client_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/client_push.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32791 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/merginproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:17.256916 mergin-client-0.8.2/mergin/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/test/sqlite_con.py
--rw-r--r--   0 runner    (1001) docker     (123)    77314 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-08 16:09:07.000000 mergin-client-0.8.2/mergin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:17.256916 mergin-client-0.8.2/mergin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 16:09:17.000000 mergin-client-0.8.2/mergin_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 16:09:17.256916 mergin-client-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-08 16:09:07.000000 mergin-client-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:24:04.113427 mergin-client-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-17 11:23:51.000000 mergin-client-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 11:24:04.113427 mergin-client-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-17 11:23:51.000000 mergin-client-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:24:04.113427 mergin-client-0.8.3/mergin/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275794 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/cert.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21492 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40210 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32367 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/client_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/client_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/merginproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:24:04.113427 mergin-client-0.8.3/mergin/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/test/sqlite_con.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78314 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 11:23:51.000000 mergin-client-0.8.3/mergin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:24:04.113427 mergin-client-0.8.3/mergin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 11:24:04.000000 mergin-client-0.8.3/mergin_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:24:04.113427 mergin-client-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 11:23:51.000000 mergin-client-0.8.3/setup.py
```

### Comparing `mergin-client-0.8.2/LICENSE` & `mergin-client-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/PKG-INFO` & `mergin-client-0.8.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergin-client
-Version: 0.8.2
+Version: 0.8.3
 Summary: Mergin Maps utils and client
 Home-page: https://github.com/MerginMaps/mergin-py-client
 Author: Lutra Consulting Ltd.
 Author-email: info@merginmaps.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mergin-client-0.8.2/README.md` & `mergin-client-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,20 @@
 you can use "login" command to get authorization token.
 It will ask for password and then output environment variable with auth token. The returned token
 is not permanent - it will expire after several hours.
 ```
 $ mergin --username john login
 Password: topsecret
 Login successful!
-To set the MERGIN_AUTH variable run:
+To set the MERGIN_AUTH variable run in Linux:
 export MERGIN_AUTH="Bearer ......."
+In Windows:
+SET MERGIN_AUTH=Bearer .......
 ```
+When setting the variable in Windows you do not quote the value.
 
 When the MERGIN_AUTH env variable is set (or passed with `--auth-token` command line argument),
 it is possible to run other commands without specifying username/password.
 
 
 ## Development
```

#### html2text {}

```diff
@@ -62,23 +62,24 @@
 mergin status ``` 2. pull changes from Mergin Maps service ``` $ mergin pull
 ``` 3. push local changes to Mergin Maps service ``` $ mergin push ``` ###
 Using CLI with auth token If you plan to run `mergin` command multiple times
 and you wish to avoid logging in every time, you can use "login" command to get
 authorization token. It will ask for password and then output environment
 variable with auth token. The returned token is not permanent - it will expire
 after several hours. ``` $ mergin --username john login Password: topsecret
-Login successful! To set the MERGIN_AUTH variable run: export
-MERGIN_AUTH="Bearer ......." ``` When the MERGIN_AUTH env variable is set (or
-passed with `--auth-token` command line argument), it is possible to run other
-commands without specifying username/password. ## Development ### Installing
-deps Python 3.7+ required. Create `mergin/deps` folder where [geodiff](https://
-github.com/MerginMaps/geodiff) lib is supposed to be and install dependencies:
-``` rm -r mergin/deps mkdir mergin/deps pip install python-dateutil pytz pip
-install pygeodiff --target=mergin/deps ``` For using mergin client with its
-dependencies packaged locally run: ``` pip install wheel python3 setup.py sdist
-bdist_wheel mkdir -p mergin/deps pip wheel -r mergin_client.egg-info/
-requires.txt -w mergin/deps unzip mergin/deps/pygeodiff-*.whl -d mergin/deps
-pip install --editable . ``` ### Tests For running test do: ``` cd mergin
-export TEST_MERGIN_URL= # testing server export TEST_API_USERNAME= export
-TEST_API_PASSWORD= export TEST_API_USERNAME2= export TEST_API_PASSWORD2= pip
-install pytest pytest-cov coveralls pytest --cov-report html --cov=mergin
-mergin/test/ ```
+Login successful! To set the MERGIN_AUTH variable run in Linux: export
+MERGIN_AUTH="Bearer ......." In Windows: SET MERGIN_AUTH=Bearer ....... ```
+When setting the variable in Windows you do not quote the value. When the
+MERGIN_AUTH env variable is set (or passed with `--auth-token` command line
+argument), it is possible to run other commands without specifying username/
+password. ## Development ### Installing deps Python 3.7+ required. Create
+`mergin/deps` folder where [geodiff](https://github.com/MerginMaps/geodiff) lib
+is supposed to be and install dependencies: ``` rm -r mergin/deps mkdir mergin/
+deps pip install python-dateutil pytz pip install pygeodiff --target=mergin/
+deps ``` For using mergin client with its dependencies packaged locally run:
+``` pip install wheel python3 setup.py sdist bdist_wheel mkdir -p mergin/deps
+pip wheel -r mergin_client.egg-info/requires.txt -w mergin/deps unzip mergin/
+deps/pygeodiff-*.whl -d mergin/deps pip install --editable . ``` ### Tests For
+running test do: ``` cd mergin export TEST_MERGIN_URL= # testing server export
+TEST_API_USERNAME= export TEST_API_PASSWORD= export TEST_API_USERNAME2= export
+TEST_API_PASSWORD2= pip install pytest pytest-cov coveralls pytest --cov-report
+html --cov=mergin mergin/test/ ```
```

### Comparing `mergin-client-0.8.2/mergin/cert.pem` & `mergin-client-0.8.3/mergin/cert.pem`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/mergin/cli.py` & `mergin-client-0.8.3/mergin/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pip puts these tools).
 """
 
 from datetime import datetime, timezone
 import click
 import json
 import os
+import platform
 import sys
 import time
 import traceback
 
 from mergin import (
     ClientError,
     InvalidProject,
@@ -173,15 +174,19 @@
 @click.pass_context
 def login(ctx):
     """Login to the service and see how to set the token environment variable."""
     mc = ctx.obj["client"]
     if mc is not None:
         click.secho("Login successful!", fg="green")
         token = mc._auth_session["token"]
-        click.secho(f'To set the MERGIN_AUTH variable run:\nexport MERGIN_AUTH="{token}"')
+        if platform.system() == "Windows":
+            hint = f"To set the MERGIN_AUTH variable run:\nset MERGIN_AUTH={token}"
+        else:
+            hint = f'To set the MERGIN_AUTH variable run:\nexport MERGIN_AUTH="{token}"'
+        click.secho(hint)
 
 
 @cli.command()
 @click.argument("project")
 @click.option("--public", is_flag=True, default=False, help="Public project, visible to everyone")
 @click.option(
     "--from-dir",
```

### Comparing `mergin-client-0.8.2/mergin/client.py` & `mergin-client-0.8.3/mergin/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,16 +198,25 @@
             request.add_header("Authorization", self._auth_session["token"])
         request.add_header("User-Agent", self.user_agent_info())
         try:
             return self.opener.open(request)
         except urllib.error.HTTPError as e:
             if e.headers.get("Content-Type", "") == "application/problem+json":
                 info = json.load(e)
-                raise ClientError(info.get("detail"))
-            raise ClientError(e.read().decode("utf-8"))
+                err_detail = info.get("detail")
+            else:
+                err_detail = e.read().decode("utf-8")
+
+            error_msg = (
+                f"HTTP Error: {e.code} {e.reason}\n"
+                f"URL: {request.get_full_url()}\n"
+                f"Method: {request.get_method()}\n"
+                f"Detail: {err_detail}"
+            )
+            raise ClientError(error_msg)
         except urllib.error.URLError as e:
             # e.g. when DNS resolution fails (no internet connection?)
             raise ClientError("Error requesting " + request.full_url + ": " + str(e))
 
     def get(self, path, data=None, headers={}):
         url = urllib.parse.urljoin(self.url, urllib.parse.quote(path))
         if data:
```

### Comparing `mergin-client-0.8.2/mergin/client_pull.py` & `mergin-client-0.8.3/mergin/client_pull.py`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/mergin/client_push.py` & `mergin-client-0.8.3/mergin/client_push.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 """
 
 import json
 import hashlib
 import pprint
 import tempfile
 import concurrent.futures
+import os
 
 from .common import UPLOAD_CHUNK_SIZE, ClientError
 from .merginproject import MerginProject
 
 
 class UploadJob:
     """Keeps all the important data about a pending upload job"""
@@ -282,14 +283,16 @@
     except Exception as e:
         job.mp.log.error("Failed to apply push changes: " + str(e))
         job.mp.log.info("--- push aborted")
         raise ClientError("Failed to apply push changes: " + str(e))
 
     job.tmp_dir.cleanup()  # delete our temporary dir and all its content
 
+    remove_diff_files(job)
+
     job.mp.log.info("--- push finished - new project version " + job.server_resp["version"])
 
 
 def push_project_cancel(job):
     """
     To be called (from main thread) to cancel a job that has uploads in progress.
     Returns once all background tasks have exited (may block for a bit of time).
@@ -312,7 +315,17 @@
 def _do_upload(item, job):
     """runs in worker thread"""
     if job.is_cancelled:
         return
 
     item.upload_blocking(job.mc, job.mp)
     job.transferred_size += item.size
+
+
+def remove_diff_files(job) -> None:
+    """Looks for diff files in the job and removes them."""
+
+    for change in job.changes["updated"]:
+        if "diff" in change.keys():
+            diff_file = job.mp.fpath_meta(change["diff"]["path"])
+            if os.path.exists(diff_file):
+                os.remove(diff_file)
```

### Comparing `mergin-client-0.8.2/mergin/common.py` & `mergin-client-0.8.3/mergin/common.py`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/mergin/merginproject.py` & `mergin-client-0.8.3/mergin/merginproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,14 +353,16 @@
                     file["diff"] = {
                         "path": diff_name,
                         "checksum": generate_checksum(diff_file),
                         "size": diff_size,
                         "mtime": datetime.fromtimestamp(os.path.getmtime(diff_file), tzlocal()),
                     }
                 else:
+                    if os.path.exists(diff_file):
+                        os.remove(diff_file)
                     not_updated.append(file)
             except (pygeodiff.GeoDiffLibError, pygeodiff.GeoDiffLibConflictError) as e:
                 self.log.warning("failed to create changeset for " + path)
                 # probably the database schema has been modified if geodiff cannot create changeset.
                 # we will need to do full upload of the file
                 pass
```

### Comparing `mergin-client-0.8.2/mergin/report.py` & `mergin-client-0.8.3/mergin/report.py`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/mergin/test/test_client.py` & `mergin-client-0.8.3/mergin/test/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import tempfile
 import subprocess
 import shutil
 from datetime import datetime, timedelta, date
 import pytest
 import pytz
 import sqlite3
+import glob
 
 from .. import InvalidProject
 from ..client import MerginClient, ClientError, MerginProject, LoginError, decode_token_data, TokenError, ServerType
 from ..client_push import push_project_async, push_project_cancel
 from ..utils import (
     generate_checksum,
     get_versions_with_file_changes,
@@ -615,15 +616,15 @@
 
     # try to upload
     got_right_err = False
     try:
         mc.push_project(project_dir)
     except ClientError as e:
         # Expecting "You have reached a data limit" 400 server error msg.
-        assert str(e) == "You have reached a data limit"
+        assert "You have reached a data limit" in str(e)
         got_right_err = True
     assert got_right_err
 
     # Expecting empty project
     project_info = get_project_info(mc, API_USER, test_project)
     assert project_info["version"] == "v0"
     assert project_info["disk_usage"] == 0
@@ -1886,7 +1887,31 @@
     assert info["namespace"] == API_USER
     assert info["project_name"] == test_project
     assert info["name"] == "v2"
     assert info["author"] == API_USER
     created = datetime.strptime(info["created"], "%Y-%m-%dT%H:%M:%SZ")
     assert created.date() == date.today()
     assert info["changes"]["updated"][0]["size"] == 98304
+
+
+def test_clean_diff_files(mc):
+    test_project = "test_clean"
+    project = API_USER + "/" + test_project
+    project_dir = os.path.join(TMP_DIR, test_project)  # primary project dir for updates
+    project_dir_2 = os.path.join(TMP_DIR, test_project + "_2")  # concurrent project dir
+
+    cleanup(mc, project, [project_dir, project_dir_2])
+    # create remote project
+    shutil.copytree(TEST_DATA_DIR, project_dir)
+    mc.create_project_and_push(test_project, project_dir)
+
+    # test push changes with diffs:
+    mp = MerginProject(project_dir)
+    f_updated = "base.gpkg"
+    # step 1) base.gpkg updated to inserted_1_A (inserted A feature)
+    shutil.move(mp.fpath(f_updated), mp.fpath_meta(f_updated))  # make local copy for changeset calculation
+    shutil.copy(mp.fpath("inserted_1_A.gpkg"), mp.fpath(f_updated))
+    mc.push_project(project_dir)
+
+    diff_files = glob.glob("*-diff-*", root_dir=os.path.split(mp.fpath_meta("inserted_1_A.gpkg"))[0])
+
+    assert diff_files == []
```

### Comparing `mergin-client-0.8.2/mergin/utils.py` & `mergin-client-0.8.3/mergin/utils.py`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/mergin_client.egg-info/PKG-INFO` & `mergin-client-0.8.3/mergin_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergin-client
-Version: 0.8.2
+Version: 0.8.3
 Summary: Mergin Maps utils and client
 Home-page: https://github.com/MerginMaps/mergin-py-client
 Author: Lutra Consulting Ltd.
 Author-email: info@merginmaps.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mergin-client-0.8.2/mergin_client.egg-info/SOURCES.txt` & `mergin-client-0.8.3/mergin_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mergin-client-0.8.2/setup.py` & `mergin-client-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2019 Lutra Consulting. All rights reserved.
 # Do not distribute without the express permission of the author.
 
 from setuptools import setup, find_packages
 
 setup(
     name='mergin-client',
-    version='0.8.2',
+    version='0.8.3',
     url='https://github.com/MerginMaps/mergin-py-client',
     license='MIT',
     author='Lutra Consulting Ltd.',
     author_email='info@merginmaps.com',
     description='Mergin Maps utils and client',
     long_description='Mergin Maps utils and client',
```

