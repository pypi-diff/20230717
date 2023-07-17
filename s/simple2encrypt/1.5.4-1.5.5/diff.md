# Comparing `tmp/simple2encrypt-1.5.4.tar.gz` & `tmp/simple2encrypt-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.4.tar", last modified: Mon Jul 17 02:44:58 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.5.tar", last modified: Mon Jul 17 03:03:21 2023, max compression
```

## Comparing `simple2encrypt-1.5.4.tar` & `simple2encrypt-1.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 02:44:58.980712 simple2encrypt-1.5.4/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 02:44:58.980712 simple2encrypt-1.5.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.4/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.4/example_decrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.4/example_encrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.4/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 02:44:58.980712 simple2encrypt-1.5.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     5124 2023-07-17 02:44:28.000000 simple2encrypt-1.5.4/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 02:44:58.980712 simple2encrypt-1.5.4/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      155 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 02:44:58.000000 simple2encrypt-1.5.4/simple2encrypt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)     6246 2023-07-17 02:25:16.000000 simple2encrypt-1.5.4/simple2encrypt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.5/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.5/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.5/example_decrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.5/example_encrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.5/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     5122 2023-07-17 03:03:04.000000 simple2encrypt-1.5.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     6246 2023-07-17 03:03:04.000000 simple2encrypt-1.5.5/simple2encrypt.py
```

### Comparing `simple2encrypt-1.5.4/LICENSE` & `simple2encrypt-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.4/PKG-INFO` & `simple2encrypt-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.4
+Version: 1.5.5
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -160,14 +160,14 @@
 
 To decrypt file:
 ```
 aes-decrypt [file_path] [key_path]
 ```
 ## Version
 
-The current version of `encryption_utils` is 1.5.4
+The current version of `encryption_utils` is 1.5.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.5.4/example_decrypt.py` & `simple2encrypt-1.5.5/example_decrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.4/example_encrypt.py` & `simple2encrypt-1.5.5/example_encrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.4/example_message.py` & `simple2encrypt-1.5.5/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.4/setup.py` & `simple2encrypt-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,35 +151,35 @@
 
 To decrypt file:
 ```
 aes-decrypt [file_path] [key_path]
 ```
 ## Version
 
-The current version of `encryption_utils` is 1.5.4
+The current version of `encryption_utils` is 1.5.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.5.4',
+    version='1.5.5',
     description='Utility functions for encryption and file operations',
     author='nhman-python',
     author_email='wbgblfix@duck.com',
     url='https://github.com/nhman-python/crypto-utils',
     license='MIT',
     long_description=description,
     long_description_content_type='text/markdown',
     py_modules=['simple2encrypt', 'example_message', 'example_encrypt', 'example_decrypt'],
     install_requires=[
         'pycryptodome',  # Dependency on pycryptodome package
     ],
     entry_points={
-        'console_scripts': ['aes-key = encryption_utils:main', 'aes-message = example_message:main',
+        'console_scripts': ['aes-key = simple2encrypt:main', 'aes-message = example_message:main',
                             'aes-encrypt = example_encrypt:main', 'aes-decrypt = example_decrypt:main'],
     },
 )
```

### Comparing `simple2encrypt-1.5.4/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.5.5/simple2encrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.4
+Version: 1.5.5
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -160,14 +160,14 @@
 
 To decrypt file:
 ```
 aes-decrypt [file_path] [key_path]
 ```
 ## Version
 
-The current version of `encryption_utils` is 1.5.4
+The current version of `encryption_utils` is 1.5.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.5.4/simple2encrypt.py` & `simple2encrypt-1.5.5/simple2encrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.4'
+__version__ = '1.5.5'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
```

