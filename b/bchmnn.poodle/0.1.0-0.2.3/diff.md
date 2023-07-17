# Comparing `tmp/bchmnn.poodle-0.1.0.tar.gz` & `tmp/bchmnn.poodle-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bchmnn.poodle-0.1.0.tar", last modified: Fri Jul  7 18:06:21 2023, max compression
+gzip compressed data, was "bchmnn.poodle-0.2.3.tar", last modified: Mon Jul 17 15:26:34 2023, max compression
```

## Comparing `bchmnn.poodle-0.1.0.tar` & `bchmnn.poodle-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.726875 bchmnn.poodle-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 18:06:21.726875 bchmnn.poodle-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:06:21.726875 bchmnn.poodle-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.718875 bchmnn.poodle-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 18:06:21.000000 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 18:06:21.000000 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:06:21.000000 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 18:06:21.000000 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 18:06:21.000000 bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/poodle/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/poodle/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/poodle/auth/handler/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/handler/abstract_sso_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/handler/browser_sso_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/poodle/auth/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/provider/cli_credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/provider/credential_provider_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/auth/provider/generic_credential_provider_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/corews.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/poodle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.722875 bchmnn.poodle-0.1.0/src/poodle/types/
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/jsonable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/types/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:21.726875 bchmnn.poodle-0.1.0/src/poodle/util/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/parse_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/url_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 18:05:49.000000 bchmnn.poodle-0.1.0/src/poodle/util/win_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 15:26:34.000000 bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/poodle/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/corews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/poodle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.095934 bchmnn.poodle-0.2.3/poodle/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/jsonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/types/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/poodle/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/parse_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/poodle/util/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 15:25:50.000000 bchmnn.poodle-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:26:34.099934 bchmnn.poodle-0.2.3/setup.cfg
```

### Comparing `bchmnn.poodle-0.1.0/LICENSE` & `bchmnn.poodle-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.1.0/PKG-INFO` & `bchmnn.poodle-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.1.0
-Summary: Moodle SDK for python
+Version: 0.2.3
+Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -792,17 +792,14 @@
     await moodle.auth()
     # do some stuff
 ```
 
 ## Features
 
 - [ ] authentication using os browser
-  - [x] windows (callback by registering url schema using windows registry)
-  - [ ] \*nix (callback by registering url schema using ??)
-  - [ ] osx (callback by registering url schema using ??)
 - [x] caching
 - [ ] types
   - [x] core_webservice_get_site_info
   - [x] core_enrol_get_users_courses
   - [x] core_course_get_contents
   - [x] core_group_get_course_groups
   - [x] mod_assign_get_assignments
```

### Comparing `bchmnn.poodle-0.1.0/README.md` & `bchmnn.poodle-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -100,17 +100,14 @@
     await moodle.auth()
     # do some stuff
 ```
 
 ## Features
 
 - [ ] authentication using os browser
-  - [x] windows (callback by registering url schema using windows registry)
-  - [ ] \*nix (callback by registering url schema using ??)
-  - [ ] osx (callback by registering url schema using ??)
 - [x] caching
 - [ ] types
   - [x] core_webservice_get_site_info
   - [x] core_enrol_get_users_courses
   - [x] core_course_get_contents
   - [x] core_group_get_course_groups
   - [x] mod_assign_get_assignments
```

### Comparing `bchmnn.poodle-0.1.0/pyproject.toml` & `bchmnn.poodle-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bchmnn.poodle"
-version = "0.1.0"
-description = "Moodle SDK for python"
+version = "0.2.3"
+description = "Python Moodle SDK"
 readme = "README.md"
 authors = [{ name = "Jacob Bachmann", email = "jacob.bachmann@posteo.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "License :: OSI Approved :: MIT License",
@@ -19,26 +19,39 @@
 keywords = ["moodle", "sdk", "api"]
 dependencies = [
     "aiohttp >= 3.8.0",
 ]
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
-dev = ["black", "pip-tools", "bumpver", "build", "twine", "git-changelog"]
+dev = [
+    "black",
+    "pip-tools",
+    "bumpver",
+    "build",
+    "twine",
+    "git-changelog",
+    "mypy",
+    "pylint",
+    "isort"
+]
 
 [project.urls]
 Homepage = "https://github.com/bchmnn/poodle"
 
+[tool.setuptools.package-data]
+"poodle" = ["py.typed"]
+
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "feat: release v{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"'
 ]
-"src/poodle/__init__.py" = ["{version}"]
+"poodle/__init__.py" = ["{version}"]
```

### Comparing `bchmnn.poodle-0.1.0/src/bchmnn.poodle.egg-info/PKG-INFO` & `bchmnn.poodle-0.2.3/bchmnn.poodle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.1.0
-Summary: Moodle SDK for python
+Version: 0.2.3
+Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -792,17 +792,14 @@
     await moodle.auth()
     # do some stuff
 ```
 
 ## Features
 
 - [ ] authentication using os browser
-  - [x] windows (callback by registering url schema using windows registry)
-  - [ ] \*nix (callback by registering url schema using ??)
-  - [ ] osx (callback by registering url schema using ??)
 - [x] caching
 - [ ] types
   - [x] core_webservice_get_site_info
   - [x] core_enrol_get_users_courses
   - [x] core_course_get_contents
   - [x] core_group_get_course_groups
   - [x] mod_assign_get_assignments
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/auth/provider/generic_credential_provider_interface.py` & `bchmnn.poodle-0.2.3/poodle/credentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,41 @@
+from getpass import getpass
 from typing import Tuple
 
-from .credential_provider_interface import CredentialProviderInterface
+from .util.loggable import Loggable
+
+
+class CredentialProviderInterface(Loggable):
+    _priority: int
+    _id_provider_url: str
+
+    def __init__(self, id_provider_url: str, priority: int, name="CredentialProvider"):
+        super().__init__(name)
+        self._id_provider_url = id_provider_url
+        self._priority = priority
+
+    @property
+    def priority(self) -> int:
+        return self._priority
+
+    @property
+    def id_provider_url(self) -> str:
+        return self._id_provider_url
+
+    @property
+    def name(self) -> str:
+        return "LoginProviderInterface"
 
 
 class GenericCredentialProviderInterface(CredentialProviderInterface):
     _username: str
     _password: str
 
-    def __init__(self, id_provider_url, priority):
-        super().__init__(id_provider_url, priority)
+    def __init__(self, id_provider_url, priority, name):
+        super().__init__(id_provider_url, priority, name)
 
     @property
     def username(self) -> str:
         return self._username
 
     @property
     def password(self) -> str:
@@ -25,7 +48,21 @@
         process is triggered.
         """
         return ("", "")
 
     @property
     def name(self) -> str:
         return "GenericLoginProviderInterface"
+
+
+class CLICredentialProvider(GenericCredentialProviderInterface):
+    def __init__(self, id_provider_url="*", priority=1):
+        super().__init__(id_provider_url, priority, name="CLICredentialProvider")
+
+    def retrieve(self) -> Tuple[str, str]:
+        self._username = input("Username: ")
+        self._password = getpass("Password: ")
+        return (self._username, self.password)
+
+    @property
+    def name(self) -> str:
+        return "CLILoginProvider"
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/corews.py` & `bchmnn.poodle-0.2.3/poodle/corews.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import typing
-from typing import Dict
+from typing import Dict, Mapping, Optional
 from urllib import parse
 
 import aiohttp
 
-from .types.exception import CoreConnectionError, CoreWSError
 from .constants import CONTENT_TYPE, X_WWW_FORM_URLENCODED
+from .types.exception import CoreAjaxWSError, CoreConnectionError, CoreWSError
 from .util.parse_form import parse_form
 from .util.tokens import Tokens
 
 
 class CoreWS(aiohttp.ClientSession):
     _url: str
     _tokens: Tokens
@@ -23,50 +23,64 @@
     def tokens(self):
         return None
 
     @tokens.setter
     def tokens(self, value: Tokens):
         self._tokens = value
 
-    async def call(self, method: str, data={}, presets: Dict[str, typing.Any] = {}):
+    async def call(
+        self,
+        method: str,
+        data: Optional[Mapping[str, typing.Any]] = None,
+        presets: Optional[Mapping[str, typing.Any]] = None,
+    ):
         """
         ref: moodleapp/src/core/services/ws.ts::CoreWSProvider::call
         """
-        data["wsfunction"] = method
-        data["wstoken"] = self._tokens.token
+        _data = dict(data) if data is not None else {}
+        _presets = dict(presets) if presets is not None else {}
+        _data["wsfunction"] = method
+        _data["wstoken"] = self._tokens.token
 
         url = (
             self._url
             + "/webservice/rest/server.php?moodlewsrestformat=json&wsfunction="
             + method
         )
-        _data = parse_form(data)
+        __data = parse_form(_data)
         res = await self.post(
             url,
-            data=_data,
+            data=__data,
             headers={CONTENT_TYPE: X_WWW_FORM_URLENCODED},
         )
-        payload = await res.text()
-        if payload is None and not presets.get("response_expected"):
-            payload = "[{}]"
+        response = await res.text()
+        if response is None and not _presets.get("response_expected"):
+            response = "[{}]"
 
-        if payload is None:
+        if response is None:
             raise CoreConnectionError("connection error")
-        result = json.loads(payload)
+        result = json.loads(response)
 
         if "exception" in result:
             raise CoreWSError(
                 result["exception"], result["errorcode"], result["message"]
             )
 
         return result
 
     async def call_ajax(
-        self, method: str, data: dict = {}, presets: Dict[str, bool] = {}
+        self,
+        method: str,
+        data: Optional[dict] = None,
+        presets: Optional[Dict[str, bool]] = None,
     ):
+        if data is None:
+            data = {}
+        if presets is None:
+            presets = {}
         ajax_data = [{"index": 0, "methodname": method, "args": data}]
 
         script = "service.php"
         if presets.get("use_get") and presets.get("no_login"):
             script = "service-nologin.php"
 
         url = self._url + "/lib/ajax/" + script + "?info=" + method
@@ -83,16 +97,18 @@
 
         payload = await res.text()
 
         if payload is None and not presets.get("response_expected"):
             payload = "[{}]"
 
         if payload is None:
-            raise Exception("connection error")
+            raise CoreConnectionError("connection error")
 
         result = json.loads(payload)
         result = result[0]
 
         if "error" in result and result["error"] is not False:
-            raise Exception(result["exception"])
+            raise CoreAjaxWSError(
+                result["exception"], result["errorcode"], result["message"]
+            )
 
         return result["data"]
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/poodle.py` & `bchmnn.poodle-0.2.3/poodle/poodle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,289 +1,175 @@
 import inspect
 import logging
 import re
-from typing import Any, Dict, Generic, List, Optional, Type, TypedDict, TypeVar
+from typing import Any, List, Optional
 
-import aiohttp
-
-from .types.exception import CoreWSError
-
-
-from .auth.handler.abstract_sso_handler import AbstractSSOHandler
-from .auth.handler.browser_sso_handler import BrowserSSOHandler
+from .auth import AbstractSSOHandler, BrowserSSOHandler
 from .corews import CoreWS
-from .types.assign import (
-    AddonModAssignGetAssignments,
-    AddonModAssignGetSubmissions,
-    AddonModAssignParticipant,
-)
-from .types.groups import CoreGroupGetCourseGroup
-from .types.course import CoreCourseGetContentsWSSection
-from .types.courses import CoreEnrolledCourseData
-from .types.site import CoreSiteInfo, CoreSitePublicConfig
+from .types.exception import (AuthError, CourseNotFoundError,
+                              MissingPrivateAccessKeyError)
+from .types.methods import DataTypeT, MoodleMethod, MoodleMethods, ReturnTypeT
+from .types.site import CoreSitePublicConfig
 from .util.cache import Cache, CacheItem
-from .util.logging import Loggable
-from .util.tokens import TokenPolicy, Tokens
-
-T = TypeVar("T")
-U = TypeVar("U", bound=TypedDict)
+from .util.loggable import Loggable
+from .util.tokens import Tokens
 
 
-class MoodleMethod(TypedDict, Generic[T, U]):
-    key: str
-    type: Type[T]
-    data: Type[U]
-
-
-class NoArgs(TypedDict):
-    pass
-
-
-class CoreEnrolGetUsersCoursesArgs(TypedDict):
-    # TODO add missing args
-    userid: int
-    returnusercount: int  # 0 for False, 1 for True
-
-
-class CoreCourseGetContentsArgs(TypedDict):
-    # TODO add missing args
-    courseid: int
-
-
-class CoreGroupGetCourseGroupsArgs(TypedDict):
-    # TODO add missing args
-    courseid: int
-
-
-class ModAssignGetAssignmentsArgs(TypedDict):
-    # TODO add missing args
-    courseids: List[int]
-
-
-class ModAssignGetSubmissionsArgs(TypedDict):
-    # TODO add missing args
-    assignmentids: List[int]
-
-
-class ModAssignParticipantArgs(TypedDict):
-    # TODO add missing args
-    assignid: int
-    groupid: int
-    filter: str
-
-
-class MoodleMethods:
-    CORE_WEBSERVICE_GET_SITE_INFO: MoodleMethod[CoreSiteInfo, NoArgs] = {
-        "key": "core_webservice_get_site_info",
-        "type": CoreSiteInfo,
-        "data": NoArgs,
-    }
-
-    CORE_ENROL_GET_USERS_COURSES: MoodleMethod[
-        List[CoreEnrolledCourseData], CoreEnrolGetUsersCoursesArgs
-    ] = {
-        "key": "core_enrol_get_users_courses",
-        "type": List[CoreEnrolledCourseData],
-        "data": CoreEnrolGetUsersCoursesArgs,
-    }
-
-    CORE_COURSE_GET_CONTENTS: MoodleMethod[
-        List[CoreCourseGetContentsWSSection], CoreCourseGetContentsArgs
-    ] = {
-        "key": "core_course_get_contents",
-        "type": List[CoreCourseGetContentsWSSection],
-        "data": CoreCourseGetContentsArgs,
-    }
-
-    CORE_GROUP_GET_COURSE_GROUPS: MoodleMethod[
-        List[CoreGroupGetCourseGroup], CoreGroupGetCourseGroupsArgs
-    ] = {
-        "key": "core_group_get_course_groups",
-        "type": List[CoreGroupGetCourseGroup],
-        "data": CoreGroupGetCourseGroupsArgs,
-    }
-
-    MOD_ASSIGN_GET_ASSIGNMENTS: MoodleMethod[
-        AddonModAssignGetAssignments, ModAssignGetAssignmentsArgs
-    ] = {
-        "key": "mod_assign_get_assignments",
-        "type": AddonModAssignGetAssignments,
-        "data": ModAssignGetAssignmentsArgs,
-    }
-
-    MOD_ASSIGN_GET_SUBMISSIONS: MoodleMethod[
-        AddonModAssignGetSubmissions, ModAssignGetSubmissionsArgs
-    ] = {
-        "key": "mod_assign_get_submissions",
-        "type": AddonModAssignGetSubmissions,
-        "data": ModAssignGetSubmissionsArgs,
-    }
-
-    # mod_assign_list_participants
-    MOD_ASSIGN_LIST_PARTICIPANTS: MoodleMethod[
-        List[AddonModAssignParticipant], ModAssignParticipantArgs
-    ] = {
-        "key": "mod_assign_list_participants",
-        "type": List[AddonModAssignParticipant],
-        "data": ModAssignParticipantArgs,
-    }
-
-
-class Poodle(Loggable):
-    _url: str
-    _corews: CoreWS
-    _cache: Dict[str, Any]
+class Poodle(Loggable, CoreWS):
     cache: Cache = Cache()
     _auth_handlers: List[AbstractSSOHandler]
-    _token_policy: TokenPolicy
 
     def __init__(
         self,
         url: str,
-        auth_handlers: List[AbstractSSOHandler] = [],
-        token_policy: Optional[TokenPolicy] = None,
+        auth_handlers: Optional[List[AbstractSSOHandler]] = None,
     ):
-        self.init_logger("Poodle", level=logging.DEBUG)
-        self._url = url
-        self._cache = {}
+        Loggable.__init__(self, "Poodle", logging.WARN)
+        CoreWS.__init__(self, url)
+        if auth_handlers is None:
+            auth_handlers = []
         self._auth_handlers = [BrowserSSOHandler(0)]
         self._auth_handlers.extend(auth_handlers)
-        self._token_policy = (
-            token_policy if token_policy is not None else TokenPolicy.DONT_CACHE()
-        )
 
     @property
     def url(self):
         return self._url
 
     async def __aenter__(self):
-        self._corews = await CoreWS(self._url).__aenter__()
+        await super(CoreWS, self).__aenter__()
         return self
 
     async def __aexit__(self, *args, **kwargs):
-        await self._corews.__aexit__(*args, **kwargs)
+        await super(CoreWS, self).__aexit__(*args, **kwargs)
 
-    async def auth(self):
-        if self._token_policy.cache:
-            tokens = self._token_policy.retrieve()
-            if tokens is not None:
-                self._corews.tokens = tokens
-                try:
-                    await self.core_webservice_get_site_info()
-                    return
-                except CoreWSError as e:
-                    self._logger.warn(
-                        f"CoreWS raised error {e.errorcode}: {str(e)}. Reauthenticating"
-                    )
+    async def authenticate(self):
         self._auth_handlers.sort(key=lambda handler: handler.priority, reverse=True)
         public_config = await self.public_config()
         for auth_handler in self._auth_handlers:
             if set(auth_handler.id_provider_urls).intersection(
                 [
                     "*",
                     *map(
                         lambda identityprovider: identityprovider.url,
                         public_config.identityproviders,
                     ),
                 ]
             ):
                 if inspect.iscoroutinefunction(auth_handler.authenticate):
-                    tokens = await auth_handler.authenticate(
-                        public_config, self._corews
-                    )
+                    tokens = await auth_handler.authenticate(public_config, self)
                 else:
-                    tokens = auth_handler.authenticate(public_config, self._corews)
+                    tokens = auth_handler.authenticate(public_config, self)
                 if isinstance(tokens, Tokens):
-                    if self._token_policy.cache:
-                        self._token_policy.persist(tokens)
-                    self._corews.tokens = tokens
+                    self.tokens = tokens
                     return
-                else:
-                    raise Exception("Tokens has invalid type")
-        raise Exception("Authentication failed")
+                raise AuthError("Tokens has invalid type")
+        raise AuthError("Authentication failed")
 
-    async def get(
-        self, method: MoodleMethod[T, U], data: U = {}, usecache=True, refetch=False
-    ) -> T:
+    async def fetch(
+        self,
+        method: MoodleMethod[Any, ReturnTypeT, DataTypeT],
+        data: Optional[DataTypeT] = None,
+        usecache=True,
+        refetch=False,
+    ) -> ReturnTypeT:
         key = method["key"]
-        type = method["type"]
-        cacheitem: CacheItem = {"key": key, "type": type}
+        return_type = method["type"]
+        cacheitem: CacheItem = {"key": key, "type": return_type}
         if usecache and not refetch:
-            item = self.cache.get(cacheitem)
-            if item is not None:
-                return item
-        self._logger.debug(f"Fetching {key} ...")
-        if hasattr(type, "_name") and getattr(type, "_name") == "List":
-            type = getattr(type, "__args__")[0]
-            item = [type(**entry) for entry in await self._corews.call(key, data=data)]
-        else:
-            item = type(**await self._corews.call(key, data=data))
+            _item = self.cache.get(cacheitem)
+            if _item is not None:
+                return _item
+        self.logger.debug("Fetching %s ...", key)
+        item = return_type(**await self.call(key, data))  # type: ignore
         if usecache:
-            self.cache.set(cacheitem, item)  # type: ignore
+            self.cache.set(cacheitem, item)
+        return item
+
+    async def fetch_list(
+        self,
+        method: MoodleMethod[List, ReturnTypeT, DataTypeT],
+        data: Optional[DataTypeT] = None,
+        usecache=True,
+        refetch=False,
+    ) -> List[ReturnTypeT]:
+        key = method["key"]
+        return_type = method["type"]
+        cacheitem: CacheItem = {"key": key, "type": return_type}
+        if usecache and not refetch:
+            _item = self.cache.get(cacheitem)
+            if _item is not None:
+                return _item
+        self.logger.debug("Fetching %s ...", key)
+        item = [return_type(**entry) for entry in await self.call(key, data)]
+        if usecache:
+            self.cache.set(cacheitem, item)
         return item  # type: ignore
 
     async def public_config(self) -> CoreSitePublicConfig:
         method = "tool_mobile_get_public_config"
-        cachekey = method
-        if cachekey in self._cache.keys():
-            self._logger.debug(f"Fetching {cachekey}. Cache hit!")
-            return self._cache[cachekey]
-        self._logger.debug(f"Fetching {cachekey} ...")
+        cacheitem: CacheItem = {"key": method, "type": CoreSitePublicConfig}
+        item = self.cache.get(cacheitem)
+        if item is not None:
+            self.logger.debug("Fetching %s. Cache hit!", method)
+            return item
+        self.logger.debug("Fetching %s ...", method)
         public_config = CoreSitePublicConfig(
-            **await self._corews.call_ajax(
+            **await self.call_ajax(
                 method,
                 presets={"use_get": True, "no_login": True},
             )
         )
-        self._cache["tool_mobile_get_public_config"] = public_config
+        self.cache.set(cacheitem, public_config)
         return public_config
 
     async def core_webservice_get_site_info(self):
-        return await self.get(MoodleMethods.CORE_WEBSERVICE_GET_SITE_INFO)
+        return await self.fetch(MoodleMethods.CORE_WEBSERVICE_GET_SITE_INFO)
 
     @staticmethod
     def fix_file_url(url: str, token: str) -> str:
         return re.sub(
             r"(\/webservice)?\/pluginfile\.php", f"/tokenpluginfile.php/{token}", url
         )
 
     async def fetch_file(self, url):
         token = (await self.core_webservice_get_site_info()).userprivateaccesskey
         if token is None:
-            raise Exception("Current site is missing userprivateaccesskey")
-        return await self._corews.get(self.fix_file_url(url, token))
+            raise MissingPrivateAccessKeyError(
+                "Current site is missing userprivateaccesskey"
+            )
+        return await self.get(self.fix_file_url(url, token))
 
     async def core_enrol_get_users_courses(self, userid: Optional[int] = None):
         if userid is None:
             userid = (await self.core_webservice_get_site_info()).userid
-        return await self.get(
+        return await self.fetch_list(
             MoodleMethods.CORE_ENROL_GET_USERS_COURSES,
             {"userid": userid, "returnusercount": 0},
             usecache=False,
         )
 
     async def get_user_courses(self, name: str, userid: Optional[int] = None):
         courses = await self.core_enrol_get_users_courses(userid)
         return [item for item in courses if name.lower() in item.fullname.lower()]
 
     async def get_user_course(self, name: str, userid: Optional[int] = None):
         courses = await self.get_user_courses(name, userid)
         if len(courses) == 0:
-            raise Exception(f"Could not find course: '{name}'")
+            raise CourseNotFoundError(f"Could not find course: '{name}'")
         return courses[0]
 
     async def core_course_get_contents(self, courseid: int):
-        return await self.get(
+        return await self.fetch_list(
             MoodleMethods.CORE_COURSE_GET_CONTENTS,
             {"courseid": courseid},
             usecache=False,
         )
 
     async def mod_assign_get_assignments(self, courseids: List[int]):
-        return await self.get(
+        return await self.fetch(
             MoodleMethods.MOD_ASSIGN_GET_ASSIGNMENTS,
             {"courseids": courseids},
             usecache=False,
         )
 
     async def get_assignments(self, courseid: int):
         return (
@@ -294,37 +180,37 @@
         assignments = await self.get_assignments(courseid)
         if (
             index >= 0
             and index >= len(assignments)
             or index < 0
             and -index >= len(assignments)
         ):
-            raise Exception("Index out of bounds")
+            raise IndexError("Index out of bounds")
         return assignments[index]
 
     async def mod_assign_get_submissions(self, assignmentids: List[int]):
-        return await self.get(
+        return await self.fetch(
             MoodleMethods.MOD_ASSIGN_GET_SUBMISSIONS,
             {"assignmentids": assignmentids},
             usecache=False,
         )
 
     async def get_submissions(self, assignmentid: int):
         return (
             (await self.mod_assign_get_submissions([assignmentid]))
             .assignments[0]
             .submissions
         )
 
     async def mod_assign_list_participants(self, assignid: int):
-        return await self.get(
+        return await self.fetch_list(
             MoodleMethods.MOD_ASSIGN_LIST_PARTICIPANTS,
             {"assignid": assignid, "groupid": 0, "filter": ""},
             usecache=False,
         )
 
     async def core_group_get_course_groups(self, courseid: int):
-        return await self.get(
+        return await self.fetch_list(
             MoodleMethods.CORE_GROUP_GET_COURSE_GROUPS,
             {"courseid": courseid},
             usecache=False,
         )
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/assign.py` & `bchmnn.poodle-0.2.3/poodle/types/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,30 +440,30 @@
     ] = None  # The expected date for marking the submissions.
     teamsubmission: int  # If enabled, students submit as a team.
     requireallteammemberssubmit: int  # If enabled, all team members must submit.
     teamsubmissiongroupingid: int  # The grouping id for the team submission groups.
     blindmarking: int  # If enabled, hide identities until reveal identities actioned.
     hidegrader: Optional[int] = None  # @since 3.7. If enabled, hide grader to student.
     revealidentities: int  # Show identities for a blind marking assignment.
-    attemptreopenmethod: AddonModAssignAttemptReopenMethodValues  # Method used to control opening new attempts.
+    # Method used to control opening new attempts.
+    attemptreopenmethod: AddonModAssignAttemptReopenMethodValues
     maxattempts: int  # Maximum number of attempts allowed.
     markingworkflow: int  # Enable marking workflow.
     markingallocation: int  # Enable marking allocation.
     requiresubmissionstatement: int  # Student must accept submission statement.
     preventsubmissionnotingroup: Optional[
         int
     ] = None  # Prevent submission not in group.
     submissionstatement: Optional[str] = None  # Submission statement formatted.
     submissionstatementformat: Optional[
         int
     ] = None  # Submissionstatement format (1 = HTML, 0 = MOODLE, 2 = PLAIN or 4 = MARKDOWN).
     configs: List[AddonModAssignConfig] = []  # Configuration settings.
-    intro: Optional[
-        str
-    ] = None  # Assignment intro, not allways returned because it deppends on the activity configuration.
+    # Assignment intro, not allways returned because it deppends on the activity configuration.
+    intro: Optional[str] = None
     introformat: Optional[
         int
     ] = None  # Intro format (1 = HTML, 0 = MOODLE, 2 = PLAIN or 4 = MARKDOWN).
     introfiles: Optional[List[CoreWSExternalFile]] = None
     introattachments: Optional[List[CoreWSExternalFile]] = None
     activity: Optional[str] = None  # @since 4.0. Description of activity.
     activityformat: Optional[int] = None  # @since 4.0. Format of activity.
@@ -548,15 +548,16 @@
                 self.warnings = [CoreWSExternalWarning(**entry) for entry in warnings]
 
 
 class AddonModAssignParticipantCustomField(Jsonable):
     type: str  # The type of the custom field - text field, checkbox...
     value: str  # The value of the custom field.
     name: str  # The name of the custom field.
-    shortname: str  # The shortname of the custom field - to be able to build the field class in the code.
+    # The shortname of the custom field - to be able to build the field class in the code.
+    shortname: str
 
     def __init__(self, **entries):
         self.__dict__.update(entries)
 
 
 class AddonModAssignParticipantPreference(Jsonable):
     name: str  # The name of the preferences.
@@ -638,17 +639,16 @@
     ] = None  # User custom fields (also known as user profile fields).
     prefernces: Optional[
         List[AddonModAssignParticipantPreference]
     ] = None  # Users preferences.
     recordid: Optional[int] = None  # @since 3.7. Record id.
     groups: Optional[List[AddonModAssignParticipantGroup]] = None  # User groups.
     roles: Optional[List[AddonModAssignParticipantRole]] = None  # User roles.
-    enrolledcourses: Optional[
-        List[AddonModAssignParticipantEnrolledCourses]
-    ] = None  # Courses where the user is enrolled - limited by which courses the user is able to see.
+    # Courses where the user is enrolled - limited by which courses the user is able to see.
+    enrolledcourses: Optional[List[AddonModAssignParticipantEnrolledCourses]] = None
     submitted: bool  # Have they submitted their assignment.
     requiregrading: bool  # Is their submission waiting for grading.
     grantedextension: Optional[bool] = None  # Have they been granted an extension.
     groupid: Optional[int] = None  # For group assignments this is the group id.
     groupname: Optional[str] = None  # For group assignments this is the group name.
 
     def __init__(self, **entries):
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/course.py` & `bchmnn.poodle-0.2.3/poodle/types/course.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/courses.py` & `bchmnn.poodle-0.2.3/poodle/types/courses.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     enablecompletion: Optional[
         bool
     ] = None  # True if completion is enabled, otherwise false.
     startdate: Optional[int] = None  # Timestamp when the course start.
     enddate: Optional[int] = None  # Timestamp when the course end.
 
     def __init__(self, **entries):
-        self.__dict__.update(entries)
+        CoreCourseBasicData.__init__(self, **entries)
 
 
 class CoreEnrolledCourseData(CoreEnrolledCourseBasicData, Jsonable):
     """
     Course Data model received when the user is enrolled.
     """
 
@@ -65,15 +65,15 @@
         bool
     ] = None  # @since 3.11. Whether the activity completion conditions are shown or not.
     timemodified: Optional[
         int
     ] = None  # @since 4.0. Last time course settings were updated (timestamp).
 
     def __init__(self, **entries):
-        self.__dict__.update(entries)
+        CoreEnrolledCourseBasicData.__init__(self, **entries)
         keys = entries.keys()
         if "overviewfiles" in keys:
             overviewfiles = entries["overviewfiles"]
             if overviewfiles is not None:
                 self.overviewfiles = [
                     CoreWSExternalFile(**entry) for entry in overviewfiles
                 ]
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/site.py` & `bchmnn.poodle-0.2.3/poodle/types/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import IntEnum
 from typing import List, Optional
 
-from .jsonable import Jsonable
-from .ws import CoreWSExternalWarning
+from poodle.types.jsonable import Jsonable
+from poodle.types.ws import CoreWSExternalWarning
 
 
 class CoreSiteQRCodeType(Jsonable, IntEnum):
     QR_CODE_DISABLED = 0  # QR code disabled value
     QR_CODE_URL = 1  # QR code type URL value
     QR_CODE_LOGIN = 2  # QR code type login value
 
@@ -143,17 +143,16 @@
     ] = []  # Advanced features availability.
     usercanmanageownfiles: Optional[
         bool
     ] = None  # True if the user can manage his own files.
     userquota: Optional[
         int
     ] = None  # User quota (bytes). 0 means user can ignore the quota.
-    usermaxuploadfilesize: Optional[
-        int
-    ] = None  # User max upload file size (bytes). -1 means the user can ignore the upload file size.
+    # User max upload file size (bytes). -1 means the user can ignore the upload file size.
+    usermaxuploadfilesize: Optional[int] = None
     userhomepage: Optional[
         CoreSiteInfoUserHomepage
     ] = None  # The default home page for the user.
     userprivateaccesskey: Optional[
         str
     ] = None  # Private user access key for fetching files.
     siteid: Optional[int] = None  # Site course ID.
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/tag.py` & `bchmnn.poodle-0.2.3/poodle/types/tag.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.1.0/src/poodle/types/ws.py` & `bchmnn.poodle-0.2.3/poodle/types/ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from .jsonable import Jsonable
+from poodle.types.jsonable import Jsonable
 
 
 # Structure of warnings returned by WS.
 class CoreWSExternalWarning(Jsonable):
     item: Optional[str] = None
     itemid: Optional[int] = None
     warningcode: Optional[
```

### Comparing `bchmnn.poodle-0.1.0/src/poodle/util/parse_form.py` & `bchmnn.poodle-0.2.3/poodle/util/parse_form.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import urllib.parse
 from typing import Any, Dict, List
 
 
 def is_primitive(value: Any):
-    return type(value) is int or type(value) is str or type(value) is bool
+    return isinstance(value, (int, str, bool))
 
 
 def is_collection(value: Any):
-    return type(value) is set or type(value) is list
+    return isinstance(value, (set, list))
 
 
-def _parse_form(data: Any, prefix: str = "") -> List:
+def _parse_form(data: Any, prefix: str = "") -> List[str]:
     if data is None:
         return []
     if is_primitive(data):
-        value = str(data).lower() if type(data) is bool else str(data)
+        value = str(data).lower() if isinstance(data, bool) else str(data)
         return [urllib.parse.quote(prefix) + "=" + urllib.parse.quote(value)]
-    result = []
+    result: List[str] = []
     if is_collection(data):
         for i, value in enumerate(data):
-            value = data[i]
             result = result + _parse_form(
                 value, prefix + (f"{i}" if prefix == "" else f"[{i}]")
             )
     else:
-        dict = data.__dict__ if hasattr(data, "__dict__") else data
-        for key in dict.keys():
-            value = dict[key]
+        dictionary = data.__dict__ if hasattr(data, "__dict__") else data
+        for key in dictionary.keys():
+            value = dictionary[key]
             result = result + _parse_form(
                 value, prefix + (f"{key}" if prefix == "" else f"[{key}]")
             )
     return result
 
 
 def parse_form(data: Dict[str, Any]):
```

