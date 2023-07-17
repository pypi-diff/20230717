# Comparing `tmp/maxia_pipedrive-1.1.tar.gz` & `tmp/maxia_pipedrive-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxia_pipedrive-1.1.tar", last modified: Mon Jul 17 13:22:10 2023, max compression
+gzip compressed data, was "maxia_pipedrive-1.3.tar", last modified: Mon Jul 17 14:01:13 2023, max compression
```

## Comparing `maxia_pipedrive-1.1.tar` & `maxia_pipedrive-1.3.tar`

### file list

```diff
@@ -1,19 +1,11 @@
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.737013 maxia_pipedrive-1.1/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.1/LICENSE
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:22:10.737013 maxia_pipedrive-1.1/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       92 2023-07-17 13:21:25.000000 maxia_pipedrive-1.1/README.md
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.524385 maxia_pipedrive-1.1/maxia_pipedrive/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/__init__.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/consts.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/data_handler.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.000000 maxia_pipedrive-1.1/maxia_pipedrive/models.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/relations.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/tests.py
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.703473 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      396 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/SOURCES.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/dependency_links.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/requires.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/top_level.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-17 13:22:10.748485 maxia_pipedrive-1.1/setup.cfg
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1738 2023-07-17 13:21:04.000000 maxia_pipedrive-1.1/setup.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:01:13.383021 maxia_pipedrive-1.3/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      719 2023-07-17 14:01:13.385525 maxia_pipedrive-1.3/PKG-INFO
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:01:13.377008 maxia_pipedrive-1.3/maxia_pipedrive/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      595 2023-07-17 13:58:38.994926 maxia_pipedrive-1.3/maxia_pipedrive/__init__.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.638225 maxia_pipedrive-1.3/maxia_pipedrive/consts.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.717216 maxia_pipedrive-1.3/maxia_pipedrive/data_handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.494181 maxia_pipedrive-1.3/maxia_pipedrive/models.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.718218 maxia_pipedrive-1.3/maxia_pipedrive/relations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.727350 maxia_pipedrive-1.3/maxia_pipedrive/tests.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       62 2023-07-17 13:01:45.554947 maxia_pipedrive-1.3/setup.cfg
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1738 2023-07-17 13:59:41.064579 maxia_pipedrive-1.3/setup.py
```

### Comparing `maxia_pipedrive-1.1/PKG-INFO` & `maxia_pipedrive-1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: maxia_pipedrive
-Version: 1.1
+Version: 1.3
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
```

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/consts.py` & `maxia_pipedrive-1.3/maxia_pipedrive/consts.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/data_handler.py` & `maxia_pipedrive-1.3/maxia_pipedrive/data_handler.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/models.py` & `maxia_pipedrive-1.3/maxia_pipedrive/models.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/relations.py` & `maxia_pipedrive-1.3/maxia_pipedrive/relations.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/setup.py` & `maxia_pipedrive-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 setup(
     # How you named your package folder (MyLib)
     name='maxia_pipedrive',
     packages=['maxia_pipedrive'],   # Chose the same as "name"
-    version='1.1',      # Start with a small number and increase it with every change you make
+    version='1.3',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Maxia Pipedrive API handler',
     author='Max.ia Education',                   # Type in your name
     author_email='luiz@maxia.education',      # Type in your E-Mail
     # Provide either the link to your github or to your website
```

