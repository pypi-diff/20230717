# Comparing `tmp/simple2encrypt-1.5.1.tar.gz` & `tmp/simple2encrypt-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.1.tar", last modified: Sun Jul 16 21:52:43 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.2.tar", last modified: Mon Jul 17 01:03:36 2023, max compression
```

## Comparing `simple2encrypt-1.5.1.tar` & `simple2encrypt-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     5318 2023-07-16 21:52:21.000000 simple2encrypt-1.5.1/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1305 2023-07-16 21:48:50.000000 simple2encrypt-1.5.1/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3909 2023-07-16 21:50:43.000000 simple2encrypt-1.5.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:03:36.508540 simple2encrypt-1.5.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-17 01:03:36.504540 simple2encrypt-1.5.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     6245 2023-07-17 01:02:46.000000 simple2encrypt-1.5.2/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1305 2023-07-16 21:48:50.000000 simple2encrypt-1.5.2/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 01:03:36.508540 simple2encrypt-1.5.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3909 2023-07-17 01:03:01.000000 simple2encrypt-1.5.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 01:03:36.504540 simple2encrypt-1.5.2/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-17 01:03:36.000000 simple2encrypt-1.5.2/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.5.1/LICENSE` & `simple2encrypt-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.1/PKG-INFO` & `simple2encrypt-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.1
+Version: 1.5.2
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,14 +120,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5.1
+The current version of `encryption_utils` is 1.5.2
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.5.1/encryption_utils.py` & `simple2encrypt-1.5.2/encryption_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
-    def __init__(self, key, data):
+    def __init__(self, key: bytes, data: bytes):
         """
         Initialize the Encryption object with the key and data.
         :param key: Encryption key
         :param data: Data to be encrypted or decrypted
         """
         self.key = key
         self.data = data
 
-    def encrypt(self):
+    def encrypt(self) -> bytes:
         """
         Encrypt the data using the AES algorithm.
         :return: Encrypted data
         """
         cipher = AES.new(self.key, AES.MODE_CBC)
         encrypted_data = cipher.encrypt(pad(self.data, cipher.block_size))
         return cipher.iv + encrypted_data
 
-    def decrypt(self):
+    def decrypt(self) -> bytes:
         """
         Decrypt the data using the AES algorithm.
         :return: Decrypted data
         """
         initialization_vector = self.data[:AES.block_size]  # Extract the IV from the data
         cipher = AES.new(self.key, AES.MODE_CBC, iv=initialization_vector)
         decrypted_data = cipher.decrypt(self.data[AES.block_size:])
@@ -57,21 +57,44 @@
     :param key: The key for encryption.
     :raises ValueError: If the provided folder path is not a directory.
     """
     if not os.path.isdir(folder_path):
         raise ValueError("Expected a folder path, but received a different type of path.")
 
     for file in os.listdir(folder_path):
-        file_path = os.path.join(folder_path, file)
-        if os.path.isfile(file_path):
-            data = read_binary(file_path)
+        full_path = os.path.join(folder_path, file)
+        if os.path.isfile(full_path):
+            data = read_binary(full_path)
             encryption = Encryption(key, data)
             encrypted_data = encryption.encrypt()
-            new_file_path = file_path + add_extension
+            new_file_path = full_path + add_extension
             write_binary(new_file_path, encrypted_data)
+            os.remove(full_path)
+
+
+def folder_dencrypt(folder_path: str, key: bytes) -> None:
+    """
+    Decrypts all files within a given folder.
+
+    :param folder_path: Path to the folder containing the files to be decrypted.
+    :param key: The key for decryption.
+    :raises ValueError: If the provided folder path is not a directory.
+    """
+    if not os.path.isdir(folder_path):
+        raise ValueError("Expected a folder path, but received a different type of path.")
+
+    for file in os.listdir(folder_path):
+        full_path = os.path.join(folder_path, file)
+        if os.path.isfile(full_path):
+            data = read_binary(full_path)
+            encryption = Encryption(key, data)
+            encrypted_data = encryption.encrypt()
+            new_file_path = delete_extension(full_path)
+            write_binary(new_file_path, encrypted_data)
+            os.remove(full_path)
 
 
 def delete_extension(path: str) -> str:
     """
     Remove the last file extension from a path.
 
     :param path: The file path
@@ -110,15 +133,15 @@
         raise FileNotFoundError(f"File '{file_path}' not found.")
     if os.path.isdir(file_path):
         raise ValueError("Path is a directory. File path is expected.")
     with open(file_path, 'rb') as f:
         return f.read()
 
 
-def write_binary(file_path, data):
+def write_binary(file_path, data) -> bool:
     """
     Write binary data to a file.
     :param file_path: Path of the file to write the data to
     :param data:  write
     :return: True if the file was saved successfully
     """
     if os.path.exists(file_path):
@@ -149,20 +172,19 @@
     the main function calls it to create the secret key
     :return:
     """
     parser = argparse.ArgumentParser(prog='encrypt data', description='create new encryption key')
     parser.add_argument('filename', type=str, help='name of the secret file to save example my-key.key')
     parser.add_argument('password', type=str, help='Password for key generation')
     args = parser.parse_args()
-
+    password = args.password
     file_name = args.filename
     try:
-        key = generate_key(args.password, length=32)
-        key_path = args.filename
-        write_binary(key_path, key)
+        key = generate_key(password, length=32)
+        write_binary(file_name, key)
         print(f"A new file was created based on your password. The file name is: {key_path}")
     except (ValueError, FileExistsError, FileNotFoundError) as write_error:
         print(write_error)
         sys.exit()
 
 
 if __name__ == '__main__':
```

### Comparing `simple2encrypt-1.5.1/example_message.py` & `simple2encrypt-1.5.2/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.1/setup.py` & `simple2encrypt-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,26 +111,26 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5.1
+The current version of `encryption_utils` is 1.5.2
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.5.1',
+    version='1.5.2',
     description='Utility functions for encryption and file operations',
     author='nhman-python',
     author_email='wbgblfix@duck.com',
     url='https://github.com/nhman-python/crypto-utils',
     license='MIT',
     long_description=description,
     long_description_content_type='text/markdown',
```

### Comparing `simple2encrypt-1.5.1/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.5.2/simple2encrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5.1
+Version: 1.5.2
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,14 +120,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5.1
+The current version of `encryption_utils` is 1.5.2
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

