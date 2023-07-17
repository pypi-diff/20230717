# Comparing `tmp/ptlibs-0.0.6.tar.gz` & `tmp/ptlibs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptlibs-0.0.6.tar", last modified: Mon Mar 28 16:02:30 2022, max compression
+gzip compressed data, was "ptlibs-1.0.0.tar", last modified: Mon Jul 17 18:13:06 2023, max compression
```

## Comparing `ptlibs-0.0.6.tar` & `ptlibs-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:02:30.301841 ptlibs-0.0.6/
--rw-r--r--   0 kali      (1000) kali      (1000)     1508 2022-03-28 16:02:30.301841 ptlibs-0.0.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1168 2022-03-28 15:57:35.000000 ptlibs-0.0.6/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:02:30.301841 ptlibs-0.0.6/ptlibs/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:30.000000 ptlibs-0.0.6/ptlibs/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      785 2022-03-28 15:17:38.000000 ptlibs-0.0.6/ptlibs/ptdefs.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1233 2022-01-31 10:13:09.000000 ptlibs-0.0.6/ptlibs/ptjsonlib.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10233 2022-03-28 15:37:02.000000 ptlibs-0.0.6/ptlibs/ptmisclib.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:02:30.301841 ptlibs-0.0.6/ptlibs.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1508 2022-03-28 16:02:30.000000 ptlibs-0.0.6/ptlibs.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      243 2022-03-28 16:02:30.000000 ptlibs-0.0.6/ptlibs.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:02:30.000000 ptlibs-0.0.6/ptlibs.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2022-03-28 16:02:30.000000 ptlibs-0.0.6/ptlibs.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2022-03-28 16:02:30.000000 ptlibs-0.0.6/ptlibs.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:02:30.301841 ptlibs-0.0.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      661 2022-03-28 16:01:29.000000 ptlibs-0.0.6/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.803499 ptlibs-1.0.0/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    35149 2023-07-17 17:40:35.000000 ptlibs-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2442 2023-07-17 18:13:06.803499 ptlibs-1.0.0/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1880 2023-07-17 18:04:26.000000 ptlibs-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.799499 ptlibs-1.0.0/ptlibs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1115 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptcharsethelper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      753 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptdefs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4328 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptjsonlib.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6542 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptmisclib.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2096 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptnethelper.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5118 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptpathtypedetector.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5949 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/ptprinthelper.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.803499 ptlibs-1.0.0/ptlibs/threads/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1042 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/arraylock.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1316 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/printlock.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1783 2023-07-17 17:40:35.000000 ptlibs-1.0.0/ptlibs/threads/ptthreads.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-17 18:13:06.799499 ptlibs-1.0.0/ptlibs.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2442 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        7 2023-07-17 18:13:06.000000 ptlibs-1.0.0/ptlibs.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-17 18:13:06.803499 ptlibs-1.0.0/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      816 2023-07-17 17:42:13.000000 ptlibs-1.0.0/setup.py
```

### Comparing `ptlibs-0.0.6/PKG-INFO` & `ptlibs-1.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-Metadata-Version: 2.1
-Name: ptlibs
-Version: 0.0.6
-Summary: Support library for penterepTools
-Home-page: https://www.penterep.com/
-Author: Penterep
-Author-email: info@penterep.com
-License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
 
 # PTLIBS
 > Support library for penterepTools
 
 ## Installation
 ```
 pip install ptlibs
 ```
 
 ## Version History
 ```
+- 1.0.0
+    - Cookie redirect fix
+- 0.1.3
+    - ptpathtypedetector - get_type() method tweaks
+    - arraylock - new ThreadSafeArray class
+    - added windows support (for tools that do not use functions that depend on fcntl, termios libraries)
+- 0.1.2
+    - Unification with type hints changes
+- 0.1.1
+    - Cached requests are now saved into /tmp/pentereptools/
+    - Updated load_url_from_web_or_temp function
+    - Requests are now being saved along with parsed request and response objects as a string
+    - Other small changes to make ptscripts work properly
+- 0.0.7 - 0.1.0
+    - Unification with ptthreads
+    - Added type hints
+    - ptmisclib split into multiple classes
+    - Implemented parsing of url to nodes
 - 0.0.5 - 0.0.6
     - Implemented new printing method
-    - New 'WARNNING' definition added to ptdefs
+    - New 'WARNING' definition added to ptdefs
 - 0.0.4
     - removed 3rd party ipaddress module dependency
 - 0.0.3
     - Replaced some characters in ptdefs
     - Added new methods to ptmisclib
 - 0.0.1 - 0.0.2
     - Alpha releases
 ```
 
 ## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptlibs is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptlibs is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with ptlibs.  If not, see <https://www.gnu.org/licenses/>.
-
+along with ptlibs.  If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `ptlibs-0.0.6/setup.py` & `ptlibs-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="ptlibs",
-    description="Support library for penterepTools",
-    author="Penterep",
-    author_email="info@penterep.com",
-    url="https://www.penterep.com/",
-    version="0.0.6",
-    license="GPLv3+",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-    ],
-    python_requires = '>=3.6',
-    install_requires=["requests"],
-    long_description=long_description,
-    long_description_content_type="text/markdown"
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="ptlibs",
+    description="Support library for penterepTools",
+    author="Penterep",
+    author_email="info@penterep.com",
+    url="https://www.penterep.com/",
+    version="1.0.0",
+    license="GPLv3+",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
+    ],
+    python_requires = '>=3.6',
+    install_requires=["requests"],
+    long_description=long_description,
+    long_description_content_type="text/markdown"
 )
```

