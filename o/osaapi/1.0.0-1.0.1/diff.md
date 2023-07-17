# Comparing `tmp/osaapi-1.0.0.tar.gz` & `tmp/osaapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osaapi-1.0.0.tar", max compression
+gzip compressed data, was "osaapi-1.0.1.tar", max compression
```

## Comparing `osaapi-1.0.0.tar` & `osaapi-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11320 2023-07-17 13:48:35.795511 osaapi-1.0.0/LICENSE
--rw-r--r--   0        0        0     7286 2023-07-17 13:48:35.795511 osaapi-1.0.0/README.md
--rw-r--r--   0        0        0    55239 2023-07-17 13:48:35.795511 osaapi-1.0.0/osaapi/__init__.py
--rw-r--r--   0        0        0     1250 2023-07-17 13:48:58.787456 osaapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 osaapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11320 2023-07-17 14:51:18.738845 osaapi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7286 2023-07-17 14:51:18.738845 osaapi-1.0.1/README.md
+-rw-r--r--   0        0        0    55227 2023-07-17 14:51:18.738845 osaapi-1.0.1/osaapi/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-17 14:51:46.696495 osaapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 osaapi-1.0.1/PKG-INFO
```

### Comparing `osaapi-1.0.0/LICENSE` & `osaapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osaapi-1.0.0/README.md` & `osaapi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `osaapi-1.0.0/osaapi/__init__.py` & `osaapi-1.0.1/osaapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1409,18 +1409,18 @@
             self.__server__ = conn.__server__
             self.__server__._ServerProxy__verbose = conn.__server__._ServerProxy__verbose
 
         def rescheduleTask(self, **kwargs):
             return self.__server__.pem.tasks.rescheduleTask(kwargs)
 
         def getTaskLog(self, **kwargs):
-            return self.__server__.pem.tasks.getTaskLog(kwargs)
+            return self.__server__.pem.getTaskLog(kwargs)
 
         def cancelJob(self, **kwargs):
-            return self.__server__.pem.tasks.cancelJob(kwargs)
+            return self.__server__.pem.cancelJob(kwargs)
 
     def create_account(self, first_name=None, last_name=None, account_type='C',
                        branded_domain=None, parent_account_id=None, **kwargs):
         """
         Possible values for the account_type:
             'C': Indicates that the Account is created for Customer. Default value.
             'R': Indicates that the Account is created for Reseller.
```

### Comparing `osaapi-1.0.0/pyproject.toml` & `osaapi-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osaAPI"
-version = "v1.0.0"
+version = "v1.0.1"
 description = ""
 authors = ["Ingrammicro Inc.", "Rahul Mondal <rahul.mondal@ingrammicro.com>"]
 readme = "README.md"
 packages = [{include = "osaapi"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
```

### Comparing `osaapi-1.0.0/PKG-INFO` & `osaapi-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osaapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Ingrammicro Inc.
 Requires-Python: >=3.7,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

