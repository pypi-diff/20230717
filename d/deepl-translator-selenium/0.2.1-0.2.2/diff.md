# Comparing `tmp/deepl-translator_selenium-0.2.1.tar.gz` & `tmp/deepl-translator_selenium-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl-translator_selenium-0.2.1.tar", last modified: Mon Jul 17 00:26:01 2023, max compression
+gzip compressed data, was "deepl-translator_selenium-0.2.2.tar", last modified: Mon Jul 17 01:32:46 2023, max compression
```

## Comparing `deepl-translator_selenium-0.2.1.tar` & `deepl-translator_selenium-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.740112 deepl-translator_selenium-0.2.1/
--rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:26:01.739999 deepl-translator_selenium-0.2.1/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      406 2023-07-17 00:23:16.000000 deepl-translator_selenium-0.2.1/README.md
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739401 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/
--rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      361 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 lunox      (501) staff       (20)       55 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/entry_points.txt
--rw-r--r--   0 lunox      (501) staff       (20)       15 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/requires.txt
--rw-r--r--   0 lunox      (501) staff       (20)       25 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/top_level.txt
--rw-r--r--   0 lunox      (501) staff       (20)     1738 2023-07-16 23:58:48.000000 deepl-translator_selenium-0.2.1/main.py
--rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-17 00:26:01.740147 deepl-translator_selenium-0.2.1/setup.cfg
--rw-r--r--   0 lunox      (501) staff       (20)      352 2023-07-17 00:25:56.000000 deepl-translator_selenium-0.2.1/setup.py
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739514 deepl-translator_selenium-0.2.1/subtitle/
--rw-r--r--   0 lunox      (501) staff       (20)     2020 2023-07-17 00:07:23.000000 deepl-translator_selenium-0.2.1/subtitle/helper.py
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739719 deepl-translator_selenium-0.2.1/translator/
--rw-r--r--   0 lunox      (501) staff       (20)     4196 2023-07-16 16:03:25.000000 deepl-translator_selenium-0.2.1/translator/deepl.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 01:32:46.855891 deepl-translator_selenium-0.2.2/
+-rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 01:32:46.855767 deepl-translator_selenium-0.2.2/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)     1691 2023-07-17 00:36:35.000000 deepl-translator_selenium-0.2.2/README.md
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 01:32:46.855227 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/
+-rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      361 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       55 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       15 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/requires.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       25 2023-07-17 01:32:46.000000 deepl-translator_selenium-0.2.2/deepl_translator_selenium.egg-info/top_level.txt
+-rw-r--r--   0 lunox      (501) staff       (20)     1738 2023-07-16 23:58:48.000000 deepl-translator_selenium-0.2.2/main.py
+-rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-17 01:32:46.855930 deepl-translator_selenium-0.2.2/setup.cfg
+-rw-r--r--   0 lunox      (501) staff       (20)      352 2023-07-17 01:32:44.000000 deepl-translator_selenium-0.2.2/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 01:32:46.855344 deepl-translator_selenium-0.2.2/subtitle/
+-rw-r--r--   0 lunox      (501) staff       (20)     2020 2023-07-17 00:07:23.000000 deepl-translator_selenium-0.2.2/subtitle/helper.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 01:32:46.855569 deepl-translator_selenium-0.2.2/translator/
+-rw-r--r--   0 lunox      (501) staff       (20)     4196 2023-07-16 16:03:25.000000 deepl-translator_selenium-0.2.2/translator/deepl.py
```

### Comparing `deepl-translator_selenium-0.2.1/main.py` & `deepl-translator_selenium-0.2.2/main.py`

 * *Files identical despite different names*

### Comparing `deepl-translator_selenium-0.2.1/subtitle/helper.py` & `deepl-translator_selenium-0.2.2/subtitle/helper.py`

 * *Files identical despite different names*

### Comparing `deepl-translator_selenium-0.2.1/translator/deepl.py` & `deepl-translator_selenium-0.2.2/translator/deepl.py`

 * *Files identical despite different names*

