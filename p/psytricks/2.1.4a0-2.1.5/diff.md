# Comparing `tmp/psytricks-2.1.4a0.tar.gz` & `tmp/psytricks-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.4a0.tar", max compression
+gzip compressed data, was "psytricks-2.1.5.tar", max compression
```

## Comparing `psytricks-2.1.4a0.tar` & `psytricks-2.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.4a0/LICENSE
--rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.4a0/README.md
--rw-r--r--   0        0        0     1116 2023-06-14 14:00:52.880002 psytricks-2.1.4a0/pyproject.toml
--rw-r--r--   0        0        0       97 2023-06-14 14:00:52.880002 psytricks-2.1.4a0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6150 2023-06-14 14:00:52.884002 psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.4a0/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.4a0/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.4a0/src/psytricks/mappings.py
--rw-r--r--   0        0        0    24280 2023-06-14 13:59:13.038825 psytricks-2.1.4a0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 psytricks-2.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.5/LICENSE
+-rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.5/README.md
+-rw-r--r--   0        0        0     1112 2023-07-17 20:45:24.275203 psytricks-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-07-17 20:45:24.279203 psytricks-2.1.5/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6146 2023-07-17 20:45:24.279203 psytricks-2.1.5/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.5/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.5/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.5/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.5/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    24643 2023-07-17 20:43:21.773770 psytricks-2.1.5/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 psytricks-2.1.5/PKG-INFO
```

### Comparing `psytricks-2.1.4a0/LICENSE` & `psytricks-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/README.md` & `psytricks-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/pyproject.toml` & `psytricks-2.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.4-a.0"
+version = "2.1.5"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.5/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.4-a.0"
+$Version = "2.1.5"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.5/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.5/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.5/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/cli.py` & `psytricks-2.1.5/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/decoder.py` & `psytricks-2.1.5/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/literals.py` & `psytricks-2.1.5/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/mappings.py` & `psytricks-2.1.5/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4a0/src/psytricks/wrapper.py` & `psytricks-2.1.5/src/psytricks/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,16 +373,16 @@
     def validate_version(self, server_ver):
         """Validate the server version against the local module.
 
         Parse the version strings of the local module and the server response
         and compare them for equality (ignoring the 4th component, which may
         denote a pre- or development-release).
 
-        If the 3rd component (PATCH level) is differing a warning message will
-        be issued to the log but the method will still return True.
+        If the 3rd component (PATCH level) is differing a message will be issued
+        to the debug log but the method will still return True.
 
         Parameters
         ----------
         server_ver : dict
             The dict parsed from the JSON response when sending a `version` GET
             request to the server.
 
@@ -448,28 +448,28 @@
                 f"['ErrorMessage']: {status['ErrorMessage']}\n"
             )
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"Error fetching response payload status: {ex}")
             log.warning(response.text)
             raise ValueError(f"Malformed response: {response.text}") from ex
 
-    def send_get_request(self, raw_url: str) -> list:
+    def send_get_request(self, raw_url: str):
         """Common method to perform a `GET` request and process the response.
 
         Parameters
         ----------
         raw_url : str
             The part of the URL that will be appended to `self.base_url`.
 
         Returns
         -------
-        list(str)
-            The parsed `JSON` of the response. Will be an empty list in case
-            something went wrong performing the GET request or processing the
-            response.
+        list or dict or None
+            The parsed `JSON` of the response, often a dict or a list of dict.
+            Will be an empty list in case something went wrong performing the
+            GET request or processing the response.
         """
         try:
             response = requests.get(self.base_url + raw_url, timeout=self.timeout)
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"GET request [{raw_url}] failed: {ex}")
             raise ex
 
@@ -496,18 +496,19 @@
             The parameters to pass as `JSON` payload to the POST request.
         no_json : bool
             If set to `True` the response is expected to contain no `JSON` and
             an empty list will be returned.
 
         Returns
         -------
-        list(str)
-            The parsed `JSON` of the response. Will be an empty list in case
-            something went wrong performing the POST request or processing the
-            response (or in case the `no_json` parameter was set to `True`).
+        list
+            The parsed `JSON` of the response, usually a list of dict. Will be
+            an empty list in case something went wrong performing the POST
+            request or processing the response (or in case the `no_json`
+            parameter was set to `True`).
         """
         try:
             response = requests.post(
                 self.base_url + raw_url, json=payload, timeout=self.timeout
             )
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"POST request [{raw_url}] failed: {ex}")
@@ -522,48 +523,50 @@
         return response.json(object_hook=parse_powershell_json)
 
     def get_machine_status(self) -> list:
         """Send a `GET` request with `GetMachineStatus`.
 
         Returns
         -------
-        dict
-            The `Data` dict parsed from the JSON returned by the REST service.
+        list(dict)
+            The `Data` dicts parsed from the JSON returned by the REST service.
         """
         log.debug("Requesting current status of machines...")
         return self.send_get_request("GetMachineStatus")["Data"]
 
     def get_sessions(self) -> list:
         """Send a `GET` request with `GetSessions`.
 
         Returns
         -------
-        dict
-            The `Data` dict parsed from the JSON returned by the REST service.
+        list(dict)
+            The `Data` dicts parsed from the JSON returned by the REST service,
+            containing details about the currently existing sessions.
         """
         log.debug("Requesting current sessions...")
         return self.send_get_request("GetSessions")["Data"]
 
     def get_access_users(self, group: str) -> list:
         """Send a `GET` request with `GetAccessUsers`.
 
         Parameters
         ----------
         group : str
             The name of the Delivery Group to request users having access.
 
         Returns
         -------
-        dict
-            The `Data` dict parsed from the JSON returned by the REST service.
+        list(dict)
+            The `Data` dicts parsed from the JSON returned by the REST service,
+            containing the user objects having access to the given group.
         """
         log.debug(f"Requesting users having access to group [{group}]...")
         return self.send_get_request(f"GetAccessUsers/{group}")["Data"]
 
-    def disconnect_session(self, machine: str) -> list:
+    def disconnect_session(self, machine: str) -> dict:
         """Send a `POST` request with `DisconnectSession`.
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to disconnect the session on.
 
@@ -598,27 +601,29 @@
             permissions to the given group should be adapted.
         disable : bool
             A flag requesting the permissions for the given username(s) to be
             removed (if True) instead of being added (if False).
 
         Returns
         -------
-        dict
-            The `Data` dict parsed from the JSON returned by the REST service.
+        list(dict)
+            The `Data` dicts parsed from the JSON returned by the REST service,
+            containing the user objects having access to the given group *after*
+            the operation has been performed.
         """
         verb = "Removing" if disable else "Adding"
         log.debug(f"{verb} access to group [{group}] for user(s) [{users}]...")
         payload = {
             "Group": group,
             "UserNames": users,
             "RemoveAccess": disable,
         }
         return self.send_post_request("SetAccessUsers", payload)["Data"]
 
-    def set_maintenance(self, machine: str, disable: bool) -> list:
+    def set_maintenance(self, machine: str, disable: bool) -> dict:
         """Send a `POST` request with `SetMaintenanceMode`.
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to modify maintenance mode on.
         disable : bool
@@ -658,15 +663,15 @@
             "DNSName": machine,
             "Text": message,
             "Title": title,
             "MessageStyle": style,
         }
         self.send_post_request("SendSessionMessage", payload, no_json=True)
 
-    def perform_poweraction(self, machine: str, action: Action) -> None:
+    def perform_poweraction(self, machine: str, action: Action) -> dict:
         """Send a `POST` request with `MachinePowerAction`.
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to disconnect the session on.
         action : str
```

### Comparing `psytricks-2.1.4a0/PKG-INFO` & `psytricks-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.4a0
+Version: 2.1.5
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

