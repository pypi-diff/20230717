# Comparing `tmp/protarrow-0.1.6.tar.gz` & `tmp/protarrow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.1.6.tar", max compression
+gzip compressed data, was "protarrow-0.2.0.tar", max compression
```

## Comparing `protarrow-0.1.6.tar` & `protarrow-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-07-13 11:19:23.064791 protarrow-0.1.6/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-13 11:19:23.064791 protarrow-0.1.6/README.md
--rw-r--r--   0        0        0      754 2023-07-13 11:19:46.945755 protarrow-0.1.6/protarrow/__init__.py
--rw-r--r--   0        0        0    19405 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18960 2023-07-13 11:19:23.068791 protarrow-0.1.6/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1859 2023-07-13 11:19:46.941755 protarrow-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-07-17 07:11:44.131515 protarrow-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-17 07:11:44.131515 protarrow-0.2.0/README.md
+-rw-r--r--   0        0        0      754 2023-07-17 07:12:15.540588 protarrow-0.2.0/protarrow/__init__.py
+-rw-r--r--   0        0        0    19721 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7596 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18960 2023-07-17 07:11:44.135515 protarrow-0.2.0/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1859 2023-07-17 07:12:15.540588 protarrow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.0/PKG-INFO
```

### Comparing `protarrow-0.1.6/LICENSE` & `protarrow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/README.md` & `protarrow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/protarrow/__init__.py` & `protarrow-0.2.0/protarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.1.6/protarrow/arrow_to_proto.py` & `protarrow-0.2.0/protarrow/arrow_to_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,17 @@
         for message in self.messages:
             self.message = message
             yield self
         self.message = None
 
     def __call__(self, scalar: pa.Scalar) -> None:
         value = self.converter(scalar) if scalar.is_valid else None
-        if value is not None:
+        # `self.message` can be null for nested messages.
+        # We'd expect the scalar to be either null or the default value in this case
+        if self.message is not None and value is not None:
             if self.nullable:
                 getattr(self.message, self.field_descriptor.name).value = value
             else:
                 setattr(self.message, self.field_descriptor.name, value)
 
 
 class AppendAssigner(collections.abc.Iterable):
@@ -280,17 +282,18 @@
         self.sizes = sizes
         self.converter = converter
         self.attribute = None
 
     def __iter__(self) -> Iterator[Callable[[pa.Scalar], None]]:
         assert self.attribute is None
         for message, size in zip(self.messages, self.sizes):
-            self.attribute = getattr(message, self.field_descriptor.name)
-            for _ in range(size):
-                yield self
+            if message is not None:
+                self.attribute = getattr(message, self.field_descriptor.name)
+                for _ in range(size):
+                    yield self
         self.attribute = None
 
     def __call__(self, scalar: pa.Scalar) -> None:
         self.attribute.append(self.converter(scalar))
 
 
 @dataclasses.dataclass
@@ -308,17 +311,18 @@
         self.converter = get_converter(
             self.field_descriptor.message_type.fields_by_name["key"], key_arrow_type
         )
 
     def __iter__(self) -> Iterator[Callable[[pa.Scalar], Message]]:
         assert self.attribute is None
         for message, offset in zip(self.messages, self.sizes):
-            self.attribute = getattr(message, self.field_descriptor.name)
-            for _ in range(offset):
-                yield self
+            if message is not None:
+                self.attribute = getattr(message, self.field_descriptor.name)
+                for _ in range(offset):
+                    yield self
         self.attribute = None
 
     def __call__(self, scalar: pa.Scalar) -> Message:
         return self.attribute[self.converter(scalar)]
 
 
 def _direct_assign_map(attribute: MessageMap, key: Any, value: Any):
@@ -359,17 +363,18 @@
             if (value_descriptor.type == FieldDescriptor.TYPE_MESSAGE)
             else _direct_assign_map
         )
 
     def __iter__(self) -> Iterator[Callable[[pa.Scalar, pa.Scalar], Message]]:
         assert self.attribute is None
         for message, size in zip(self.messages, self.sizes):
-            self.attribute = getattr(message, self.field_descriptor.name)
-            for _ in range(size):
-                yield self
+            if message is not None:
+                self.attribute = getattr(message, self.field_descriptor.name)
+                for _ in range(size):
+                    yield self
         self.attribute = None
 
     def __call__(self, key: pa.Scalar, value: pa.Scalar):
         self.assigner(
             self.attribute,
             self.key_converter(key),
             self.value_converter(value) if value.is_valid else None,
```

### Comparing `protarrow-0.1.6/protarrow/cast_to_proto.py` & `protarrow-0.2.0/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/protarrow/common.py` & `protarrow-0.2.0/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/protarrow/message_extractor.py` & `protarrow-0.2.0/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/protarrow/proto_to_arrow.py` & `protarrow-0.2.0/protarrow/proto_to_arrow.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.6/pyproject.toml` & `protarrow-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.1.6"
+version = "0.2.0"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.1.6/PKG-INFO` & `protarrow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.1.6
+Version: 0.2.0
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
```

