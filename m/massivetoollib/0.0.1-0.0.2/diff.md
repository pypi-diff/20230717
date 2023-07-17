# Comparing `tmp/massivetoollib-0.0.1.tar.gz` & `tmp/massivetoollib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "massivetoollib-0.0.1.tar", last modified: Sat Jul 15 14:32:41 2023, max compression
+gzip compressed data, was "massivetoollib-0.0.2.tar", last modified: Mon Jul 17 20:28:08 2023, max compression
```

## Comparing `massivetoollib-0.0.1.tar` & `massivetoollib-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:32:41.519007 massivetoollib-0.0.1/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 massivetoollib-0.0.1/LICENCE
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:32:41.519007 massivetoollib-0.0.1/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 massivetoollib-0.0.1/README.md
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:32:41.519007 massivetoollib-0.0.1/massivetoollib/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       58 2023-07-15 14:02:24.000000 massivetoollib-0.0.1/massivetoollib/__init__.py
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      124 2023-07-15 13:37:34.000000 massivetoollib-0.0.1/massivetoollib/ang.py
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1265 2023-07-15 13:57:51.000000 massivetoollib-0.0.1/massivetoollib/numconvert.py
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:32:41.519007 massivetoollib-0.0.1/massivetoollib.egg-info/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:32:41.000000 massivetoollib-0.0.1/massivetoollib.egg-info/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      293 2023-07-15 14:32:41.000000 massivetoollib-0.0.1/massivetoollib.egg-info/SOURCES.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:32:41.000000 massivetoollib-0.0.1/massivetoollib.egg-info/dependency_links.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-15 14:32:41.000000 massivetoollib-0.0.1/massivetoollib.egg-info/requires.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       15 2023-07-15 14:32:41.000000 massivetoollib-0.0.1/massivetoollib.egg-info/top_level.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-15 14:32:41.519007 massivetoollib-0.0.1/setup.cfg
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1422 2023-07-15 14:31:50.000000 massivetoollib-0.0.1/setup.py
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-17 20:28:08.786182 massivetoollib-0.0.2/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 massivetoollib-0.0.2/LICENCE
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-17 20:28:08.786182 massivetoollib-0.0.2/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 massivetoollib-0.0.2/README.md
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-17 20:28:08.786182 massivetoollib-0.0.2/massivetoollib/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       34 2023-07-17 20:21:35.000000 massivetoollib-0.0.2/massivetoollib/__init__.py
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     9314 2023-07-17 20:20:56.000000 massivetoollib-0.0.2/massivetoollib/numconvert.py
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-17 20:28:08.786182 massivetoollib-0.0.2/massivetoollib.egg-info/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-17 20:28:08.000000 massivetoollib-0.0.2/massivetoollib.egg-info/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      271 2023-07-17 20:28:08.000000 massivetoollib-0.0.2/massivetoollib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-17 20:28:08.000000 massivetoollib-0.0.2/massivetoollib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-17 20:28:08.000000 massivetoollib-0.0.2/massivetoollib.egg-info/requires.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       15 2023-07-17 20:28:08.000000 massivetoollib-0.0.2/massivetoollib.egg-info/top_level.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-17 20:28:08.786182 massivetoollib-0.0.2/setup.cfg
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1413 2023-07-17 20:27:36.000000 massivetoollib-0.0.2/setup.py
```

### Comparing `massivetoollib-0.0.1/PKG-INFO` & `massivetoollib-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massivetoollib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

### Comparing `massivetoollib-0.0.1/massivetoollib.egg-info/PKG-INFO` & `massivetoollib-0.0.2/massivetoollib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massivetoollib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

### Comparing `massivetoollib-0.0.1/setup.py` & `massivetoollib-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 try:
     long_description = open("README.md").read()
 except IOError:
     long_description = ""
 
 setup(
     name="massivetoollib",
-    version="0.0.1",
+    version="0.0.2",
     description="A pip generic developer package",
     license="MIT",
     author="AngeloChDev",
     author_email="angeloch.dev@gmail.com",
     url="https://github.com/AngeloChDev",
     packages=find_packages(),
     test_suite='tests',
     install_requires=[
-        'requests>=2.25.0',
-        'fastecdsa>=2.2.1;platform_system!="Windows"',
-        'ecdsa>=0.17;platform_system=="Windows"',
-        'SQLAlchemy>=1.4.28',
-        'numpy==1.19.5;python_version<"3.8"',
-        'numpy>=1.21.0;python_version>="3.8"',
+         'requests>=2.25.0',
+      'fastecdsa>=2.2.1;platform_system!="Windows"',
+      'ecdsa>=0.17;platform_system=="Windows"',
+      'SQLAlchemy>=1.4.28',
+      'numpy==1.19.5;python_version<"3.8"',
+      'numpy>=1.21.0;python_version>="3.8"',
     ],
     long_description=long_description,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.10",
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

