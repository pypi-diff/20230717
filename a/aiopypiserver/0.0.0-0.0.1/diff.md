# Comparing `tmp/aiopypiserver-0.0.0.tar.gz` & `tmp/aiopypiserver-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopypiserver-0.0.0.tar", last modified: Sat Jul 15 04:26:35 2023, max compression
+gzip compressed data, was "aiopypiserver-0.0.1.tar", last modified: Mon Jul 17 10:51:06 2023, max compression
```

## Comparing `aiopypiserver-0.0.0.tar` & `aiopypiserver-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 04:26:35.855195 aiopypiserver-0.0.0/
--rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      957 2023-07-15 04:26:35.855195 aiopypiserver-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-07-15 04:25:32.000000 aiopypiserver-0.0.0/README.md
--rw-rw-rw-   0        0        0      722 2023-07-15 04:18:59.000000 aiopypiserver-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 04:26:35.856194 aiopypiserver-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 04:26:35.831196 aiopypiserver-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 04:26:35.838198 aiopypiserver-0.0.0/src/aiopypiserver/
--rw-rw-rw-   0        0        0       92 2023-07-15 04:14:43.000000 aiopypiserver-0.0.0/src/aiopypiserver/__init__.py
--rw-rw-rw-   0        0        0       29 2023-07-14 23:15:16.000000 aiopypiserver-0.0.0/src/aiopypiserver/main.py
-drwxrwxrwx   0        0        0        0 2023-07-15 04:26:35.852194 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/
--rw-rw-rw-   0        0        0      957 2023-07-15 04:26:35.000000 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-07-15 04:26:35.000000 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 04:26:35.000000 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-15 04:26:35.000000 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-15 04:26:35.000000 aiopypiserver-0.0.0/src/aiopypiserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 04:26:35.853196 aiopypiserver-0.0.0/tests/
--rw-rw-rw-   0        0        0       78 2023-07-15 04:14:43.000000 aiopypiserver-0.0.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.814149 aiopypiserver-0.0.1/
+-rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2244 2023-07-17 10:51:06.813148 aiopypiserver-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/README.md
+-rw-rw-rw-   0        0        0      790 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:51:06.814149 aiopypiserver-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.776635 aiopypiserver-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.786152 aiopypiserver-0.0.1/src/aiopypiserver/
+-rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/src/aiopypiserver/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/src/aiopypiserver/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.811149 aiopypiserver-0.0.1/src/aiopypiserver/assets/
+-rw-rw-rw-   0        0        0      505 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/src/aiopypiserver/assets/index.html
+-rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/src/aiopypiserver/assets/list.html
+-rw-rw-rw-   0        0        0    10076 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/src/aiopypiserver/webserver.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.802148 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/
+-rw-rw-rw-   0        0        0     2244 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 10:51:06.000000 aiopypiserver-0.0.1/src/aiopypiserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 10:51:06.812148 aiopypiserver-0.0.1/tests/
+-rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.1/tests/test_server.py
```

### Comparing `aiopypiserver-0.0.0/LICENSE` & `aiopypiserver-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.0/pyproject.toml` & `aiopypiserver-0.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopypiserver"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
     {name="Jamie Walton"}
 ]
 description = "Do what pypiserver does, but with aiohttp."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
@@ -20,8 +20,11 @@
     "Operating System :: OS Independent",
     "Environment :: Console",
     "Development Status :: 1 - Planning",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jamie0walton/aiopypiserver"
-"Bug Tracker" = "https://github.com/jamie0walton/aiopypiserver/issues"
+"Bug Tracker" = "https://github.com/jamie0walton/aiopypiserver/issues"
+
+[project.scripts]
+aiopypiserver = "aiopypiserver:commandline_run"
```

