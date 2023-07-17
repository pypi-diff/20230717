# Comparing `tmp/platform-library-0.1.1.tar.gz` & `tmp/platform-library-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.1.1.tar", last modified: Mon Jul 17 10:25:13 2023, max compression
+gzip compressed data, was "platform-library-0.1.2.tar", last modified: Mon Jul 17 10:53:48 2023, max compression
```

## Comparing `platform-library-0.1.1.tar` & `platform-library-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,43 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.305067 platform-library-0.1.1/
--rw-r--r--   0 Artyom     (501) staff       (20)     1072 2023-07-17 10:23:17.000000 platform-library-0.1.1/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:25:13.304948 platform-library-0.1.1/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.1.1/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.1.1/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      585 2023-07-17 10:24:50.000000 platform-library-0.1.1/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-07-17 10:25:13.305107 platform-library-0.1.1/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.301920 platform-library-0.1.1/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.303310 platform-library-0.1.1/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      538 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.302102 platform-library-0.1.1/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.303975 platform-library-0.1.1/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.304425 platform-library-0.1.1/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.1.1/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.1.1/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.1.1/src/plib/licensing/exceptions.py
--rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.1.1/src/plib/licensing/models.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.304657 platform-library-0.1.1/src/plib/tracing/
--rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.1.1/src/plib/tracing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.1.1/src/plib/tracing/utils.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.845278 platform-library-0.1.2/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1072 2023-07-17 10:23:17.000000 platform-library-0.1.2/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:53:48.845125 platform-library-0.1.2/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.1.2/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.1.2/README.md
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.840504 platform-library-0.1.2/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:53:48.000000 platform-library-0.1.2/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      813 2023-07-17 10:53:48.000000 platform-library-0.1.2/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-07-17 10:53:48.000000 platform-library-0.1.2/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-07-17 10:53:48.000000 platform-library-0.1.2/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       14 2023-07-17 10:53:48.000000 platform-library-0.1.2/platform_library.egg-info/top_level.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)      641 2023-07-17 10:53:44.000000 platform-library-0.1.2/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-07-17 10:53:48.845325 platform-library-0.1.2/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.839013 platform-library-0.1.2/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.839207 platform-library-0.1.2/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.840935 platform-library-0.1.2/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.1.2/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.1.2/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.1.2/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.1.2/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.841357 platform-library-0.1.2/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.1.2/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.1.2/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.1.2/src/plib/licensing/exceptions.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.1.2/src/plib/licensing/models.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.841569 platform-library-0.1.2/src/plib/tracing/
+-rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.1.2/src/plib/tracing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.1.2/src/plib/tracing/utils.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.839324 platform-library-0.1.2/venv/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:53:48.844848 platform-library-0.1.2/venv/bin/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1175 2023-03-06 07:38:00.000000 platform-library-0.1.2/venv/bin/activate_this.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      637 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      759 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)     1104 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      836 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      659 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      825 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)     1763 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      644 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      680 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      916 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      645 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 Artyom     (501) staff       (20)      713 2023-03-06 07:40:47.000000 platform-library-0.1.2/venv/bin/rstpep2html.py
```

### Comparing `platform-library-0.1.1/LICENSE` & `platform-library-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/PKG-INFO` & `platform-library-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for easy developing Platform
 Author: Artyom Vakilov
 License: MIT License
         
         Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.1.1/README.md` & `platform-library-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.1.2/platform_library.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for easy developing Platform
 Author: Artyom Vakilov
 License: MIT License
         
         Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `platform-library-0.1.1/src/plib/auth/encrypt.py` & `platform-library-0.1.2/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/plib/auth/o2auth.py` & `platform-library-0.1.2/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/plib/licensing/api.py` & `platform-library-0.1.2/src/plib/licensing/api.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/plib/licensing/exceptions.py` & `platform-library-0.1.2/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/plib/tracing/__init__.py` & `platform-library-0.1.2/src/plib/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.1/src/plib/tracing/utils.py` & `platform-library-0.1.2/src/plib/tracing/utils.py`

 * *Files identical despite different names*

