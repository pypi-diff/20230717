# Comparing `tmp/dj-veryfi-0.1.5.tar.gz` & `tmp/dj-veryfi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-veryfi-0.1.5.tar", last modified: Sun Jul 16 00:40:47 2023, max compression
+gzip compressed data, was "dist/dj-veryfi-0.1.7.tar", last modified: Mon Jul 17 14:18:42 2023, max compression
```

## Comparing `dj-veryfi-0.1.5.tar` & `dj-veryfi-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/
--rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.5/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)       66 2023-07-16 00:30:32.000000 dj-veryfi-0.1.5/MANIFEST.in
--rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-16 00:08:30.000000 dj-veryfi-0.1.5/README
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      294 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/dj_veryfi.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.5/fields.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/migrations/
--rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.5/migrations/0001_initial.py
--rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.5/migrations/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.5/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:40:47.000000 dj-veryfi-0.1.5/setup.cfg
--rw-r--r--   0 tony      (1000) tony      (1000)       83 2023-07-16 00:10:10.000000 dj-veryfi-0.1.5/setup.py
--rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.5/veryfi.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.7/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     2883 2023-07-17 14:07:47.000000 dj-veryfi-0.1.7/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)      149 2023-07-15 18:29:43.000000 dj-veryfi-0.1.7/apps.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3501 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      312 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/requires.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       43 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/dj_veryfi.egg-info/top_level.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)     1758 2023-07-15 22:01:27.000000 dj-veryfi-0.1.7/fields.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/migrations/
+-rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.7/migrations/0001_initial.py
+-rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.7/migrations/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      235 2023-07-15 22:01:46.000000 dj-veryfi-0.1.7/models.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       86 2023-07-16 00:47:58.000000 dj-veryfi-0.1.7/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      697 2023-07-17 14:18:42.000000 dj-veryfi-0.1.7/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)      154 2023-07-17 14:17:27.000000 dj-veryfi-0.1.7/setup.py
+-rw-r--r--   0 tony      (1000) tony      (1000)     2063 2023-07-15 22:03:59.000000 dj-veryfi-0.1.7/tests.py
+-rw-r--r--   0 tony      (1000) tony      (1000)      398 2023-07-15 18:33:52.000000 dj-veryfi-0.1.7/veryfi.py
```

### Comparing `dj-veryfi-0.1.5/LICENSE` & `dj-veryfi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.5/PKG-INFO` & `dj-veryfi-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.5
+Version: 0.1.7
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -50,15 +50,15 @@
     VERYFI_CLIENT_ID = "Your client ID"
     VERYFI_CLIENT_SECRET = "Your client secret"
     VERYFI_USERNAME = "Your username"
     VERYFI_API_KEY = "Your api key"
 
 
 ## Usage
-Once you have a django project, dj-veryfi installed and setedup, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
+Once you have a django project, dj-veryfi installed and set up, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
    
     from django.db import models
     from dj_veryfi.fields import OCRInvoiceOrReceiptField
     
     class Document(models.Model):
         created_at = models.Datetime.FIeld(auto_now_add=True)
         name = models.CharFied(max_length=100)
```

### Comparing `dj-veryfi-0.1.5/README` & `dj-veryfi-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     VERYFI_CLIENT_ID = "Your client ID"
     VERYFI_CLIENT_SECRET = "Your client secret"
     VERYFI_USERNAME = "Your username"
     VERYFI_API_KEY = "Your api key"
 
 
 ## Usage
-Once you have a django project, dj-veryfi installed and setedup, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
+Once you have a django project, dj-veryfi installed and set up, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
    
     from django.db import models
     from dj_veryfi.fields import OCRInvoiceOrReceiptField
     
     class Document(models.Model):
         created_at = models.Datetime.FIeld(auto_now_add=True)
         name = models.CharFied(max_length=100)
```

### Comparing `dj-veryfi-0.1.5/dj_veryfi.egg-info/PKG-INFO` & `dj-veryfi-0.1.7/dj_veryfi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-veryfi
-Version: 0.1.5
+Version: 0.1.7
 Summary: Django integration for Veryfi OCR API.
 Home-page: https://github.com/tonykamillo/dj-veryfi
 Author: Tony Kamillo
 Author-email: tonykamillo@gmail.com
 License: DBAD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -50,15 +50,15 @@
     VERYFI_CLIENT_ID = "Your client ID"
     VERYFI_CLIENT_SECRET = "Your client secret"
     VERYFI_USERNAME = "Your username"
     VERYFI_API_KEY = "Your api key"
 
 
 ## Usage
-Once you have a django project, dj-veryfi installed and setedup, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
+Once you have a django project, dj-veryfi installed and set up, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
    
     from django.db import models
     from dj_veryfi.fields import OCRInvoiceOrReceiptField
     
     class Document(models.Model):
         created_at = models.Datetime.FIeld(auto_now_add=True)
         name = models.CharFied(max_length=100)
```

### Comparing `dj-veryfi-0.1.5/fields.py` & `dj-veryfi-0.1.7/fields.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.5/migrations/0001_initial.py` & `dj-veryfi-0.1.7/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.5/setup.cfg` & `dj-veryfi-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = dj-veryfi
-version = 0.1.5
+version = 0.1.7
 description = Django integration for Veryfi OCR API.
-long_description = file: README
+long_description = file: README.md
 url = https://github.com/tonykamillo/dj-veryfi
 author = Tony Kamillo
 author_email = tonykamillo@gmail.com
 license = DBAD
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

