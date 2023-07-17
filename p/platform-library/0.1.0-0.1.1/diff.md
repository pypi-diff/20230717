# Comparing `tmp/platform-library-0.1.0.tar.gz` & `tmp/platform-library-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.1.0.tar", last modified: Thu Jun 15 08:23:56 2023, max compression
+gzip compressed data, was "platform-library-0.1.1.tar", last modified: Mon Jul 17 10:25:13 2023, max compression
```

## Comparing `platform-library-0.1.0.tar` & `platform-library-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.639548 platform-library-0.1.0/
--rw-r--r--   0 Artyom     (501) staff       (20)     1078 2023-05-17 10:19:03.000000 platform-library-0.1.0/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-06-15 08:23:56.639375 platform-library-0.1.0/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.1.0/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.1.0/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      620 2023-06-15 08:23:21.000000 platform-library-0.1.0/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-06-15 08:23:56.639608 platform-library-0.1.0/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.635114 platform-library-0.1.0/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.636776 platform-library-0.1.0/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-06-15 08:23:56.000000 platform-library-0.1.0/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      538 2023-06-15 08:23:56.000000 platform-library-0.1.0/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-06-15 08:23:56.000000 platform-library-0.1.0/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-06-15 08:23:56.000000 platform-library-0.1.0/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-06-15 08:23:56.000000 platform-library-0.1.0/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.635307 platform-library-0.1.0/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.637523 platform-library-0.1.0/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.1.0/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.1.0/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.1.0/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.1.0/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.638584 platform-library-0.1.0/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.1.0/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.1.0/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.1.0/src/plib/licensing/exceptions.py
--rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.1.0/src/plib/licensing/models.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-06-15 08:23:56.638990 platform-library-0.1.0/src/plib/tracing/
--rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.1.0/src/plib/tracing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.1.0/src/plib/tracing/utils.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.305067 platform-library-0.1.1/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1072 2023-07-17 10:23:17.000000 platform-library-0.1.1/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:25:13.304948 platform-library-0.1.1/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.1.1/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.1.1/README.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      585 2023-07-17 10:24:50.000000 platform-library-0.1.1/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-07-17 10:25:13.305107 platform-library-0.1.1/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.301920 platform-library-0.1.1/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.303310 platform-library-0.1.1/src/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1656 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      538 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       66 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-07-17 10:25:13.000000 platform-library-0.1.1/src/platform_library.egg-info/top_level.txt
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.302102 platform-library-0.1.1/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.303975 platform-library-0.1.1/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.1.1/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.304425 platform-library-0.1.1/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.1.1/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4714 2023-06-02 08:23:17.000000 platform-library-0.1.1/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.1.1/src/plib/licensing/exceptions.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      134 2023-06-02 08:23:17.000000 platform-library-0.1.1/src/plib/licensing/models.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-07-17 10:25:13.304657 platform-library-0.1.1/src/plib/tracing/
+-rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.1.1/src/plib/tracing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.1.1/src/plib/tracing/utils.py
```

### Comparing `platform-library-0.1.0/LICENSE` & `platform-library-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 3DiVi Platform Library
+Copyright (c) 2023 Platform Library
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.1.0/PKG-INFO` & `platform-library-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.1.0
-Summary: A library for easy developing 3DiVi Platform
-Author-email: Artyom Vakilov <a.vakilov@3divi.com>
+Version: 0.1.1
+Summary: A library for easy developing Platform
+Author: Artyom Vakilov
 License: MIT License
         
-        Copyright (c) 2023 3DiVi Platform Library
+        Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.1.0/README.md` & `platform-library-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.1.1/src/platform_library.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.1.0
-Summary: A library for easy developing 3DiVi Platform
-Author-email: Artyom Vakilov <a.vakilov@3divi.com>
+Version: 0.1.1
+Summary: A library for easy developing Platform
+Author: Artyom Vakilov
 License: MIT License
         
-        Copyright (c) 2023 3DiVi Platform Library
+        Copyright (c) 2023 Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.1.0/src/platform_library.egg-info/SOURCES.txt` & `platform-library-0.1.1/src/platform_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/auth/encrypt.py` & `platform-library-0.1.1/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/auth/o2auth.py` & `platform-library-0.1.1/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/licensing/api.py` & `platform-library-0.1.1/src/plib/licensing/api.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/licensing/exceptions.py` & `platform-library-0.1.1/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/tracing/__init__.py` & `platform-library-0.1.1/src/plib/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.1.0/src/plib/tracing/utils.py` & `platform-library-0.1.1/src/plib/tracing/utils.py`

 * *Files identical despite different names*

