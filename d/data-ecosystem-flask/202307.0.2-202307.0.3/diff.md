# Comparing `tmp/data_ecosystem_flask-202307.0.2.tar.gz` & `tmp/data_ecosystem_flask-202307.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202307.0.2.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202307.0.3.tar", max compression
```

## Comparing `data_ecosystem_flask-202307.0.2.tar` & `data_ecosystem_flask-202307.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      863 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0     1155 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/__init__.py
--rw-r--r--   0        0        0    41602 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    13216 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0    28571 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0     2082 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0    16945 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0     1572 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/download.html
--rw-r--r--   0        0        0      432 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/error.html
--rw-r--r--   0        0        0     2723 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0     1905 2023-07-17 03:03:08.472189 data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/upload.html
--rw-r--r--   0        0        0    11357 2023-07-17 03:03:08.516189 data_ecosystem_flask-202307.0.2/license.md
--rw-r--r--   0        0        0     2559 2023-07-17 03:09:37.323715 data_ecosystem_flask-202307.0.2/pyproject.toml
--rw-r--r--   0        0        0    15040 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/readme.md
--rw-r--r--   0        0        0      126 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-17 03:03:08.520189 data_ecosystem_flask-202307.0.2/setup.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.2/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0     1155 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/__init__.py
+-rw-r--r--   0        0        0    41602 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    13216 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0    28571 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0    16945 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0     1572 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/download.html
+-rw-r--r--   0        0        0      432 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0     1905 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/upload.html
+-rw-r--r--   0        0        0    11357 2023-07-17 03:11:53.333704 data_ecosystem_flask-202307.0.3/license.md
+-rw-r--r--   0        0        0     2559 2023-07-17 03:18:42.623935 data_ecosystem_flask-202307.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15040 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/readme.md
+-rw-r--r--   0        0        0      126 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.3/PKG-INFO
```

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/__init__.py` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app_startup.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/download.html` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/download.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/log_file.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/data_ecosystem_flask/templates/upload.html` & `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/upload.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/license.md` & `data_ecosystem_flask-202307.0.3/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/pyproject.toml` & `data_ecosystem_flask-202307.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202307.0.2"
+version="202307.0.3"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `data_ecosystem_flask-202307.0.2/readme.md` & `data_ecosystem_flask-202307.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.2/PKG-INFO` & `data_ecosystem_flask-202307.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202307.0.2
+Version: 202307.0.3
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

