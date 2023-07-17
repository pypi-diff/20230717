# Comparing `tmp/requestsbankrko-0.2.3.tar.gz` & `tmp/requestsbankrko-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.3.tar", last modified: Mon Jul 17 07:41:13 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.4.tar", last modified: Mon Jul 17 11:16:14 2023, max compression
```

## Comparing `requestsbankrko-0.2.3.tar` & `requestsbankrko-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29033 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 07:41:13.000000 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 07:41:13.000000 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:41:13.000000 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 07:41:13.000000 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 07:41:13.000000 requestsbankrko-0.2.3/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:41:13.075205 requestsbankrko-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    56956 2023-07-17 07:41:04.000000 requestsbankrko-0.2.3/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 11:16:14.000000 requestsbankrko-0.2.4/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:16:14.082993 requestsbankrko-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56956 2023-07-17 11:16:04.000000 requestsbankrko-0.2.4/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.3/LICENSE` & `requestsbankrko-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.3/PKG-INFO` & `requestsbankrko-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.3
+Version: 0.2.4
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.3/pyproject.toml` & `requestsbankrko-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.3"
+version = "0.2.4"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.3/src/bank_methods.py` & `requestsbankrko-0.2.4/src/bank_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,15 +849,15 @@
     base_url_test = 'https://api-billy-crm.testkontur.ru/'
 
 
     def __init__(self, json, test):
         super().__init__()
         self.test = test
         self.json = json
-        self.headers = {'x-Auth-CustomToken': os.environ.get('kontur_token')}
+        self.headers = {'x-Auth-CustomToken': os.environ.get('kontur_token_test') if test else os.environ.get('kontur_token_prod')}
 
     def do_json(self):
         self.prospective_sale_id = self.response_json.get('ProspectiveSaleId')
         if self.prospective_sale_id is not None:
             self.success = True
             return self.suc_resp()
         results = self.response_json.get('Results')
```

### Comparing `requestsbankrko-0.2.3/src/open_methods.py` & `requestsbankrko-0.2.4/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.3/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.4/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.3
+Version: 0.2.4
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.3/src/zip_functions.py` & `requestsbankrko-0.2.4/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.3/tests/test_bank_methods.py` & `requestsbankrko-0.2.4/tests/test_bank_methods.py`

 * *Files identical despite different names*

