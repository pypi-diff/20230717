# Comparing `tmp/simple2encrypt-1.5.2.tar.gz` & `tmp/simple2encrypt-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.2.tar", last modified: Mon Jul 17 01:03:36 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.3.tar", last modified: Mon Jul 17 01:15:20 2023, max compression
```

## Comparing `simple2encrypt-1.5.2.tar` & `simple2encrypt-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:03:36.508540 simple2encrypt-1.5.2/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-17 01:03:36.504540 simple2encrypt-1.5.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     6245 2023-07-17 01:02:46.000000 simple2encrypt-1.5.2/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1305 2023-07-16 21:48:50.000000 simple2encrypt-1.5.2/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 01:03:36.508540 simple2encrypt-1.5.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3909 2023-07-17 01:03:01.000000 simple2encrypt-1.5.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:03:36.504540 simple2encrypt-1.5.2/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:15:20.040560 simple2encrypt-1.5.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4487 2023-07-17 01:15:20.040560 simple2encrypt-1.5.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     6246 2023-07-17 01:11:11.000000 simple2encrypt-1.5.3/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1305 2023-07-16 21:48:50.000000 simple2encrypt-1.5.3/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 01:15:20.040560 simple2encrypt-1.5.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     4866 2023-07-17 01:14:39.000000 simple2encrypt-1.5.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:15:20.040560 simple2encrypt-1.5.3/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4487 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-17 01:15:19.000000 simple2encrypt-1.5.3/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.5.2/LICENSE` & `simple2encrypt-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.2/PKG-INFO` & `simple2encrypt-1.5.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.2
+Version: 1.5.3
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,14 +24,44 @@
 pip install simple2encrypt
 ```
 
 ## Usage
 simple2encrypt
 ### Encryption
 
+folder_encrypt
+--------------
+
+.. py:function:: folder_encrypt(folder_path: str, key: bytes, add_extension: str = '.enc') -> None
+
+   Encrypts all files within a given folder.
+
+   :param folder_path: Path to the folder containing the files to be encrypted.
+   :type folder_path: str
+   :param key: The key for encryption.
+   :type key: bytes
+   :param add_extension: Add the extension to the end of the file (default: '.enc')
+   :type add_extension: str, optional
+   :raises ValueError: If the provided folder path is not a directory.
+   :returns: None
+
+folder_decrypt
+--------------
+
+.. py:function:: folder_decrypt(folder_path: str, key: bytes) -> None
+
+   Decrypts all files within a given folder.
+
+   :param folder_path: Path to the folder containing the files to be decrypted.
+   :type folder_path: str
+   :param key: The key for decryption.
+   :type key: bytes
+   :raises ValueError: If the provided folder path is not a directory.
+   :returns: None
+
 
 To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the 
 library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
@@ -120,14 +150,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5.2
+The current version of `encryption_utils` is 1.5.3
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.5.2/encryption_utils.py` & `simple2encrypt-1.5.3/encryption_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.2'
+__version__ = '1.5.3'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
@@ -82,18 +82,18 @@
     if not os.path.isdir(folder_path):
         raise ValueError("Expected a folder path, but received a different type of path.")
 
     for file in os.listdir(folder_path):
         full_path = os.path.join(folder_path, file)
         if os.path.isfile(full_path):
             data = read_binary(full_path)
-            encryption = Encryption(key, data)
-            encrypted_data = encryption.encrypt()
+            decryption = Encryption(key, data)
+            decrypted_data = decryption.decrypt()
             new_file_path = delete_extension(full_path)
-            write_binary(new_file_path, encrypted_data)
+            write_binary(new_file_path, decrypted_data)
             os.remove(full_path)
 
 
 def delete_extension(path: str) -> str:
     """
     Remove the last file extension from a path.
 
@@ -177,15 +177,15 @@
     parser.add_argument('password', type=str, help='Password for key generation')
     args = parser.parse_args()
     password = args.password
     file_name = args.filename
     try:
         key = generate_key(password, length=32)
         write_binary(file_name, key)
-        print(f"A new file was created based on your password. The file name is: {key_path}")
+        print(f"A new file was created based on your password. The file name is: {file_name}")
     except (ValueError, FileExistsError, FileNotFoundError) as write_error:
         print(write_error)
         sys.exit()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `simple2encrypt-1.5.2/example_message.py` & `simple2encrypt-1.5.3/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.2/setup.py` & `simple2encrypt-1.5.3/simple2encrypt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-from setuptools import setup
+Metadata-Version: 2.1
+Name: simple2encrypt
+Version: 1.5.3
+Summary: Utility functions for encryption and file operations
+Home-page: https://github.com/nhman-python/crypto-utils
+Author: nhman-python
+Author-email: wbgblfix@duck.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
-description = """
 # Encryption Utils
 
 `encryption_utils` is a Python library that provides utility functions for encryption and file operations. It 
 includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, 
 reading and writing binary data from/to files, and handling user input.
 
 ## Installation
@@ -15,14 +24,44 @@
 pip install simple2encrypt
 ```
 
 ## Usage
 simple2encrypt
 ### Encryption
 
+folder_encrypt
+--------------
+
+.. py:function:: folder_encrypt(folder_path: str, key: bytes, add_extension: str = '.enc') -> None
+
+   Encrypts all files within a given folder.
+
+   :param folder_path: Path to the folder containing the files to be encrypted.
+   :type folder_path: str
+   :param key: The key for encryption.
+   :type key: bytes
+   :param add_extension: Add the extension to the end of the file (default: '.enc')
+   :type add_extension: str, optional
+   :raises ValueError: If the provided folder path is not a directory.
+   :returns: None
+
+folder_decrypt
+--------------
+
+.. py:function:: folder_decrypt(folder_path: str, key: bytes) -> None
+
+   Decrypts all files within a given folder.
+
+   :param folder_path: Path to the folder containing the files to be decrypted.
+   :type folder_path: str
+   :param key: The key for decryption.
+   :type key: bytes
+   :raises ValueError: If the provided folder path is not a directory.
+   :returns: None
+
 
 To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the 
 library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
@@ -111,34 +150,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5.2
+The current version of `encryption_utils` is 1.5.3
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
 
-"""
-
-setup(
-    name='simple2encrypt',
-    version='1.5.2',
-    description='Utility functions for encryption and file operations',
-    author='nhman-python',
-    author_email='wbgblfix@duck.com',
-    url='https://github.com/nhman-python/crypto-utils',
-    license='MIT',
-    long_description=description,
-    long_description_content_type='text/markdown',
-    py_modules=['encryption_utils', 'example_message'],
-    install_requires=[
-        'pycryptodome',  # Dependency on pycryptodome package
-    ],
-    entry_points={
-        'console_scripts': ['aes-key = encryption_utils:main', 'aes-message = example_message:main', ],
-    },
-)
```

