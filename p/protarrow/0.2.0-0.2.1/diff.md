# Comparing `tmp/protarrow-0.2.0.tar.gz` & `tmp/protarrow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.2.0.tar", max compression
+gzip compressed data, was "protarrow-0.2.1.tar", max compression
```

## Comparing `protarrow-0.2.0.tar` & `protarrow-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-07-17 07:11:44.131515 protarrow-0.2.0/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-17 07:11:44.131515 protarrow-0.2.0/README.md
--rw-r--r--   0        0        0      754 2023-07-17 07:12:15.540588 protarrow-0.2.0/protarrow/__init__.py
--rw-r--r--   0        0        0    19721 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18960 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1859 2023-07-17 07:12:15.540588 protarrow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-07-17 08:19:59.212122 protarrow-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-17 08:19:59.212122 protarrow-0.2.1/README.md
+-rw-r--r--   0        0        0      754 2023-07-17 08:20:19.840129 protarrow-0.2.1/protarrow/__init__.py
+-rw-r--r--   0        0        0    19745 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7596 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18960 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1859 2023-07-17 08:20:19.840129 protarrow-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.1/PKG-INFO
```

### Comparing `protarrow-0.2.0/LICENSE` & `protarrow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/README.md` & `protarrow-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/protarrow/__init__.py` & `protarrow-0.2.1/protarrow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.2.0/protarrow/arrow_to_proto.py` & `protarrow-0.2.1/protarrow/arrow_to_proto.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     array: pa.Array, field_descriptor: FieldDescriptor, messages: Iterable[Message]
 ) -> None:
     if field_descriptor.label == FieldDescriptor.LABEL_REPEATED:
         _extract_repeated_field(array, field_descriptor, messages)
     elif field_descriptor.message_type in TEMPORAL_CONVERTERS:
         extractor = TEMPORAL_CONVERTERS[field_descriptor.message_type](array.type)
         for message, value in zip(messages, array):
-            if value.is_valid:
+            if value.is_valid and message is not None:
                 getattr(
                     message,
                     field_descriptor.name,
                 ).MergeFrom(extractor(value))
     elif (
         field_descriptor.type == FieldDescriptor.TYPE_MESSAGE
         and field_descriptor.message_type not in NULLABLE_TYPES
```

### Comparing `protarrow-0.2.0/protarrow/cast_to_proto.py` & `protarrow-0.2.1/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/protarrow/common.py` & `protarrow-0.2.1/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/protarrow/message_extractor.py` & `protarrow-0.2.1/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/protarrow/proto_to_arrow.py` & `protarrow-0.2.1/protarrow/proto_to_arrow.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.0/pyproject.toml` & `protarrow-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.2.0"
+version = "0.2.1"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.2.0/PKG-INFO` & `protarrow-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
```

