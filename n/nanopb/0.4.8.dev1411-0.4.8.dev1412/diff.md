# Comparing `tmp/nanopb-0.4.8.dev1411.tar.gz` & `tmp/nanopb-0.4.8.dev1412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.8.dev1411.tar", max compression
+gzip compressed data, was "nanopb-0.4.8.dev1412.tar", max compression
```

## Comparing `nanopb-0.4.8.dev1411.tar` & `nanopb-0.4.8.dev1412.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4366 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/README.md
--rw-r--r--   0        0        0        0 2023-07-10 02:36:48.804970 nanopb-0.4.8.dev1411/nanopb/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 02:36:48.804970 nanopb-0.4.8.dev1411/nanopb/generator/__init__.py
--rwxr-xr-x   0        0        0   107186 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/nanopb_generator.py
--rwxr-xr-x   0        0        0      460 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/nanopb_generator.py2
--rw-r--r--   0        0        0     5820 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/platformio_generator.py
--rw-r--r--   0        0        0      126 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/proto/Makefile
--rw-r--r--   0        0        0     4565 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/proto/__init__.py
--rw-r--r--   0        0        0     3318 2023-07-10 02:36:48.832972 nanopb-0.4.8.dev1411/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2121 2023-07-10 02:36:48.952980 nanopb-0.4.8.dev1411/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2023 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/proto/_utils.py
--rw-r--r--   0        0        0    36277 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/proto/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     6923 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/proto/nanopb.proto
--rw-r--r--   0        0        0     4690 2023-07-10 02:36:48.964981 nanopb-0.4.8.dev1411/nanopb/generator/proto/nanopb_pb2.py
--rwxr-xr-x   0        0        0     1577 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/protoc
--rwxr-xr-x   0        0        0      374 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/protoc-gen-nanopb
--rwxr-xr-x   0        0        0      554 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/protoc-gen-nanopb-py2
--rw-r--r--   0        0        0      449 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/protoc-gen-nanopb.bat
--rw-r--r--   0        0        0      302 2023-07-06 07:47:51.000000 nanopb-0.4.8.dev1411/nanopb/generator/protoc.bat
--rw-r--r--   0        0        0     1065 2023-07-10 02:36:48.996983 nanopb-0.4.8.dev1411/pyproject.toml
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 nanopb-0.4.8.dev1411/PKG-INFO
+-rw-r--r--   0        0        0     4366 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 02:37:41.869196 nanopb-0.4.8.dev1412/nanopb/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 02:37:41.869196 nanopb-0.4.8.dev1412/nanopb/generator/__init__.py
+-rwxr-xr-x   0        0        0   107186 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/nanopb_generator.py
+-rwxr-xr-x   0        0        0      460 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/nanopb_generator.py2
+-rw-r--r--   0        0        0     5832 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/platformio_generator.py
+-rw-r--r--   0        0        0      126 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/proto/Makefile
+-rw-r--r--   0        0        0     4565 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/proto/__init__.py
+-rw-r--r--   0        0        0     3318 2023-07-17 02:37:41.893196 nanopb-0.4.8.dev1412/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2121 2023-07-17 02:37:41.989197 nanopb-0.4.8.dev1412/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2023 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/proto/_utils.py
+-rw-r--r--   0        0        0    36277 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/proto/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     6923 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/proto/nanopb.proto
+-rw-r--r--   0        0        0     4690 2023-07-17 02:37:41.997197 nanopb-0.4.8.dev1412/nanopb/generator/proto/nanopb_pb2.py
+-rwxr-xr-x   0        0        0     1577 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/protoc
+-rwxr-xr-x   0        0        0      374 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/protoc-gen-nanopb
+-rwxr-xr-x   0        0        0      554 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/protoc-gen-nanopb-py2
+-rw-r--r--   0        0        0      449 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/protoc-gen-nanopb.bat
+-rw-r--r--   0        0        0      302 2023-07-12 19:25:31.000000 nanopb-0.4.8.dev1412/nanopb/generator/protoc.bat
+-rw-r--r--   0        0        0     1065 2023-07-17 02:37:42.025197 nanopb-0.4.8.dev1412/pyproject.toml
+-rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 nanopb-0.4.8.dev1412/PKG-INFO
```

### Comparing `nanopb-0.4.8.dev1411/README.md` & `nanopb-0.4.8.dev1412/README.md`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/nanopb_generator.py` & `nanopb-0.4.8.dev1412/nanopb/generator/nanopb_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/platformio_generator.py` & `nanopb-0.4.8.dev1412/nanopb/generator/platformio_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 project_dir = env.subst("$PROJECT_DIR")
 build_dir = env.subst("$BUILD_DIR")
 
 generated_src_dir = os.path.join(build_dir, 'nanopb', 'generated-src')
 generated_build_dir = os.path.join(build_dir, 'nanopb', 'generated-build')
 md5_dir = os.path.join(build_dir, 'nanopb', 'md5')
 
-nanopb_protos = env.GetProjectOption("custom_nanopb_protos", "")
+nanopb_protos =  env.subst(env.GetProjectOption("custom_nanopb_protos", ""))
 nanopb_plugin_options = env.GetProjectOption("custom_nanopb_options", "")
 
 if not nanopb_protos:
     print("[nanopb] No generation needed.")
 else:
     if isinstance(nanopb_plugin_options, (list, tuple)):
         nanopb_plugin_options = " ".join(nanopb_plugin_options)
```

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/__init__.py` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jul  6 07:47:51 2023 UTC, .py size: 4565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a771 a664 d511 0000  U........q.d....
+00000000: 550d 0d0a 0000 0000 2bfe ae64 d511 0000  U.......+..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6404 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jul  6 07:47:51 2023 UTC, .py size: 2023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a771 a664 e707 0000  U........q.d....
+00000000: 550d 0d0a 0000 0000 2bfe ae64 e707 0000  U.......+..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 8400 5a04 6404  d.l.Z.d.d...Z.d.
 00000050: 6405 8400 5a05 6406 6407 8400 5a06 6507  d...Z.d.d...Z.e.
 00000060: 6408 6b02 723e 6506 8300 0100 6401 5300  d.k.r>e.....d.S.
 00000070: 2909 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
```

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/_utils.py` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/_utils.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/google/protobuf/descriptor.proto` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/nanopb.proto` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/nanopb.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/proto/nanopb_pb2.py` & `nanopb-0.4.8.dev1412/nanopb/generator/proto/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/protoc` & `nanopb-0.4.8.dev1412/nanopb/generator/protoc`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/nanopb/generator/protoc-gen-nanopb-py2` & `nanopb-0.4.8.dev1412/nanopb/generator/protoc-gen-nanopb-py2`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.8.dev1411/pyproject.toml` & `nanopb-0.4.8.dev1412/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanopb"
-version = "0.4.8-dev1411"
+version = "0.4.8-dev1412"
 description = "Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system."
 authors = ["Petteri Aimonen <jpa@npb.mail.kapsi.fi>"]
 license = "Zlib"
 repository = "https://github.com/nanopb/nanopb/"
 readme = "README.md"
 homepage = "https://jpa.kapsi.fi/nanopb/"
 documentation = "https://jpa.kapsi.fi/nanopb/docs/index.html"
```

### Comparing `nanopb-0.4.8.dev1411/PKG-INFO` & `nanopb-0.4.8.dev1412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanopb
-Version: 0.4.8.dev1411
+Version: 0.4.8.dev1412
 Summary: Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system.
 Home-page: https://jpa.kapsi.fi/nanopb/
 License: Zlib
 Keywords: protobuf,protoc
 Author: Petteri Aimonen
 Author-email: jpa@npb.mail.kapsi.fi
 Requires-Python: >=2.7
```

