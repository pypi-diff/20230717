# Comparing `tmp/md2cf-2.2.0.tar.gz` & `tmp/md2cf-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/md2cf-2.2.0.tar", last modified: Sun Jul  9 01:00:17 2023, max compression
+gzip compressed data, was "dist/md2cf-2.2.1.tar", last modified: Mon Jul 17 15:36:05 2023, max compression
```

## Comparing `md2cf-2.2.0.tar` & `md2cf-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-09 01:00:17.000000 md2cf-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-09 01:00:11.000000 md2cf-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/confluence_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/ignored_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-09 01:00:16.000000 md2cf-2.2.0/md2cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:00:16.000000 md2cf-2.2.0/md2cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:00:17.000000 md2cf-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-09 01:00:11.000000 md2cf-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 15:36:05.000000 md2cf-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-17 15:35:59.000000 md2cf-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/confluence_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/ignored_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:36:05.000000 md2cf-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 15:35:59.000000 md2cf-2.2.1/setup.py
```

### Comparing `md2cf-2.2.0/PKG-INFO` & `md2cf-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.2.0
+Version: 2.2.1
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
```

### Comparing `md2cf-2.2.0/README.md` & `md2cf-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/__main__.py` & `md2cf-2.2.1/md2cf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/api.py` & `md2cf-2.2.1/md2cf/api.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/confluence_renderer.py` & `md2cf-2.2.1/md2cf/confluence_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,16 +101,18 @@
     def plain_text_body(self, text):
         body_tag = ConfluenceTag("plain-text-body", cdata=True)
         body_tag.text = text
         return body_tag
 
     def link(self, link, title, text):
         parsed_link = urlparse(link)
-        if self.enable_relative_links and (
-            not parsed_link.scheme and not parsed_link.netloc
+        if (
+            self.enable_relative_links
+            and (not parsed_link.scheme and not parsed_link.netloc)
+            and parsed_link.path
         ):
             # relative link
             replacement_link = f"md2cf-internal-link-{uuid.uuid4()}"
             self.relative_links.append(
                 RelativeLink(
                     # make sure to unquote the url as relative paths
                     # might have escape sequences
```

### Comparing `md2cf-2.2.0/md2cf/document.py` & `md2cf-2.2.1/md2cf/document.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/ignored_files.py` & `md2cf-2.2.1/md2cf/ignored_files.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/tui.py` & `md2cf-2.2.1/md2cf/tui.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf/upsert.py` & `md2cf-2.2.1/md2cf/upsert.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.0/md2cf.egg-info/PKG-INFO` & `md2cf-2.2.1/md2cf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.2.0
+Version: 2.2.1
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
```

### Comparing `md2cf-2.2.0/setup.py` & `md2cf-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="md2cf",
-    version="2.2.0",
+    version="2.2.1",
     packages=["md2cf"],
     url="https://github.com/iamjackg/md2cf",
     license="MIT",
     author="Jack Gaino",
     author_email="md2cf@jackgaino.com",
     description="Convert Markdown documents to Confluence",
     long_description=long_description,
```

