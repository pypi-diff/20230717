# Comparing `tmp/deepl_translator-0.1.8.tar.gz` & `tmp/deepl_translator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl_translator-0.1.8.tar", last modified: Sun Jul 16 15:47:42 2023, max compression
+gzip compressed data, was "deepl_translator-0.1.9.tar", last modified: Sun Jul 16 23:57:26 2023, max compression
```

## Comparing `deepl_translator-0.1.8.tar` & `deepl_translator-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:47:42.415360 deepl_translator-0.1.8/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:47:42.415249 deepl_translator-0.1.8/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.8/README.md
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:47:42.415102 deepl_translator-0.1.8/deepl_translator.egg-info/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      302 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/SOURCES.txt
--rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/dependency_links.txt
--rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/entry_points.txt
--rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/requires.txt
--rw-r--r--   0 lunox      (501) staff       (20)       37 2023-07-16 15:47:42.000000 deepl_translator-0.1.8/deepl_translator.egg-info/top_level.txt
--rw-r--r--   0 lunox      (501) staff       (20)     1789 2023-07-16 15:46:58.000000 deepl_translator-0.1.8/deepl_translator.py
--rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 15:47:42.415398 deepl_translator-0.1.8/setup.cfg
--rw-r--r--   0 lunox      (501) staff       (20)      335 2023-07-16 15:47:19.000000 deepl_translator-0.1.8/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 23:57:26.689822 deepl_translator-0.1.9/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 23:57:26.689703 deepl_translator-0.1.9/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.9/README.md
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 23:57:26.689086 deepl_translator-0.1.9/deepl_translator.egg-info/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      341 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/entry_points.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/requires.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       37 2023-07-16 23:57:26.000000 deepl_translator-0.1.9/deepl_translator.egg-info/top_level.txt
+-rw-r--r--   0 lunox      (501) staff       (20)     1787 2023-07-16 16:07:43.000000 deepl_translator-0.1.9/deepl_translator.py
+-rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 23:57:26.689859 deepl_translator-0.1.9/setup.cfg
+-rw-r--r--   0 lunox      (501) staff       (20)      348 2023-07-16 23:57:14.000000 deepl_translator-0.1.9/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 23:57:26.689202 deepl_translator-0.1.9/subtitle/
+-rw-r--r--   0 lunox      (501) staff       (20)     2005 2023-07-16 09:52:05.000000 deepl_translator-0.1.9/subtitle/helper.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 23:57:26.689428 deepl_translator-0.1.9/translator/
+-rw-r--r--   0 lunox      (501) staff       (20)     4196 2023-07-16 16:03:25.000000 deepl_translator-0.1.9/translator/deepl.py
```

### Comparing `deepl_translator-0.1.8/deepl_translator.py` & `deepl_translator-0.1.9/deepl_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 # from subtitle.helper import Helper as Subtitle
-from .subtitle.helper import  Helper as Subtitle
-from .translator.deepl import DeepL as DeepLTranslator
+from subtitle.helper import  Helper as Subtitle
+from translator.deepl import DeepL as DeepLTranslator
 import os
 
 
 def _create_output_directory_if_not_exist(output_directory: str):
     isExist = os.path.exists(output_directory)
     if not isExist:
         os.makedirs(output_directory)
```

