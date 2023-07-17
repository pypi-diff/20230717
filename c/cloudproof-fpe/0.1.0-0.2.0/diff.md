# Comparing `tmp/cloudproof_fpe-0.1.0-cp37-abi3-win_amd64.whl.zip` & `tmp/cloudproof_fpe-0.2.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 258242 bytes, number of entries: 7
--rw-r--r--  4.6 unx     8286 b- defN 23-Apr-06 16:35 cloudproof_fpe-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-06 16:35 cloudproof_fpe-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      164 b- defN 23-Apr-06 16:35 cloudproof_fpe/__init__.py
--rw-r--r--  4.6 unx       27 b- defN 23-Apr-06 16:35 cloudproof_fpe/py.typed
--rw-r--r--  4.6 unx     7440 b- defN 23-Apr-06 16:35 cloudproof_fpe/__init__.pyi
--rwxr-xr-x  4.6 unx   529920 b- defN 23-Apr-06 16:35 cloudproof_fpe/cloudproof_fpe.pyd
--rw-r--r--  4.6 unx      563 b- defN 23-Apr-06 16:35 cloudproof_fpe-0.1.0.dist-info/RECORD
-7 files, 546496 bytes uncompressed, 257246 bytes compressed:  52.9%
+Zip file size: 276119 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     8357 b- defN 23-Jul-17 11:22 cloudproof_fpe-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-17 11:22 cloudproof_fpe-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    32275 b- defN 23-Jul-17 11:22 cloudproof_fpe-0.2.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     6428 b- defN 23-Jul-17 11:22 cloudproof_fpe/__init__.pyi
+-rw-r--r--  4.6 unx       27 b- defN 23-Jul-17 11:22 cloudproof_fpe/py.typed
+-rw-r--r--  4.6 unx      164 b- defN 23-Jul-17 11:22 cloudproof_fpe/__init__.py
+-rwxr-xr-x  4.6 unx   545792 b- defN 23-Jul-17 11:22 cloudproof_fpe/cloudproof_fpe.pyd
+-rw-r--r--  4.6 unx      676 b- defN 23-Jul-17 11:22 cloudproof_fpe-0.2.0.dist-info/RECORD
+8 files, 593813 bytes uncompressed, 274937 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: cloudproof_fpe-0.1.0.dist-info/METADATA
+Filename: cloudproof_fpe-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cloudproof_fpe-0.1.0.dist-info/WHEEL
+Filename: cloudproof_fpe-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cloudproof_fpe/__init__.py
+Filename: cloudproof_fpe-0.2.0.dist-info/license_files/LICENSE.md
+Comment: 
+
+Filename: cloudproof_fpe/__init__.pyi
 Comment: 
 
 Filename: cloudproof_fpe/py.typed
 Comment: 
 
-Filename: cloudproof_fpe/__init__.pyi
+Filename: cloudproof_fpe/__init__.py
 Comment: 
 
 Filename: cloudproof_fpe/cloudproof_fpe.pyd
 Comment: 
 
-Filename: cloudproof_fpe-0.1.0.dist-info/RECORD
+Filename: cloudproof_fpe-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudproof_fpe/__init__.pyi

```diff
@@ -5,87 +5,75 @@
     """
 
     def __init__(self, alphabet_id: str):
         """
         Initialize the FormatPreservingEncryption instance with a given
         alphabet type.
 
-        :param alphabet_type: A string indicating the type of alphabet to be used
-        for the encryption. Currently, only the following options are supported:
-            - "numeric",
-            - "hexa_decimal",
-            - "alpha_lower",
-            - "alpha_upper",
-            - "alpha",
-            - "alpha_numeric",
-            - "utf",
-            - "chinese",
-            - "latin1sup",
-            - "latin1sup_alphanum",.
+        Args:
+            alphabet_type (str): A string indicating the type of alphabet to be used
+                for the encryption. Currently, only the following options are supported:
+                - "numeric",
+                - "hexa_decimal",
+                - "alpha_lower",
+                - "alpha_upper",
+                - "alpha",
+                - "alpha_numeric",
+                - "utf",
+                - "chinese",
+                - "latin1sup",
+                - "latin1sup_alphanum".
         """
     def encrypt(self, key: bytes, tweak: bytes, plaintext: str) -> str:
         """
-        Encrypt a plaintext using the specified key and tweak.
+        Encrypts a plaintext using the specified key and tweak.
+
+        Args:
+            key (bytes): A bytes object containing the key to be used for the encryption.
+            tweak (bytes): A bytes object containing the tweak to be used for the encryption.
+            plaintext (str): A string containing the plaintext to be encrypted.
 
-        :param key: A bytes object containing the key to be used for the encryption.
-        :param tweak: A bytes object containing the tweak to be used for the encryption.
-        :param plaintext: A string containing the plaintext to be encrypted.
-        :return: A string containing the ciphertext produced by encrypting the plaintext
-        using the specified key and tweak.
+        Returns:
+            str: A string containing the ciphertext produced by encrypting the plaintext
+                using the specified key and tweak.
         """
     def decrypt(self, key: bytes, tweak: bytes, ciphertext: str) -> str:
         """
-        Decrypt a ciphertext using the specified key and tweak.
+        Decrypts a ciphertext using the specified key and tweak.
 
-        :param key: A bytes object containing the key to be used for the decryption.
-        :param tweak: A bytes object containing the tweak to be used for the decryption.
-        :param ciphertext: A string containing the ciphertext to be decrypted.
-        :return: A string containing the plaintext produced by decrypting the ciphertext
-        using the specified key and tweak.
+        Args:
+            key (bytes): A bytes object containing the key to be used for the decryption.
+            tweak (bytes): A bytes object containing the tweak to be used for the decryption.
+            ciphertext (str): A string containing the ciphertext to be decrypted.
+
+        Returns:
+            str: A string containing the plaintext produced by decrypting the ciphertext
+                using the specified key and tweak.
         """
     def extend_with(self, additional_characters: str) -> None:
         """
         Extends the current alphabet with additional characters.
 
         Args:
-            additional_characters (str): A string containing the additional
-            characters to add to the alphabet.
+            additional_characters (str): A string containing the additional characters
+                to add to the alphabet.
 
         Returns:
             None: This method does not return anything.
         """
 
 class Integer:
     """
     A class that represents an integer in a finite field and provides
     methods for encryption and decryption using the FPE (Format Preserving
     Encryption) algorithm.
 
     Parameters:
         radix (int): The radix used for the integer.
         digits (int): The number of digits used for the integer.
-
-    Methods:
-        encrypt(key: bytes, tweak: bytes, plaintext: int) -> int:
-            Encrypts a plaintext integer using the FPE algorithm with the
-            given key and tweak.
-
-        decrypt(key: bytes, tweak: bytes, ciphertext: int) -> int:
-            Decrypts a ciphertext integer using the FPE algorithm with the
-            given key and tweak.
-
-        encrypt_big(key: bytes, tweak: bytes, plaintext: str) -> str:
-            Encrypts a plaintext string using the FPE algorithm with the
-            given key and tweak. The plaintext string is first converted to
-            a big integer using the radix of the Integer instance.
-
-        decrypt_big(key: bytes, tweak: bytes, ciphertext: str) -> str:
-            Decrypts a ciphertext string using the FPE algorithm with the
-            given key and tweak. The ciphertext string is first converted to
-            a big integer using the radix of the Integer instance.
     """
 
     def __init__(self, radix: int, digits: int):
         """
         Initializes a new Integer object with the given radix and number of digits.
 
         Args:
@@ -144,40 +132,39 @@
             str: The decrypted string.
         """
 
 class Float:
     """
     A class representing a floating point number and providing methods for
     encrypting and decrypting floating point numbers using a specified key and tweak.
-
-    Methods:
-        encrypt(key: bytes, tweak: bytes, plaintext: int) -> int:
-            Encrypts a plaintext floating point number using the specified key and tweak.
-
-        decrypt(key: bytes, tweak: bytes, ciphertext: int) -> int:
-            Decrypts a ciphertext floating point number using the specified key and tweak.
     """
 
     def __init__(self):
         """
         Initializes a new Float object.
         """
     def encrypt(self, key: bytes, tweak: bytes, plaintext: float) -> float:
         """
         Encrypts the given plaintext floating point number using the specified key and tweak,
         and returns the ciphertext.
 
-        :param key: A bytes object representing the encryption key.
-        :param tweak: A bytes object representing the encryption tweak.
-        :param plaintext: An int representing the plaintext floating point number to encrypt.
-        :return: An int representing the ciphertext value.
+        Args:
+            key (bytes): A bytes object representing the encryption key.
+            tweak (bytes): A bytes object representing the encryption tweak.
+            plaintext (float): A float representing the plaintext floating point number to encrypt.
+
+        Returns:
+            float: A float representing the ciphertext value.
         """
     def decrypt(self, key: bytes, tweak: bytes, ciphertext: float) -> float:
         """
         Decrypts the given ciphertext floating point number using the specified key and tweak,
         and returns the plaintext.
 
-        :param key: A bytes object representing the encryption key.
-        :param tweak: A bytes object representing the encryption tweak.
-        :param ciphertext: An int representing the ciphertext value to decrypt.
-        :return: An int representing the plaintext floating point number.
+        Args:
+            key (bytes): A bytes object representing the encryption key.
+            tweak (bytes): A bytes object representing the encryption tweak.
+            ciphertext (float): A float representing the ciphertext value to decrypt.
+
+        Returns:
+            float: the plaintext floating point number.
         """
```

## Comparing `cloudproof_fpe-0.1.0.dist-info/METADATA` & `cloudproof_fpe-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cloudproof_fpe
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: cffi
+License-File: LICENSE.md
 Summary: Cosmian Cloudproof FPE library
 Author: Théophile Brézot<theophile.brezot@cosmian.com>
 Author-email: Théophile Brézot<theophile.brezot@cosmian.com>
-License: MIT/Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/cosmian/cloudproof_rust/
 
 # Format Preserving Encryption
 
 This library provides `Format Preserving Encryption` (FPE) techniques for use in a zero-trust environment. These techniques are based on FPE-FF1 which is described in [NIST:800-38G](https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-38g.pdf).
 
 <!-- toc -->
```

## Comparing `cloudproof_fpe-0.1.0.dist-info/RECORD` & `cloudproof_fpe-0.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-cloudproof_fpe-0.1.0.dist-info/METADATA,sha256=cR_jryJmFeut98lGb6LeQQyl2Jp-7a0EAm0DStmMmwE,8286
-cloudproof_fpe-0.1.0.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
-cloudproof_fpe/__init__.py,sha256=Ftbrv3gmtkLB3qesCINBGE38IczafGD83Lq9K2pjPC4,164
+cloudproof_fpe-0.2.0.dist-info/METADATA,sha256=f8P6dwHnkp4mZ0V_Ng6yqSx1BGUyGLcNscP5QuCAFUw,8357
+cloudproof_fpe-0.2.0.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+cloudproof_fpe-0.2.0.dist-info/license_files/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
+cloudproof_fpe/__init__.pyi,sha256=2ygKnpQUMr121Vc8qJCDmDl_Xuv8ikbNQw4YUrjJEfc,6428
 cloudproof_fpe/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
-cloudproof_fpe/__init__.pyi,sha256=q-XG-0f4A1OfeO1vfsW1-FDnx1ClunisV2F7kXRQrjg,7440
-cloudproof_fpe/cloudproof_fpe.pyd,sha256=bGkcT3fglB1kDyczjO-zCc37sENTWtRMeVNIG9LvEBY,529920
-cloudproof_fpe-0.1.0.dist-info/RECORD,,
+cloudproof_fpe/__init__.py,sha256=Ftbrv3gmtkLB3qesCINBGE38IczafGD83Lq9K2pjPC4,164
+cloudproof_fpe/cloudproof_fpe.pyd,sha256=P8oMkD-0VAroNj4AKAG92IlWux3EuOBb6JJ2Fd3SGeg,545792
+cloudproof_fpe-0.2.0.dist-info/RECORD,,
```

