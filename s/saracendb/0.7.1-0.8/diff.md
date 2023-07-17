# Comparing `tmp/saracendb-0.7.1.tar.gz` & `tmp/saracendb-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.7.1.tar", last modified: Fri Jul 14 10:46:26 2023, max compression
+gzip compressed data, was "saracendb-0.8.tar", last modified: Mon Jul 17 09:24:08 2023, max compression
```

## Comparing `saracendb-0.7.1.tar` & `saracendb-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.567581 saracendb-0.7.1/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4536 2023-07-14 10:46:26.567452 saracendb-0.7.1/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.7.1/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.566610 saracendb-0.7.1/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)    11316 2023-07-14 10:45:58.000000 saracendb-0.7.1/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.567279 saracendb-0.7.1/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4536 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-14 10:46:26.567614 saracendb-0.7.1/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      925 2023-07-14 10:46:07.000000 saracendb-0.7.1/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-17 09:24:08.551818 saracendb-0.8/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-17 09:24:08.551639 saracendb-0.8/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.8/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-17 09:24:08.550520 saracendb-0.8/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)    11705 2023-07-17 09:23:23.000000 saracendb-0.8/saracendb/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-17 09:24:08.551417 saracendb-0.8/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-17 09:24:08.000000 saracendb-0.8/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-17 09:24:08.000000 saracendb-0.8/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-17 09:24:08.000000 saracendb-0.8/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-17 09:24:08.000000 saracendb-0.8/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-17 09:24:08.000000 saracendb-0.8/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-17 09:24:08.551867 saracendb-0.8/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-17 09:23:33.000000 saracendb-0.8/setup.py
```

### Comparing `saracendb-0.7.1/PKG-INFO` & `saracendb-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.7.1
+Version: 0.8
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.7.1/README.md` & `saracendb-0.8/README.md`

 * *Files identical despite different names*

### Comparing `saracendb-0.7.1/saracendb/__init__.py` & `saracendb-0.8/saracendb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,22 @@
     def find(self, key: str, value: str) -> list:
         """Returns a list of dicts that contain the given key/value pair."""
         matching_entries = []
         for entry in self.__data[self.__coll]:
             if key in entry and entry[key] == value:
                 matching_entries.append(entry)
         return matching_entries
+    
+    def filter(self, keys: list, values: list) -> list:
+        """Returns a list of dicts that contain the given key/value pairs."""
+        matching_entries = []
+        for entry in self.__data[self.__coll]:
+            if all(key in entry and entry[key] == value for key, value in zip(keys, values)):
+                matching_entries.append(entry)
+        return matching_entries
 
     def get(self, id: int) -> dict:
         """Returns the entry with the given id in the current collection, or None if no entry is found."""
         for entry in self.__data[self.__coll]:
             if entry['#'] == id:
                 return entry
         print(f'No entry found with id: {id} in collection: {self.__coll}')
```

### Comparing `saracendb-0.7.1/saracendb.egg-info/PKG-INFO` & `saracendb-0.8/saracendb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.7.1
+Version: 0.8
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.7.1/setup.py` & `saracendb-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.7.1'
+VERSION = '0.8'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

