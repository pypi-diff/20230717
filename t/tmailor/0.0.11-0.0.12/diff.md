# Comparing `tmp/tmailor-0.0.11.tar.gz` & `tmp/tmailor-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmailor-0.0.11.tar", last modified: Sun Jul 16 13:42:58 2023, max compression
+gzip compressed data, was "tmailor-0.0.12.tar", last modified: Mon Jul 17 08:56:33 2023, max compression
```

## Comparing `tmailor-0.0.11.tar` & `tmailor-0.0.12.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/
--rw-r--r--   0 runner    (1000) runner    (1000)     1082 2023-07-16 13:37:58.000000 tmailor-0.0.11/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 13:42:58.296985 tmailor-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2306 2023-07-16 13:37:58.000000 tmailor-0.0.11/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-16 13:42:58.296985 tmailor-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1016 2023-07-16 13:42:06.000000 tmailor-0.0.11/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/
--rw-r--r--   0 runner    (1000) runner    (1000)       35 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3917 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/ext/
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/ext/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       72 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/headers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2036 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/objects.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 08:56:33.273519 tmailor-0.0.12/
+-rw-------   0 runner    (1000) runner    (1000)     1082 2023-07-17 08:54:06.000000 tmailor-0.0.12/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-17 08:56:33.273519 tmailor-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2306 2023-07-16 13:37:58.000000 tmailor-0.0.12/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-17 08:56:33.273519 tmailor-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1016 2023-07-17 08:54:24.000000 tmailor-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 08:56:33.269519 tmailor-0.0.12/tmailor/
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2023-07-17 08:55:16.000000 tmailor-0.0.12/tmailor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3917 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 08:56:33.273519 tmailor-0.0.12/tmailor/ext/
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/ext/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 08:56:33.273519 tmailor-0.0.12/tmailor/ext/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       72 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/ext/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/ext/utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/ext/utilities/headers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2036 2023-07-16 13:37:58.000000 tmailor-0.0.12/tmailor/ext/utilities/objects.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-17 08:56:33.273519 tmailor-0.0.12/tmailor.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-17 08:56:32.000000 tmailor-0.0.12/tmailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-17 08:56:32.000000 tmailor-0.0.12/tmailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-17 08:56:32.000000 tmailor-0.0.12/tmailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-07-17 08:56:32.000000 tmailor-0.0.12/tmailor.egg-info/top_level.txt
```

### Comparing `tmailor-0.0.11/LICENSE` & `tmailor-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.11/PKG-INFO` & `tmailor-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmailor
-Version: 0.0.11
+Version: 0.0.12
 Summary: A temporary email address is: a library that provides email addresses without registration, used to receive incoming emails without disclosing your actual email.
 Home-page: https://github.com/heromr/tmailor
 Author: HeroMR
 Author-email: mrhero4006@gmail.com
 License: MIT
 Keywords: python,tmailor,temp mail,disposable email,temp mailbox,fake email
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmailor Version: 0.0.11 Summary: A temporary email
+Metadata-Version: 2.1 Name: tmailor Version: 0.0.12 Summary: A temporary email
 address is: a library that provides email addresses without registration, used
 to receive incoming emails without disclosing your actual email. Home-page:
 https://github.com/heromr/tmailor Author: HeroMR Author-email:
 mrhero4006@gmail.com License: MIT Keywords: python,tmailor,temp mail,disposable
 email,temp mailbox,fake email Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
```

### Comparing `tmailor-0.0.11/README.md` & `tmailor-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.11/setup.py` & `tmailor-0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
 	long_description = f.read()
 
-VERSION = "0.0.11"
+VERSION = "0.0.12"
 DESCRIPTION = "A temporary email address is: a library that provides email addresses without registration, used to receive incoming emails without disclosing your actual email."
 
 setup(name="tmailor",
       version=VERSION,
       description=DESCRIPTION,
       author="HeroMR",
       author_email="mrhero4006@gmail.com",
```

### Comparing `tmailor-0.0.11/tmailor/client.py` & `tmailor-0.0.12/tmailor/client.py`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.11/tmailor/ext/utilities/exceptions.py` & `tmailor-0.0.12/tmailor/ext/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.11/tmailor/ext/utilities/objects.py` & `tmailor-0.0.12/tmailor/ext/utilities/objects.py`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.11/tmailor.egg-info/PKG-INFO` & `tmailor-0.0.12/tmailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmailor
-Version: 0.0.11
+Version: 0.0.12
 Summary: A temporary email address is: a library that provides email addresses without registration, used to receive incoming emails without disclosing your actual email.
 Home-page: https://github.com/heromr/tmailor
 Author: HeroMR
 Author-email: mrhero4006@gmail.com
 License: MIT
 Keywords: python,tmailor,temp mail,disposable email,temp mailbox,fake email
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmailor Version: 0.0.11 Summary: A temporary email
+Metadata-Version: 2.1 Name: tmailor Version: 0.0.12 Summary: A temporary email
 address is: a library that provides email addresses without registration, used
 to receive incoming emails without disclosing your actual email. Home-page:
 https://github.com/heromr/tmailor Author: HeroMR Author-email:
 mrhero4006@gmail.com License: MIT Keywords: python,tmailor,temp mail,disposable
 email,temp mailbox,fake email Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
```

