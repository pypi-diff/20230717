# Comparing `tmp/Janex-0.0.6a0.tar.gz` & `tmp/Janex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.6a0.tar", last modified: Thu Jul 13 20:17:26 2023, max compression
+gzip compressed data, was "Janex-0.0.7.tar", last modified: Mon Jul 17 14:59:03 2023, max compression
```

## Comparing `Janex-0.0.6a0.tar` & `Janex-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-13 20:17:26.594670 Janex-0.0.6a0/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-13 20:17:26.589587 Janex-0.0.6a0/Janex/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-13 20:17:26.594232 Janex-0.0.6a0/Janex/JanexSub/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.6a0/Janex/JanexSub/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.6a0/Janex/JanexSub/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     5046 2023-07-13 20:15:28.000000 Janex-0.0.6a0/Janex/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.6a0/Janex/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Janex-0.0.6a0/Janex/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-13 20:17:26.593704 Janex-0.0.6a0/Janex.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-13 20:17:26.000000 Janex-0.0.6a0/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      279 2023-07-13 20:17:26.000000 Janex-0.0.6a0/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-13 20:17:26.000000 Janex-0.0.6a0/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-13 20:17:26.000000 Janex-0.0.6a0/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-13 20:17:26.000000 Janex-0.0.6a0/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.6a0/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-13 20:17:26.594475 Janex-0.0.6a0/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     3027 2023-07-11 10:41:46.000000 Janex-0.0.6a0/README.md
--rw-r--r--   0 cipher     (501) staff       (20)     1289 2023-07-13 20:15:43.000000 Janex-0.0.6a0/Setup.py
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-13 20:17:26.594720 Janex-0.0.6a0/setup.cfg
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.490299 Janex-0.0.7/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.487177 Janex-0.0.7/Janex/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.489998 Janex-0.0.7/Janex/JanexSub/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.7/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.7/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)       20 2023-07-17 14:57:49.000000 Janex-0.0.7/Janex/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.7/Janex/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)     5046 2023-07-17 14:57:41.000000 Janex-0.0.7/Janex/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.489695 Janex-0.0.7/Janex.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      279 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.7/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-17 14:59:03.490169 Janex-0.0.7/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     3029 2023-07-17 10:56:37.000000 Janex-0.0.7/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)     1283 2023-07-17 14:58:26.000000 Janex-0.0.7/Setup.py
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:59:03.490339 Janex-0.0.7/setup.cfg
```

### Comparing `Janex-0.0.6a0/Janex/__init__.py` & `Janex-0.0.7/Janex/main.py`

 * *Files identical despite different names*

### Comparing `Janex-0.0.6a0/Janex.egg-info/PKG-INFO` & `Janex-0.0.7/Janex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.6a0
+Version: 0.0.7
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -96,9 +96,9 @@
 <h3> Functionality </h3>
 
 <h4>Version 0.0.5</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
-- Support for Darwin, Unix-like and Windows ✓
+- Support for Darwin, Linux (GNU) and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.6a0/LICENSE` & `Janex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.6a0/PKG-INFO` & `Janex-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.6a0
+Version: 0.0.7
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -96,9 +96,9 @@
 <h3> Functionality </h3>
 
 <h4>Version 0.0.5</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
-- Support for Darwin, Unix-like and Windows ✓
+- Support for Darwin, Linux (GNU) and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.6a0/README.md` & `Janex-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,9 +83,9 @@
 <h3> Functionality </h3>
 
 <h4>Version 0.0.5</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
-- Support for Darwin, Unix-like and Windows ✓
+- Support for Darwin, Linux (GNU) and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.6a0/Setup.py` & `Janex-0.0.7/Setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.6-alpha",
+    version="0.0.7",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex/',
 
     # your Email address
```

