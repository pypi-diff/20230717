# Comparing `tmp/boonnano-3.1.6.tar.gz` & `tmp/boonnano-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonnano-3.1.6.tar", last modified: Wed Jan 26 14:37:40 2022, max compression
+gzip compressed data, was "boonnano-3.2.0.tar", last modified: Mon Jul 17 16:54:13 2023, max compression
```

## Comparing `boonnano-3.1.6.tar` & `boonnano-3.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2022-01-26 14:37:40.370325 boonnano-3.1.6/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2020-11-16 16:38:06.000000 boonnano-3.1.6/LICENSE
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2857 2022-01-26 14:37:40.369950 boonnano-3.1.6/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2400 2020-11-16 16:38:06.000000 boonnano-3.1.6/README.md
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2022-01-26 14:37:40.367158 boonnano-3.1.6/boonnano/
--rw-r--r--   0 jimturnquist   (502) staff       (20)    34877 2022-01-26 14:26:14.000000 boonnano-3.1.6/boonnano/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3053 2021-05-18 13:50:46.000000 boonnano-3.1.6/boonnano/rest.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2022-01-26 14:37:40.369478 boonnano-3.1.6/boonnano.egg-info/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2857 2022-01-26 14:37:39.000000 boonnano-3.1.6/boonnano.egg-info/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)      223 2022-01-26 14:37:40.000000 boonnano-3.1.6/boonnano.egg-info/SOURCES.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2022-01-26 14:37:39.000000 boonnano-3.1.6/boonnano.egg-info/dependency_links.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       14 2022-01-26 14:37:39.000000 boonnano-3.1.6/boonnano.egg-info/requires.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)        9 2022-01-26 14:37:39.000000 boonnano-3.1.6/boonnano.egg-info/top_level.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2022-01-26 14:37:40.370441 boonnano-3.1.6/setup.cfg
--rw-r--r--   0 jimturnquist   (502) staff       (20)      679 2022-01-26 14:37:20.000000 boonnano-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:54:13.315988 boonnano-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 16:54:05.000000 boonnano-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-17 16:54:13.315988 boonnano-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-17 16:54:05.000000 boonnano-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:54:13.315988 boonnano-3.2.0/boonnano/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 16:54:05.000000 boonnano-3.2.0/boonnano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42047 2023-07-17 16:54:05.000000 boonnano-3.2.0/boonnano/expert_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:54:13.315988 boonnano-3.2.0/boonnano.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-17 16:54:13.000000 boonnano-3.2.0/boonnano.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 16:54:13.000000 boonnano-3.2.0/boonnano.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:54:13.000000 boonnano-3.2.0/boonnano.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 16:54:13.000000 boonnano-3.2.0/boonnano.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 16:54:13.000000 boonnano-3.2.0/boonnano.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:54:13.315988 boonnano-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 16:54:05.000000 boonnano-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:54:13.315988 boonnano-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36367 2023-07-17 16:54:05.000000 boonnano-3.2.0/tests/test_client.py
```

### Comparing `boonnano-3.1.6/LICENSE` & `boonnano-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boonnano-3.1.6/PKG-INFO` & `boonnano-3.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: boonnano
-Version: 3.1.6
+Version: 3.2.0
 Summary: A SDK package for utilizing the BoonLogic nano API
 Home-page: https://github.com/boonlogic/Python_API
 Author: BoonLogic
 Author-email: elise@boonlogic.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Logo](https://github.com/boonlogic/expert-python-sdk/blob/master/docs/BoonLogic.png?raw=true)
+
 # Python SDK Documentation
 This python package allows ease of access to calls to the BoonLogic Nano API.
 
 - __Website__: [boonlogic.com](https://boonlogic.com)
 - __Documentation__: [Boon Docs Main Page](https://docs.boonlogic.com)
-- __Clustering__: [Clustering with the expert-python-sdk](docs/Tutorial_The_General_Pipeline.md)
-- __Autotuning__: [Autotuning with the expert-python-sdk](docs/How_To_Autotune_Data.md)
-- __Results__: [Results after clustering](docs/How_To_Generate_Cluster_Results.md)
-- __SDK Functional Breakdown__: [expert-python-sdk classes and methods](docs/boonnano/index.html)
+- __Clustering__: [Clustering with the expert-python-sdk]({{ site.baseurl}}/docs/Tutorial_The_General_Pipeline.md)
+- __Autotuning__: [Autotuning with the expert-python-sdk]({{ site.baseurl}}/docs/How_To_Autotune_Data.md)
+- __Results__: [Results after clustering]({{ site.baseurl}}/docs/How_To_Generate_Cluster_Results.md)
+- __SDK Functional Breakdown__: [expert-python-sdk classes and methods]({{ site.baseurl}}/docs/boonnano/index.html)(docs/boonnano/index.html)
 
 ---------
 ## Installation
 
 The BoonNano SDK is a Python3 project and can be installed via pip.
 
 ```
@@ -61,40 +62,36 @@
 **connect-example.py**
 
 ```python
 import boonnano as bn
 import json
 import sys
 
-# create new nano handle
+#
+# connectivity example for boonnano
+#
+
 try:
-    nano = bn.NanoHandle('default')
-except bn.BoonException as be:
-    print(be)
-    sys.exit(1)
+    # create client handle
+    nano = bn.ExpertClient.from_license_file(license_id='default')
 
-# open/attach to nano
-success, response = nano.open_nano('my-instance')
-if not success:
-    print("open_nano failed: {}".format(response))
-    sys.exit(1)
+    # open/attach to nano
+    instance_id = 'my-instance'
+    nano.open_nano(instance_id)
+
+    # retrieve server version
+    response = nano.get_version()
+    print(json.dumps(response, indent=4))
 
-# fetch the version information for this nano instance
-success, response = nano.get_version()
-if not success:
-    print("get_version failed: {}".format(response))
-    sys.exit(1)
-print(json.dumps(response, indent=4))
+    # close/detach the nano instance
+    nano.close_nano(instance_id)
 
-# close/detach the nano instance
-success, response = nano.close_nano()
-if not success:
-    print("close_nano failed: {}".format(response))
+except bn.BoonException as be:
+    print(be.message)
     sys.exit(1)
-
 ```
 
 Running the connect-test.py script should yield something like:
 
 ```sh
 % python connect-example.py
 {
@@ -103,9 +100,7 @@
     "nano-secure": "3c40f1d6",
     "builder": "f5db0682",
     "expert-api": "f6643822",
     "expert-common": "c0575a50",
     "swagger-ui": "914af396"
 }
 ```
-
-
```

### Comparing `boonnano-3.1.6/README.md` & `boonnano-3.2.0/boonnano.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+Metadata-Version: 2.1
+Name: boonnano
+Version: 3.2.0
+Summary: A SDK package for utilizing the BoonLogic nano API
+Home-page: https://github.com/boonlogic/Python_API
+Author: BoonLogic
+Author-email: elise@boonlogic.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Logo](https://github.com/boonlogic/expert-python-sdk/blob/master/docs/BoonLogic.png?raw=true)
+
 # Python SDK Documentation
 This python package allows ease of access to calls to the BoonLogic Nano API.
 
 - __Website__: [boonlogic.com](https://boonlogic.com)
 - __Documentation__: [Boon Docs Main Page](https://docs.boonlogic.com)
-- __Clustering__: [Clustering with the expert-python-sdk](docs/Tutorial_The_General_Pipeline.md)
-- __Autotuning__: [Autotuning with the expert-python-sdk](docs/How_To_Autotune_Data.md)
-- __Results__: [Results after clustering](docs/How_To_Generate_Cluster_Results.md)
-- __SDK Functional Breakdown__: [expert-python-sdk classes and methods](docs/boonnano/index.html)
+- __Clustering__: [Clustering with the expert-python-sdk]({{ site.baseurl}}/docs/Tutorial_The_General_Pipeline.md)
+- __Autotuning__: [Autotuning with the expert-python-sdk]({{ site.baseurl}}/docs/How_To_Autotune_Data.md)
+- __Results__: [Results after clustering]({{ site.baseurl}}/docs/How_To_Generate_Cluster_Results.md)
+- __SDK Functional Breakdown__: [expert-python-sdk classes and methods]({{ site.baseurl}}/docs/boonnano/index.html)(docs/boonnano/index.html)
 
 ---------
 ## Installation
 
 The BoonNano SDK is a Python3 project and can be installed via pip.
 
 ```
@@ -46,40 +62,36 @@
 **connect-example.py**
 
 ```python
 import boonnano as bn
 import json
 import sys
 
-# create new nano handle
+#
+# connectivity example for boonnano
+#
+
 try:
-    nano = bn.NanoHandle('default')
-except bn.BoonException as be:
-    print(be)
-    sys.exit(1)
+    # create client handle
+    nano = bn.ExpertClient.from_license_file(license_id='default')
 
-# open/attach to nano
-success, response = nano.open_nano('my-instance')
-if not success:
-    print("open_nano failed: {}".format(response))
-    sys.exit(1)
+    # open/attach to nano
+    instance_id = 'my-instance'
+    nano.open_nano(instance_id)
+
+    # retrieve server version
+    response = nano.get_version()
+    print(json.dumps(response, indent=4))
 
-# fetch the version information for this nano instance
-success, response = nano.get_version()
-if not success:
-    print("get_version failed: {}".format(response))
-    sys.exit(1)
-print(json.dumps(response, indent=4))
+    # close/detach the nano instance
+    nano.close_nano(instance_id)
 
-# close/detach the nano instance
-success, response = nano.close_nano()
-if not success:
-    print("close_nano failed: {}".format(response))
+except bn.BoonException as be:
+    print(be.message)
     sys.exit(1)
-
 ```
 
 Running the connect-test.py script should yield something like:
 
 ```sh
 % python connect-example.py
 {
```

### Comparing `boonnano-3.1.6/boonnano/__init__.py` & `boonnano-3.2.0/boonnano/expert_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,207 +1,325 @@
-from urllib3 import ProxyManager
-from urllib3 import PoolManager
-from urllib3 import Timeout
 from functools import wraps
 import json
 import os
 import tarfile
-from .rest import simple_get
-from .rest import simple_delete
-from .rest import simple_post
-from .rest import multipart_post
+import gzip
+
+import requests
 import numpy as np
 
 # urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-__all__ = ['BoonException', 'NanoHandle']
-
-
 ############################
 # BoonNano Python API v3.1 #
 ############################
 
 
 class BoonException(Exception):
-    def __init__(self, message):
+    def __init__(self, code=None, message=None):
+        self.status_code = code
         self.message = message
 
 
-class NanoHandle:
+class LicenseProfile:
+    def __init__(
+        self,
+        api_key: str = None,
+        api_tenant: str = None,
+        server: str = None,
+        proxy_server: str = None,
+    ):
+        self.api_key = api_key
+        self.api_tenant = api_tenant
+        self.server = server
+        self.proxy_server = proxy_server
+
+
+class ExpertClient:
+
+    """Primary handle for BoonNano Pod instances
+
+    This is the primary handle to manage a nano pod instance
+
+    Environment:
+    BOON_SSL_CERT: specifies location of ssl certification
+    BOON_SSL_VERIFY: verify cert of server (default is true, ignored if http connection)
+    BOON_TIMEOUT: request timeout (default is 300)
+    """
+
+    def __init__(self, profile: LicenseProfile = None):
+        self.results = [
+            "ID",
+            "SI",
+            "RI",
+            "FI",
+            "DI",
+            "AD",
+            "AH",
+            "AM",
+            "AW",
+            "NI",
+            "NS",
+            "NW",
+            "OM",
+            "PI",
+        ]
+        self.user_agent = "Boon Logic / expert-python-sdk / requests"
+        self.server = profile.server
+        self.proxy_server = profile.proxy_server
+        self.api_key = profile.api_key
+        self.api_tenant = profile.api_tenant
+        self.numeric_format = ""
+
+        if self.server is None:
+            raise BoonException(400, "server not specified")
+        if self.api_key is None:
+            raise BoonException(400, "api-key not specified")
+        if self.api_tenant is None:
+            raise BoonException(400, "api-tenant not specified")
+
+        self.ssl_cert = os.environ.get("BOON_SSL_CERT", None)
+        self.ssl_verify = os.environ.get("BOON_SSL_VERIFY", "true").lower() == "true"
+        self.timeout = int(os.environ.get("BOON_TIMEOUT", "300"))
+
+        # set up base url
+        self.url = self.server + "/expert/v3"
+        if "http" not in self.server:
+            self.url = "http://" + self.url
 
-    def __init__(self, license_id='default', license_file="~/.BoonLogic.license", timeout=120.0, verify=True, cert=None):
+    @classmethod
+    def from_license_file(
+        cls, license_file: str = "~/.BoonLogic.license", license_id: str = "default"
+    ):
         """Primary handle for BoonNano Pod instances
 
-        The is the primary handle to manage a nano pod instance
+         This is the primary handle to manage a nano pod instance
 
         Args:
-            license_id (str): license identifier label found within the .BoonLogic.license configuration file
-            license_file (str): path to .BoonLogic license file
-            timeout (float): read timeout for http requests
-            verify:  Either a boolean, in which case it controls whether we verify the server’s TLS certificate, or a string, in which case it must be a path to a CA bundle to use
-            cert (bool): if String, path to ssl client cert file (.pem). If Tuple, (‘cert’, ‘key’) pair.
-        
+        license_file (str): path to .BoonLogic license file
+        license_id (str): license identifier label found within the .BoonLogic.license configuration file
 
         Environment:
-            BOON_LICENSE_FILE: sets license_file path
-            BOON_LICENSE_ID: sets license_id
-            BOON_API_KEY: overrides the api-key as found in .BoonLogic.license file
-            BOON_API_TENANT: overrides the api-tenant as found in .BoonLogic.license file
-            BOON_SERVER: overrides the server as found in .BoonLogic.license file
-            PROXY_SERVER: overrides the proxy server as found in .BoonLogic.license file
-            BOON_SSL_CERT: path to ssl client cert file (.pem)
-            BOON_SSL_VERIFY: Either a boolean, in which case it controls whether we verify the server’s TLS certificate, or a string, in which case it must be a path to a CA bundle to use
-
-
-        Example:
-            ```python
-            try:
-                nano = bn.NanoHandle()
-            except bn.BoonException as be:
-                print(be)
-                sys.exit(1)
-            ```
-
-        """
-        self.license_id = None
-        self.api_key = None
-        self.api_tenant = None
-        self.instance = ''
-        self.numeric_format = ''
-
-        env_license_file = os.environ.get('BOON_LICENSE_FILE', None)
-        env_license_id = os.environ.get('BOON_LICENSE_ID', None)
-        env_api_key = os.environ.get('BOON_API_KEY', None)
-        env_api_tenant = os.environ.get('BOON_API_TENANT', None)
-        env_server = os.environ.get('BOON_SERVER', None)
-        env_proxy_server = os.environ.get('PROXY_SERVER', None)
-        env_cert = os.environ.get('BOON_SSL_CERT', None)
-        env_verify = os.environ.get('BOON_SSL_VERIFY', None)
-
-        # certificates
-        self.cert = 'CERT_REQUIRED' if env_cert else {None: 'CERT_NONE', True: 'CERT_REQUIRED'}[cert]
-        if env_verify:
-            if env_verify.lower() == 'false':
-                self.verify = False
-            elif env_verify.lower() == 'true':
-                self.verify = True
-            else:
-                self.verify = env_verify
-        else:
-            self.verify = verify
-
-        # when license_id comes in as None, use 'default'
-        if license_id is None:
-            license_id = 'default'
+        BOON_LICENSE_FILE: Specifies location of BOON_LICENSE_FILE.  This will override the license_file parameter
+        BOON_LICENSE_ID: Specifies the profile id.  This will override the license_id parameter
+        """
 
-        license_file = env_license_file if env_license_file else license_file
-        self.license_id = env_license_id if env_license_id else license_id
+        license_file = os.environ.get("BOON_LICENSE_FILE", license_file)
+        license_id = os.environ.get("BOON_LICENSE_ID", license_id)
 
         license_path = os.path.expanduser(license_file)
         if not os.path.exists(license_path):
-            raise BoonException("license file {} does not exist".format(license_path))
+            raise BoonException(404, 'license_file "{}" not found'.format(license_path))
+
         try:
-            with open(license_path, "r") as json_file:
-                file_data = json.load(json_file)
+            with open(license_path, "r") as f:
+                file_data = json.load(f)
         except json.JSONDecodeError as e:
             raise BoonException(
-                "json formatting error in .BoonLogic.license file, {}, line: {}, col: {}".format(e.msg, e.lineno,
-                                                                                                     e.colno))       
-        try:
-            license_data = file_data[self.license_id]
-        except KeyError:
-            raise BoonException("license_id \"{}\" not found in license file".format(self.license_id))
-
-        try:
-            self.api_key = env_api_key if env_api_key else license_data['api-key']
-        except KeyError:
-            raise BoonException("\"api-key\" is missing from the specified license in license file")
+                400,
+                "JSON formatting error in license file: {}, line: {}, col: {}, message:{}".format(
+                    license_path, e.lineno, e.colno, e.msg
+                ),
+            )
 
-        try:
-            self.api_tenant = env_api_tenant if env_api_tenant else license_data['api-tenant']
-        except KeyError:
-            raise BoonException("\"api-tenant\" is missing from the specified license in license file")
+        if license_id not in file_data:
+            raise BoonException(
+                404,
+                'license_id "{}" not found in license file {}'.format(
+                    license_id, license_path
+                ),
+            )
+
+        profile = file_data[license_id]
+
+        server = profile.get("server", None)
+        proxy_server = profile.get("proxy-server", None)
+        api_key = profile.get("api-key", None)
+        api_tenant = profile.get("api-tenant", None)
+
+        return cls(
+            profile=LicenseProfile(
+                server=server,
+                proxy_server=proxy_server,
+                api_key=api_key,
+                api_tenant=api_tenant,
+            )
+        )
 
+    @classmethod
+    def from_dict(cls, profile_dict: dict = None):
         try:
-            self.server = env_server if env_server else license_data['server']
-        except KeyError:
-            raise BoonException("\"server\" is missing from the specified license in license file")
-
-        self.proxy_server = env_proxy_server 
-        if not self.proxy_server and 'proxy-server' in license_data.keys():
-            self.proxy_server = license_data['proxy-server']
-
-        # set up base url
-        self.url = self.server + '/expert/v3/'
-        if "http" not in self.server:
-            self.url = "http://" + self.url
-
-        # create pool manager
-        timeout_inst = Timeout(connect=30.0, read=timeout)
-        if self.proxy_server:
-            # proxy pool
-            self.http = ProxyManager(self.proxy_server, maxsize=10, timeout=timeout_inst, cert_reqs=self.cert)
-        else:
-            # non-proxy pool
-            self.http = PoolManager(timeout=timeout_inst, cert_reqs=self.cert)
+            server = profile_dict.get("server", None)
+            api_key = profile_dict.get("api-key", None)
+            api_tenant = profile_dict.get("api-tenant", None)
+            proxy_server = profile_dict.get("proxy-server", None)
+        except json.JSONDecodeError as e:
+            raise BoonException(400, "JSON formatting error, message:{}".format(e.msg))
+        return cls(
+            profile=LicenseProfile(
+                server=server,
+                proxy_server=proxy_server,
+                api_key=api_key,
+                api_tenant=api_tenant,
+            )
+        )
 
     def _is_configured(f):
         @wraps(f)
         def inner(*args, **kwargs):
-            if args[0].numeric_format not in ['int16', 'uint16', 'float32']:
-                return False, "nano instance is not configured"
+            if args[0].numeric_format not in ["int16", "uint16", "float32"]:
+                raise BoonException(400, "nano instance is not configured")
             return f(*args, **kwargs)
 
         return inner
 
-    def open_nano(self, instance_id):
+    def _api_call(self, method, url, headers, body=None, fields=None):
+        """Make a REST call to the Expert server and handle the response"""
+        headers["x-token"] = self.api_key
+        headers["User-Agent"] = self.user_agent
+
+        if "Content-Type" in headers and "json" in headers["Content-Type"]:
+            body = json.dumps(body)
+
+        if method == "POST" and body is not None and len(body) > 10000:
+            headers["content-encoding"] = "gzip"
+            body = gzip.compress(body.encode("utf-8"))
+
+        try:
+            response = requests.request(
+                method=method,
+                url=url,
+                headers=headers,
+                data=body,
+                verify=self.ssl_verify,
+                timeout=self.timeout,
+                cert=self.ssl_cert,
+                files=fields,
+            )
+        except requests.exceptions.Timeout:
+            # request timed out
+            raise BoonException(500, "request timed out")
+        except requests.exceptions.ConnectionError:
+            raise BoonException(500, "server does not exist")
+
+        if response.status_code > 299:
+            try:
+                msg = response.json()
+                try:
+                    msg = msg.get("message", "no message")
+                except AttributeError:
+                    pass
+            except json.JSONDecodeError:
+                msg = response.text
+            raise BoonException(response.status_code, msg)
+
+        try:
+            respbody = response.json()
+        except Exception:
+            # save nano or load data
+            return response.content
+
+        # if code is returned in the message, it should agree with the header
+        if (
+            isinstance(respbody, dict)
+            and "code" in respbody
+            and respbody["code"] != response.status_code
+        ):
+            raise BoonException(respbody["code"], respbody.get("message", "no message"))
+
+        if isinstance(respbody, dict) and "errorMessage" in respbody:
+            raise BoonException(500, respbody["errorMessage"])
+
+        return response
+
+    def _format_results(self, results):
+        results_str = ""
+        if str(results) == "All":
+            results_str = ",".join(self.results)
+        elif results is not None:
+            results_str = results if isinstance(results, str) else ",".join(results)
+        return results_str
+
+    def open_nano(self, instance_id: str):
         """Creates or attaches to a nano pod instance
 
         Args:
             instance_id (str): instance identifier to assign to new pod instance
 
         Returns:
-            boolean: true if successful (instance is created or attached)
+            response (dict): metadata about the instance
+
+        """
+
+        url = (
+            self.url + "/nanoInstance/" + instance_id + "?api-tenant=" + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
+
+    def get_nano_instance(self, instance_id: str):
+        """Get instance info
 
-            str: None when result is true, error string when result=false
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
+        Returns:
+            response (dict): metadata about the instance
 
         """
-        instance_cmd = self.url + 'nanoInstance/' + instance_id + '?api-tenant=' + self.api_tenant
 
-        success, response = simple_post(self, instance_cmd)
-        if not success:
-            return False, response
+        url = (
+            self.url + "/nanoInstance/" + instance_id + "?api-tenant=" + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-        self.instance = instance_id
-        return success, response
+        return response.json()
 
-    def close_nano(self):
+    def close_nano(self, instance_id: str):
         """Closes the pod instance
 
-        Returns:
-            result (boolean):  true if successful (nano pod instance was closed)
-            response (str): None when result is true, error string when result=false
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
 
         """
-        close_cmd = self.url + 'nanoInstance/' + self.instance + '?api-tenant=' + self.api_tenant
 
-        # delete instance
-        result, response = simple_delete(self, close_cmd)
-        if not result:
-            return result, response
-
-        self.http.clear()
-        return result, None
-
-    def create_config(self, feature_count, numeric_format, cluster_mode='batch', min_val=0, max_val=1,
-                      weight=1, label=None,
-                      percent_variation=0.05, streaming_window=1, accuracy=0.99,
-                      autotune_pv=True, autotune_range=True, autotune_by_feature=True, autotune_max_clusters=1000,
-                      exclusions=None, streaming_autotune=True, streaming_buffer=10000, anomaly_history_window=10000,
-                      learning_numerator=10, learning_denominator=10000, learning_max_clusters=1000, learning_samples=1000000):
+        url = (
+            self.url + "/nanoInstance/" + instance_id + "?api-tenant=" + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        self._api_call("DELETE", url, headers)
+
+    def create_config(
+        self,
+        feature_count: int,
+        numeric_format: str,
+        cluster_mode: str = "batch",
+        min_val=0,
+        max_val=1,
+        weight=1,
+        label=None,
+        percent_variation: float = 0.05,
+        streaming_window: int = 1,
+        accuracy: float = 0.99,
+        autotune_pv: bool = True,
+        autotune_range: bool = True,
+        autotune_by_feature: bool = True,
+        autotune_max_clusters: int = 1000,
+        exclusions: list = None,
+        streaming_autotune: bool = True,
+        streaming_buffer: int = 10000,
+        anomaly_history_window: int = 10000,
+        learning_numerator: int = 10,
+        learning_denominator: int = 10000,
+        learning_max_clusters: int = 1000,
+        learning_samples: int = 1000000,
+    ):
         """Generate a configuration template for the given parameters
 
         A discrete configuration is specified as a list of min, max, weights, and labels
 
         Args:
             feature_count (int): number of features per vector
             numeric_format (str): numeric type of data (one of "float32", "uint16", or "int16")
@@ -227,614 +345,919 @@
             learning_numerator (int): max number of new clusters learned
             learning_denominator (int): number of samples over which the new clusters are learned
             learning_max_clusters (int): max number of clusters before turning off learning
             learning_samples (int): max number of samples before turning off learning
 
 
         Returns:
-            result (boolean): true if successful (configuration was successfully created)
-            response (dict or str): configuration dictionary when result is true, error string when result is false
+            config (dict): configuration dictionary
 
         """
 
         if isinstance(min_val, int) or isinstance(min_val, float):
             min_val = [min_val] * feature_count
         if isinstance(max_val, int) or isinstance(max_val, float):
             max_val = [max_val] * feature_count
         if isinstance(weight, int):
             weight = [weight] * feature_count
 
         if exclusions is None:
             exclusions = []
 
         config = {}
-        config['clusterMode'] = cluster_mode
-        config['numericFormat'] = numeric_format
-        config['features'] = []
-
-        if (isinstance(min_val, list) or isinstance(min_val, np.ndarray)) and (
-                isinstance(max_val, list) or isinstance(max_val, np.ndarray)) and (
-                isinstance(weight, list) or isinstance(weight, np.ndarray)):
+        config["clusterMode"] = cluster_mode
+        config["numericFormat"] = numeric_format
+        config["features"] = []
+
+        if (
+            (isinstance(min_val, list) or isinstance(min_val, np.ndarray))
+            and (isinstance(max_val, list) or isinstance(max_val, np.ndarray))
+            and (isinstance(weight, list) or isinstance(weight, np.ndarray))
+        ):
             if len(min_val) != len(max_val) or len(min_val) != len(weight):
-                return False, "parameters must be lists of the same length"
+                raise BoonException(
+                    message="parameters must be lists of the same length"
+                )
 
             for min, max, w in zip(min_val, max_val, weight):
                 tempDict = {}
-                tempDict['minVal'] = min
-                tempDict['maxVal'] = max
-                tempDict['weight'] = w
-                config['features'].append(tempDict)
+                tempDict["minVal"] = min
+                tempDict["maxVal"] = max
+                tempDict["weight"] = w
+                config["features"].append(tempDict)
         else:
-            return False, "min_val, max_val and weight must be list or numpy array"
+            raise BoonException(
+                message="min_val, max_val and weight must be list or numpy array"
+            )
 
         if isinstance(label, list):
             if len(label) != len(min_val):
-                return False, "label must be the same length as other parameters"
+                raise BoonException(
+                    message="label must be the same length as other parameters"
+                )
             for i, l in enumerate(label):
-                config['features'][i]['label'] = l
+                config["features"][i]["label"] = l
         elif label:
-            return False, "label must be list"
+            raise BoonException(message="label must be list")
 
-        config['percentVariation'] = percent_variation
-        config['accuracy'] = accuracy
-        config['streamingWindowSize'] = streaming_window
-
-        config['autoTuning'] = {}
-        config['autoTuning']['autoTuneByFeature'] = autotune_by_feature
-        config['autoTuning']['autoTunePV'] = autotune_pv
-        config['autoTuning']['autoTuneRange'] = autotune_range
-        config['autoTuning']['maxClusters'] = autotune_max_clusters
+        config["percentVariation"] = percent_variation
+        config["accuracy"] = accuracy
+        config["streamingWindowSize"] = streaming_window
+
+        config["autoTuning"] = {}
+        config["autoTuning"]["autoTuneByFeature"] = autotune_by_feature
+        config["autoTuning"]["autoTunePV"] = autotune_pv
+        config["autoTuning"]["autoTuneRange"] = autotune_range
+        config["autoTuning"]["maxClusters"] = autotune_max_clusters
         if isinstance(exclusions, list):
-            config['autoTuning']['exclusions'] = exclusions
+            config["autoTuning"]["exclusions"] = exclusions
         elif exclusions:
-            return False, 'exclusions must be a list'
-
-        if config['clusterMode'] == 'streaming':
-            config['streaming'] = {}
-            config['streaming']['enableAutoTuning'] = streaming_autotune
-            config['streaming']['samplesToBuffer'] = streaming_buffer
-            config['streaming']['anomalyHistoryWindow'] = anomaly_history_window
-            config['streaming']['learningRateNumerator'] = learning_numerator
-            config['streaming']['learningRateDenominator'] = learning_denominator
-            config['streaming']['learningMaxClusters'] = learning_max_clusters
-            config['streaming']['learningMaxSamples'] = learning_samples
-
-        return True, config
-
-    def configure_nano(self, feature_count=1, numeric_format='float32', cluster_mode='batch', min_val=0, max_val=1,
-                       weight=1, label=None,
-                       percent_variation=.05, streaming_window=1, accuracy=.99,
-                       autotune_pv=True, autotune_range=True, autotune_by_feature=True, autotune_max_clusters=1000,
-                       exclusions=None,
-                       streaming_autotune=True, streaming_buffer=10000, anomaly_history_window=10000,
-                       learning_numerator=10, learning_denominator=10000, learning_max_clusters=1000, learning_samples=1000000,
-                       config=None):
+            raise BoonException(message="exclusions must be a list")
 
+        if config["clusterMode"] == "streaming":
+            config["streaming"] = {}
+            config["streaming"]["enableAutoTuning"] = streaming_autotune
+            config["streaming"]["samplesToBuffer"] = streaming_buffer
+            config["streaming"]["anomalyHistoryWindow"] = anomaly_history_window
+            config["streaming"]["learningRateNumerator"] = learning_numerator
+            config["streaming"]["learningRateDenominator"] = learning_denominator
+            config["streaming"]["learningMaxClusters"] = learning_max_clusters
+            config["streaming"]["learningMaxSamples"] = learning_samples
+
+        return config
+
+    def configure_nano(
+        self,
+        instance_id: str,
+        feature_count: int = 1,
+        numeric_format: str = "float32",
+        cluster_mode: str = "batch",
+        min_val=0,
+        max_val=1,
+        weight=1,
+        label=None,
+        percent_variation: float = 0.05,
+        streaming_window: int = 1,
+        accuracy: float = 0.99,
+        autotune_pv: bool = True,
+        autotune_range: bool = True,
+        autotune_by_feature: bool = True,
+        autotune_max_clusters: int = 1000,
+        exclusions: list = None,
+        streaming_autotune: bool = True,
+        streaming_buffer: int = 10000,
+        anomaly_history_window: int = 10000,
+        learning_numerator: int = 10,
+        learning_denominator: int = 10000,
+        learning_max_clusters: int = 1000,
+        learning_samples: int = 1000000,
+        config: dict = None,
+    ):
         """Returns the posted clustering configuration
 
-         Args:
-             feature_count (int): number of features per vector
-             numeric_format (str): numeric type of data (one of "float32", "uint16", or "int16")
-             cluster_mode (str): 'streaming' or 'batch' mode to run expert
-             min_val: list of minimum values per feature, if specified as a single value, use that on all features
-             max_val: list of maximum values per feature, if specified as a single value, use that on all features
-             weight: influence each column has on creating a new cluster
-             label (list): name of each feature (if applicable)
-             percent_variation (float): amount of variation within each cluster
-             streaming_window (integer): number of consecutive vectors treated as one inference (parametric parameter)
-             accuracy (float): statistical accuracy of the clusters
-             autotune_pv (bool): whether to autotune the percent variation
-             autotune_range (bool): whether to autotune the min and max values
-             autotune_by_feature (bool): whether to have individually set min and max values for each feature
-             autotune_max_clusters (int): max number of clusters allowed
-             exclusions (list): features to exclude while autotuning
-             streaming_autotune (bool): whether to autotune while in streaming mode
-             streaming_buffer (int): number of samples to autotune on
-             anomaly_history_window (int): number of samples to use for AH calculation
-             learning_numerator (int): max number of new clusters learned
-             learning_denominator (int): number of samples over which the new clusters are learned
-             learning_max_clusters (int): max number of clusters before turning off learning
-             learning_samples (int): max number of samples before turning off learning
-             config (dict): dictionary of configuration parameters
-
-         Returns:
-             result (boolean): true if successful (configuration was successfully loaded into nano pod instance)
-             response (dict or str): configuration dictionary when result is true, error string when result is false
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+            feature_count (int): number of features per vector
+            numeric_format (str): numeric type of data (one of "float32", "uint16", or "int16")
+            cluster_mode (str): 'streaming' or 'batch' mode to run expert
+            min_val: list of minimum values per feature, if specified as a single value, use that on all features
+            max_val: list of maximum values per feature, if specified as a single value, use that on all features
+            weight: influence each column has on creating a new cluster
+            label (list): name of each feature (if applicable)
+            percent_variation (float): amount of variation within each cluster
+            streaming_window (integer): number of consecutive vectors treated as one inference (parametric parameter)
+            accuracy (float): statistical accuracy of the clusters
+            autotune_pv (bool): whether to autotune the percent variation
+            autotune_range (bool): whether to autotune the min and max values
+            autotune_by_feature (bool): whether to have individually set min and max values for each feature
+            autotune_max_clusters (int): max number of clusters allowed
+            exclusions (list): features to exclude while autotuning
+            streaming_autotune (bool): whether to autotune while in streaming mode
+            streaming_buffer (int): number of samples to autotune on
+            anomaly_history_window (int): number of samples to use for AH calculation
+            learning_numerator (int): max number of new clusters learned
+            learning_denominator (int): number of samples over which the new clusters are learned
+            learning_max_clusters (int): max number of clusters before turning off learning
+            learning_samples (int): max number of samples before turning off learning
+            config (dict): dictionary of configuration parameters
+
+        Returns:
+            response (dict): configuration dictionary
 
-         """
+        """
 
         if config is None:
-            success, config = self.create_config(feature_count, numeric_format, cluster_mode, min_val, max_val, weight,
-                                                 label, percent_variation, streaming_window, accuracy,
-                                                 autotune_pv, autotune_range, autotune_by_feature,
-                                                 autotune_max_clusters, exclusions,
-                                                 streaming_autotune, streaming_buffer, anomaly_history_window,
-                                                 learning_numerator, learning_denominator,
-                                                 learning_max_clusters, learning_samples)
-            if not success:
-                return False, config
-        body = json.dumps(config)
-
-        config_cmd = self.url + 'clusterConfig/' + self.instance + '?api-tenant=' + self.api_tenant
-        result, response = simple_post(self, config_cmd, body=body)
-        if result:
-            self.numeric_format = config['numericFormat']
+            config = self.create_config(
+                feature_count,
+                numeric_format,
+                cluster_mode,
+                min_val,
+                max_val,
+                weight,
+                label,
+                percent_variation,
+                streaming_window,
+                accuracy,
+                autotune_pv,
+                autotune_range,
+                autotune_by_feature,
+                autotune_max_clusters,
+                exclusions,
+                streaming_autotune,
+                streaming_buffer,
+                anomaly_history_window,
+                learning_numerator,
+                learning_denominator,
+                learning_max_clusters,
+                learning_samples,
+            )
+
+        body = config
+
+        url = (
+            self.url
+            + "/clusterConfig/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers, body)
 
-        return result, response
+        self.numeric_format = config["numericFormat"]
+
+        return response.json()
 
     def nano_list(self):
         """Returns list of nano instances allocated for a pod
 
         Returns:
-            result (boolean):  true if successful (list was returned)
-            response (str): json dictionary of pod instances when result=true, error string when result=false
+            response (dict): json dictionary of pod instances
 
         """
 
-        # build command
-        instance_cmd = self.url + 'nanoInstances' + '?api-tenant=' + self.api_tenant
+        url = self.url + "/nanoInstances/" + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-        return simple_get(self, instance_cmd)
+        return response.json()
 
     @_is_configured
-    def save_nano(self, filename):
+    def save_nano(self, instance_id: str, filename: str):
         """serialize a nano pod instance and save to a local file
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             filename (str): path to local file where saved pod instance should be written
 
-        Returns:
-            result (boolean):  true if successful (pod instance was written)
-            response (str): None when result is true, error string when result=false
-
         """
 
-        # build command
-        snapshot_cmd = self.url + 'snapshot/' + self.instance + '?api-tenant=' + self.api_tenant
-
-        # serialize nano
-        result, response = simple_get(self, snapshot_cmd)
-        if not result:
-            return result, response
+        url = self.url + "/snapshot/" + instance_id + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
         # at this point, the call succeeded, saves the result to a local file
         try:
-            with open(filename, 'wb') as fp:
+            with open(filename, "wb") as fp:
                 fp.write(response)
         except Exception as e:
-            return False, e.strerror
-
-        return True, None
+            raise BoonException(message=str(e))
 
-    def restore_nano(self, filename):
+    def restore_nano(self, instance_id: str, filename: str):
         """Restore a nano pod instance from local file
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             filename (str): path to local file containing saved pod instance
 
         Returns:
-            result (boolean):  true if successful (nano pod instance was restored)
-            response (str): None when result is true, error string when result=false
+            response (dict): config dictionary of the uploaded nano
 
         """
 
         # verify that input file is a valid nano file (gzip'd tar with Magic Number)
         try:
-            with tarfile.open(filename, 'r:gz') as tp:
-                with tp.extractfile('/CommonState/MagicNumber') as magic_fp:
+            with tarfile.open(filename, "r:gz") as tp:
+                with tp.extractfile("CommonState/MagicNumber") as magic_fp:
                     magic_num = magic_fp.read()
-                    if magic_num != b'\xda\xba':
-                        return False, 'file {} is not a Boon Logic nano-formatted file, bad magic number'.format(
-                            filename)
+                    if magic_num != b"\xda\xba":
+                        raise BoonException(
+                            message="file {} is not a Boon Logic nano-formatted file, bad magic number".format(
+                                filename
+                            )
+                        )
         except KeyError:
-            return False, 'file {} is not a Boon Logic nano-formatted file'.format(filename)
+            raise BoonException(
+                message="file {} is not a Boon Logic nano-formatted file".format(
+                    filename
+                )
+            )
         except Exception as e:
-            return False, 'corrupt file {}'.format(filename)
+            raise BoonException(message="corrupt file {}".format(filename))
 
-        with open(filename, 'rb') as fp:
+        with open(filename, "rb") as fp:
             nano = fp.read()
 
-        # build command
-        snapshot_cmd = self.url + 'snapshot/' + self.instance + '?api-tenant=' + self.api_tenant
-
-        fields = {'snapshot': (filename, nano)}
+        fields = {"snapshot": (filename, nano)}
 
-        result, response = multipart_post(self, snapshot_cmd, fields=fields)
+        url = self.url + "/snapshot/" + instance_id + "?api-tenant=" + self.api_tenant
+        headers = {}
+        response = self._api_call("POST", url, headers, fields=fields)
 
-        if not result:
-            return result, response
+        response = response.json()
 
-        self.numeric_format = response['numericFormat']
+        self.numeric_format = response["numericFormat"]
 
-        return True, response
+        return response
 
     @_is_configured
-    def autotune_config(self):
+    def autotune_config(self, instance_id: str):
         """Autotunes the percent variation, min and max for each feature
 
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
+        """
+
+        url = self.url + "/autoTune/" + instance_id + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        self._api_call("POST", url, headers)
+
+    @_is_configured
+    def get_autotune_array(self, instance_id: str):
+        """Gets the autotune elbow
+
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
         Returns:
-            result (boolean): true if successful (autotuning was completed)
-            response (dict or str): configuration dictionary when result is true, error string when result is false
+            response (list): 2D array of the autotuning elbox values
 
         """
 
-        # build command
-        config_cmd = self.url + 'autoTune/' + self.instance + '?api-tenant=' + self.api_tenant
+        url = (
+            self.url
+            + "/autotuneArray/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-        # autotune parameters
-        return simple_post(self, config_cmd)
+        return response.json()
 
     @_is_configured
-    def get_config(self):
+    def get_config(self, instance_id: str):
         """Gets the configuration for this nano pod instance
 
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
         Returns:
-            result (boolean): true if successful (configuration was found)
-            response (dict or str): configuration dictionary when result is true, error string when result is false
+            response (dict): configuration dictionary
 
         """
-        config_cmd = self.url + 'clusterConfig/' + self.instance + '?api-tenant=' + self.api_tenant
-        return simple_get(self, config_cmd)
+
+        url = (
+            self.url
+            + "/clusterConfig/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
 
     @_is_configured
-    def load_file(self, file, file_type, gzip=False, append_data=False):
+    def load_file(
+        self,
+        instance_id: str,
+        file: str,
+        file_type: str,
+        gzip: bool = False,
+        append_data: bool = False,
+    ):
         """Load nano data from a file
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             file (str): local path to data file
             file_type (str): file type specifier, must be either 'cvs' or 'raw'
             gzip (boolean): true if file is gzip'd, false if not gzip'd
             append_data (boolean): true if data should be appended to previous data, false if existing
                 data should be truncated
 
-        Returns:
-            result (boolean): true if successful (file was successful loaded into nano pod instance)
-            response (str): None when result is true, error string when result=false
-
         """
 
         # load the data file
         try:
-            with open(file, 'rb') as fp:
+            with open(file, "rb") as fp:
                 file_data = fp.read()
         except FileNotFoundError as e:
-            return False, e.strerror
+            raise BoonException(message=e.strerror)
         except Exception as e:
-            return False, e
+            raise BoonException(message=str(e))
 
         # verify file_type is set correctly
-        if file_type not in ['csv', 'csv-c', 'raw', 'raw-n']:
-            return False, 'file_type must be "csv", "csv-c", "raw" or "raw-n"'
+        if file_type not in ["csv", "csv-c", "raw", "raw-n"]:
+            raise BoonException(
+                message='file_type must be "csv", "csv-c", "raw" or "raw-n"'
+            )
 
         file_name = os.path.basename(file)
 
-        fields = {'data': (file_name, file_data)}
-
-        # build command
-        dataset_cmd = self.url + 'data/' + self.instance + '?api-tenant=' + self.api_tenant
-        dataset_cmd += '&fileType=' + file_type
-        dataset_cmd += '&gzip=' + str(gzip).lower()
-        dataset_cmd += '&appendData=' + str(append_data).lower()
+        fields = {"data": (file_name, file_data)}
 
-        return multipart_post(self, dataset_cmd, fields=fields)
+        url = (
+            self.url
+            + "/data/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&fileType="
+            + file_type
+            + "&appendData="
+            + str(append_data).lower()
+            + "&gzip="
+            + str(gzip).lower()
+        )
+        headers = {}
+        self._api_call("POST", url, headers, fields=fields)
 
     @_is_configured
-    def load_data(self, data, append_data=False):
+    def load_data(self, instance_id: str, data: list, append_data: bool = False):
         """Load nano data from an existing numpy array or simple python list
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             data (np.ndarray or list): numpy array or list of data values
             append_data (boolean): true if data should be appended to previous data, false if existing
                 data should be truncated
 
-        Returns:
-            result (boolean): true if successful (data was successful loaded into nano pod instance)
-            response (str): None when result is true, error string when result=false
-
         """
-        data = normalize_nano_data(data, self.numeric_format)
-        file_name = 'dummy_filename.bin'
-        file_type = 'raw'
 
-        fields = {'data': (file_name, data)}
+        data = normalize_nano_data(data, self.numeric_format)
+        file_name = "dummy_filename.bin"
+        file_type = "raw"
 
-        # build command
-        dataset_cmd = self.url + 'data/' + self.instance + '?api-tenant=' + self.api_tenant
-        dataset_cmd += '&fileType=' + file_type
-        dataset_cmd += '&appendData=' + str(append_data).lower()
+        fields = {"data": (file_name, data)}
 
-        return multipart_post(self, dataset_cmd, fields=fields)
+        url = (
+            self.url
+            + "/data/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&fileType="
+            + file_type
+            + "&appendData="
+            + str(append_data).lower()
+        )
+        headers = {}
+        self._api_call("POST", url, headers, fields=fields)
 
-    def set_learning_status(self, status):
+    def set_learning_enabled(self, instance_id: str, status: bool):
         """returns list of nano instances allocated for a pod
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             status (boolean): true or false of whether to learning is on or off
 
         Returns:
-            result (boolean):  true if successful (list was returned)
-            response (str): json dictionary of pod instances when result=true, error string when result=false
+            response (boolean): status of learning
+
+        """
+        if status not in [True, False]:
+            raise BoonException(400, "status must be a boolean")
+
+        url = (
+            self.url
+            + "/learning/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&enable="
+            + str(status).lower()
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
+
+    @_is_configured
+    def is_learning_enabled(self, instance_id: str):
+        """Results in relation to each cluster/overall stats
+
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
+        Returns:
+            response (boolean): learning on/off status
+
+        """
+
+        url = self.url + "/learning/" + instance_id + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
+
+    def set_root_cause_enabled(self, instance_id: str, status: bool):
+        """configures whether or not to save new clusters coming in for root cause analysis
+
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+            status (boolean): true or false of whether root cause is on or off
+
+        Returns:
+            response (boolean): status of root cause
 
         """
         if status not in [True, False]:
-            return False, 'status must be a boolean'
-        # build command
-        learning_cmd = self.url + 'learning/' + self.instance + '?enable=' + str(
-            status).lower() + '&api-tenant=' + self.api_tenant
+            raise BoonException(400, "status must be a boolean")
+
+        url = (
+            self.url
+            + "/rootCause/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&enable="
+            + str(status).lower()
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
+
+    @_is_configured
+    def is_root_cause_enabled(self, instance_id: str):
+        """Results in relation to each cluster/overall stats
 
-        return simple_post(self, learning_cmd)
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
 
-    def set_root_cause_status(self, status):
+        Returns:
+            response (boolean): root cause on/off status
+
+        """
+
+        url = self.url + "/rootCause/" + instance_id + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
+
+    def set_clipping_detection_enabled(self, instance_id: str, status: bool):
         """configures whether or not to save new clusters coming in for root cause analysis
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             status (boolean): true or false of whether root cause is on or off
 
         Returns:
-            result (boolean):  true if successful (list was returned)
-            response (str): status of root cause
+            response (boolean): status of nano clipping detection
 
         """
         if status not in [True, False]:
-            return False, 'status must be a boolean'
-        # build command
-        learning_cmd = self.url + 'rootCause/' + self.instance + '?enable=' + str(
-            status).lower() + '&api-tenant=' + self.api_tenant
+            raise BoonException(400, "status must be a boolean")
+
+        url = (
+            self.url
+            + "/clippingDetection/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&enable="
+            + str(status).lower()
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
+
+    @_is_configured
+    def is_clipping_detection_enabled(self, instance_id: str):
+        """Results in relation to each cluster/overall stats
+
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
+        Returns:
+            response (boolean): nano clipping detection on/off status
 
-        return simple_post(self, learning_cmd)
+        """
+
+        url = (
+            self.url
+            + "/clippingDetection/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-    def run_nano(self, results=None):
-        """Clusters the data in the nano pod buffer and returns the specified results
+        return response.json()
+
+    def run_nano(self, instance_id: str, results: str = None):
+        f"""Clusters the data in the nano pod buffer and returns the specified results
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             results (str): comma separated list of result specifiers
 
                 ID = cluster ID
 
                 SI = smoothed anomaly index
 
                 RI = raw anomaly index
 
                 FI = frequency index
 
                 DI = distance index
 
-                All = ID,SI,RI,FI,DI
+                AD = anomaly detection
+
+                AH = anomaly history
+
+                AM = anomaly metric
+
+                AW = anomaly warning level
+
+                NI = novelty index
+
+                NS = smoothed novelty index
+
+                NW = novelty warning level
+
+                PI = probability index
+
+                OM = operational mode
+
+                All = {",".join(self.results)}
+
+        Returns:
+            response (dict): dictionary of results
+
+        """
+
+        results_str = self._format_results(results)
+
+        url = self.url + "/nanoRun/" + instance_id + "?api-tenant=" + self.api_tenant
+        if results is not None:
+            url += "&results=" + results_str
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
+
+    @_is_configured
+    def prune_ids(self, instance_id: str, id_list: list = []):
+        """Get root cause
+
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+            id_list (list): list of IDs to remove from the model
 
         Returns:
-            result (boolean): true if successful (nano was successfully run)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): metadata about the updated model
 
         """
 
-        results_str = ''
-        if str(results) == 'All':
-            results_str = 'ID,SI,RI,FI,DI'
-        elif results:
-            for result in results.split(','):
-                if result not in ['ID', 'SI', 'RI', 'FI', 'DI']:
-                    return False, 'unknown result "{}" found in results parameter'.format(result)
-            results_str = results
+        url = (
+            self.url + "/pruneCluster/" + instance_id + "?api-tenant=" + self.api_tenant
+        )
 
-        # build command
-        nano_cmd = self.url + 'nanoRun/' + self.instance + '?api-tenant=' + self.api_tenant
-        if results:
-            nano_cmd += '&results=' + results_str
+        if isinstance(id_list, int):
+            id_list = [id_list]
 
-        return simple_post(self, nano_cmd)
+        if len(id_list) != 0:
+            # IDs
+            id_list = [str(element) for element in id_list]
+            url += "&clusterID=[" + ",".join(id_list) + "]"
+        else:
+            raise BoonException(message="Must specify cluster IDs to analyze")
+
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("POST", url, headers)
+
+        return response.json()
 
     @_is_configured
-    def run_streaming_nano(self, data, results=None):
-        """Load streaming data into self-autotuning nano pod instance, run the nano and return results
+    def run_streaming_nano(self, instance_id: str, data: list, results: str = None):
+        f"""Load streaming data into self-autotuning nano pod instance, run the nano and return results
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             data (np.ndarray or list): numpy array or list of data values
             results (str): comma separated list of result specifiers
 
                 ID = cluster ID
 
                 SI = smoothed anomaly index
 
                 RI = raw anomaly index
 
                 FI = frequency index
 
                 DI = distance index
 
-                All = ID,SI,RI,FI,DI
+                AD = anomaly detection
+
+                AH = anomaly history
+
+                AM = anomaly metric
+
+                AW = anomaly warning level
+
+                NI = novelty index
+
+                NS = smoothed novelty index
+
+                NW = novelty warning level
+
+                PI = probability index
+
+                OM = operational mode
+
+                All = {",".join(self.results)}
 
         Returns:
-            result (boolean): true if successful (data was successful streamed to nano pod instance)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): dictionary of results
 
         """
+
         data = normalize_nano_data(data, self.numeric_format)
-        file_name = 'dummy_filename.bin'
-        file_type = 'raw'
+        file_name = "dummy_filename.bin"
+        file_type = "raw"
 
-        fields = {'data': (file_name, data)}
+        fields = {"data": (file_name, data)}
 
-        results_str = ''
-        if str(results) == 'All':
-            results_str = 'ID,SI,RI,FI,DI'
-        elif results:
-            for result in results.split(','):
-                if result not in ['ID', 'SI', 'RI', 'FI', 'DI']:
-                    return False, 'unknown result "{}" found in results parameter'.format(result)
-            results_str = results
-
-        # build command
-        streaming_cmd = self.url + 'nanoRunStreaming/' + self.instance + '?api-tenant=' + self.api_tenant
-        streaming_cmd += '&fileType=' + file_type
-        if results:
-            streaming_cmd += '&results=' + results_str
+        results_str = self._format_results(results)
 
-        return multipart_post(self, streaming_cmd, fields=fields)
+        url = (
+            self.url
+            + "/nanoRunStreaming/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&fileType="
+            + file_type
+        )
+        if results is not None:
+            url += "&results=" + results_str
+        headers = {}
+        response = self._api_call("POST", url, headers, fields=fields)
+
+        return response.json()
 
     def get_version(self):
         """Version information for this nano pod
 
         Returns:
-            result (boolean): true if successful (version information was retrieved)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): dictionary of version information
 
         """
 
-        # build command (minus the v3 portion)
-        version_cmd = self.url[:-3] + 'version' + '?api-tenant=' + self.api_tenant
-        return simple_get(self, version_cmd)
+        url = self.url[:-3] + "/version" + "?api-tenant=" + self.api_tenant
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
 
     @_is_configured
-    def get_buffer_status(self):
+    def get_buffer_status(self, instance_id: str):
         """Results related to the bytes processed/in the buffer
 
+        Args:
+            instance_id (str): instance identifier to assign to new pod instance
+
         Returns:
-            result (boolean): true if successful (nano was successfully run)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): dictionary of buffer statistics
 
         """
-        status_cmd = self.url + 'bufferStatus/' + self.instance + '?api-tenant=' + self.api_tenant
-        return simple_get(self, status_cmd)
+
+        url = (
+            self.url + "/bufferStatus/" + instance_id + "?api-tenant=" + self.api_tenant
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
 
     @_is_configured
-    def get_nano_results(self, results='All'):
-        """Results per pattern
+    def get_nano_results(self, instance_id: str, results: str = "All"):
+        f"""Results per pattern
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             results (str): comma separated list of results
 
                 ID = cluster ID
 
                 SI = smoothed anomaly index
 
                 RI = raw anomaly index
 
                 FI = frequency index
 
                 DI = distance index
 
-                All = ID,SI,RI,FI,DI
+                AD = anomaly detection
+
+                AH = anomaly history
+
+                AM = anomaly metric
+
+                AW = anomaly warning level
+
+                NI = novelty index
+
+                NS = smoothed novelty index
+
+                NW = novelty warning level
+
+                PI = probability index
+
+                OM = operational mode
+
+                All = {",".join(self.results)}
 
         Returns:
-            result (boolean): true if successful (nano was successfully run)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): dictionary of results
 
         """
-        # build results command
-        if str(results) == 'All':
-            results_str = 'ID,SI,RI,FI,DI'
-        else:
-            for result in results.split(','):
-                if result not in ['ID', 'SI', 'RI', 'FI', 'DI']:
-                    return False, 'unknown result "{}" found in results parameter'.format(result)
-            results_str = results
+        results_str = self._format_results(results)
 
-        # build command
-        results_cmd = self.url + 'nanoResults/' + self.instance + '?api-tenant=' + self.api_tenant
-        results_cmd += '&results=' + results_str
+        url = (
+            self.url
+            + "/nanoResults/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&results="
+            + results_str
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-        return simple_get(self, results_cmd)
+        return response.json()
 
     @_is_configured
-    def get_nano_status(self, results='All'):
+    def get_nano_status(self, instance_id: str, results: str = "All"):
         """Results in relation to each cluster/overall stats
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             results (str): comma separated list of results
 
                 PCA = principal components (includes 0 cluster)
 
                 clusterGrowth = indexes of each increase in cluster (includes 0 cluster)
 
                 clusterSizes = number of patterns in each cluster (includes 0 cluster)
 
                 anomalyIndexes = anomaly index (includes 0 cluster)
 
                 frequencyIndexes = frequency index (includes 0 cluster)
 
+                anomalyThreshold = RI threshold
+
                 distanceIndexes = distance index (includes 0 cluster)
 
                 totalInferences = total number of patterns clustered (overall)
 
                 averageInferenceTime = time in milliseconds to cluster per
                     pattern (not available if uploading from serialized nano) (overall)
 
                 numClusters = total number of clusters (includes 0 cluster) (overall)
 
-                All = PCA,clusterGrowth,clusterSizes,anomalyIndexes,frequencyIndexes,distanceIndexes,totalInferences,numClusters
+                All = PCA,clusterGrowth,clusterSizes,anomalyIndexes,frequencyIndexes,distanceIndexes,totalInferences,numClusters,clusterDistances
 
         Returns:
-            result (boolean): true if successful (nano was successfully run)
-            response (dict or str): dictionary of results when result is true, error message when result = false
+            response (dict): dictionary of results
 
         """
 
         # build results command
-        if str(results) == 'All':
-            results_str = 'PCA,clusterGrowth,clusterSizes,anomalyIndexes,frequencyIndexes,' \
-                          'distanceIndexes,totalInferences,numClusters'
+        if str(results) == "All":
+            results_str = (
+                "PCA,clusterGrowth,clusterSizes,anomalyIndexes,frequencyIndexes,"
+                "distanceIndexes,totalInferences,numClusters,clusterDistances,anomalyThreshold"
+            )
         else:
-            for result in results.split(','):
-                if result not in ['PCA', 'clusterGrowth', 'clusterSizes', 'anomalyIndexes', 'frequencyIndexes',
-                                  'distanceIndexes', 'totalInferences', 'numClusters', 'averageInferenceTime']:
-                    return False, 'unknown result "{}" found in results parameter'.format(result)
-            results_str = results
-
-        # build command
-        results_cmd = self.url + 'nanoStatus/' + self.instance + '?api-tenant=' + self.api_tenant
-        results_cmd = results_cmd + '&results=' + results_str
+            results_str = results if isinstance(results, str) else ",".join(results)
 
-        return simple_get(self, results_cmd)
-
-    def get_root_cause(self, id_list=[], pattern_list=[]):
+        url = (
+            self.url
+            + "/nanoStatus/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+            + "&results="
+            + results_str
+        )
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
+
+        return response.json()
+
+    def get_root_cause(
+        self, instance_id: str, id_list: list = [], pattern_list: list = []
+    ):
         """Get root cause
 
         Args:
+            instance_id (str): instance identifier to assign to new pod instance
             id_list (list): list of IDs to return the root cause for
             pattern_list (list): list of pattern vectors to calculate the root cause against the model
 
         Returns:
-            A list containing the root cause for each pattern/id provided for a sensor:
-
-                [float]
-
-        Raises:
-            BoonException: if Amber cloud gives non-200 response
+            response (list): list containing the root cause for each pattern/id provided for a sensor
         """
 
-        if len(id_list) != 0 and len(pattern_list) != 0:
-            raise BoonException('Cannot specify both list of ID(s) and list of pattern(s).')
-        rc_cmd = self.url + 'rootCauseAnalysis/' + self.instance + '?api-tenant=' + self.api_tenant
+        url = (
+            self.url
+            + "/rootCauseAnalysis/"
+            + instance_id
+            + "?api-tenant="
+            + self.api_tenant
+        )
+
         if len(id_list) != 0:
             # IDs
             id_list = [str(element) for element in id_list]
-            rc_cmd = rc_cmd + '&clusterID=[' + ",".join(id_list) + ']'
+            url += "&clusterID=[" + ",".join(id_list) + "]"
         elif len(pattern_list) != 0:
             # patterns
             if len(np.array(pattern_list).shape) == 1:  # only 1 pattern provided
                 pattern_list = [pattern_list]
-            else:
-                for i, pattern in enumerate(pattern_list):
-                    pattern_list[i] = ','.join([str(element) for element in pattern])
-            rc_cmd = rc_cmd + '&pattern=[[' + "],[".join(pattern_list) + ']]'
-        else:
-            raise BoonException('Must specify either cluster IDs or patterns to analyze')
+            for i, pattern in enumerate(pattern_list):
+                pattern_list[i] = ",".join([str(element) for element in pattern])
+            url += "&pattern=[[" + "],[".join(pattern_list) + "]]"
+
+        headers = {"Content-Type": "application/json"}
+        response = self._api_call("GET", url, headers)
 
-        return simple_get(self, rc_cmd)
+        return response.json()
 
 
 def normalize_nano_data(data, numeric_format):
     # Whatever type data comes in as, cast it to numpy array
     data = np.asarray(data)
 
     # Cast numpy array to correct numeric type for serialization
-    if numeric_format == 'int16':
+    if numeric_format == "int16":
         data = data.astype(np.int16)
-    elif numeric_format == 'float32':
+    elif numeric_format == "float32":
         data = data.astype(np.float32)
-    elif numeric_format == 'uint16':
+    elif numeric_format == "uint16":
         data = data.astype(np.uint16)
 
     # Serialize to binary blob
-    data = data.tostring()
+    data = data.tobytes()
 
     return data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `boonnano-3.1.6/setup.py` & `boonnano-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='boonnano',
-    version='3.1.6',
+    version='3.2.0',
     author="BoonLogic",
     author_email="elise@boonlogic.com",
     packages=['boonnano'],
     install_requires=['urllib3','numpy'],
     description="A SDK package for utilizing the BoonLogic nano API",
     long_description=long_description,
     license='MIT',
```

