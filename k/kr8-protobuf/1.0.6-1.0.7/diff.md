# Comparing `tmp/kr8_protobuf-1.0.6.tar.gz` & `tmp/kr8_protobuf-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kr8_protobuf-1.0.6.tar", last modified: Mon Jul 17 17:28:46 2023, max compression
+gzip compressed data, was "dist/kr8_protobuf-1.0.7.tar", last modified: Mon Jul 17 17:57:31 2023, max compression
```

## Comparing `kr8_protobuf-1.0.6.tar` & `kr8_protobuf-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:28:46.000000 kr8_protobuf-1.0.6/
--rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-17 17:28:46.000000 kr8_protobuf-1.0.6/PKG-INFO
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:28:46.000000 kr8_protobuf-1.0.6/kr8_protobuf/
--rw-r--r--   0 raeth      (501) staff       (20)     2142 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/authentication_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     5733 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/authentication_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1023 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/common_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)      159 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/common_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1864 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/user_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     2486 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/kr8_protobuf/user_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1664 2023-07-17 17:28:45.000000 kr8_protobuf-1.0.6/setup.py
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/
+-rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/PKG-INFO
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/kr8_protobuf/
+-rw-r--r--   0 raeth      (501) staff       (20)     1668 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     3970 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     2142 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     5733 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1170 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/common_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)      159 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/common_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1864 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/user_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     2486 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/user_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1664 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/setup.py
```

### Comparing `kr8_protobuf-1.0.6/PKG-INFO` & `kr8_protobuf-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kr8_protobuf
-Version: 1.0.6
+Version: 1.0.7
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `kr8_protobuf-1.0.6/kr8_protobuf/authentication_pb2.py` & `kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.6/kr8_protobuf/authentication_pb2_grpc.py` & `kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.6/kr8_protobuf/common_pb2.py` & `kr8_protobuf-1.0.7/kr8_protobuf/common_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x63ommon\"%\n\x08\x44ocument\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x63ommon\"%\n\x08\x44ocument\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x19\n\x0bGetItemByID\x12\n\n\x02id\x18\x01 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_DOCUMENT']._serialized_start=24
   _globals['_DOCUMENT']._serialized_end=61
+  _globals['_GETITEMBYID']._serialized_start=63
+  _globals['_GETITEMBYID']._serialized_end=88
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kr8_protobuf-1.0.6/kr8_protobuf/user_pb2.py` & `kr8_protobuf-1.0.7/kr8_protobuf/user_pb2.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.6/kr8_protobuf/user_pb2_grpc.py` & `kr8_protobuf-1.0.7/kr8_protobuf/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.6/setup.py` & `kr8_protobuf-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'kr8_protobuf',         # How you named your package folder (MyLib)
   packages = ['kr8_protobuf'],   # Chose the same as "name"
-  version = '1.0.6',      # Start with a small number and increase it with every change you make
+  version = '1.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

