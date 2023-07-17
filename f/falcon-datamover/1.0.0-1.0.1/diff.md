# Comparing `tmp/falcon-datamover-1.0.0.tar.gz` & `tmp/falcon-datamover-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/arif/falcon-pypi/dist/.tmp-6f4hsbcu/falcon-datamover-1.0.0.tar", last modified: Fri Jul  7 07:24:44 2023, max compression
+gzip compressed data, was "/home/arif/falcon-pypi/dist/.tmp-egd0p4ui/falcon-datamover-1.0.1.tar", last modified: Mon Jul 17 06:25:01 2023, max compression
```

## Comparing `falcon-datamover-1.0.0.tar` & `falcon-datamover-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 arif      (1003) arif      (1003)        0 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/
--rw-rw-r--   0 arif      (1003) arif      (1003)     1114 2023-07-07 04:23:35.000000 falcon-datamover-1.0.0/LICENSE
--rw-rw-r--   0 arif      (1003) arif      (1003)     3092 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/PKG-INFO
--rw-rw-r--   0 arif      (1003) arif      (1003)     1321 2023-07-07 07:21:05.000000 falcon-datamover-1.0.0/README.md
--rw-rw-r--   0 arif      (1003) arif      (1003)      939 2023-07-07 07:21:16.000000 falcon-datamover-1.0.0/pyproject.toml
--rw-rw-r--   0 arif      (1003) arif      (1003)       38 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/setup.cfg
--rw-rw-r--   0 arif      (1003) arif      (1003)       48 2023-07-07 07:20:14.000000 falcon-datamover-1.0.0/setup.py
-drwxrwxr-x   0 arif      (1003) arif      (1003)        0 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/src/
-drwxrwxr-x   0 arif      (1003) arif      (1003)        0 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/src/falcon/
--rw-rw-r--   0 arif      (1003) arif      (1003)       59 2023-07-07 04:20:46.000000 falcon-datamover-1.0.0/src/falcon/__init__.py
--rw-rw-r--   0 arif      (1003) arif      (1003)    12569 2023-07-07 06:42:56.000000 falcon-datamover-1.0.0/src/falcon/__main__.py
--rw-rw-r--   0 arif      (1003) arif      (1003)      593 2023-06-25 09:13:05.000000 falcon-datamover-1.0.0/src/falcon/configs.py
--rw-rw-r--   0 arif      (1003) arif      (1003)      422 2023-07-07 04:45:14.000000 falcon-datamover-1.0.0/src/falcon/logs.py
--rw-rw-r--   0 arif      (1003) arif      (1003)     9112 2023-05-25 22:49:33.000000 falcon-datamover-1.0.0/src/falcon/search.py
--rw-rw-r--   0 arif      (1003) arif      (1003)     1513 2023-06-25 08:57:50.000000 falcon-datamover-1.0.0/src/falcon/utils.py
-drwxrwxr-x   0 arif      (1003) arif      (1003)        0 2023-07-07 07:24:44.523732 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/
--rw-rw-r--   0 arif      (1003) arif      (1003)     3092 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1003) arif      (1003)      435 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1003) arif      (1003)        1 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1003) arif      (1003)       48 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1003) arif      (1003)      157 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/requires.txt
--rw-rw-r--   0 arif      (1003) arif      (1003)        7 2023-07-07 07:24:44.000000 falcon-datamover-1.0.0/src/falcon_datamover.egg-info/top_level.txt
+drwxrwxr-x   0 arif      (1005) arif      (1005)        0 2023-07-17 06:25:01.891791 falcon-datamover-1.0.1/
+-rw-rw-r--   0 arif      (1005) arif      (1005)     1114 2023-07-07 05:04:07.000000 falcon-datamover-1.0.1/LICENSE
+-rw-rw-r--   0 arif      (1005) arif      (1005)     3092 2023-07-17 06:25:01.891791 falcon-datamover-1.0.1/PKG-INFO
+-rw-rw-r--   0 arif      (1005) arif      (1005)     1321 2023-07-07 16:52:46.000000 falcon-datamover-1.0.1/README.md
+-rw-rw-r--   0 arif      (1005) arif      (1005)      939 2023-07-17 06:24:49.000000 falcon-datamover-1.0.1/pyproject.toml
+-rw-rw-r--   0 arif      (1005) arif      (1005)       38 2023-07-17 06:25:01.891791 falcon-datamover-1.0.1/setup.cfg
+-rw-rw-r--   0 arif      (1005) arif      (1005)       48 2023-07-07 16:52:46.000000 falcon-datamover-1.0.1/setup.py
+drwxrwxr-x   0 arif      (1005) arif      (1005)        0 2023-07-17 06:25:01.887791 falcon-datamover-1.0.1/src/
+drwxrwxr-x   0 arif      (1005) arif      (1005)        0 2023-07-17 06:25:01.887791 falcon-datamover-1.0.1/src/falcon/
+-rw-rw-r--   0 arif      (1005) arif      (1005)       59 2023-07-17 06:24:07.000000 falcon-datamover-1.0.1/src/falcon/__init__.py
+-rw-rw-r--   0 arif      (1005) arif      (1005)    12569 2023-07-17 06:07:06.000000 falcon-datamover-1.0.1/src/falcon/__main__.py
+-rw-rw-r--   0 arif      (1005) arif      (1005)      593 2023-07-07 05:04:07.000000 falcon-datamover-1.0.1/src/falcon/configs.py
+-rw-rw-r--   0 arif      (1005) arif      (1005)      422 2023-07-07 05:04:07.000000 falcon-datamover-1.0.1/src/falcon/logs.py
+-rw-rw-r--   0 arif      (1005) arif      (1005)     9112 2023-07-17 05:08:28.000000 falcon-datamover-1.0.1/src/falcon/search.py
+-rw-rw-r--   0 arif      (1005) arif      (1005)     1561 2023-07-17 06:16:12.000000 falcon-datamover-1.0.1/src/falcon/utils.py
+drwxrwxr-x   0 arif      (1005) arif      (1005)        0 2023-07-17 06:25:01.887791 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/
+-rw-rw-r--   0 arif      (1005) arif      (1005)     3092 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/PKG-INFO
+-rw-rw-r--   0 arif      (1005) arif      (1005)      435 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/SOURCES.txt
+-rw-rw-r--   0 arif      (1005) arif      (1005)        1 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/dependency_links.txt
+-rw-rw-r--   0 arif      (1005) arif      (1005)       48 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/entry_points.txt
+-rw-rw-r--   0 arif      (1005) arif      (1005)      157 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/requires.txt
+-rw-rw-r--   0 arif      (1005) arif      (1005)        7 2023-07-17 06:25:01.000000 falcon-datamover-1.0.1/src/falcon_datamover.egg-info/top_level.txt
```

### Comparing `falcon-datamover-1.0.0/LICENSE` & `falcon-datamover-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon-datamover-1.0.0/PKG-INFO` & `falcon-datamover-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-datamover
-Version: 1.0.0
+Version: 1.0.1
 Summary: Online File Transfer Optimization
 Author-email: Md Arifuzzaman <arif@nevada.unr.edu>
 License: MIT License
         
         Copyright (c) 2023 HIGH PERFORMANCE COMPUTING AND NETWORKING (HPCN) LAB, UNR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `falcon-datamover-1.0.0/README.md` & `falcon-datamover-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `falcon-datamover-1.0.0/pyproject.toml` & `falcon-datamover-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "falcon-datamover"
-version = "1.0.0"
+version = "1.0.1"
 description = "Online File Transfer Optimization"
 readme = "README.md"
 authors = [{ name = "Md Arifuzzaman", email = "arif@nevada.unr.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `falcon-datamover-1.0.0/src/falcon/__main__.py` & `falcon-datamover-1.0.1/src/falcon/__main__.py`

 * *Files identical despite different names*

### Comparing `falcon-datamover-1.0.0/src/falcon/configs.py` & `falcon-datamover-1.0.1/src/falcon/configs.py`

 * *Files identical despite different names*

### Comparing `falcon-datamover-1.0.0/src/falcon/search.py` & `falcon-datamover-1.0.1/src/falcon/search.py`

 * *Files identical despite different names*

### Comparing `falcon-datamover-1.0.0/src/falcon/utils.py` & `falcon-datamover-1.0.1/src/falcon/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,12 +43,13 @@
     def parse_files(self):
         root = self.configs["data_dir"]
         files = []
 
         if pathlib.Path(root).exists():
             root = root if root[-1] == "/" else root + "/"
 
-            for path in glob.glob(root + "**", recursive=True):
-                files.append(path.replace(root, ""))
+            for fpath in glob.glob(root + "**", recursive=True):
+                if os.path.isfile(fpath):
+                    files.append(fpath.replace(root, ""))
 
         return files
```

### Comparing `falcon-datamover-1.0.0/src/falcon_datamover.egg-info/PKG-INFO` & `falcon-datamover-1.0.1/src/falcon_datamover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-datamover
-Version: 1.0.0
+Version: 1.0.1
 Summary: Online File Transfer Optimization
 Author-email: Md Arifuzzaman <arif@nevada.unr.edu>
 License: MIT License
         
         Copyright (c) 2023 HIGH PERFORMANCE COMPUTING AND NETWORKING (HPCN) LAB, UNR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

