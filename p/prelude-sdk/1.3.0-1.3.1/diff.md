# Comparing `tmp/prelude-sdk-1.3.0.tar.gz` & `tmp/prelude-sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.3.0.tar", last modified: Tue Jun 27 14:54:28 2023, max compression
+gzip compressed data, was "prelude-sdk-1.3.1.tar", last modified: Mon Jul 17 14:58:50 2023, max compression
```

## Comparing `prelude-sdk-1.3.0.tar` & `prelude-sdk-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307729 prelude-sdk-1.3.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-27 14:54:28.307780 prelude-sdk-1.3.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.303319 prelude-sdk-1.3.0/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.305134 prelude-sdk-1.3.0/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2416 2023-06-23 19:11:07.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3711 2023-06-08 13:35:49.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.305841 prelude-sdk-1.3.0/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2964 2023-06-21 16:09:59.000000 prelude-sdk-1.3.0/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.303859 prelude-sdk-1.3.0/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-27 14:54:28.307986 prelude-sdk-1.3.0/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307430 prelude-sdk-1.3.0/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.0/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307643 prelude-sdk-1.3.0/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.0/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.757562 prelude-sdk-1.3.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-07-17 14:58:50.757637 prelude-sdk-1.3.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.753462 prelude-sdk-1.3.1/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.1/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.755252 prelude-sdk-1.3.1/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2440 2023-07-11 13:50:34.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5462 2023-07-11 13:50:34.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3727 2023-07-11 13:50:34.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2089 2023-07-17 14:47:48.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.1/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.755798 prelude-sdk-1.3.1/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.1/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.3.1/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     3201 2023-07-17 14:47:48.000000 prelude-sdk-1.3.1/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.754011 prelude-sdk-1.3.1/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-07-17 14:58:50.000000 prelude-sdk-1.3.1/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-07-17 14:58:50.000000 prelude-sdk-1.3.1/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-07-17 14:58:50.000000 prelude-sdk-1.3.1/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-07-17 14:58:50.000000 prelude-sdk-1.3.1/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-07-17 14:58:50.000000 prelude-sdk-1.3.1/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-07-17 14:58:50.757897 prelude-sdk-1.3.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.757175 prelude-sdk-1.3.1/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.1/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.1/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 14:58:50.757455 prelude-sdk-1.3.1/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.1/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.1/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.1/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.1/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.1/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.3.0/LICENSE` & `prelude-sdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/PKG-INFO` & `prelude-sdk-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.0/README.md` & `prelude-sdk-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.3.1/prelude_sdk/controllers/build_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     def update_test(self, test_id, name=None, unit=None, techniques=None, advisory=None):
         """ Update a test """
         body = dict()
         if name:
             body['name'] = name
         if unit:
             body['unit'] = unit
-        if techniques:
+        if techniques is not None:
             body['techniques'] = techniques
-        if advisory:
+        if advisory is not None:
             body['advisory'] = advisory
 
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.3.1/prelude_sdk/controllers/detect_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     @verify_credentials
     def update_endpoint(self, endpoint_id, host=None, edr_id=None, tags=None):
         """ Update an endpoint in your account """
         body = dict()
         if host:
             body['host'] = host
-        if edr_id:
+        if edr_id is not None:
             body['edr_id'] = edr_id
-        if tags:
+        if tags is not None:
             body['tags'] = tags
 
         res = requests.post(
             f'{self.account.hq}/detect/endpoint/{endpoint_id}',
             headers=self.account.headers,
             json=body,
             timeout=10
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.3.1/prelude_sdk/controllers/iam_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
             raise Exception(res.text)
         return res.text
 
     @verify_credentials
     def update_account(self, mode: int = None, company: str = None):
         """ Update properties on an account """
         body = dict()
-        if mode != None:
+        if mode is not None:
             body['mode'] = mode
-        if company:
+        if company is not None:
             body['company'] = company
 
         res = requests.put(
             f'{self.account.hq}/iam/account',
             headers=self.account.headers,
             json=body,
             timeout=10
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.3.1/prelude_sdk/controllers/partner_controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,58 +5,58 @@
 
 class PartnerController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def attach(self, name: str, api: str, user: str, secret: str):
+    def attach(self, partner_code: int, api: str, user: str, secret: str):
         """ Attach a partner to your account """
         params = dict(api=api, user=user, secret=secret)
         res = requests.post(
-            f'{self.account.hq}/partner/{name}',
+            f'{self.account.hq}/partner/{partner_code}',
             headers=self.account.headers,
             json=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def detach(self, name: str):
+    def detach(self, partner_code: int):
         """ Detach a partner from your Detect account """
         res = requests.delete(
-            f'{self.account.hq}/partner/{name}',
+            f'{self.account.hq}/partner/{partner_code}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.text
         raise Exception(res.text)
         
     @verify_credentials
-    def endpoints(self, partner_name: str, platform: str, hostname: str = '', offset: int = 0, count: int = 100):
+    def endpoints(self, partner_code: int, platform: str, hostname: str = '', offset: int = 0, count: int = 100):
         """ Get a list of endpoints from all partners """
         params = dict(platform=platform, hostname=hostname, offset=offset, count=count)
         res = requests.get(
-            f'{self.account.hq}/partner/endpoints/{partner_name}',
+            f'{self.account.hq}/partner/endpoints/{partner_code}',
             headers=self.account.headers,
             params=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def deploy(self, partner_name: str, host_ids: list):
+    def deploy(self, partner_code: int, host_ids: list):
         """ Deploy probes on all specified partner endpoints """
         params = dict(host_ids=host_ids)
         res = requests.post(
-            f'{self.account.hq}/partner/deploy/{partner_name}',
+            f'{self.account.hq}/partner/deploy/{partner_code}',
             headers=self.account.headers,
             json=params,
             timeout=30
         )
         if not res.status_code == 200:
             raise Exception(res.text)
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk/models/account.py` & `prelude-sdk-1.3.1/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/prelude_sdk/models/codes.py` & `prelude-sdk-1.3.1/prelude_sdk/models/codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     CLEANUP_ERROR = 103
     NOT_RELEVANT = 104
     QUARANTINED_1 = 105
     OUTBOUND_SECURE = 106
     EXPLOIT_PREVENTED = 107
     NO_TEST = 108
     IS_RELEVANT = 109
+    FALSE_POSITIVE = 110
     ENDPOINT_BLOCKED = 126
     QUARANTINED_2 = 127
     PROCESS_KILLED_3 = 137
     UNEXPECTED = 256
 
     @classmethod
     def _missing_(cls, value):
@@ -106,15 +107,16 @@
                 ExitCode.UNPROTECTED,
                 ExitCode.IS_RELEVANT,
             ],
             State.ERROR: [
                 ExitCode.ERROR,
                 ExitCode.MALFORMED_VST,
                 ExitCode.TIMEOUT,
-                ExitCode.UNEXPECTED
+                ExitCode.UNEXPECTED,
+                ExitCode.FALSE_POSITIVE
             ],
             State.NOT_RELEVANT: [
                 ExitCode.NOT_RELEVANT,
                 ExitCode.NO_TEST
             ]
         }
 
@@ -130,7 +132,18 @@
     @classmethod
     def normalize(cls, dos: str):
         try:
             arch = dos.split('-', 1)[-1]
             return dos[:-len(arch)].lower() + cls[arch.lower()].value
         except (KeyError, IndexError, AttributeError):
             return cls.none.value
+
+
+class Control(Enum):
+    INVALID = 0
+    CROWDSTRIKE = 1
+    DEFENDER = 2
+    SPLUNK = 3
+
+    @classmethod
+    def _missing_(cls, value):
+        return Control.INVALID
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.3.1/prelude_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.0/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.3.1/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/setup.cfg` & `prelude-sdk-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.3.0
+version = 1.3.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.3.0/tests/conftest.py` & `prelude-sdk-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/tests/test_build_controller.py` & `prelude-sdk-1.3.1/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/tests/test_detect_controller.py` & `prelude-sdk-1.3.1/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/tests/test_iam_controller.py` & `prelude-sdk-1.3.1/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.0/tests/test_probe_controller.py` & `prelude-sdk-1.3.1/tests/test_probe_controller.py`

 * *Files identical despite different names*

