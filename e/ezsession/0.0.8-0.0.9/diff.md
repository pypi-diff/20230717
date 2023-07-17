# Comparing `tmp/ezsession-0.0.8.tar.gz` & `tmp/ezsession-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsession-0.0.8.tar", last modified: Sat Jul  8 23:09:23 2023, max compression
+gzip compressed data, was "ezsession-0.0.9.tar", last modified: Mon Jul 17 15:09:05 2023, max compression
```

## Comparing `ezsession-0.0.8.tar` & `ezsession-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:09:23.581614 ezsession-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 23:09:13.000000 ezsession-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-08 23:09:23.581614 ezsession-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-08 23:09:13.000000 ezsession-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 23:09:13.000000 ezsession-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 23:09:13.000000 ezsession-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:09:23.581614 ezsession-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-08 23:09:13.000000 ezsession-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:09:23.577614 ezsession-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:09:23.577614 ezsession-0.0.8/src/ezsession/
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-08 23:09:13.000000 ezsession-0.0.8/src/ezsession/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:09:23.581614 ezsession-0.0.8/src/ezsession.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-08 23:09:23.000000 ezsession-0.0.8/src/ezsession.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 23:09:23.000000 ezsession-0.0.8/src/ezsession.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:09:23.000000 ezsession-0.0.8/src/ezsession.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 23:09:23.000000 ezsession-0.0.8/src/ezsession.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 23:09:23.000000 ezsession-0.0.8/src/ezsession.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:09:05.342071 ezsession-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 15:08:53.000000 ezsession-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-17 15:09:05.342071 ezsession-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-17 15:08:53.000000 ezsession-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 15:08:53.000000 ezsession-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 15:08:53.000000 ezsession-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:09:05.342071 ezsession-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-17 15:08:53.000000 ezsession-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:09:05.342071 ezsession-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:09:05.342071 ezsession-0.0.9/src/ezsession/
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-17 15:08:53.000000 ezsession-0.0.9/src/ezsession/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:09:05.342071 ezsession-0.0.9/src/ezsession.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-17 15:09:05.000000 ezsession-0.0.9/src/ezsession.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-17 15:09:05.000000 ezsession-0.0.9/src/ezsession.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:09:05.000000 ezsession-0.0.9/src/ezsession.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 15:09:05.000000 ezsession-0.0.9/src/ezsession.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 15:09:05.000000 ezsession-0.0.9/src/ezsession.egg-info/top_level.txt
```

### Comparing `ezsession-0.0.8/PKG-INFO` & `ezsession-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 [![GitHub](https://img.shields.io/badge/GitHub-Sponsor%20Josh%20XT-blue?logo=github&style=plastic)](https://github.com/sponsors/Josh-XT) [![PayPal](https://img.shields.io/badge/PayPal-Sponsor%20Josh%20XT-blue.svg?logo=paypal&style=plastic)](https://paypal.me/joshxt) [![Ko-Fi](https://img.shields.io/badge/Kofi-Sponsor%20Josh%20XT-blue.svg?logo=kofi&style=plastic)](https://ko-fi.com/joshxt)
```

### Comparing `ezsession-0.0.8/README.md` & `ezsession-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.8/setup.py` & `ezsession-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ezsession",
-    version="0.0.8",
+    version="0.0.9",
     description="A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `ezsession-0.0.8/src/ezsession/__init__.py` & `ezsession-0.0.9/src/ezsession/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,12 +114,14 @@
                 "Authorization": auth_request["token_type"]
                 + " "
                 + auth_request["access_token"],
                 "Content-Type": "application/json",
                 "Accept": "application/json",
             }
         else:
-            session.headers.update(auth)
+            # Delete auth type
+            del auth["type"]
+            session.headers.update(**auth)
     for key in auth:
         if key not in input_keys:
             session.headers.update({key: auth[key]})
     return session
```

### Comparing `ezsession-0.0.8/src/ezsession.egg-info/PKG-INFO` & `ezsession-0.0.9/src/ezsession.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 [![GitHub](https://img.shields.io/badge/GitHub-Sponsor%20Josh%20XT-blue?logo=github&style=plastic)](https://github.com/sponsors/Josh-XT) [![PayPal](https://img.shields.io/badge/PayPal-Sponsor%20Josh%20XT-blue.svg?logo=paypal&style=plastic)](https://paypal.me/joshxt) [![Ko-Fi](https://img.shields.io/badge/Kofi-Sponsor%20Josh%20XT-blue.svg?logo=kofi&style=plastic)](https://ko-fi.com/joshxt)
```

