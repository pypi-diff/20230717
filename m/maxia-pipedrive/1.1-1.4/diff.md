# Comparing `tmp/maxia_pipedrive-1.1.tar.gz` & `tmp/maxia_pipedrive-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxia_pipedrive-1.1.tar", last modified: Mon Jul 17 13:22:10 2023, max compression
+gzip compressed data, was "maxia_pipedrive-1.4.tar", last modified: Mon Jul 17 14:21:09 2023, max compression
```

## Comparing `maxia_pipedrive-1.1.tar` & `maxia_pipedrive-1.4.tar`

### file list

```diff
@@ -1,19 +1,31 @@
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
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:09.541003 maxia_pipedrive-1.4/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.4/LICENSE
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-17 14:21:09.542994 maxia_pipedrive-1.4/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       95 2023-07-17 14:14:03.000000 maxia_pipedrive-1.4/README.md
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:08.708790 maxia_pipedrive-1.4/maxia_pipedrive/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      595 2023-07-17 13:58:38.000000 maxia_pipedrive-1.4/maxia_pipedrive/__init__.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:09.500868 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/__init__.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    14893 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/deals.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1092 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/fields.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2388 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/followers.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      166 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     8012 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/organizations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1979 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/persons.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2064 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/products.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      193 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/stages.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      190 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/users.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    20937 2023-07-17 13:12:38.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/utils.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/consts.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/data_handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.000000 maxia_pipedrive-1.4/maxia_pipedrive/models.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/relations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/tests.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:08.919899 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      827 2023-07-17 14:21:08.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/SOURCES.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/dependency_links.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/requires.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/top_level.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-17 14:21:09.553974 maxia_pipedrive-1.4/setup.cfg
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1799 2023-07-17 14:20:55.000000 maxia_pipedrive-1.4/setup.py
```

### Comparing `maxia_pipedrive-1.1/LICENSE` & `maxia_pipedrive-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/PKG-INFO` & `maxia_pipedrive-1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: maxia_pipedrive
-Version: 1.1
+Version: 1.4
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/consts.py` & `maxia_pipedrive-1.4/maxia_pipedrive/consts.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/data_handler.py` & `maxia_pipedrive-1.4/maxia_pipedrive/data_handler.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/models.py` & `maxia_pipedrive-1.4/maxia_pipedrive/models.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive/relations.py` & `maxia_pipedrive-1.4/maxia_pipedrive/relations.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.1/maxia_pipedrive.egg-info/PKG-INFO` & `maxia_pipedrive-1.4/maxia_pipedrive.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: maxia-pipedrive
-Version: 1.1
+Version: 1.4
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `maxia_pipedrive-1.1/setup.py` & `maxia_pipedrive-1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from distutils.core import setup
+# from distutils.core import setup
+from setuptools import setup, find_packages
+version = '1.4'
 setup(
     # How you named your package folder (MyLib)
     name='maxia_pipedrive',
-    packages=['maxia_pipedrive'],   # Chose the same as "name"
-    version='1.1',      # Start with a small number and increase it with every change you make
+    packages=find_packages(),   # Chose the same as "name"
+    version=version,      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Maxia Pipedrive API handler',
     author='Max.ia Education',                   # Type in your name
     author_email='luiz@maxia.education',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/Max-ia-Education/maxia_pipedrive_api',
     # I explain this later on
-    download_url='https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.1.tar.gz',
+    download_url=f'https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz',
     #   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
         'numpy',
         'pandas',
         'tqdm'
     ],
     classifiers=[
```

