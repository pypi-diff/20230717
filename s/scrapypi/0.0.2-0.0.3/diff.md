# Comparing `tmp/scrapypi-0.0.2.tar.gz` & `tmp/scrapypi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapypi-0.0.2.tar", last modified: Sun Jul 16 21:05:41 2023, max compression
+gzip compressed data, was "scrapypi-0.0.3.tar", last modified: Mon Jul 17 14:05:48 2023, max compression
```

## Comparing `scrapypi-0.0.2.tar` & `scrapypi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.638242 scrapypi-0.0.2/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      173 2023-07-16 21:04:21.000000 scrapypi-0.0.2/CHANGELOG.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-07-16 19:52:15.000000 scrapypi-0.0.2/LICENCE.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.2/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      793 2023-07-16 21:05:41.638242 scrapypi-0.0.2/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       84 2023-07-16 20:57:10.000000 scrapypi-0.0.2/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.634242 scrapypi-0.0.2/scrapypi/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-16 21:01:59.000000 scrapypi-0.0.2/scrapypi/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1131 2023-07-16 20:14:05.000000 scrapypi-0.0.2/scrapypi/scrapypi.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-16 21:05:41.638242 scrapypi-0.0.2/scrapypi.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      793 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      291 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-07-16 21:05:40.000000 scrapypi-0.0.2/scrapypi.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-16 21:05:41.638242 scrapypi-0.0.2/setup.cfg
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1225 2023-07-16 21:03:40.000000 scrapypi-0.0.2/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-17 14:05:48.444318 scrapypi-0.0.3/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      281 2023-07-17 13:42:48.000000 scrapypi-0.0.3/CHANGELOG.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-07-17 13:44:26.000000 scrapypi-0.0.3/LICENCE.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.3/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2245 2023-07-17 14:05:48.444318 scrapypi-0.0.3/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1421 2023-07-17 13:43:56.000000 scrapypi-0.0.3/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-17 14:05:48.440318 scrapypi-0.0.3/scrapypi/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-17 12:40:34.000000 scrapypi-0.0.3/scrapypi/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3878 2023-07-17 13:49:00.000000 scrapypi-0.0.3/scrapypi/handler.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2202 2023-07-17 13:51:25.000000 scrapypi-0.0.3/scrapypi/scrapypi.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-17 14:05:48.440318 scrapypi-0.0.3/scrapypi/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-17 12:33:53.000000 scrapypi-0.0.3/scrapypi/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      214 2023-07-17 12:36:27.000000 scrapypi-0.0.3/scrapypi/stubs/scrapypi.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-17 14:05:48.440318 scrapypi-0.0.3/scrapypi.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2245 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      367 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       24 2023-07-17 14:05:48.000000 scrapypi-0.0.3/scrapypi.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-17 14:05:48.444318 scrapypi-0.0.3/setup.cfg
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1990 2023-07-17 14:04:15.000000 scrapypi-0.0.3/setup.py
```

