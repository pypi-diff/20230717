# Comparing `tmp/platform-library-0.2.0.tar.gz` & `tmp/platform-library-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.2.0.tar", last modified: Mon Jul 17 11:54:03 2023, max compression
+gzip compressed data, was "platform-library-0.3.0.tar", last modified: Mon Jul 17 13:07:53 2023, max compression
```

## Comparing `platform-library-0.2.0.tar` & `platform-library-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,28 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.184117 platform-library-0.2.0/
--rw-r--r--   0 Artyom     (501) staff       (20)     1072 2023-07-17 10:23:17.000000 platform-library-0.2.0/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 11:54:03.183992 platform-library-0.2.0/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.2.0/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.2.0/README.md
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.181265 platform-library-0.2.0/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 11:54:03.000000 platform-library-0.2.0/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      813 2023-07-17 11:54:03.000000 platform-library-0.2.0/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-07-17 11:54:03.000000 platform-library-0.2.0/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-07-17 11:54:03.000000 platform-library-0.2.0/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       14 2023-07-17 11:54:03.000000 platform-library-0.2.0/platform_library.egg-info/top_level.txt
--rw-r--r--   0 Artyom     (501) staff       (20)      641 2023-07-17 11:53:38.000000 platform-library-0.2.0/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-07-17 11:54:03.184157 platform-library-0.2.0/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.179890 platform-library-0.2.0/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.180076 platform-library-0.2.0/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.181715 platform-library-0.2.0/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.2.0/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.2.0/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.2.0/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.2.0/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.182149 platform-library-0.2.0/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.2.0/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.2.0/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.2.0/src/plib/licensing/exceptions.py
--rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.2.0/src/plib/licensing/models.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.182397 platform-library-0.2.0/src/plib/tracing/
--rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.2.0/src/plib/tracing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.2.0/src/plib/tracing/utils.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.180190 platform-library-0.2.0/venv/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 11:54:03.183841 platform-library-0.2.0/venv/bin/
--rw-r--r--   0 Artyom     (501) staff       (20)     1175 2023-03-06 07:38:00.000000 platform-library-0.2.0/venv/bin/activate_this.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      637 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2html.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      759 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)     1104 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      836 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      659 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2man.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      825 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)     1763 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      644 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      680 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      916 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      645 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 Artyom     (501) staff       (20)      713 2023-03-06 07:40:47.000000 platform-library-0.2.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.437466 platform-library-0.3.0/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1072 2023-07-17 10:23:17.000000 platform-library-0.3.0/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 13:07:53.437345 platform-library-0.3.0/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.3.0/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.3.0/README.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      632 2023-07-17 13:03:12.000000 platform-library-0.3.0/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-07-17 13:07:53.437506 platform-library-0.3.0/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.434660 platform-library-0.3.0/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.435840 platform-library-0.3.0/src/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 13:07:53.000000 platform-library-0.3.0/src/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      538 2023-07-17 13:07:53.000000 platform-library-0.3.0/src/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-07-17 13:07:53.000000 platform-library-0.3.0/src/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-07-17 13:07:53.000000 platform-library-0.3.0/src/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-07-17 13:07:53.000000 platform-library-0.3.0/src/platform_library.egg-info/top_level.txt
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.434852 platform-library-0.3.0/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.436260 platform-library-0.3.0/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.3.0/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.3.0/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.3.0/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.3.0/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.436952 platform-library-0.3.0/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.3.0/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.3.0/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.3.0/src/plib/licensing/exceptions.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.3.0/src/plib/licensing/models.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 13:07:53.437190 platform-library-0.3.0/src/plib/tracing/
+-rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.3.0/src/plib/tracing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.3.0/src/plib/tracing/utils.py
```

### Comparing `platform-library-0.2.0/LICENSE` & `platform-library-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/PKG-INFO` & `platform-library-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library for easy developing Platform
 Author: Artyom Vakilov
 License: MIT License
         
         Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.2.0/README.md` & `platform-library-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/platform_library.egg-info/PKG-INFO` & `platform-library-0.3.0/src/platform_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library for easy developing Platform
 Author: Artyom Vakilov
 License: MIT License
         
         Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.2.0/pyproject.toml` & `platform-library-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "platform-library"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Artyom Vakilov" },
 ]
 
 description = "A library for easy developing Platform"
 readme = "README-public.md"
 license = { file="LICENSE" }
@@ -21,9 +21,9 @@
 
 dependencies = [
     "PyJWT == 2.7.0",
     "requests == 2.31.0",
     "opentelemetry-exporter-otlp == 1.19.0"
 ]
 
-[tool.setuptools.packages.find]
-exclude = ["README.md"]
+[tool.setuptools]
+include-package-data = false
```

### Comparing `platform-library-0.2.0/src/plib/auth/encrypt.py` & `platform-library-0.3.0/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/src/plib/auth/o2auth.py` & `platform-library-0.3.0/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/src/plib/licensing/api.py` & `platform-library-0.3.0/src/plib/licensing/api.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/src/plib/licensing/exceptions.py` & `platform-library-0.3.0/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/src/plib/tracing/__init__.py` & `platform-library-0.3.0/src/plib/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.2.0/src/plib/tracing/utils.py` & `platform-library-0.3.0/src/plib/tracing/utils.py`

 * *Files identical despite different names*

