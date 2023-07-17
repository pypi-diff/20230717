# Comparing `tmp/mwdb-iocextract-1.1.3.tar.gz` & `tmp/mwdb-iocextract-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwdb-iocextract-1.1.3.tar", last modified: Fri Jun 30 12:55:49 2023, max compression
+gzip compressed data, was "mwdb-iocextract-1.1.4.tar", last modified: Mon Jul 17 12:04:06 2023, max compression
```

## Comparing `mwdb-iocextract-1.1.3.tar` & `mwdb-iocextract-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxr-x   0 psrok1    (1000) psrok1    (1000)        0 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)     7100 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/PKG-INFO
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)     6737 2022-02-08 14:51:44.000000 mwdb-iocextract-1.1.3/README.md
-drwxrwxr-x   0 psrok1    (1000) psrok1    (1000)        0 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)     7100 2023-06-30 12:55:49.000000 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/PKG-INFO
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      365 2023-06-30 12:55:49.000000 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/SOURCES.txt
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)        1 2023-06-30 12:55:49.000000 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/dependency_links.txt
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)       44 2023-06-30 12:55:49.000000 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/requires.txt
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)       16 2023-06-30 12:55:49.000000 mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/top_level.txt
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)       74 2022-02-08 14:51:44.000000 mwdb-iocextract-1.1.3/pyproject.toml
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      101 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/setup.cfg
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      695 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/setup.py
-drwxrwxr-x   0 psrok1    (1000) psrok1    (1000)        0 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/src/
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      364 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/__init__.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      310 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/api.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      342 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/errors.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)    11043 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/model.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)    10778 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/modules.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)      936 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/run.py
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)     1145 2023-06-30 12:53:49.000000 mwdb-iocextract-1.1.3/src/test_misp.py
-drwxrwxr-x   0 psrok1    (1000) psrok1    (1000)        0 2023-06-30 12:55:49.313042 mwdb-iocextract-1.1.3/tests/
--rw-rw-r--   0 psrok1    (1000) psrok1    (1000)     1133 2022-02-08 14:51:44.000000 mwdb-iocextract-1.1.3/tests/test_parse_regression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      334 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/src/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/api.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12444 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/src/model.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/src/modules.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/run.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/test_misp.py
```

### Comparing `mwdb-iocextract-1.1.3/PKG-INFO` & `mwdb-iocextract-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.1.3
+Version: 1.1.4
 Summary: Mwdb config parser
 Home-page: UNKNOWN
 Author: msm
 Author-email: msm@cert.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `mwdb-iocextract-1.1.3/README.md` & `mwdb-iocextract-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.3/mwdb_iocextract.egg-info/PKG-INFO` & `mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.1.3
+Version: 1.1.4
 Summary: Mwdb config parser
 Home-page: UNKNOWN
 Author: msm
 Author-email: msm@cert.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `mwdb-iocextract-1.1.3/setup.py` & `mwdb-iocextract-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().split('\n')
 
 setuptools.setup(
     name="mwdb-iocextract",
-    version="1.1.3",
+    version="1.1.4",
     author="msm",
     author_email="msm@cert.pl",
     package_dir={"mwdb_iocextract": "src"},
     packages=["mwdb_iocextract"],
     description="Mwdb config parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mwdb-iocextract-1.1.3/src/model.py` & `mwdb-iocextract-1.1.4/src/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,57 +110,83 @@
         self.url = urlparse(url)
         if self.url.hostname is None:
             self.url = urlparse("unknown://" + url)
 
         self.location_type = location_type
 
     @property
-    def ip(self):
+    def ip(self) -> Optional[str]:
         if self.url.hostname and is_ipv4(self.url.hostname):
             return self.url.hostname
         return None
 
     @property
-    def domain(self):
+    def domain(self) -> Optional[str]:
         if self.url.hostname and not is_ipv4(self.url.hostname):
             return self.url.hostname
         return None
 
     @property
-    def port(self):
+    def port(self) -> Optional[int]:
         return self.url.port
 
     @property
-    def path(self):
+    def path(self) -> str:
         return self.url.path
 
     @property
-    def pretty_url(self):
+    def query(self) -> str:
+        return self.url.query
+
+    @property
+    def scheme(self) -> Optional[str]:
+        scheme = self.url.scheme
+        # `unknown://` scheme is a placeholder used for URLs with a missing scheme
+        # that we unfortunately have to support.
+        if scheme == "unknown":
+            return None
+        return scheme
+
+    @property
+    def pretty_url(self) -> str:
         url = self.url.geturl()
         if url.startswith("unknown://"):
             return url[len("unknown://") :]
         return url
 
     def to_misp(self) -> MISPObject:
-        obj = MISPObject("url", standalone=False)
-        obj.add_attribute("url", self.pretty_url)
+        if any((self.scheme, self.path, self.query, self.url.fragment)):
+            misp_object_type = "url"
+        else:
+            misp_object_type = "domain-ip"
+
+        obj = MISPObject(misp_object_type, standalone=False)
+
+        # url-specific attributes
+        if self.scheme:
+            obj.add_attribute("url", self.pretty_url)
+        if self.path:
+            obj.add_attribute("resource_path", self.path)
+        if self.url.fragment:
+            obj.add_attribute("fragment", self.url.fragment)
+        if self.query:
+            obj.add_attribute("query_string", self.query)
+
+        # generic attributes that apply to both url and domain-ip
         if self.ip:
             a = obj.add_attribute("ip", self.ip)
             if a is not None:
                 a.add_tag(f"mwdb:location_type:{self.location_type.value}")
         if self.domain:
             a = obj.add_attribute("domain", self.domain)
             if a is not None:
                 a.add_tag(f"mwdb:location_type:{self.location_type.value}")
         if self.port:
             obj.add_attribute("port", self.port)
-        if self.path:
-            obj.add_attribute("resource_path", self.path)
-        if self.url.query:
-            obj.add_attribute("query_string", self.url.query)
+
         return obj
 
     def prettyprint(self) -> str:
         """Pretty print for debugging"""
         return "NetLoc " + self.pretty_url
 
 
@@ -172,15 +198,16 @@
         self.rsa_keys: List[RsaKey] = []
         self.ecdsa_curves: List[EcdsaCurve] = []
         self.keys: List[Tuple[str, str]] = []  # (keytype, hexencoded key)
         self.passwords: List[str] = []
         self.network_locations: List[NetworkLocation] = []
         self.mutexes: List[str] = []
         self.dropped_filenames: List[str] = []
-        self.emails: List[str] = []
+        self.emails_to: List[str] = []
+        self.emails_from: List[str] = []
         self.ransom_messages: List[str] = []
         self.campaign_ids: List[str] = []
 
     def add_rsa_key(self, rsakey: RsaKey) -> None:
         self.rsa_keys.append(rsakey)
 
     def add_ecdsa_curve(self, ecdsa_curve: EcdsaCurve) -> None:
@@ -243,16 +270,19 @@
 
     def add_drop_filename(self, filename: str) -> None:
         self.dropped_filenames.append(filename)
 
     def add_mutex(self, mutex: str) -> None:
         self.mutexes.append(mutex)
 
-    def add_email(self, email: str) -> None:
-        self.emails.append(email)
+    def add_email_to(self, email: str) -> None:
+        self.emails_to.append(email)
+
+    def add_email_from(self, email: str) -> None:
+        self.emails_from.append(email)
 
     def add_ransom_message(self, ransom_message: str) -> None:
         self.ransom_messages.append(ransom_message)
 
     def add_campaign_id(self, campaign_id: str) -> None:
         self.campaign_ids.append(campaign_id)
 
@@ -278,18 +308,25 @@
             mutex_obj = MISPObject("mutex", standalone=False)
             for mutex in self.mutexes:
                 mutex_obj.add_attribute("name", mutex)
                 to_return.append(mutex_obj)
         for netloc in self.network_locations:
             to_return.append(netloc.to_misp())
         # TODO self.dropped_filenames
-        for email in self.emails:
+        for email in self.emails_to:
             obj = MISPObject("email", standalone=False)
             obj.add_attribute("to", email)
             to_return.append(obj)
+        for email in self.emails_from:
+            obj = MISPObject("email", standalone=False)
+            obj.add_attribute("from", email)
+            to_return.append(obj)
+
+        # filter out objects without any attributes
+        to_return = list(filter(lambda x: bool(x.attributes), to_return))
 
         return to_return
 
     def prettyprint(self) -> str:
         """Pretty print for debugging"""
         result = []
         for rsa_key in self.rsa_keys:
@@ -302,16 +339,18 @@
             result.append("Password " + password)
         for netloc in self.network_locations:
             result.append(netloc.prettyprint())
         for mutex in self.mutexes:
             result.append("Mutex " + mutex)
         for drop_filename in self.dropped_filenames:
             result.append("Drop " + drop_filename)
-        for email in self.emails:
-            result.append("Email " + email)
+        for email in self.emails_to:
+            result.append("EmailTo " + email)
+        for email in self.emails_from:
+            result.append("EmailFrom " + email)
         for ransom_message in self.ransom_messages:
             result.append("RansomMessage: " + ransom_message)
         for campaign_id in self.campaign_ids:
             result.append("CampaignId: " + campaign_id)
         return "\n".join(result)
 
     def __bool__(self) -> bool:
@@ -319,12 +358,13 @@
             [
                 self.rsa_keys,
                 self.keys,
                 self.passwords,
                 self.network_locations,
                 self.mutexes,
                 self.dropped_filenames,
-                self.emails,
+                self.emails_to,
+                self.emails_from,
                 self.ransom_messages,
                 self.campaign_ids,
             ]
         )
```

### Comparing `mwdb-iocextract-1.1.3/src/modules.py` & `mwdb-iocextract-1.1.4/src/modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     for name in ["mutex", "mtx"]:
         for mutex in safe_get_list(config, name):
             iocs.add_mutex(mutex)
 
     for name in ["email", "emails"]:
         for email in safe_get_list(config, name):
-            iocs.add_email(email)
+            iocs.add_email_to(email)
 
     for ransom_message in safe_get_list(config, "ransommessage"):
         iocs.add_ransom_message(ransom_message)
 
     for name in ["encryptionkey", "key", "keys"]:
         for key in safe_get_list(config, name):
             iocs.add_key("unknown", key)
@@ -182,15 +182,15 @@
 
 
 @module("hawkeye")
 def parse_hawkeye(config: Dict[str, Any]) -> IocCollection:
     iocs = IocCollection()
 
     if config.get("EmailUsername"):
-        iocs.add_email(config["EmailUsername"])
+        iocs.add_email_to(config["EmailUsername"])
 
     return iocs
 
 
 @module("trickbot")
 def parse_trickbot(config: Dict[str, Any]) -> IocCollection:
     iocs = IocCollection()
@@ -371,7 +371,60 @@
             if e == 0x10001:
                 iocs.add_rsa_key(RsaKey(n=n, e=e))
                 del config["rsa_pub"]
         except Exception:
             pass
 
     return iocs
+
+
+@module("agenttesla")
+def parse_agenttesla(config: Dict[str, Any]) -> IocCollection:
+    iocs = IocCollection()
+
+    if config.get("email"):
+        iocs.add_email_from(config["email"])
+        del config["email"]
+
+    if config.get("email_to"):
+        iocs.add_email_to(config["email_to"])
+        del config["email_to"]
+
+    return iocs
+
+
+@module("formbook")
+def parse_formbook(config: Dict[str, Any]) -> IocCollection:
+    iocs = IocCollection()
+
+    if "urls" in config:
+        del config["urls"]
+
+    if "c2_url" in config:
+        iocs.try_add_url(config["c2_url"])
+        del config["c2_url"]
+
+    return iocs
+
+
+@module("cobaltstrike")
+def parse_cobaltstrike(config: Dict[str, Any]) -> IocCollection:
+    iocs = IocCollection()
+
+    if config.get("payload_type", "").endswith("stager"):
+        for url_row in config.get("stager_url", []):
+            url = url_row["url"]
+            iocs.try_add_url(url)
+    else:
+        beacon_type = config.get("beacon_type", [None])[0]
+        if beacon_type in ("HTTP", "HTTPS"):
+            scheme = beacon_type.lower()
+            port = config["port"]
+            c2 = config["server,get-uri"].split(",")
+
+            for i in range(0, len(c2), 2):
+                hostname, path = c2[i], c2[i + 1]
+                iocs.try_add_url(f"{scheme}://{hostname}:{port}{path}")
+
+            del config["urls"]
+
+    return iocs
```

### Comparing `mwdb-iocextract-1.1.3/src/run.py` & `mwdb-iocextract-1.1.4/src/run.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.3/src/test_misp.py` & `mwdb-iocextract-1.1.4/src/test_misp.py`

 * *Files identical despite different names*

