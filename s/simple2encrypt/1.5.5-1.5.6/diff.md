# Comparing `tmp/simple2encrypt-1.5.5.tar.gz` & `tmp/simple2encrypt-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.5.tar", last modified: Mon Jul 17 03:03:21 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.6.tar", last modified: Mon Jul 17 09:26:45 2023, max compression
```

## Comparing `simple2encrypt-1.5.5.tar` & `simple2encrypt-1.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.5/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.5/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.5/example_decrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.5/example_encrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.5/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     5122 2023-07-17 03:03:04.000000 simple2encrypt-1.5.5/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 03:03:21.656743 simple2encrypt-1.5.5/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4607 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 03:03:21.000000 simple2encrypt-1.5.5/simple2encrypt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)     6246 2023-07-17 03:03:04.000000 simple2encrypt-1.5.5/simple2encrypt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.6/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     5052 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.6/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.6/example_decrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.6/example_encrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.6/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     5567 2023-07-17 09:26:20.000000 simple2encrypt-1.5.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5052 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     9433 2023-07-17 09:26:27.000000 simple2encrypt-1.5.6/simple2encrypt.py
```

### Comparing `simple2encrypt-1.5.5/LICENSE` & `simple2encrypt-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.5/example_decrypt.py` & `simple2encrypt-1.5.6/example_decrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.5/example_encrypt.py` & `simple2encrypt-1.5.6/example_encrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.5/example_message.py` & `simple2encrypt-1.5.6/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.5/simple2encrypt.py` & `simple2encrypt-1.5.6/simple2encrypt.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.5'
+__version__ = '1.5.6'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
@@ -55,46 +55,46 @@
     :param add_extension: Add the extension to the end of the file
     :param folder_path: Path to the folder containing the files to be encrypted.
     :param key: The key for encryption.
     :raises ValueError: If the provided folder path is not a directory.
     """
     if not os.path.isdir(folder_path):
         raise ValueError("Expected a folder path, but received a different type of path.")
-
+    os.chdir(folder_path)
     for file in os.listdir(folder_path):
-        full_path = os.path.join(folder_path, file)
-        if os.path.isfile(full_path):
-            data = read_binary(full_path)
+
+        if os.path.isfile(folder_path):
+            data = read_binary(file)
             encryption = Encryption(key, data)
             encrypted_data = encryption.encrypt()
-            new_file_path = full_path + add_extension
+            new_file_path = file + add_extension
             write_binary(new_file_path, encrypted_data)
-            os.remove(full_path)
+            os.remove(file)
 
 
 def folder_dencrypt(folder_path: str, key: bytes) -> None:
     """
     Decrypts all files within a given folder.
 
     :param folder_path: Path to the folder containing the files to be decrypted.
     :param key: The key for decryption.
     :raises ValueError: If the provided folder path is not a directory.
     """
     if not os.path.isdir(folder_path):
         raise ValueError("Expected a folder path, but received a different type of path.")
-
+    os.chdir(folder_path)
     for file in os.listdir(folder_path):
-        full_path = os.path.join(folder_path, file)
-        if os.path.isfile(full_path):
-            data = read_binary(full_path)
+
+        if os.path.isfile(file):
+            data = read_binary(file)
             decryption = Encryption(key, data)
             decrypted_data = decryption.decrypt()
-            new_file_path = delete_extension(full_path)
+            new_file_path = delete_extension(file)
             write_binary(new_file_path, decrypted_data)
-            os.remove(full_path)
+            os.remove(file)
 
 
 def delete_extension(path: str) -> str:
     """
     Remove the last file extension from a path.
 
     :param path: The file path
@@ -149,14 +149,92 @@
     if os.path.isdir(file_path):
         raise ValueError("Path is a directory. File path is expected.")
     with open(file_path, 'wb') as f:
         f.write(data)
         return True
 
 
+def encrypt_walk_dirs(folder_path: str, key: bytes, extension: str = '.enc') -> None:
+    """
+    Walks through the specified folder path and encrypts all files using the provided AES key.
+
+    :param folder_path: The absolute folder path to walk on and encrypt files within.
+    :param key: The AES key used for encryption.
+    :param extension: Optional. The extension to add to the new encrypted file. Defaults to '.enc'.
+
+    :return: None
+
+    :raises PermissionError: If there is a permission error while accessing or modifying files.
+    :raises FileExistsError: If a file with the new name already exists in the destination.
+    :raises FileNotFoundError: If the specified file is not found.
+    :raises ValueError: If there is an error in the provided data or key.
+    """
+    for root, dirs, files in os.walk(folder_path):
+        for file in files:
+            file_path = os.path.join(root, file)
+            try:
+                # Read the binary data from the file
+                data = read_binary(file_path)
+
+                # Encrypt the data using the provided AES key
+                encrypt = Encryption(key, data)
+                encrypted_data = encrypt.encrypt()
+
+                # Remove the original file
+                os.remove(file_path)
+
+                # Create the new filename with the specified extension
+                new_file = f'{file_path}{extension}'
+
+                # Write the encrypted data to the new file
+                write_binary(new_file, encrypted_data)
+
+            except (PermissionError, FileExistsError, FileNotFoundError, ValueError) as err:
+                # Raise the error to be handled by the calling code
+                raise err
+
+
+def decrypt_walk_dirs(folder_path: str, key: bytes) -> None:
+    """
+    Walks through the specified folder path and decrypts all files using the provided AES key.
+
+    :param folder_path: The absolute folder path to walk on and decrypt files within.
+    :param key: The AES key used for decryption.
+    :return: None
+
+    :raises PermissionError: If there is a permission error while accessing or modifying files.
+    :raises FileExistsError: If a file with the new name already exists in the destination.
+    :raises FileNotFoundError: If the specified file is not found.
+    :raises ValueError: If there is an error in the provided data or key.
+    """
+    for root, dirs, files in os.walk(folder_path):
+        for file in files:
+            file_path = os.path.join(root, file)
+            try:
+                # Read the binary data from the file
+                data = read_binary(file_path)
+
+                # Decrypt the data using the provided AES key
+                encrypt = Encryption(key, data)
+                encrypted_data = encrypt.decrypt()
+
+                # Remove the original file
+                os.remove(file_path)
+
+                # Create the new filename with the specified extension
+                new_file = delete_extension(file_path)
+
+                # Write the decrypted data to the new file
+                write_binary(new_file, encrypted_data)
+
+            except (PermissionError, FileExistsError, FileNotFoundError, ValueError) as err:
+                # Raise the error to be handled by the calling code
+                raise err
+
+
 def custom_input(question: str) -> str:
     """
     Take a question as input from the user and return their response.
     :param question: Question to ask the user
     :return: Users response
     """
     try:
```

