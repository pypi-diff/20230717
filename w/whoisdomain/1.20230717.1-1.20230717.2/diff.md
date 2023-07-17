# Comparing `tmp/whoisdomain-1.20230717.1.tar.gz` & `tmp/whoisdomain-1.20230717.2.tar.gz`

## Comparing `whoisdomain-1.20230717.1.tar` & `whoisdomain-1.20230717.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/main.py
--rw-r--r--   0        0        0   132495 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/.gitignore
--rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/pyproject.toml
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/main.py
+-rw-r--r--   0        0        0   132546 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/.gitignore
+-rw-r--r--   0        0        0     9949 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/pyproject.toml
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.2/PKG-INFO
```

### Comparing `whoisdomain-1.20230717.1/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230717.2/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/whoisdomain/_1_query.py` & `whoisdomain-1.20230717.2/whoisdomain/_1_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import subprocess
 import time
 import sys
 import os
 import platform
 import json
+import shutil
 from .exceptions import WhoisCommandFailed, WhoisCommandTimeout
 
 from typing import Dict, List, Optional, Tuple
 
 
 # PYTHON_VERSION = sys.version_info[0]
 CACHE: Dict[str, Tuple[int, str]] = {}
 CACHE_MAX_AGE = 60 * 60 * 48  # 48h
 
+IS_WINDOWS = platform.system() == "Windows"
+
+if not IS_WINDOWS and shutil.which("stdbuf"):
+    STDBUF_OFF_CMD = ["stdbuf", "-o0"]
+else:
+    STDBUF_OFF_CMD = []
+
 
 def _cache_load(cf: str) -> None:
     if not os.path.isfile(cf):
         return
 
     global CACHE
     f = open(cf, "r")
@@ -84,15 +92,15 @@
     domain = ".".join(dl)
 
     if " " in wh:
         whList = wh.split(" ")
     else:
         whList = [wh]
 
-    if platform.system() == "Windows":
+    if IS_WINDOWS:
         if wh == "whois":  # only if the use did not specify what whois to use
             if os.path.exists("whois.exe"):
                 wh = r".\whois.exe"
             else:
                 find = False
                 paths = os.environ["path"].split(";")
                 for path in paths:
@@ -118,14 +126,15 @@
 
 def _do_whois_query(
     dl: List[str],
     ignore_returncode: bool,
     server: Optional[str] = None,
     verbose: bool = False,
     timeout: Optional[float] = None,
+    parse_partial_response: bool = False,
     wh: str = "whois",
     simplistic: bool = False,
 ) -> str:
     # if getenv[TEST_WHOIS_PYTON] fake whois by reading static data from a file
     # this wasy we can actually implemnt a test run with known data in and expected data out
     if os.getenv("TEST_WHOIS_PYTHON"):
         return _testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
@@ -137,27 +146,32 @@
         wh=wh,
     )
     if verbose:
         print(cmd, wh, file=sys.stderr)
 
     # LANG=en is added to make the ".jp" output consist across all environments
     p = subprocess.Popen(
-        cmd,
+        # STDBUF_OFF_CMD needed to not lose data on kill
+        STDBUF_OFF_CMD + cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         env={"LANG": "en"} if dl[-1] in ".jp" else None,
     )
 
     try:
         r = p.communicate(timeout=timeout)[0].decode(errors="ignore")
     except subprocess.TimeoutExpired:
         # Kill the child process & flush any output buffers
         p.kill()
-        p.communicate()
-        raise WhoisCommandTimeout(f"timeout: query took more then {timeout} seconds")
+        r = p.communicate()[0].decode(errors="ignore")
+        # In most cases whois servers returns partial domain data really fast
+        # after that delay occurs (probably intentional) before returning contact data.
+        # Add this option to cover those cases
+        if not parse_partial_response or not r:
+            raise WhoisCommandTimeout(f"timeout: query took more then {timeout} seconds")
 
     if verbose:
         print(r, file=sys.stderr)
 
     if ignore_returncode is False and p.returncode not in [0, 1]:
         # network error, "fgets: Connection reset by peer" fix, ignore
         if "fgets: Connection reset by peer" in r:
@@ -183,14 +197,15 @@
     cache_file: Optional[str] = None,
     cache_age: int = CACHE_MAX_AGE,
     slow_down: int = 0,
     ignore_returncode: bool = False,
     server: Optional[str] = None,
     verbose: bool = False,
     timeout: Optional[float] = None,
+    parse_partial_response: bool = False,
     wh: str = "whois",
     simplistic: bool = False,
 ) -> str:
     k = ".".join(dl)
 
     if cache_file:
         if verbose:
@@ -212,14 +227,15 @@
             int(time.time()),
             _do_whois_query(
                 dl=dl,
                 ignore_returncode=ignore_returncode,
                 server=server,
                 verbose=verbose,
                 timeout=timeout,
+                parse_partial_response=parse_partial_response,
                 wh=wh,
                 simplistic=simplistic,
             ),
         )
 
         if cache_file:
             _cache_save(cache_file)
```

### Comparing `whoisdomain-1.20230717.1/whoisdomain/_2_parse.py` & `whoisdomain-1.20230717.2/whoisdomain/_2_parse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230717.2/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/whoisdomain/__init__.py` & `whoisdomain-1.20230717.2/whoisdomain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     slow_down: int = 0,
     ignore_returncode: bool = False,
     server: Optional[str] = None,
     verbose: bool = False,
     with_cleanup_results: bool = False,
     include_raw_whois_text: bool = False,
     timeout: Optional[float] = None,
+    parse_partial_response: bool = False,
     wh: str = "whois",
     simplistic: bool = False,
     withRedacted: bool = False,
 ) -> Optional[Domain]:
 
     try:
         whois_str = do_query(
@@ -270,14 +271,15 @@
             cache_file=cache_file,
             cache_age=cache_age,
             slow_down=slow_down,
             ignore_returncode=ignore_returncode,
             server=server,
             verbose=verbose,
             timeout=timeout,
+            parse_partial_response=parse_partial_response,
             wh=wh,
             simplistic=simplistic,
         )
     except Exception as e:
         if simplistic:
             return Domain(
                 data={},
@@ -340,14 +342,15 @@
     server: Optional[str] = None,
     verbose: bool = False,
     with_cleanup_results: bool = False,
     internationalized: bool = False,
     include_raw_whois_text: bool = False,
     return_raw_text_for_unsupported_tld: bool = False,
     timeout: Optional[float] = None,
+    parse_partial_response: bool = False,
     cmd: str = "whois",
     simplistic: bool = False,
     withRedacted: bool = False,
 ) -> Optional[Domain]:
     """
     force=True          Don't use cache.
     cache_file=<path>   Use file to store cache not only memory.
@@ -362,14 +365,16 @@
     ignore_returncode:  if true and the whois command fails with code 1, still process the data returned as normal.
     verbose:            if true, print relevant information on steps taken to standard error
     include_raw_whois_text:
                         if reqested the full response is also returned.
     return_raw_text_for_unsupported_tld:
                         if the tld is unsupported, just try it anyway but return only the raw text.
     timeout:            timeout in seconds for the whois command to return a result.
+    parse_partial_response:
+                        try to parse partial response when cmd timed out (stdbuf should be in PATH for best results)
     cmd:                explicitly specify the path to the whois you want to use.
     simplistic:         when simplistic is True we return None for most exceptions and dont pass info why we have no data.
     withRedacted:       show redacted output , default no redacted data is shown
     """
 
     global LastWhois
     LastWhois["Try"] = []  # init on start of query
@@ -460,14 +465,15 @@
             slow_down=slow_down,
             ignore_returncode=ignore_returncode,
             server=server,
             verbose=verbose,
             with_cleanup_results=with_cleanup_results,
             include_raw_whois_text=include_raw_whois_text,
             timeout=timeout,
+            parse_partial_response=parse_partial_response,
             wh=wh,
             simplistic=simplistic,
             withRedacted=withRedacted,
         )
         if result:
             return result
```

### Comparing `whoisdomain-1.20230717.1/whoisdomain/exceptions.py` & `whoisdomain-1.20230717.2/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/whoisdomain/main.py` & `whoisdomain-1.20230717.2/whoisdomain/main.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230717.2/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,18 +660,22 @@
     "creation_date": r"Registered:\s?(.+)",
     "expiration_date": r"Expires:\s?(.+)",
     "name_servers": r"Nameserver:\s*(.+)\s*",
     "status": r"\nStatus:\s?(.+)",
 }
 
 ZZ["lv"] = {
-    "extend": "ru",
-    "creation_date": r"Registered:\s*(.+)\n",
+    "extend": "com",
+    "domain_name": r"domain:\s*(.+)",
+    "creation_date": r"Registered:\s*(.+)\n",  # actually there seem to be no dates
     "updated_date": r"Changed:\s*(.+)\n",
+    "expiration_date": r"paid-till:\s*(.+)",
+    "name_servers": r"nserver:\s*(.+)",
     "status": r"Status:\s?(.+)",
+    "_server": "whois.nic.lv",
 }
 
 ZZ["me"] = {
     # lines have \r
     "extend": "biz",
     "creation_date": r"Creation Date:\s?(.+)",
     "expiration_date": r"Expiry Date:\s?(.+)",
@@ -894,40 +898,28 @@
 ZZ["ru"] = {
     "extend": "com",
     "domain_name": r"domain:\s*(.+)",
     "creation_date": r"created:\s*(.+)",
     "expiration_date": r"paid-till:\s*(.+)",
     "name_servers": r"nserver:\s*(.+)",
     "status": r"state:\s*(.+)",
+    "_server": " whois.tcinet.ru",
 }
-ZZ["com.ru"] = {
-    "extend": "ru",
-    # "domain_name": r"^domain:\s*(.+)",
-    "_server": "whois.nic.ru",
-    # test: mining.com.ru
-}
+ZZ["com.ru"] = {"extend": "ru", "_server": "whois.nic.ru"}  # test: mining.com.ru
+
 # Russian city sub-domains
 ZZ["msk.ru"] = {"extend": "com.ru"}  # test with: mining.msk.ru
 ZZ["spb.ru"] = {"extend": "com.ru"}  # test with iac.spb.ru
 
 # Rossíyskaya Federátsiya) is the Cyrillic country code top-level domain for the Russian Federation,
 # In the Domain Name System it has the ASCII DNS name xn--p1ai.
 
-ZZ["ru.rf"] = {
-    "extend": "ru",
-    "_server": "whois.tcinet.ru",
-}
-ZZ["рф"] = {
-    "extend": "ru",
-    "_server": "whois.tcinet.ru",
-}
-ZZ["xn--p1ai"] = {
-    "extend": "ru",
-    "_server": "whois.tcinet.ru",
-}
+ZZ["ru.rf"] = {"extend": "ru"}
+ZZ["рф"] = {"extend": "ru"}
+ZZ["xn--p1ai"] = {"extend": "ru"}
 
 ZZ["sa"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s*(.+\.sa)\s",
     "registrant": r"Registrant:\n*(.+)\n",
     "name_servers": r"Name Servers:\s*(.+)\s*(.+)?",
     "registrant_country": None,
```

### Comparing `whoisdomain-1.20230717.1/.gitignore` & `whoisdomain-1.20230717.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/README.md` & `whoisdomain-1.20230717.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -200,13 +200,16 @@
 ## Author's
   * this is a rename copy of original work done in: https://github.com/DannyCork/python-whois
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
+
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
-  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test dockumented), also update the tld: ru, the newlines are note needed.
+  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
+  * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
+
```

### Comparing `whoisdomain-1.20230717.1/pyproject.toml` & `whoisdomain-1.20230717.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230717.1/PKG-INFO` & `whoisdomain-1.20230717.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230717.1
+Version: 1.20230717.2
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -221,13 +221,16 @@
 ## Author's
   * this is a rename copy of original work done in: https://github.com/DannyCork/python-whois
   * the project is also related to the project: https://github.com/gen1us2k/python-whois
   * both seem derived from a older google.code site: https://code.google.com/archive/p/python-whois
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
+
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
-  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test dockumented), also update the tld: ru, the newlines are note needed.
+  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
+  * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
+
```

