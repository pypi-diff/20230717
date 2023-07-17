# Comparing `tmp/simple2encrypt-1.5.7.tar.gz` & `tmp/simple2encrypt-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.7.tar", last modified: Mon Jul 17 09:54:31 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.8.tar", last modified: Mon Jul 17 10:42:13 2023, max compression
```

## Comparing `simple2encrypt-1.5.7.tar` & `simple2encrypt-1.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.7/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     8316 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.7/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.7/example_decrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.7/example_encrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.7/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     8831 2023-07-17 09:54:17.000000 simple2encrypt-1.5.7/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     8316 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)     9433 2023-07-17 09:31:45.000000 simple2encrypt-1.5.7/simple2encrypt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 10:42:13.372395 simple2encrypt-1.5.8/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.8/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     8370 2023-07-17 10:42:13.372395 simple2encrypt-1.5.8/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.8/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.8/example_decrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.8/example_encrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.8/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 10:42:13.372395 simple2encrypt-1.5.8/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     8885 2023-07-17 10:41:54.000000 simple2encrypt-1.5.8/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 10:42:13.368395 simple2encrypt-1.5.8/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     8370 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 10:42:13.000000 simple2encrypt-1.5.8/simple2encrypt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     9433 2023-07-17 10:42:00.000000 simple2encrypt-1.5.8/simple2encrypt.py
```

### Comparing `simple2encrypt-1.5.7/LICENSE` & `simple2encrypt-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.7/PKG-INFO` & `simple2encrypt-1.5.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1
-Name: simple2encrypt
-Version: 1.5.7
-Summary: Utility functions for encryption and file operations
-Home-page: https://github.com/nhman-python/crypto-utils
-Author: nhman-python
-Author-email: wbgblfix@duck.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+from setuptools import setup
 
+description = """
 ---
 
 # simple2encrypt
 
 `simple2encrypt` is a Python library that provides utility functions for encryption and file operations. It includes 
 functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and 
 writing binary data from/to files, and handling user input.
@@ -45,15 +36,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of encrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 encrypt_walk_dirs(folder_path, key)
 print("Folder encryption completed.")
@@ -69,15 +60,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of decrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 decrypt_walk_dirs(folder_path, key)
 print("Folder decryption completed.")
@@ -92,15 +83,15 @@
 def folder_encrypt(folder_path: str, key: bytes, add_extension: str = '.enc') -> None:
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be encrypted.
 - `key` (bytes): The key used for encryption.
 - `add_extension` (str): Optional. The extension to add to the end of the encrypted files. Defaults to '.enc'.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of folder_encrypt function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 folder_encrypt(folder_path, key)
 print("Folder encryption completed.")
@@ -113,93 +104,93 @@
 def folder_decrypt(folder_path: str, key: bytes) -> None:
 
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be decrypted.
 - `key` (bytes): The key used for decryption.
 
-** Example Usage: **
+**Example Usage:**
 ```
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 folder_decrypt(folder_path, key)
 print("Folder decryption completed.")
 ```
 These functions traverse through the specified folder path and perform encryption or decryption on all files within the folder. The `folder_encrypt` function encrypts the files using the provided key and adds an optional extension to the encrypted files. The `folder_decrypt` function decrypts the files using the provided key and removes any file extensions.
 
 Both functions raise a `ValueError` if the provided folder path is not a directory.
 
-### ** Other Utility Functions **
+### **Other Utility Functions**
 
 
 #### `delete_extension(file_path: str) -> str`
 
 Removes the file extension from the given file path and returns the resulting filename without the extension.
 
 - `file_path` (str): The path of the file with an extension.
 
-** Example Usage: **
+**Example Usage:**
 ```
 path = '/my_secret/folder/file.txt.enc'  # File path with extension
 file_name = delete_extension(path)
 print("File name without extension:", file_name)
 # output /my_secret/folder/file.txt
 ```
 
 #### `generate_key(password: str, length: int) -> bytes`
 
 Generates an encryption key based on the provided password and length.
 
 - `password` (str): The password for key generation.
 - `length` (int): The length of the key (choose from [16, 24, 32]).
 
-** Example Usage: **
+**Example Usage:**
 ```
 password = 'mysecretpassword'  # Password for key generation
 key = generate_key(password, length=32)
 print("Generated key:", key)
 write_binary('new-key.bin', key)
 ```
 
 #### `read_binary(file_path: str) -> bytes`
 
 Reads binary data from the specified file and returns it as bytes.
 
 - `file_path` (str): The path of the file to read.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to read
 data = read_binary(file_path)
 print("Read data:", data)
 ```
 
 #### `write_binary(file_path: str, data: bytes) -> None`
 
 Writes the given binary data to the specified file.
 
 - `file_path` (str): The path of the file to write.
 - `data` (bytes): The binary data to write.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to write
 data = write_binary(file_path, data)
 print("Write data:", data)
 print("Data written to file successfully.")
 ```
 
 #### `custom_input(question: str) -> str`
 
 Prompts the user with the provided question and returns their input as a string.
 
 - `question` (str): The question to ask the user.
 
-** Example Usage: **
+**Example Usage:**
 ```
 question = "Enter your name: "
 user_name = custom_input(question)
 print("User name:", user_name)
 ```
 
 ### Command-Line Interface
@@ -240,15 +231,38 @@
 This command will decrypt the encrypted file at `file_path` using the encryption key at `key_path`. The decrypted 
 file will replace the original encrypted file.
 
 **Note:** Ensure that the necessary file paths and encryption keys are provided for the command-line interface to work correctly.
 
 ## Version
 
-The current version of `simple2encrypt` is 1.5.7
+The current version of `simple2encrypt` is 1.5.8
 
 ## License
 
 This library is distributed under the MIT License. See the [LICENSE](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE) file for more information.
 
+join us on telegram [@python_tip_israel](https://t.me/python_tip_israel)
+
 ---
 
+"""
+
+setup(
+    name='simple2encrypt',
+    version='1.5.8',
+    description='Utility functions for encryption and file operations',
+    author='nhman-python',
+    author_email='wbgblfix@duck.com',
+    url='https://github.com/nhman-python/crypto-utils',
+    license='MIT',
+    long_description=description,
+    long_description_content_type='text/markdown',
+    py_modules=['simple2encrypt', 'example_message', 'example_encrypt', 'example_decrypt'],
+    install_requires=[
+        'pycryptodome',  # Dependency on pycryptodome package
+    ],
+    entry_points={
+        'console_scripts': ['aes-key = simple2encrypt:main', 'aes-message = example_message:main',
+                            'aes-encrypt = example_encrypt:main', 'aes-decrypt = example_decrypt:main'],
+    },
+)
```

### Comparing `simple2encrypt-1.5.7/example_decrypt.py` & `simple2encrypt-1.5.8/example_decrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.7/example_encrypt.py` & `simple2encrypt-1.5.8/example_encrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.7/example_message.py` & `simple2encrypt-1.5.8/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.7/setup.py` & `simple2encrypt-1.5.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-from setuptools import setup
+Metadata-Version: 2.1
+Name: simple2encrypt
+Version: 1.5.8
+Summary: Utility functions for encryption and file operations
+Home-page: https://github.com/nhman-python/crypto-utils
+Author: nhman-python
+Author-email: wbgblfix@duck.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
-description = """
 ---
 
 # simple2encrypt
 
 `simple2encrypt` is a Python library that provides utility functions for encryption and file operations. It includes 
 functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and 
 writing binary data from/to files, and handling user input.
@@ -36,15 +45,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of encrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 encrypt_walk_dirs(folder_path, key)
 print("Folder encryption completed.")
@@ -60,15 +69,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of decrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 decrypt_walk_dirs(folder_path, key)
 print("Folder decryption completed.")
@@ -83,15 +92,15 @@
 def folder_encrypt(folder_path: str, key: bytes, add_extension: str = '.enc') -> None:
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be encrypted.
 - `key` (bytes): The key used for encryption.
 - `add_extension` (str): Optional. The extension to add to the end of the encrypted files. Defaults to '.enc'.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of folder_encrypt function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 folder_encrypt(folder_path, key)
 print("Folder encryption completed.")
@@ -104,93 +113,93 @@
 def folder_decrypt(folder_path: str, key: bytes) -> None:
 
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be decrypted.
 - `key` (bytes): The key used for decryption.
 
-** Example Usage: **
+**Example Usage:**
 ```
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 folder_decrypt(folder_path, key)
 print("Folder decryption completed.")
 ```
 These functions traverse through the specified folder path and perform encryption or decryption on all files within the folder. The `folder_encrypt` function encrypts the files using the provided key and adds an optional extension to the encrypted files. The `folder_decrypt` function decrypts the files using the provided key and removes any file extensions.
 
 Both functions raise a `ValueError` if the provided folder path is not a directory.
 
-### ** Other Utility Functions **
+### **Other Utility Functions**
 
 
 #### `delete_extension(file_path: str) -> str`
 
 Removes the file extension from the given file path and returns the resulting filename without the extension.
 
 - `file_path` (str): The path of the file with an extension.
 
-** Example Usage: **
+**Example Usage:**
 ```
 path = '/my_secret/folder/file.txt.enc'  # File path with extension
 file_name = delete_extension(path)
 print("File name without extension:", file_name)
 # output /my_secret/folder/file.txt
 ```
 
 #### `generate_key(password: str, length: int) -> bytes`
 
 Generates an encryption key based on the provided password and length.
 
 - `password` (str): The password for key generation.
 - `length` (int): The length of the key (choose from [16, 24, 32]).
 
-** Example Usage: **
+**Example Usage:**
 ```
 password = 'mysecretpassword'  # Password for key generation
 key = generate_key(password, length=32)
 print("Generated key:", key)
 write_binary('new-key.bin', key)
 ```
 
 #### `read_binary(file_path: str) -> bytes`
 
 Reads binary data from the specified file and returns it as bytes.
 
 - `file_path` (str): The path of the file to read.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to read
 data = read_binary(file_path)
 print("Read data:", data)
 ```
 
 #### `write_binary(file_path: str, data: bytes) -> None`
 
 Writes the given binary data to the specified file.
 
 - `file_path` (str): The path of the file to write.
 - `data` (bytes): The binary data to write.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to write
 data = write_binary(file_path, data)
 print("Write data:", data)
 print("Data written to file successfully.")
 ```
 
 #### `custom_input(question: str) -> str`
 
 Prompts the user with the provided question and returns their input as a string.
 
 - `question` (str): The question to ask the user.
 
-** Example Usage: **
+**Example Usage:**
 ```
 question = "Enter your name: "
 user_name = custom_input(question)
 print("User name:", user_name)
 ```
 
 ### Command-Line Interface
@@ -231,36 +240,17 @@
 This command will decrypt the encrypted file at `file_path` using the encryption key at `key_path`. The decrypted 
 file will replace the original encrypted file.
 
 **Note:** Ensure that the necessary file paths and encryption keys are provided for the command-line interface to work correctly.
 
 ## Version
 
-The current version of `simple2encrypt` is 1.5.7
+The current version of `simple2encrypt` is 1.5.8
 
 ## License
 
 This library is distributed under the MIT License. See the [LICENSE](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE) file for more information.
 
----
+join us on telegram [@python_tip_israel](https://t.me/python_tip_israel)
 
-"""
+---
 
-setup(
-    name='simple2encrypt',
-    version='1.5.7',
-    description='Utility functions for encryption and file operations',
-    author='nhman-python',
-    author_email='wbgblfix@duck.com',
-    url='https://github.com/nhman-python/crypto-utils',
-    license='MIT',
-    long_description=description,
-    long_description_content_type='text/markdown',
-    py_modules=['simple2encrypt', 'example_message', 'example_encrypt', 'example_decrypt'],
-    install_requires=[
-        'pycryptodome',  # Dependency on pycryptodome package
-    ],
-    entry_points={
-        'console_scripts': ['aes-key = simple2encrypt:main', 'aes-message = example_message:main',
-                            'aes-encrypt = example_encrypt:main', 'aes-decrypt = example_decrypt:main'],
-    },
-)
```

### Comparing `simple2encrypt-1.5.7/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.5.8/simple2encrypt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.7
+Version: 1.5.8
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,15 +45,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of encrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 encrypt_walk_dirs(folder_path, key)
 print("Folder encryption completed.")
@@ -69,15 +69,15 @@
 **Raises:**
 
 - `PermissionError`: If there is a permission error while accessing or modifying files.
 - `FileExistsError`: If a file with the new name already exists in the destination.
 - `FileNotFoundError`: If the specified file is not found.
 - `ValueError`: If there is an error in the provided data or key.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of decrypt_walk_dirs function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 decrypt_walk_dirs(folder_path, key)
 print("Folder decryption completed.")
@@ -92,15 +92,15 @@
 def folder_encrypt(folder_path: str, key: bytes, add_extension: str = '.enc') -> None:
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be encrypted.
 - `key` (bytes): The key used for encryption.
 - `add_extension` (str): Optional. The extension to add to the end of the encrypted files. Defaults to '.enc'.
 
-** Example Usage: **
+**Example Usage:**
 ```
 # Example usage of folder_encrypt function
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be encrypted
 key = b'mysecretpassword'  # Encryption key need to be in this length [16, 24, 32] bit
 
 folder_encrypt(folder_path, key)
 print("Folder encryption completed.")
@@ -113,93 +113,93 @@
 def folder_decrypt(folder_path: str, key: bytes) -> None:
 
 ```
 
 - `folder_path` (str): The path to the folder containing the files to be decrypted.
 - `key` (bytes): The key used for decryption.
 
-** Example Usage: **
+**Example Usage:**
 ```
 folder_path = '/my_secret/folder'  # Path to the folder containing files to be decrypted
 key = b'mysecretpassword'  # Decryption key need to be in this length [16, 24, 32] bit
 
 folder_decrypt(folder_path, key)
 print("Folder decryption completed.")
 ```
 These functions traverse through the specified folder path and perform encryption or decryption on all files within the folder. The `folder_encrypt` function encrypts the files using the provided key and adds an optional extension to the encrypted files. The `folder_decrypt` function decrypts the files using the provided key and removes any file extensions.
 
 Both functions raise a `ValueError` if the provided folder path is not a directory.
 
-### ** Other Utility Functions **
+### **Other Utility Functions**
 
 
 #### `delete_extension(file_path: str) -> str`
 
 Removes the file extension from the given file path and returns the resulting filename without the extension.
 
 - `file_path` (str): The path of the file with an extension.
 
-** Example Usage: **
+**Example Usage:**
 ```
 path = '/my_secret/folder/file.txt.enc'  # File path with extension
 file_name = delete_extension(path)
 print("File name without extension:", file_name)
 # output /my_secret/folder/file.txt
 ```
 
 #### `generate_key(password: str, length: int) -> bytes`
 
 Generates an encryption key based on the provided password and length.
 
 - `password` (str): The password for key generation.
 - `length` (int): The length of the key (choose from [16, 24, 32]).
 
-** Example Usage: **
+**Example Usage:**
 ```
 password = 'mysecretpassword'  # Password for key generation
 key = generate_key(password, length=32)
 print("Generated key:", key)
 write_binary('new-key.bin', key)
 ```
 
 #### `read_binary(file_path: str) -> bytes`
 
 Reads binary data from the specified file and returns it as bytes.
 
 - `file_path` (str): The path of the file to read.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to read
 data = read_binary(file_path)
 print("Read data:", data)
 ```
 
 #### `write_binary(file_path: str, data: bytes) -> None`
 
 Writes the given binary data to the specified file.
 
 - `file_path` (str): The path of the file to write.
 - `data` (bytes): The binary data to write.
 
-** Example Usage: **
+**Example Usage:**
 ```
 file_path = '/new-key.bin'  # Path of the file to write
 data = write_binary(file_path, data)
 print("Write data:", data)
 print("Data written to file successfully.")
 ```
 
 #### `custom_input(question: str) -> str`
 
 Prompts the user with the provided question and returns their input as a string.
 
 - `question` (str): The question to ask the user.
 
-** Example Usage: **
+**Example Usage:**
 ```
 question = "Enter your name: "
 user_name = custom_input(question)
 print("User name:", user_name)
 ```
 
 ### Command-Line Interface
@@ -240,15 +240,17 @@
 This command will decrypt the encrypted file at `file_path` using the encryption key at `key_path`. The decrypted 
 file will replace the original encrypted file.
 
 **Note:** Ensure that the necessary file paths and encryption keys are provided for the command-line interface to work correctly.
 
 ## Version
 
-The current version of `simple2encrypt` is 1.5.7
+The current version of `simple2encrypt` is 1.5.8
 
 ## License
 
 This library is distributed under the MIT License. See the [LICENSE](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE) file for more information.
 
+join us on telegram [@python_tip_israel](https://t.me/python_tip_israel)
+
 ---
```

### Comparing `simple2encrypt-1.5.7/simple2encrypt.py` & `simple2encrypt-1.5.8/simple2encrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.7'
+__version__ = '1.5.8'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
```

