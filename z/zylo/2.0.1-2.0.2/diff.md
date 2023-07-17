# Comparing `tmp/zylo-2.0.1.tar.gz` & `tmp/zylo-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-2.0.1.tar", last modified: Mon Jul 17 17:25:12 2023, max compression
+gzip compressed data, was "zylo-2.0.2.tar", last modified: Mon Jul 17 17:37:58 2023, max compression
```

## Comparing `zylo-2.0.1.tar` & `zylo-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:25:12.484123 zylo-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:25:12.480123 zylo-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-07-17 17:24:47.000000 zylo-2.0.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-17 17:25:12.484123 zylo-2.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-17 17:23:07.000000 zylo-2.0.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:25:12.480123 zylo-2.0.1/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-17 17:19:23.000000 zylo-2.0.1/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.1/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7194 2023-07-17 17:22:44.000000 zylo-2.0.1/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-17 17:22:15.000000 zylo-2.0.1/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.1/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.1/zylo/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-2.0.1/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.1/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:25:12.480123 zylo-2.0.1/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:25:12.000000 zylo-2.0.1/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-17 17:25:12.000000 zylo-2.0.1/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 17:25:12.000000 zylo-2.0.1/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-17 17:25:12.000000 zylo-2.0.1/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-17 17:25:12.000000 zylo-2.0.1/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:37:58.790048 zylo-2.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-07-17 17:30:54.000000 zylo-2.0.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-17 17:37:58.790048 zylo-2.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-17 17:30:44.000000 zylo-2.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-17 17:19:23.000000 zylo-2.0.2/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.2/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-07-17 17:37:28.000000 zylo-2.0.2/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-17 17:30:16.000000 zylo-2.0.2/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.2/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.2/zylo/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-2.0.2/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.2/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 17:37:58.790048 zylo-2.0.2/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5221 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-17 17:37:58.000000 zylo-2.0.2/zylo.egg-info/top_level.txt
```

### Comparing `zylo-2.0.1/PKG-INFO` & `zylo-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.1
+Version: 2.0.2
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,17 +51,17 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.1
+- Beta version 2.0.2
 - Last update of beta
-- Bug fixed with update --> 2.0.1
+- Bug fixed with update --> 2.0.2
 - Improved session management & Security
 - Updated Usage Guide 1.2.1
 - Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
 
 ```python
```

### Comparing `zylo-2.0.1/README.md` & `zylo-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.1
+- Beta version 2.0.2
 - Last update of beta
-- Bug fixed with update --> 2.0.1
+- Bug fixed with update --> 2.0.2
 - Improved session management & Security
 - Updated Usage Guide 1.2.1
 - Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
 
 ```python
```

### Comparing `zylo-2.0.1/setup.py` & `zylo-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='2.0.1',
+    version='2.0.2',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
```

### Comparing `zylo-2.0.1/zylo/JwT.py` & `zylo-2.0.2/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.1/zylo/app.py` & `zylo-2.0.2/zylo/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from jinja2 import Environment, FileSystemLoader
 from .sessions import session_manager
 from .blueprint import Blueprint
 from werkzeug.urls import url_encode
 from itsdangerous import URLSafeTimedSerializer
 import json
 import mimetypes
-from urllib.parse import quote as url_quote, quote_plus as url_quote_plus, urlencode as url_encode, \
-    parse_qs as url_decode
+from urllib.parse import quote as url_quote, quote_plus as url_quote_plus, urlencode as url_encode
 from werkzeug.utils import send_from_directory, safe_join
 
 # Create the application
 class Zylo:
     def __init__(self, __name__=None):
         self.template_folder='views'
         self.url_map = Map()
@@ -175,21 +174,14 @@
 
 def send_from_directory(directory, filename, **options):
     return send_from_directory(directory, filename, **options)
 
 def url_map(rules):
     return Map(rules)
 
-def url_encode(obj, charset='utf-8', errors='strict'):
-    return url_encode(obj, charset=charset, errors=errors)
-
-def url_decode(query_string, keep_blank_values=False, strict_parsing=False, charset=None, errors=None):
-    return url_decode(query_string, keep_blank_values=keep_blank_values, strict_parsing=strict_parsing,
-                      charset=charset, errors=errors)
-
 def stream_with_context(generator_or_function):
     return stream_with_context(generator_or_function)
 
 def make_unique_key():
     return base64.urlsafe_b64encode(os.urandom(32)).rstrip(b'=').decode('ascii')
 
 def url_quote(url, safe='/', encoding=None, errors=None):
```

### Comparing `zylo-2.0.1/zylo/blueprint.py` & `zylo-2.0.2/zylo/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from werkzeug.routing import Map, Rule
 from werkzeug.exceptions import NotFound
 from werkzeug.wrappers import Request, Response
-from sessions import session_manager
-
+from .sessions import session_manager
 
 class Blueprint:
     def __init__(self, name, import_name, url_prefix=''):
         self.name = name
         self.import_name = import_name
         self.url_prefix = url_prefix
         self.url_map = Map()
```

### Comparing `zylo-2.0.1/zylo/chiper.py` & `zylo-2.0.2/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.1/zylo/limiter.py` & `zylo-2.0.2/zylo/limiter.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.1/zylo/mailer.py` & `zylo-2.0.2/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.1/zylo/sessions.py` & `zylo-2.0.2/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.1/zylo.egg-info/PKG-INFO` & `zylo-2.0.2/zylo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.1
+Version: 2.0.2
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,17 +51,17 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.1
+- Beta version 2.0.2
 - Last update of beta
-- Bug fixed with update --> 2.0.1
+- Bug fixed with update --> 2.0.2
 - Improved session management & Security
 - Updated Usage Guide 1.2.1
 - Zylo Blueprint now support Session by default
 - Addedd more functions & Bug Fixes
 
 ```python
```

