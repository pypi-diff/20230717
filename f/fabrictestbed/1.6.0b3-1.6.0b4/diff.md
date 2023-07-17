# Comparing `tmp/fabrictestbed-1.6.0b3.tar.gz` & `tmp/fabrictestbed-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.6.0b3.tar", last modified: Fri Jul 14 16:28:50 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b4.tar", last modified: Mon Jul 17 15:15:47 2023, max compression
```

## Comparing `fabrictestbed-1.6.0b3.tar` & `fabrictestbed-1.6.0b4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b3/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b3/LICENSE
--rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b3/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b3/README.md
--rw-r--r--   0        0        0       24 2023-07-14 16:28:28.781860 fabrictestbed-1.6.0b3/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b3/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b3/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b3/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b3/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    20091 2023-07-14 15:30:33.271468 fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b3/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b3/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1071 2023-07-13 18:48:30.199529 fabrictestbed-1.6.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b3/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b3/test/test_cli.py
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b4/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b4/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b4/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b4/README.md
+-rw-r--r--   0        0        0       24 2023-07-17 15:05:37.299608 fabrictestbed-1.6.0b4/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b4/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b4/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b4/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b4/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    20585 2023-07-17 15:14:15.587130 fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b4/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b4/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1071 2023-07-17 15:05:27.950690 fabrictestbed-1.6.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b4/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b4/test/test_cli.py
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b4/PKG-INFO
```

### Comparing `fabrictestbed-1.6.0b3/.gitignore` & `fabrictestbed-1.6.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/LICENSE` & `fabrictestbed-1.6.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/README.md` & `fabrictestbed-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b4/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b4/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b4/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b4/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import os
 from datetime import datetime, timedelta, timezone
 from typing import Tuple, Union, List, Any, Dict
 
 import paramiko
 from fabric_cf.orchestrator.swagger_client import Sliver, Slice
 from fabric_cf.orchestrator.swagger_client.models import PoaData
+from fabric_cm.credmgr.credmgr_proxy import TokenType
 
 from fabrictestbed.slice_editor import ExperimentTopology, AdvertisedTopology, Node, GraphFormat
 from fabrictestbed.slice_manager import CredmgrProxy, OrchestratorProxy, CmStatus, Status, SliceState
 from fabrictestbed.util.constants import Constants
 
 
 class SliceManagerException(Exception):
@@ -164,27 +165,37 @@
         status, tokens = self.cm_proxy.refresh(project_id=self.project_id, scope=self.scope,
                                                refresh_token=refresh_token, file_name=self.token_location)
         if status == CmStatus.OK:
             self.tokens = tokens
             return tokens.get(CredmgrProxy.ID_TOKEN, None), tokens.get(CredmgrProxy.REFRESH_TOKEN, None)
         raise SliceManagerException(tokens.get(CredmgrProxy.ERROR))
 
-    def revoke_token(self, *, refresh_token: str = None) -> Tuple[Status, Any]:
+    def revoke_token(self, *, refresh_token: str = None, id_token: str = None,
+                     token_type: TokenType = TokenType.Refresh) -> Tuple[Status, Any]:
         """
         Revoke a refresh token
         @param refresh_token Refresh Token to be revoked
+        @param id_token Identity Token
+        @param token_type type of the token being revoked
         @return Tuple of the status and revoked refresh token
         """
-        token_to_be_revoked = refresh_token
-        if token_to_be_revoked is None:
-            token_to_be_revoked = self.get_refresh_token()
-
-        if token_to_be_revoked is not None:
-            return self.cm_proxy.revoke(refresh_token=token_to_be_revoked)
-        return Status.FAILURE, "Refresh Token cannot be None"
+        if refresh_token is None:
+            refresh_token = self.get_refresh_token()
+        if id_token is None:
+            id_token = self.get_id_token()
+
+        return self.cm_proxy.revoke(refresh_token=refresh_token, identity_token=id_token, token_type=token_type)
+
+    def token_revoke_list(self, *, project_id: str) -> Tuple[Status, Union[Exception, List[str]]]:
+        """
+        Get Token Revoke list for a project
+        @param project_id project_id
+        @return token revoke list
+        """
+        return self.cm_proxy.token_revoke_list(project_id=project_id)
 
     def clear_token_cache(self, *, file_name: str = None):
         """
         Clear the cached token
         Should be invoked when the user changes projects
         @return:
         """
```

### Comparing `fabrictestbed-1.6.0b3/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b4/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/pyproject.toml` & `fabrictestbed-1.6.0b4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.6.0b2",
+    "fabric-credmgr-client==1.6.0b4",
     "fabric-orchestrator-client==1.5.1",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.optional-dependencies]
```

### Comparing `fabrictestbed-1.6.0b3/test/test_cli.py` & `fabrictestbed-1.6.0b4/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b3/PKG-INFO` & `fabrictestbed-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.6.0b2
+Requires-Dist: fabric-credmgr-client==1.6.0b4
 Requires-Dist: fabric-orchestrator-client==1.5.1
 Requires-Dist: paramiko
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

