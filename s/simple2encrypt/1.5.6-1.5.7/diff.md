# Comparing `tmp/simple2encrypt-1.5.6.tar.gz` & `tmp/simple2encrypt-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.6.tar", last modified: Mon Jul 17 09:26:45 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.7.tar", last modified: Mon Jul 17 09:54:31 2023, max compression
```

## Comparing `simple2encrypt-1.5.6.tar` & `simple2encrypt-1.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.6/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     5052 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.6/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.6/example_decrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.6/example_encrypt.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.6/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     5567 2023-07-17 09:26:20.000000 simple2encrypt-1.5.6/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:26:45.828267 simple2encrypt-1.5.6/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     5052 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 09:26:45.000000 simple2encrypt-1.5.6/simple2encrypt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)     9433 2023-07-17 09:26:27.000000 simple2encrypt-1.5.6/simple2encrypt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.7/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     8316 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      129 2023-07-17 02:26:01.000000 simple2encrypt-1.5.7/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1770 2023-07-17 02:39:53.000000 simple2encrypt-1.5.7/example_decrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1739 2023-07-17 02:35:08.000000 simple2encrypt-1.5.7/example_encrypt.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1303 2023-07-17 02:21:01.000000 simple2encrypt-1.5.7/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     8831 2023-07-17 09:54:17.000000 simple2encrypt-1.5.7/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-17 09:54:31.284314 simple2encrypt-1.5.7/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     8316 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      331 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       63 2023-07-17 09:54:31.000000 simple2encrypt-1.5.7/simple2encrypt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     9433 2023-07-17 09:31:45.000000 simple2encrypt-1.5.7/simple2encrypt.py
```

### Comparing `simple2encrypt-1.5.6/LICENSE` & `simple2encrypt-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.6/example_decrypt.py` & `simple2encrypt-1.5.7/example_decrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.6/example_encrypt.py` & `simple2encrypt-1.5.7/example_encrypt.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.6/example_message.py` & `simple2encrypt-1.5.7/example_message.py`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5.6/simple2encrypt.py` & `simple2encrypt-1.5.7/simple2encrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5.6'
+__version__ = '1.5.7'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
```

