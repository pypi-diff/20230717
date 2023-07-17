# Comparing `tmp/deepl-translator_selenium-0.2.0.tar.gz` & `tmp/deepl-translator_selenium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl-translator_selenium-0.2.0.tar", last modified: Mon Jul 17 00:22:53 2023, max compression
+gzip compressed data, was "deepl-translator_selenium-0.2.1.tar", last modified: Mon Jul 17 00:26:01 2023, max compression
```

## Comparing `deepl-translator_selenium-0.2.0.tar` & `deepl-translator_selenium-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:22:53.464835 deepl-translator_selenium-0.2.0/
--rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:22:53.464712 deepl-translator_selenium-0.2.0/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      402 2023-07-17 00:22:36.000000 deepl-translator_selenium-0.2.0/README.md
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:22:53.463990 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/
--rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      353 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 lunox      (501) staff       (20)       55 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/entry_points.txt
--rw-r--r--   0 lunox      (501) staff       (20)       15 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/requires.txt
--rw-r--r--   0 lunox      (501) staff       (20)       37 2023-07-17 00:22:53.000000 deepl-translator_selenium-0.2.0/deepl_translator_selenium.egg-info/top_level.txt
--rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-17 00:22:53.464874 deepl-translator_selenium-0.2.0/setup.cfg
--rw-r--r--   0 lunox      (501) staff       (20)      364 2023-07-17 00:14:06.000000 deepl-translator_selenium-0.2.0/setup.py
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:22:53.464109 deepl-translator_selenium-0.2.0/subtitle/
--rw-r--r--   0 lunox      (501) staff       (20)     2020 2023-07-17 00:07:23.000000 deepl-translator_selenium-0.2.0/subtitle/helper.py
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:22:53.464380 deepl-translator_selenium-0.2.0/translator/
--rw-r--r--   0 lunox      (501) staff       (20)     4196 2023-07-16 16:03:25.000000 deepl-translator_selenium-0.2.0/translator/deepl.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.740112 deepl-translator_selenium-0.2.1/
+-rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:26:01.739999 deepl-translator_selenium-0.2.1/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      406 2023-07-17 00:23:16.000000 deepl-translator_selenium-0.2.1/README.md
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739401 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/
+-rw-r--r--   0 lunox      (501) staff       (20)       69 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      361 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       55 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       15 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/requires.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       25 2023-07-17 00:26:01.000000 deepl-translator_selenium-0.2.1/deepl_translator_selenium.egg-info/top_level.txt
+-rw-r--r--   0 lunox      (501) staff       (20)     1738 2023-07-16 23:58:48.000000 deepl-translator_selenium-0.2.1/main.py
+-rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-17 00:26:01.740147 deepl-translator_selenium-0.2.1/setup.cfg
+-rw-r--r--   0 lunox      (501) staff       (20)      352 2023-07-17 00:25:56.000000 deepl-translator_selenium-0.2.1/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739514 deepl-translator_selenium-0.2.1/subtitle/
+-rw-r--r--   0 lunox      (501) staff       (20)     2020 2023-07-17 00:07:23.000000 deepl-translator_selenium-0.2.1/subtitle/helper.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-17 00:26:01.739719 deepl-translator_selenium-0.2.1/translator/
+-rw-r--r--   0 lunox      (501) staff       (20)     4196 2023-07-16 16:03:25.000000 deepl-translator_selenium-0.2.1/translator/deepl.py
```

### Comparing `deepl-translator_selenium-0.2.0/subtitle/helper.py` & `deepl-translator_selenium-0.2.1/subtitle/helper.py`

 * *Files identical despite different names*

### Comparing `deepl-translator_selenium-0.2.0/translator/deepl.py` & `deepl-translator_selenium-0.2.1/translator/deepl.py`

 * *Files identical despite different names*

