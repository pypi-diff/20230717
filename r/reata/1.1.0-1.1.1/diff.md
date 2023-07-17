# Comparing `tmp/reata-1.1.0.tar.gz` & `tmp/reata-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reata-1.1.0.tar", last modified: Mon Jul 17 00:37:57 2023, max compression
+gzip compressed data, was "reata-1.1.1.tar", last modified: Mon Jul 17 01:02:26 2023, max compression
```

## Comparing `reata-1.1.0.tar` & `reata-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 00:37:57.000000 reata-1.1.0/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.0/LICENSE
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-17 00:37:57.000000 reata-1.1.0/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.0/README.rst
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 00:37:57.000000 reata-1.1.0/reata/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     5832 2023-07-17 00:32:20.000000 reata-1.1.0/reata/__futures__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.0/reata/__init__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-04-13 02:09:12.000000 reata-1.1.0/reata/client.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.0/reata/schema.py
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/SOURCES.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/dependency_links.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       42 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/requires.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-07-17 00:37:57.000000 reata-1.1.0/reata.egg-info/top_level.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-07-17 00:37:57.000000 reata-1.1.0/setup.cfg
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      557 2023-07-17 00:34:17.000000 reata-1.1.0/setup.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 01:02:26.000000 reata-1.1.1/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.1/LICENSE
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-17 01:02:26.000000 reata-1.1.1/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.1/README.rst
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 01:02:26.000000 reata-1.1.1/reata/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     5709 2023-07-17 00:59:31.000000 reata-1.1.1/reata/__futures__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.1/reata/__init__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-04-13 02:09:12.000000 reata-1.1.1/reata/client.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.1/reata/schema.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/SOURCES.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/dependency_links.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       42 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/requires.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-07-17 01:02:26.000000 reata-1.1.1/reata.egg-info/top_level.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-07-17 01:02:26.000000 reata-1.1.1/setup.cfg
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      557 2023-07-17 01:00:55.000000 reata-1.1.1/setup.py
```

### Comparing `reata-1.1.0/LICENSE` & `reata-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reata-1.1.0/PKG-INFO` & `reata-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.0/README.rst` & `reata-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `reata-1.1.0/reata/__futures__.py` & `reata-1.1.1/reata/__futures__.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,17 +249,7 @@
         super().__init__(*args, **kwargs)
 
 
 class TIMESTAMP(BaseDataType):
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-
-
-
-
-
-if __name__ == "__main__":
-    # x = DECIMAL(10, 2, "NOT NULL")
-    # print(x)
-    # print(x.effective_size)
-    pass
```

### Comparing `reata-1.1.0/reata/client.py` & `reata-1.1.1/reata/client.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.0/reata/schema.py` & `reata-1.1.1/reata/schema.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.0/reata.egg-info/PKG-INFO` & `reata-1.1.1/reata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.0/setup.py` & `reata-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 src = Path(__file__).parent
 
 setup(
     name="reata",
-    version="1.1.0",
+    version="1.1.1",
     description=(
         "A simple MySQL DBAPI wrapper for simplifying "
         "data processing pipelines."
     ),
     long_description=(src/"README.rst").read_text(),
     packages=find_packages(),
     install_requires=[
```

