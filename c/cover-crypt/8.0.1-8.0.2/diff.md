# Comparing `tmp/cover_crypt-8.0.1-cp37-abi3-win_amd64.whl.zip` & `tmp/cover_crypt-8.0.2-cp37-abi3-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1025830 bytes, number of entries: 8
--rw-r--r--  4.6 unx    10833 b- defN 22-Dec-06 19:59 cover_crypt-8.0.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Dec-06 19:59 cover_crypt-8.0.1.dist-info/WHEEL
--rw-r--r--  4.6 unx    32275 b- defN 22-Dec-06 19:59 cover_crypt-8.0.1.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx      184 b- defN 22-Dec-06 19:59 cosmian_cover_crypt/__init__.py
--rw-r--r--  4.6 unx    11431 b- defN 22-Dec-06 19:59 cosmian_cover_crypt/__init__.pyi
--rw-r--r--  4.6 unx       27 b- defN 22-Dec-06 19:59 cosmian_cover_crypt/py.typed
--rwxr-xr-x  4.6 unx  2604032 b- defN 22-Dec-06 19:59 cosmian_cover_crypt/cosmian_cover_crypt.pyd
--rw-r--r--  4.6 unx      692 b- defN 22-Dec-06 19:59 cover_crypt-8.0.1.dist-info/RECORD
-8 files, 2659569 bytes uncompressed, 1024622 bytes compressed:  61.5%
+Zip file size: 460844 bytes, number of entries: 8
+-rw-r--r--  4.6 unx    10827 b- defN 23-Jan-16 12:39 cover_crypt-8.0.2.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 23-Jan-16 12:39 cover_crypt-8.0.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx    32275 b- defN 23-Jan-16 12:39 cover_crypt-8.0.2.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx       27 b- defN 23-Jan-16 12:39 cosmian_cover_crypt/py.typed
+-rw-r--r--  4.6 unx    12062 b- defN 23-Jan-16 12:39 cosmian_cover_crypt/__init__.pyi
+-rw-r--r--  4.6 unx      184 b- defN 23-Jan-16 12:39 cosmian_cover_crypt/__init__.py
+-rwxr-xr-x  4.6 unx  1006688 b- defN 23-Jan-16 12:39 cosmian_cover_crypt/cosmian_cover_crypt.abi3.so
+-rw-r--r--  4.6 unx      697 b- defN 23-Jan-16 12:39 cover_crypt-8.0.2.dist-info/RECORD
+8 files, 1062868 bytes uncompressed, 459628 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: cover_crypt-8.0.1.dist-info/METADATA
+Filename: cover_crypt-8.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cover_crypt-8.0.1.dist-info/WHEEL
+Filename: cover_crypt-8.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cover_crypt-8.0.1.dist-info/license_files/LICENSE.md
+Filename: cover_crypt-8.0.2.dist-info/license_files/LICENSE.md
 Comment: 
 
-Filename: cosmian_cover_crypt/__init__.py
+Filename: cosmian_cover_crypt/py.typed
 Comment: 
 
 Filename: cosmian_cover_crypt/__init__.pyi
 Comment: 
 
-Filename: cosmian_cover_crypt/py.typed
+Filename: cosmian_cover_crypt/__init__.py
 Comment: 
 
-Filename: cosmian_cover_crypt/cosmian_cover_crypt.pyd
+Filename: cosmian_cover_crypt/cosmian_cover_crypt.abi3.so
 Comment: 
 
-Filename: cover_crypt-8.0.1.dist-info/RECORD
+Filename: cover_crypt-8.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_cover_crypt/__init__.pyi

```diff
@@ -6,14 +6,26 @@
 
     Args:
         axis (str): policy axis the attributes belongs to
         name (str): unique attribute name within this axis
     """
 
     def __init__(self, axis: str, name: str): ...
+    def get_axis(self) -> str:
+        """Get the corresponding axis of the attribute.
+
+        Returns:
+            str
+        """
+    def get_name(self) -> str:
+        """Get the attribute name.
+
+        Returns:
+            str
+        """
     def to_string(self) -> str:
         """Creates a string representation of the attribute.
 
         Returns:
             str
         """
     @staticmethod
@@ -46,14 +58,32 @@
         """
     def is_empty(self) -> bool:
         """Check whether the attribute list is empty.
 
         Returns:
             bool
         """
+    def get_name(self) -> str:
+        """Get axis name.
+
+        Returns:
+            str
+        """
+    def get_attributes(self) -> List[str]:
+        """Get the list of attributes in the axis.
+
+        Returns:
+            List[str]
+        """
+    def is_hierarchical(self) -> bool:
+        """Check whether the axis is hierarchical.
+
+        Returns:
+            bool
+        """
     def to_string(self) -> str:
         """Creates a string representation of the policy axis.
 
         Returns:
             str
         """
```

## Comparing `cover_crypt-8.0.1.dist-info/METADATA` & `cover_crypt-8.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: cover_crypt
-Version: 8.0.1
+Version: 8.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: cffi
 License-File: LICENSE.md
 Summary: Key Policy attribute encryption based on subset cover
 Author: Théophile Brezot <theophile.brezot@cosmian.com>, Bruno Grieder <bruno.grieder@cosmian.com>
 Author-email: Théophile Brezot <theophile.brezot@cosmian.com>, Bruno Grieder <bruno.grieder@cosmian.com>
 License: MIT/Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/Cosmian/cover_crypt
 
-# CoverCrypt &emsp; [![Build Status]][actions] [![Latest Version]][crates.io]
+# CoverCrypt
 
-[build status]: https://img.shields.io/github/workflow/status/Cosmian/cosmian_cover_crypt/CI%20checks/main
-[actions]: https://github.com/Cosmian/cosmian_cover_crypt/actions?query=branch%3Amain
-[latest version]: https://img.shields.io/crates/v/cosmian_cover_crypt.svg
-[crates.io]: https://crates.io/crates/cosmian_cover_crypt
+![Build status](https://github.com/Cosmian/cover_crypt/actions/workflows/ci.yml/badge.svg)
+![Build status](https://github.com/Cosmian/cover_crypt/actions/workflows/build.yml/badge.svg)
+![latest version](<https://img.shields.io/crates/v/cosmian_cover_crypt.svg>)
 
 Implementation of the [CoverCrypt](bib/CoverCrypt.pdf) algorithm which allows
 creating ciphertexts for a set of attributes and issuing user keys with access
 policies over these attributes.
 
 <!-- toc -->
 
 - [Getting started](#getting-started)
 - [Building and testing](#building-and-testing)
   - [Building the library for a different glibc](#building-the-library-for-a-different-glibc)
-  - [Build and tests for Pyo3](#build-and-tests-for-pyo3)
 - [Features and Benchmarks](#features-and-benchmarks)
   - [Key generation](#key-generation)
   - [Serialization](#serialization)
   - [Secret key encapsulation](#secret-key-encapsulation)
   - [Secret key decapsulation](#secret-key-decapsulation)
 - [Documentation](#documentation)
+- [Releases](#releases)
 
 <!-- tocstop -->
 
 ## Getting started
 
 The following code sample introduces the CoverCrypt functionalities. It can be
 run from `examples/runme.rs` using `cargo run --example runme`.
@@ -151,14 +150,28 @@
 
 To build the FFI interface:
 
 ```bash
 cargo build --release --features interfaces
 ```
 
+To build the Python interface, run:
+
+```bash
+maturin build --release --features python
+```
+
+__Note__: when a new function or class is added to the PyO3 interface, its signature needs to be added to [`__init__.pyi`](./python/cosmian_cover_crypt/__init__.pyi).
+
+To run tests on the Python interface, run:
+
+```bash
+./python/scripts/test.sh
+```
+
 To build everything (including the FFI):
 
 ```bash
 cargo build --release --all-features
 ```
 
 The latter will build a shared library. On Linux, one can verify that the FFI
@@ -180,24 +193,14 @@
 cargo bench
 ```
 
 ### Building the library for a different glibc
 
 Go to the [build](build/glibc-2.17/) directory for an example on how to build for GLIBC 2.17
 
-### Build and tests for Pyo3
-
-> When a new function/class is added to the PyO3 interface, write its signature in `python/cosmian_cover_crypt/__init__.pyi`.
-
-- See `gitlab-ci` for release build using manylinux (<https://github.com/pypa/manylinux#manylinux>)
-
-```bash
-./python/scripts/test.sh
-```
-
 ## Features and Benchmarks
 
 In CoverCrypt, messages are encrypted using a symmetric scheme. The right
 management is performed by a novel asymmetric scheme which is used to
 encapsulate a symmetric key. This encapsulation is stored in an object called
 encrypted header, along with the symmetric ciphertext.
 
@@ -291,15 +294,15 @@
 and its encapsulation for a given set of rights.
 
 To ease the management of the encapsulations, an object `EncryptedHeader`is
 provided in the API. An encrypted header holds an encapsulation and a symmetric
 ciphertext of an optional additional data. This additional data can be useful
 to store metadata.
 
-**Note**: encapsulations grow bigger with the size of the target set of rights
+__Note__: encapsulations grow bigger with the size of the target set of rights
 and so does the encapsulation time. The following benchmark gives the size of
 the encrypted header and the encryption time given the number of rights in the
 target set (one right = one partition).
 
 ```c
 Bench header encryption size: 1 partition: 126 bytes, 3 partitions: 190 bytes
 
@@ -329,7 +332,11 @@
 A formal description and proof of the CoverCrypt scheme is given in
 [this paper](./bib/CoverCrypt.pdf).
 It also contains an interesting discussion about the implementation.
 
 The developer documentation can be found on
 [doc.rs](https://docs.rs/cosmian_cover_crypt/6.0.8/cosmian_cover_crypt/index.html)
 
+## Releases
+
+All releases can be found in the public URL [package.cosmian.com](https://package.cosmian.com).
+
```

## Comparing `cover_crypt-8.0.1.dist-info/license_files/LICENSE.md` & `cover_crypt-8.0.2.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

