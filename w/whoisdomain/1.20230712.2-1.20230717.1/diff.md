# Comparing `tmp/whoisdomain-1.20230712.2.tar.gz` & `tmp/whoisdomain-1.20230717.1.tar.gz`

## Comparing `whoisdomain-1.20230712.2.tar` & `whoisdomain-1.20230717.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/main.py
--rw-r--r--   0        0        0   132217 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/.gitignore
--rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/pyproject.toml
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 whoisdomain-1.20230712.2/PKG-INFO
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    13509 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/main.py
+-rw-r--r--   0        0        0   132495 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/.gitignore
+-rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/pyproject.toml
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 whoisdomain-1.20230717.1/PKG-INFO
```

### Comparing `whoisdomain-1.20230712.2/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230717.1/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/_1_query.py` & `whoisdomain-1.20230717.1/whoisdomain/_1_query.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/_2_parse.py` & `whoisdomain-1.20230717.1/whoisdomain/_2_parse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230717.1/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/__init__.py` & `whoisdomain-1.20230717.1/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/exceptions.py` & `whoisdomain-1.20230717.1/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/main.py` & `whoisdomain-1.20230717.1/whoisdomain/main.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230717.1/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -889,20 +889,29 @@
 
 ZZ["red"] = {
     "extend": "com",
 }
 
 ZZ["ru"] = {
     "extend": "com",
-    "domain_name": r"\ndomain:\s*(.+)",
-    "creation_date": r"\ncreated:\s*(.+)",
-    "expiration_date": r"\npaid-till:\s*(.+)",
-    "name_servers": r"\nnserver:\s*(.+)",
-    "status": r"\nstate:\s*(.+)",
+    "domain_name": r"domain:\s*(.+)",
+    "creation_date": r"created:\s*(.+)",
+    "expiration_date": r"paid-till:\s*(.+)",
+    "name_servers": r"nserver:\s*(.+)",
+    "status": r"state:\s*(.+)",
 }
+ZZ["com.ru"] = {
+    "extend": "ru",
+    # "domain_name": r"^domain:\s*(.+)",
+    "_server": "whois.nic.ru",
+    # test: mining.com.ru
+}
+# Russian city sub-domains
+ZZ["msk.ru"] = {"extend": "com.ru"}  # test with: mining.msk.ru
+ZZ["spb.ru"] = {"extend": "com.ru"}  # test with iac.spb.ru
 
 # Rossíyskaya Federátsiya) is the Cyrillic country code top-level domain for the Russian Federation,
 # In the Domain Name System it has the ASCII DNS name xn--p1ai.
 
 ZZ["ru.rf"] = {
     "extend": "ru",
     "_server": "whois.tcinet.ru",
```

### Comparing `whoisdomain-1.20230712.2/.gitignore` & `whoisdomain-1.20230717.1/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/README.md` & `whoisdomain-1.20230717.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -204,8 +204,9 @@
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
-  * 1.20230712.1 tld .edu now can have up to 10 nameservers; remove action on pull request
+  * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
+  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test dockumented), also update the tld: ru, the newlines are note needed.
```

### Comparing `whoisdomain-1.20230712.2/pyproject.toml` & `whoisdomain-1.20230717.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230712.2/PKG-INFO` & `whoisdomain-1.20230717.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230712.2
+Version: 1.20230717.1
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -225,8 +225,9 @@
   * aside from the original authors, many others already contributed to these repositories
   * if authors/contributors prefer to be named explicitly, they can add a line in Historical.txt
 
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
-  * 1.20230712.1 tld .edu now can have up to 10 nameservers; remove action on pull request
+  * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
+  * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test dockumented), also update the tld: ru, the newlines are note needed.
```

