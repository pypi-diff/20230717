# Comparing `tmp/yplib-2.5.7.tar.gz` & `tmp/yplib-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.5.7.tar", last modified: Mon Jul 17 00:30:29 2023, max compression
+gzip compressed data, was "dist\yplib-2.5.8.tar", last modified: Mon Jul 17 00:32:46 2023, max compression
```

## Comparing `yplib-2.5.7.tar` & `yplib-2.5.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 00:30:29.185144 yplib-2.5.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-17 00:30:29.185087 yplib-2.5.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 00:30:29.185144 yplib-2.5.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-17 00:30:15.000000 yplib-2.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:30:29.181836 yplib-2.5.7/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.7/yplib/db.py
--rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.7/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    33959 2023-07-17 00:29:59.000000 yplib-2.5.7/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.7/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.7/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.7/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:30:29.184289 yplib-2.5.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-17 00:30:29.000000 yplib-2.5.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-17 00:30:29.000000 yplib-2.5.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 00:30:29.000000 yplib-2.5.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 00:30:29.000000 yplib-2.5.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 00:32:46.496930 yplib-2.5.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:32:46.496930 yplib-2.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 00:32:46.497639 yplib-2.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-17 00:32:32.000000 yplib-2.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:32:46.494293 yplib-2.5.8/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.8/yplib/db.py
+-rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.8/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33959 2023-07-17 00:29:59.000000 yplib-2.5.8/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.8/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.8/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.8/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:32:46.496607 yplib-2.5.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-17 00:32:46.000000 yplib-2.5.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-17 00:32:46.000000 yplib-2.5.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:32:46.000000 yplib-2.5.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 00:32:46.000000 yplib-2.5.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.5.7/LICENSE` & `yplib-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/setup.py` & `yplib-2.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.5.7",
+  version="2.5.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.5.7/yplib/__init__.py` & `yplib-2.5.8/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/chart.py` & `yplib-2.5.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/chart_html.py` & `yplib-2.5.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/db.py` & `yplib-2.5.8/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/file.py` & `yplib-2.5.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/http_util.py` & `yplib-2.5.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/index.py` & `yplib-2.5.8/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/mail.py` & `yplib-2.5.8/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/mail_html.py` & `yplib-2.5.8/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.7/yplib/markdown.py` & `yplib-2.5.8/yplib/markdown.py`

 * *Files identical despite different names*

