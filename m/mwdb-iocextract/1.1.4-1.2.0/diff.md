# Comparing `tmp/mwdb-iocextract-1.1.4.tar.gz` & `tmp/mwdb-iocextract-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwdb-iocextract-1.1.4.tar", last modified: Mon Jul 17 12:04:06 2023, max compression
+gzip compressed data, was "mwdb-iocextract-1.2.0.tar", last modified: Mon Jul 17 13:01:33 2023, max compression
```

## Comparing `mwdb-iocextract-1.1.4.tar` & `mwdb-iocextract-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/
--rw-r--r--   0 root         (0) root         (0)     7100 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7100 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      334 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 12:04:06.000000 mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 12:04:06.459832 mwdb-iocextract-1.1.4/src/
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/api.py
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/errors.py
--rw-r--r--   0 root         (0) root         (0)    12444 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/src/model.py
--rw-r--r--   0 root         (0) root         (0)    12160 2023-07-17 12:02:11.000000 mwdb-iocextract-1.1.4/src/modules.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/run.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-07-13 12:15:28.000000 mwdb-iocextract-1.1.4/src/test_misp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     7109 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.892171 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7109 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      765 2023-07-17 12:43:41.000000 mwdb-iocextract-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/src/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/api.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12444 2023-07-17 12:02:11.000000 mwdb-iocextract-1.2.0/src/model.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2023-07-17 12:02:11.000000 mwdb-iocextract-1.2.0/src/modules.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/run.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/test_misp.py
```

### Comparing `mwdb-iocextract-1.1.4/PKG-INFO` & `mwdb-iocextract-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.1.4
+Version: 1.2.0
 Summary: Mwdb config parser
 Home-page: UNKNOWN
-Author: msm
-Author-email: msm@cert.pl
+Author: CERT Polska
+Author-email: info@cert.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mwdb-iocextract-1.1.4/README.md` & `mwdb-iocextract-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.4/mwdb_iocextract.egg-info/PKG-INFO` & `mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.1.4
+Version: 1.2.0
 Summary: Mwdb config parser
 Home-page: UNKNOWN
-Author: msm
-Author-email: msm@cert.pl
+Author: CERT Polska
+Author-email: info@cert.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mwdb-iocextract-1.1.4/setup.py` & `mwdb-iocextract-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,18 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().split('\n')
 
 setuptools.setup(
     name="mwdb-iocextract",
-    version="1.1.4",
-    author="msm",
-    author_email="msm@cert.pl",
+    version="1.2.0",
+    data_files=[('requirements.txt', ['requirements.txt'])],
+    author="CERT Polska",
+    author_email="info@cert.pl",
     package_dir={"mwdb_iocextract": "src"},
     packages=["mwdb_iocextract"],
     description="Mwdb config parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     classifiers=[
```

### Comparing `mwdb-iocextract-1.1.4/src/model.py` & `mwdb-iocextract-1.2.0/src/model.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.4/src/modules.py` & `mwdb-iocextract-1.2.0/src/modules.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.4/src/run.py` & `mwdb-iocextract-1.2.0/src/run.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.1.4/src/test_misp.py` & `mwdb-iocextract-1.2.0/src/test_misp.py`

 * *Files identical despite different names*

