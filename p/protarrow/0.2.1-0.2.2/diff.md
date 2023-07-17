# Comparing `tmp/protarrow-0.2.1.tar.gz` & `tmp/protarrow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.2.1.tar", max compression
+gzip compressed data, was "protarrow-0.2.2.tar", max compression
```

## Comparing `protarrow-0.2.1.tar` & `protarrow-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-07-17 08:19:59.212122 protarrow-0.2.1/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-17 08:19:59.212122 protarrow-0.2.1/README.md
--rw-r--r--   0        0        0      754 2023-07-17 08:20:19.840129 protarrow-0.2.1/protarrow/__init__.py
--rw-r--r--   0        0        0    19745 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18960 2023-07-17 08:19:59.216122 protarrow-0.2.1/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1859 2023-07-17 08:20:19.840129 protarrow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-07-17 11:15:48.575371 protarrow-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-17 11:15:48.575371 protarrow-0.2.2/README.md
+-rw-r--r--   0        0        0      754 2023-07-17 11:16:10.655362 protarrow-0.2.2/protarrow/__init__.py
+-rw-r--r--   0        0        0    19834 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7596 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18960 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1859 2023-07-17 11:16:10.655362 protarrow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.2/PKG-INFO
```

### Comparing `protarrow-0.2.1/LICENSE` & `protarrow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/README.md` & `protarrow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/protarrow/__init__.py` & `protarrow-0.2.2/protarrow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.2.1/protarrow/arrow_to_proto.py` & `protarrow-0.2.2/protarrow/arrow_to_proto.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,24 +173,24 @@
 class OptionalNestedIterable(collections.abc.Iterable):
     parents: Iterable[Message]
     field_descriptor: FieldDescriptor
     validity_mask: Iterable[pa.BooleanScalar]
 
     def __iter__(self) -> Iterator[Optional[Any]]:
         for parent, valid in zip(self.parents, self.validity_mask):
-            if valid.is_valid and valid.as_py():
+            if valid.is_valid and valid.as_py() and parent is not None:
                 yield getattr(parent, self.field_descriptor.name)
             else:
                 yield None
 
     def prime(self):
         """This needs to be called if there are no fields in the message"""
         empty = self.field_descriptor.message_type._concrete_class()
         for parent, valid in zip(self.parents, self.validity_mask):
-            if valid.is_valid and valid.as_py():
+            if valid.is_valid and valid.as_py() and parent is not None:
                 value = getattr(parent, self.field_descriptor.name)
                 value.MergeFrom(empty)
 
 
 @dataclasses.dataclass(frozen=True)
 class RepeatedNestedIterable(collections.abc.Iterable):
     parents: Iterable[Message]
@@ -198,16 +198,17 @@
 
     def __post_init__(self):
         assert self.field_descriptor.label == FieldDescriptor.LABEL_REPEATED
         assert self.field_descriptor.type == FieldDescriptor.TYPE_MESSAGE
 
     def __iter__(self) -> Iterator[Any]:
         for parent in self.parents:
-            for child in getattr(parent, self.field_descriptor.name):
-                yield child
+            if parent is not None:
+                for child in getattr(parent, self.field_descriptor.name):
+                    yield child
 
 
 def convert_scalar(scalar: pa.Scalar) -> Any:
     return scalar.as_py()
 
 
 def create_enum_converter(
```

### Comparing `protarrow-0.2.1/protarrow/cast_to_proto.py` & `protarrow-0.2.2/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/protarrow/common.py` & `protarrow-0.2.2/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/protarrow/message_extractor.py` & `protarrow-0.2.2/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/protarrow/proto_to_arrow.py` & `protarrow-0.2.2/protarrow/proto_to_arrow.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.1/pyproject.toml` & `protarrow-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.2.1"
+version = "0.2.2"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.2.1/PKG-INFO` & `protarrow-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
```

