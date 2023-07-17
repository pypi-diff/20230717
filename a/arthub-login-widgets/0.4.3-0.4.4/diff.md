# Comparing `tmp/arthub_login_widgets-0.4.3.tar.gz` & `tmp/arthub_login_widgets-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_login_widgets-0.4.3.tar", last modified: Mon Jul 17 10:16:18 2023, max compression
+gzip compressed data, was "arthub_login_widgets-0.4.4.tar", last modified: Mon Jul 17 10:19:09 2023, max compression
```

## Comparing `arthub_login_widgets-0.4.3.tar` & `arthub_login_widgets-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:16:18.798795 arthub_login_widgets-0.4.3/
--rw-rw-rw-   0        0        0      375 2023-07-17 10:16:18.797837 arthub_login_widgets-0.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 10:16:18.769657 arthub_login_widgets-0.4.3/arthub_login_widgets/
--rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-17 10:16:13.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/__version__.py
--rw-rw-rw-   0        0        0      590 2023-07-17 06:03:02.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/constants.py
--rw-rw-rw-   0        0        0    10243 2023-07-17 10:11:28.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/core.py
--rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:16:18.773646 arthub_login_widgets-0.4.3/arthub_login_widgets/resources/
--rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/resources/__init__.py
--rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/resources/arthub_white.png
--rw-rw-rw-   0        0        0     1073 2023-07-17 10:16:02.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/resources/style.qss
-drwxrwxrwx   0        0        0        0 2023-07-17 10:16:18.779670 arthub_login_widgets-0.4.3/arthub_login_widgets/test/
--rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/test/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_core.py
--rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_filesystem.py
--rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_imports.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:16:18.791811 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/
--rw-rw-rw-   0        0        0      375 2023-07-17 10:16:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-07-17 10:16:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:16:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-17 10:16:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-17 10:16:18.000000 arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 10:16:18.799793 arthub_login_widgets-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:19:09.652287 arthub_login_widgets-0.4.4/
+-rw-rw-rw-   0        0        0      375 2023-07-17 10:19:09.651286 arthub_login_widgets-0.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 10:19:09.620801 arthub_login_widgets-0.4.4/arthub_login_widgets/
+-rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-17 10:18:55.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/__version__.py
+-rw-rw-rw-   0        0        0      590 2023-07-17 06:03:02.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/constants.py
+-rw-rw-rw-   0        0        0    10243 2023-07-17 10:11:28.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/core.py
+-rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:19:09.625848 arthub_login_widgets-0.4.4/arthub_login_widgets/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/resources/__init__.py
+-rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/resources/arthub_white.png
+-rw-rw-rw-   0        0        0     1073 2023-07-17 10:16:02.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/resources/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-17 10:19:09.633455 arthub_login_widgets-0.4.4/arthub_login_widgets/test/
+-rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/test/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_core.py
+-rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_filesystem.py
+-rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_imports.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:19:09.645287 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-07-17 10:19:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1177 2023-07-17 10:19:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:19:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-17 10:19:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 10:19:09.000000 arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:19:09.653283 arthub_login_widgets-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.4.4/setup.py
```

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/constants.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/constants.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/core.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/filesystem.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/resources/arthub_white.png` & `arthub_login_widgets-0.4.4/arthub_login_widgets/resources/arthub_white.png`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/resources/style.qss` & `arthub_login_widgets-0.4.4/arthub_login_widgets/resources/style.qss`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_core.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_filesystem.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets/test/test_imports.py` & `arthub_login_widgets-0.4.4/arthub_login_widgets/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/arthub_login_widgets.egg-info/SOURCES.txt` & `arthub_login_widgets-0.4.4/arthub_login_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.3/setup.py` & `arthub_login_widgets-0.4.4/setup.py`

 * *Files identical despite different names*

