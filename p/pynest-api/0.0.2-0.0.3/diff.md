# Comparing `tmp/pynest-api-0.0.2.tar.gz` & `tmp/pynest-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynest-api-0.0.2.tar", last modified: Wed Jun 28 10:53:43 2023, max compression
+gzip compressed data, was "pynest-api-0.0.3.tar", last modified: Mon Jul 17 15:44:44 2023, max compression
```

## Comparing `pynest-api-0.0.2.tar` & `pynest-api-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.213614 pynest-api-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-28 10:53:20.000000 pynest-api-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-28 10:53:43.213614 pynest-api-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-06-28 10:53:20.000000 pynest-api-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/cli/click_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/common/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/orm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/requierments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/common/templates/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/core/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/core/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/database/base_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/database/orm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/decorators/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/core/decorators/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.209614 pynest-api-0.0.2/nest/marketplace/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/marketplace/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.213614 pynest-api-0.0.2/nest/marketplace/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/marketplace/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.213614 pynest-api-0.0.2/nest/marketplace/modules/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/marketplace/modules/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.213614 pynest-api-0.0.2/nest/marketplace/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:20.000000 pynest-api-0.0.2/nest/marketplace/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:53:43.213614 pynest-api-0.0.2/pynest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-28 10:53:43.000000 pynest-api-0.0.2/pynest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-28 10:53:20.000000 pynest-api-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 10:53:43.213614 pynest-api-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 15:44:19.000000 pynest-api-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-17 15:44:44.670378 pynest-api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-17 15:44:19.000000 pynest-api-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/click_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/orm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/requierments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/core/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/base_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/orm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/modules/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/modules/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/pynest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 15:44:19.000000 pynest-api-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:44:44.670378 pynest-api-0.0.3/setup.cfg
```

### Comparing `pynest-api-0.0.2/LICENSE` & `pynest-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/PKG-INFO` & `pynest-api-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,17 +34,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# PyNest
+<p align="center">
+  <img src="docs/imgs/pynest_logo-modified.png" title="pynest logo" width="200">
+</p>
+<p align="center">
+    <em>PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS</em>
+</p>
+<p align="center">
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pynest-api?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/pynest-api.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
 
-PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS. It is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
+# PyNest - Description
+
+PyNest is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
 
 With PyNest, you can build scalable and maintainable APIs with ease. The framework supports dependency injection, type annotations, decorators, and code generation, making it easy to write clean and testable code.
 
 This framework is not a direct port of NestJS to Python but rather a re-imagining of the framework specifically for Python developers, including data scientists, data analysts, and data engineers. It aims to assist them in building better and faster APIs for their data applications.
 
 ## Getting Started
 To get started with PyNest, you'll need to install it using pip:
```

### Comparing `pynest-api-0.0.2/README.md` & `pynest-api-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-# PyNest
+<p align="center">
+  <img src="docs/imgs/pynest_logo-modified.png" title="pynest logo" width="200">
+</p>
+<p align="center">
+    <em>PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS</em>
+</p>
+<p align="center">
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pynest-api?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/pynest-api.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
 
-PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS. It is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
+# PyNest - Description
+
+PyNest is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
 
 With PyNest, you can build scalable and maintainable APIs with ease. The framework supports dependency injection, type annotations, decorators, and code generation, making it easy to write clean and testable code.
 
 This framework is not a direct port of NestJS to Python but rather a re-imagining of the framework specifically for Python developers, including data scientists, data analysts, and data engineers. It aims to assist them in building better and faster APIs for their data applications.
 
 ## Getting Started
 To get started with PyNest, you'll need to install it using pip:
```

### Comparing `pynest-api-0.0.2/nest/cli/cli.py` & `pynest-api-0.0.3/nest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/cli/click_handlers.py` & `pynest-api-0.0.3/nest/cli/click_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nest.common.templates.model import generate_model
 from nest.common.templates.app import generate_app
 from nest.common.templates.main import generate_main
 from nest.common.templates.orm_config import generate_orm_config
 from nest.common.templates.readme import generate_readme_template
 from nest.common.templates.requierments import generate_requirements
 from nest.common.templates.entity import generate_entity
+from nest.common.templates.dockerfile import generate_dockerfile
 
 
 def create_file(path: Path, content: str) -> None:
     """
     Create a file at the specified path with the given content.
 
     Args:
@@ -186,14 +187,28 @@
     Returns:
         None
     """
     entity_template = generate_entity(name)
     create_file(path, entity_template)
 
 
+def create_dockerfile(path: Path) -> None:
+    """
+    Create a Dockerfile file at the specified path using a template.
+
+    Args:
+        path (Path): The path to the Dockerfile file.
+
+    Returns:
+        None
+    """
+    dockerfile_template = generate_dockerfile()
+    create_file(path, dockerfile_template)
+
+
 def install_requirements(path: Path, db_type: str) -> None:
     os.chdir(path)
     subprocess.run("python -m venv venv && source venv/bin/activate", shell=True)
     subprocess.run(["python", "-m", "pip", "install", "--upgrade", "pip"])
     subprocess.run(["pip", "install", "-r", "requirements.txt"])
     if db_type == "mysql":
         subprocess.run(["pip", "install", "mysql-connector-python==8.0.33"])
@@ -265,14 +280,17 @@
     print("service created successfully")
     create_models(examples_path / "examples_model.py", "examples")
     print("model created successfully")
     create_entity(examples_path / "examples_entity.py", "examples")
     print("entity created successfully")
     create_module(examples_path / "examples_module.py", "examples")
     print("module created successfully")
+    if db_type == "sqlite":
+        create_dockerfile(root_path / "Dockerfile")
+        print("Dockerfile created successfully")
 
     time.sleep(1)
     print("Project created successfully")
 
 
 def find_target_folder(path, target="src"):
     """
```

### Comparing `pynest-api-0.0.2/nest/common/templates/controller.py` & `pynest-api-0.0.3/nest/common/templates/controller.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/common/templates/module.py` & `pynest-api-0.0.3/nest/common/templates/module.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/common/templates/orm_config.py` & `pynest-api-0.0.3/nest/common/templates/orm_config.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/common/templates/readme.py` & `pynest-api-0.0.3/nest/common/templates/readme.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/common/templates/service.py` & `pynest-api-0.0.3/nest/common/templates/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,18 @@
     capitalized_controller_name = "".join(
         [word.capitalize() for word in split_controller_name]
     )
     template = f"""from src.{controller_name}.{controller_name}_model import {capitalized_controller_name}
 from src.{controller_name}.{controller_name}_entity import {capitalized_controller_name} as {capitalized_controller_name}Entity
 from orm_config import config
 from nest.core.decorators import db_request_handler
+from functools import lru_cache
 
 
+@lru_cache()
 class {capitalized_controller_name}Service:
 
     def __init__(self):
         self.orm_config = config
         self.session = self.orm_config.get_db()
     
     @db_request_handler
```

### Comparing `pynest-api-0.0.2/nest/core/app.py` & `pynest-api-0.0.3/nest/core/app.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/core/database/base_orm.py` & `pynest-api-0.0.3/nest/core/database/base_orm.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/core/database/orm_config.py` & `pynest-api-0.0.3/nest/core/database/orm_config.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/core/decorators/controller.py` & `pynest-api-0.0.3/nest/core/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/nest/core/decorators/database.py` & `pynest-api-0.0.3/nest/core/decorators/database.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.2/pynest_api.egg-info/PKG-INFO` & `pynest-api-0.0.3/pynest_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,17 +34,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# PyNest
+<p align="center">
+  <img src="docs/imgs/pynest_logo-modified.png" title="pynest logo" width="200">
+</p>
+<p align="center">
+    <em>PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS</em>
+</p>
+<p align="center">
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pynest-api?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/pynest-api" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/pynest-api.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
 
-PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS. It is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
+# PyNest - Description
+
+PyNest is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
 
 With PyNest, you can build scalable and maintainable APIs with ease. The framework supports dependency injection, type annotations, decorators, and code generation, making it easy to write clean and testable code.
 
 This framework is not a direct port of NestJS to Python but rather a re-imagining of the framework specifically for Python developers, including data scientists, data analysts, and data engineers. It aims to assist them in building better and faster APIs for their data applications.
 
 ## Getting Started
 To get started with PyNest, you'll need to install it using pip:
```

### Comparing `pynest-api-0.0.2/pynest_api.egg-info/SOURCES.txt` & `pynest-api-0.0.3/pynest_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 nest/cli/cli.py
 nest/cli/click_handlers.py
 nest/common/__init__.py
 nest/common/common.py
 nest/common/templates/__init__.py
 nest/common/templates/app.py
 nest/common/templates/controller.py
+nest/common/templates/dockerfile.py
 nest/common/templates/entity.py
 nest/common/templates/main.py
 nest/common/templates/model.py
 nest/common/templates/module.py
 nest/common/templates/orm_config.py
 nest/common/templates/readme.py
 nest/common/templates/requierments.py
```

### Comparing `pynest-api-0.0.2/pyproject.toml` & `pynest-api-0.0.3/pyproject.toml`

 * *Files identical despite different names*

