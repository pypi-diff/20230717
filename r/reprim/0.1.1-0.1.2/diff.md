# Comparing `tmp/reprim-0.1.1.tar.gz` & `tmp/reprim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.1.1.tar", last modified: Sat Jul 15 17:25:39 2023, max compression
+gzip compressed data, was "reprim-0.1.2.tar", last modified: Mon Jul 17 21:26:04 2023, max compression
```

## Comparing `reprim-0.1.1.tar` & `reprim-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.516977 reprim-0.1.1/
--rw-rw-rw-   0        0        0      683 2023-07-15 17:25:39.516977 reprim-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.492043 reprim-0.1.1/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.1/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20390 2023-07-15 17:24:46.000000 reprim-0.1.1/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.495036 reprim-0.1.1/RePrIm/util/
--rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.1.1/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0     3125 2023-07-15 15:22:07.000000 reprim-0.1.1/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.1/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.515980 reprim-0.1.1/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 17:25:39.516977 reprim-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-15 15:34:51.000000 reprim-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.661732 reprim-0.1.2/
+-rw-rw-rw-   0        0        0      683 2023-07-17 21:26:04.660734 reprim-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.573461 reprim-0.1.2/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.2/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20390 2023-07-15 17:24:46.000000 reprim-0.1.2/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.634298 reprim-0.1.2/RePrIm/util/
+-rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.1.2/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.1.2/RePrIm/util/lib.py
+-rw-rw-rw-   0        0        0     3125 2023-07-15 15:22:07.000000 reprim-0.1.2/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.2/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.654790 reprim-0.1.2/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 21:26:04.661732 reprim-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-17 21:25:43.000000 reprim-0.1.2/setup.py
```

### Comparing `reprim-0.1.1/PKG-INFO` & `reprim-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.1
+Version: 0.1.2
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.1/RePrIm/reprim.py` & `reprim-0.1.2/RePrIm/reprim.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.1/RePrIm/util/hardware_monitor.py` & `reprim-0.1.2/RePrIm/util/hardware_monitor.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.1/RePrIm/util/process.py` & `reprim-0.1.2/RePrIm/util/process.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.1/RePrIm/util/tools.py` & `reprim-0.1.2/RePrIm/util/tools.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.1/reprim.egg-info/PKG-INFO` & `reprim-0.1.2/reprim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.1
+Version: 0.1.2
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.1/setup.py` & `reprim-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.1.1",
+    version="0.1.2",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

