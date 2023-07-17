# Comparing `tmp/kr8_protobuf-1.0.7.tar.gz` & `tmp/kr8_protobuf-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kr8_protobuf-1.0.7.tar", last modified: Mon Jul 17 17:57:31 2023, max compression
+gzip compressed data, was "dist/kr8_protobuf-1.0.8.tar", last modified: Mon Jul 17 18:04:19 2023, max compression
```

## Comparing `kr8_protobuf-1.0.7.tar` & `kr8_protobuf-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/
--rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/PKG-INFO
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 17:57:31.000000 kr8_protobuf-1.0.7/kr8_protobuf/
--rw-r--r--   0 raeth      (501) staff       (20)     1668 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     3970 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     2142 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     5733 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1170 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/common_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)      159 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/common_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1864 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/user_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     2486 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/kr8_protobuf/user_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1664 2023-07-17 17:57:30.000000 kr8_protobuf-1.0.7/setup.py
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/
+-rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/PKG-INFO
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/
+-rw-r--r--   0 raeth      (501) staff       (20)     1643 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     3916 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     2142 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     5733 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1170 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/common_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)      159 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/common_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1864 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/user_pb2.py
+-rw-r--r--   0 raeth      (501) staff       (20)     2486 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/user_pb2_grpc.py
+-rw-r--r--   0 raeth      (501) staff       (20)     1664 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/setup.py
```

### Comparing `kr8_protobuf-1.0.7/PKG-INFO` & `kr8_protobuf-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kr8_protobuf
-Version: 1.0.7
+Version: 1.0.8
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2.py` & `kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61nalyzer.proto\x12\x08\x61nalyzer\x1a\x1bgoogle/protobuf/empty.proto\x1a\x0c\x63ommon.proto\"$\n\x04Post\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x61pproved\x18\x02 \x01(\x08\"&\n\x05Posts\x12\x1d\n\x05posts\x18\x01 \x03(\x0b\x32\x0e.analyzer.Post2\x80\x01\n\x18\x41uthenticationController\x12\x32\n\x08GetPosts\x12\x13.common.GetItemByID\x1a\x0f.analyzer.Posts\"\x00\x12\x30\n\x07GetPost\x12\x13.common.GetItemByID\x1a\x0e.analyzer.Post\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61nalyzer.proto\x12\x08\x61nalyzer\x1a\x1bgoogle/protobuf/empty.proto\x1a\x0c\x63ommon.proto\"$\n\x04Post\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x61pproved\x18\x02 \x01(\x08\"&\n\x05Posts\x12\x1d\n\x05posts\x18\x01 \x03(\x0b\x32\x0e.analyzer.Post2z\n\x12\x41nalyzerController\x12\x32\n\x08GetPosts\x12\x13.common.GetItemByID\x1a\x0f.analyzer.Posts\"\x00\x12\x30\n\x07GetPost\x12\x13.common.GetItemByID\x1a\x0e.analyzer.Post\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analyzer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_POST']._serialized_start=71
   _globals['_POST']._serialized_end=107
   _globals['_POSTS']._serialized_start=109
   _globals['_POSTS']._serialized_end=147
-  _globals['_AUTHENTICATIONCONTROLLER']._serialized_start=150
-  _globals['_AUTHENTICATIONCONTROLLER']._serialized_end=278
+  _globals['_ANALYZERCONTROLLER']._serialized_start=149
+  _globals['_ANALYZERCONTROLLER']._serialized_end=271
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/analyzer_pb2_grpc.py` & `kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import analyzer_pb2 as analyzer__pb2
 import common_pb2 as common__pb2
 
 
-class AuthenticationControllerStub(object):
+class AnalyzerControllerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetPosts = channel.unary_unary(
-                '/analyzer.AuthenticationController/GetPosts',
+                '/analyzer.AnalyzerController/GetPosts',
                 request_serializer=common__pb2.GetItemByID.SerializeToString,
                 response_deserializer=analyzer__pb2.Posts.FromString,
                 )
         self.GetPost = channel.unary_unary(
-                '/analyzer.AuthenticationController/GetPost',
+                '/analyzer.AnalyzerController/GetPost',
                 request_serializer=common__pb2.GetItemByID.SerializeToString,
                 response_deserializer=analyzer__pb2.Post.FromString,
                 )
 
 
-class AuthenticationControllerServicer(object):
+class AnalyzerControllerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetPosts(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -39,48 +39,48 @@
     def GetPost(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AuthenticationControllerServicer_to_server(servicer, server):
+def add_AnalyzerControllerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetPosts': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPosts,
                     request_deserializer=common__pb2.GetItemByID.FromString,
                     response_serializer=analyzer__pb2.Posts.SerializeToString,
             ),
             'GetPost': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPost,
                     request_deserializer=common__pb2.GetItemByID.FromString,
                     response_serializer=analyzer__pb2.Post.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'analyzer.AuthenticationController', rpc_method_handlers)
+            'analyzer.AnalyzerController', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class AuthenticationController(object):
+class AnalyzerController(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def GetPosts(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/analyzer.AuthenticationController/GetPosts',
+        return grpc.experimental.unary_unary(request, target, '/analyzer.AnalyzerController/GetPosts',
             common__pb2.GetItemByID.SerializeToString,
             analyzer__pb2.Posts.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetPost(request,
@@ -89,12 +89,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/analyzer.AuthenticationController/GetPost',
+        return grpc.experimental.unary_unary(request, target, '/analyzer.AnalyzerController/GetPost',
             common__pb2.GetItemByID.SerializeToString,
             analyzer__pb2.Post.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2.py` & `kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/authentication_pb2_grpc.py` & `kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/common_pb2.py` & `kr8_protobuf-1.0.8/kr8_protobuf/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/user_pb2.py` & `kr8_protobuf-1.0.8/kr8_protobuf/user_pb2.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.7/kr8_protobuf/user_pb2_grpc.py` & `kr8_protobuf-1.0.8/kr8_protobuf/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kr8_protobuf-1.0.7/setup.py` & `kr8_protobuf-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'kr8_protobuf',         # How you named your package folder (MyLib)
   packages = ['kr8_protobuf'],   # Chose the same as "name"
-  version = '1.0.7',      # Start with a small number and increase it with every change you make
+  version = '1.0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

