# Comparing `tmp/maxia_pipedrive-1.0.tar.gz` & `tmp/maxia_pipedrive-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxia_pipedrive-1.0.tar", last modified: Mon Jul 17 13:08:30 2023, max compression
+gzip compressed data, was "maxia_pipedrive-1.1.tar", last modified: Mon Jul 17 13:22:10 2023, max compression
```

## Comparing `maxia_pipedrive-1.0.tar` & `maxia_pipedrive-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:08:30.564764 maxia_pipedrive-1.0/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.0/LICENSE
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:08:30.565767 maxia_pipedrive-1.0/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       23 2023-07-17 12:49:20.000000 maxia_pipedrive-1.0/README.md
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:08:30.355406 maxia_pipedrive-1.0/maxia_pipedrive/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/__init__.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/consts.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/data_handler.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/models.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/relations.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.0/maxia_pipedrive/tests.py
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:08:30.531161 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:08:29.000000 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      396 2023-07-17 13:08:30.000000 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/SOURCES.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-17 13:08:29.000000 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/dependency_links.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-17 13:08:29.000000 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/requires.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-17 13:08:29.000000 maxia_pipedrive-1.0/maxia_pipedrive.egg-info/top_level.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-17 13:08:30.575387 maxia_pipedrive-1.0/setup.cfg
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1738 2023-07-17 13:08:24.000000 maxia_pipedrive-1.0/setup.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.737013 maxia_pipedrive-1.1/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.1/LICENSE
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:22:10.737013 maxia_pipedrive-1.1/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       92 2023-07-17 13:21:25.000000 maxia_pipedrive-1.1/README.md
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.524385 maxia_pipedrive-1.1/maxia_pipedrive/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/__init__.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/consts.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/data_handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.000000 maxia_pipedrive-1.1/maxia_pipedrive/models.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/relations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.1/maxia_pipedrive/tests.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 13:22:10.703473 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      702 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      396 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/SOURCES.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/dependency_links.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/requires.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-17 13:22:10.000000 maxia_pipedrive-1.1/maxia_pipedrive.egg-info/top_level.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-17 13:22:10.748485 maxia_pipedrive-1.1/setup.cfg
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1738 2023-07-17 13:21:04.000000 maxia_pipedrive-1.1/setup.py
```

### Comparing `maxia_pipedrive-1.0/LICENSE` & `maxia_pipedrive-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.0/PKG-INFO` & `maxia_pipedrive-1.1/maxia_pipedrive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: maxia_pipedrive
-Version: 1.0
+Name: maxia-pipedrive
+Version: 1.1
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.0.tar.gz
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxia_pipedrive-1.0/maxia_pipedrive/consts.py` & `maxia_pipedrive-1.1/maxia_pipedrive/consts.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.0/maxia_pipedrive/data_handler.py` & `maxia_pipedrive-1.1/maxia_pipedrive/data_handler.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.0/maxia_pipedrive/models.py` & `maxia_pipedrive-1.1/maxia_pipedrive/models.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.0/maxia_pipedrive/relations.py` & `maxia_pipedrive-1.1/maxia_pipedrive/relations.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.0/maxia_pipedrive.egg-info/PKG-INFO` & `maxia_pipedrive-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: maxia-pipedrive
-Version: 1.0
+Name: maxia_pipedrive
+Version: 1.1
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.0.tar.gz
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxia_pipedrive-1.0/setup.py` & `maxia_pipedrive-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 setup(
     # How you named your package folder (MyLib)
     name='maxia_pipedrive',
     packages=['maxia_pipedrive'],   # Chose the same as "name"
-    version='1.0',      # Start with a small number and increase it with every change you make
+    version='1.1',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Maxia Pipedrive API handler',
     author='Max.ia Education',                   # Type in your name
     author_email='luiz@maxia.education',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/Max-ia-Education/maxia_pipedrive_api',
     # I explain this later on
-    download_url='https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.0.tar.gz',
+    download_url='https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz',
     #   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
         'numpy',
         'pandas',
         'tqdm'
     ],
     classifiers=[
```

