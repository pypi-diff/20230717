# Comparing `tmp/repomanager-1.6.0.tar.gz` & `tmp/repomanager-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/repomanager-1.6.0.tar", last modified: Mon Feb  6 11:26:30 2023, max compression
+gzip compressed data, was "dist/repomanager-1.7.0.tar", last modified: Mon Jul 17 04:53:07 2023, max compression
```

## Comparing `repomanager-1.6.0.tar` & `repomanager-1.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     2322 2022-10-08 13:09:38.000000 repomanager-1.6.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     1530 2022-10-08 13:09:38.000000 repomanager-1.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-10-08 13:09:38.000000 repomanager-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2023-02-06 11:26:30.000000 repomanager-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-10-08 13:09:38.000000 repomanager-1.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1211 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     6076 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2323 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/docs/source/diagrams/
--rw-rw-rw-   0 root         (0) root         (0)    21845 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/diagrams/git_flow.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     2044 2022-10-08 13:09:38.000000 repomanager-1.6.0/docs/source/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-02-06 11:25:39.000000 repomanager-1.6.0/repomanager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-02-06 11:25:39.000000 repomanager-1.6.0/repomanager/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2022-10-08 13:09:38.000000 repomanager-1.6.0/repomanager/log.py
--rwxrwxrwx   0 root         (0) root         (0)     1141 2022-10-08 13:09:38.000000 repomanager-1.6.0/repomanager/main.py
--rw-rw-rw-   0 root         (0) root         (0)     5434 2023-02-06 11:25:39.000000 repomanager-1.6.0/repomanager/rpm.py
--rw-rw-rw-   0 root         (0) root         (0)    12776 2022-10-08 13:09:38.000000 repomanager-1.6.0/repomanager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-06 11:26:30.000000 repomanager-1.6.0/repomanager.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-06 11:26:30.000000 repomanager-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-10-08 13:09:38.000000 repomanager-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 11:26:30.000000 repomanager-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/aapg.patch
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/error.yaml
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repo_commit.yaml
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repo_master.yaml
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repo_nopatch.yaml
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repo_submodule.yaml
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repolist.yaml
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/repolist1.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2250 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/test_repomanager.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2022-10-08 13:09:38.000000 repomanager-1.6.0/tests/verif.patch
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-07-17 04:52:33.000000 repomanager-1.7.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-07-17 04:52:33.000000 repomanager-1.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-17 04:52:33.000000 repomanager-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-17 04:53:07.000000 repomanager-1.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-07-17 04:52:33.000000 repomanager-1.7.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6076 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/docs/source/diagrams/
+-rw-rw-rw-   0 root         (0) root         (0)    21845 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/diagrams/git_flow.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-17 04:52:33.000000 repomanager-1.7.0/docs/source/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/log.py
+-rwxrwxrwx   0 root         (0) root         (0)     1141 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5434 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/rpm.py
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-17 04:52:33.000000 repomanager-1.7.0/repomanager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 04:53:07.000000 repomanager-1.7.0/repomanager.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-17 04:53:07.000000 repomanager-1.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-17 04:52:33.000000 repomanager-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:53:07.000000 repomanager-1.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 04:53:03.000000 repomanager-1.7.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/aapg.patch
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/error.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repo_commit.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repo_master.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repo_nopatch.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repo_submodule.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repolist.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/repolist1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/test_repomanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-17 04:52:33.000000 repomanager-1.7.0/tests/verif.patch
```

### Comparing `repomanager-1.6.0/CONTRIBUTING.rst` & `repomanager-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/LICENSE` & `repomanager-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/Makefile` & `repomanager-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/source/conf.py` & `repomanager-1.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/source/contributing.rst` & `repomanager-1.7.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/source/diagrams/git_flow.png` & `repomanager-1.7.0/docs/source/diagrams/git_flow.png`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/source/installation.rst` & `repomanager-1.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/docs/source/usage.rst` & `repomanager-1.7.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager/constants.py` & `repomanager-1.7.0/repomanager/constants.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager/log.py` & `repomanager-1.7.0/repomanager/log.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager/main.py` & `repomanager-1.7.0/repomanager/main.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager/rpm.py` & `repomanager-1.7.0/repomanager/rpm.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager/utils.py` & `repomanager-1.7.0/repomanager/utils.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/repomanager.egg-info/SOURCES.txt` & `repomanager-1.7.0/repomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/setup.py` & `repomanager-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import codecs
-import pip
 from setuptools import setup, find_packages
 
 import repomanager
 
 # Base directory of package
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `repomanager-1.6.0/tests/test_repomanager.py` & `repomanager-1.7.0/tests/test_repomanager.py`

 * *Files identical despite different names*

### Comparing `repomanager-1.6.0/tests/verif.patch` & `repomanager-1.7.0/tests/verif.patch`

 * *Files identical despite different names*

