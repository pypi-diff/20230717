# Comparing `tmp/poslq_simple-0.1.3.tar.gz` & `tmp/poslq_simple-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poslq_simple-0.1.3.tar", last modified: Sun Jul 16 19:26:35 2023, max compression
+gzip compressed data, was "poslq_simple-0.1.5.tar", last modified: Sun Jul 16 23:39:29 2023, max compression
```

## Comparing `poslq_simple-0.1.3.tar` & `poslq_simple-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.064342 poslq_simple-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3399 2023-07-16 19:26:35.064342 poslq_simple-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2875 2023-07-16 19:23:58.000000 poslq_simple-0.1.3/README.md
--rw-rw-rw-   0        0        0      611 2023-07-16 19:25:58.000000 poslq_simple-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 19:26:35.065345 poslq_simple-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.036795 poslq_simple-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.061831 poslq_simple-0.1.3/src/poslq_simple.egg-info/
--rw-rw-rw-   0        0        0     3399 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.063336 poslq_simple-0.1.3/src/posql_simple/
--rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.3/src/posql_simple/__init__.py
--rw-rw-rw-   0        0        0     5339 2023-07-16 19:22:32.000000 poslq_simple-0.1.3/src/posql_simple/w_out_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3394 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2023-07-16 19:45:03.000000 poslq_simple-0.1.5/README.md
+-rw-rw-rw-   0        0        0      611 2023-07-16 23:37:47.000000 poslq_simple-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.651425 poslq_simple-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/src/poslq_simple.egg-info/
+-rw-rw-rw-   0        0        0     3394 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/src/posql_simple/
+-rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.5/src/posql_simple/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-07-16 22:52:41.000000 poslq_simple-0.1.5/src/posql_simple/w_out_sql.py
```

### Comparing `poslq_simple-0.1.3/LICENSE` & `poslq_simple-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.3/PKG-INFO` & `poslq_simple-0.1.5/src/poslq_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: poslq_simple
-Version: 0.1.3
+Name: poslq-simple
+Version: 0.1.5
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
 ```python
-from w_out_sql import Database, Collection
+from posql_simple import w_out_sql.py
 my_password = "hello world" # for cipher coding ( key )
 path = "./default.pst"      # use the pst extension
 my_db = Database (__pass =  password, path = path)
 my_collection_name = "clients"
 my_collection = Collection ( collect_name = my_collection_name) # creating the collection
 db.bind_new_collection(my_collection) # binding the collection to the db
```

### Comparing `poslq_simple-0.1.3/README.md` & `poslq_simple-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
 ```python
-from w_out_sql import Database, Collection
+from posql_simple import w_out_sql.py
 my_password = "hello world" # for cipher coding ( key )
 path = "./default.pst"      # use the pst extension
 my_db = Database (__pass =  password, path = path)
 my_collection_name = "clients"
 my_collection = Collection ( collect_name = my_collection_name) # creating the collection
 db.bind_new_collection(my_collection) # binding the collection to the db
```

### Comparing `poslq_simple-0.1.3/pyproject.toml` & `poslq_simple-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "poslq_simple"
-version = "0.1.3"
+version = "0.1.5"
 authors = [
   { name="enyos", email="lebedevhh@outlook.fr" },
 ]
 description = "A simple nosql json storage for small projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `poslq_simple-0.1.3/src/poslq_simple.egg-info/PKG-INFO` & `poslq_simple-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: poslq-simple
-Version: 0.1.3
+Name: poslq_simple
+Version: 0.1.5
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
 ```python
-from w_out_sql import Database, Collection
+from posql_simple import w_out_sql.py
 my_password = "hello world" # for cipher coding ( key )
 path = "./default.pst"      # use the pst extension
 my_db = Database (__pass =  password, path = path)
 my_collection_name = "clients"
 my_collection = Collection ( collect_name = my_collection_name) # creating the collection
 db.bind_new_collection(my_collection) # binding the collection to the db
```

### Comparing `poslq_simple-0.1.3/src/posql_simple/w_out_sql.py` & `poslq_simple-0.1.5/src/posql_simple/w_out_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         else:
             raise FileNotFoundError("file {fname} doesn't exist".format( fname = path))
 
     def __repr__( self ):
         return "path : {path_name}, collections : {coll}".format( path_name = self.path, coll = self.__data )
 
     def bind_new_collection(self, collection ):
-        self.__data[collection.collect_name] = collection._get_all_slot()
+        self.__data[collection.collect_name] = collection.get_all_slot()
         self.save(debug = False)
 
     def get_collection(self, coll_name : str ):
         if ( col_name in list(self.__data.keys())):
             return Collection( coll_name, self.__data[coll_name])
         else :
             print ( "[INFO] this is collection doesn't exist")
@@ -67,15 +67,15 @@
             self.bind_new_collection( result )
             return result
             
     def get_all_collections(self) -> dict :
         return self.__data
 
 class Collection:
-    def __init__(self, collect_name : str , __container_documents : list = []):
+    def __init__(self, collect_name : str , __container_documents : list = []): # by default is list ( not None )
         self.collect_name=collect_name
         self.__container_documents = __container_documents# empty list to stores one all the documents
     
     def add_record(self, record : dict ) -> bool :
         # we need to check / if it has the _id prop
         lock.acquire()
         try : 
@@ -122,25 +122,25 @@
                 found = True
                 break 
 
             counter += 1 
 
         if found : 
             self.__container_documents[counter] = cpy_new_obj
-            lock.acquire()
+            lock.release()
             return True 
 
-        lock.acquire()
+        lock.release()
         return False 
 
     # the user will provide the search function
     # this function can return a null value
     # returns a cpy of the func
     def search_by(self, slot_name : str , slot_value):
         for  slot in self.__container_documents :
             if ( slot[slot_name] == slot_value ):
                 return slot.copy() 
         return None
 
     # getter
-    def _get_all_slot(self):
+    def get_all_slot(self):
         return self.__container_documents
```

