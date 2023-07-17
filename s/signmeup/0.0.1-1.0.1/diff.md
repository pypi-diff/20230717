# Comparing `tmp/signmeup-0.0.1.tar.gz` & `tmp/signmeup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\signmeup-0.0.1.tar", last modified: Mon Jul 17 12:29:51 2023, max compression
+gzip compressed data, was "dist\signmeup-1.0.1.tar", last modified: Mon Jul 17 12:12:12 2023, max compression
```

## Comparing `signmeup-0.0.1.tar` & `signmeup-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:51.011960 signmeup-0.0.1/
--rw-rw-rw-   0        0        0       41 2023-07-17 11:11:18.000000 signmeup-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4789 2023-07-17 12:29:51.010961 signmeup-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4248 2023-06-27 18:55:07.000000 signmeup-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.971068 signmeup-0.0.1/accounts/
--rw-rw-rw-   0        0        0        0 2023-06-22 09:09:29.000000 signmeup-0.0.1/accounts/__init__.py
--rw-rw-rw-   0        0        0      167 2023-07-05 18:55:29.000000 signmeup-0.0.1/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2023-06-22 09:09:29.000000 signmeup-0.0.1/accounts/apps.py
--rw-rw-rw-   0        0        0     2213 2023-07-16 18:29:42.000000 signmeup-0.0.1/accounts/middleware.py
--rw-rw-rw-   0        0        0     4681 2023-07-12 13:39:25.000000 signmeup-0.0.1/accounts/models.py
--rw-rw-rw-   0        0        0     2622 2023-07-12 13:43:59.000000 signmeup-0.0.1/accounts/serializers.py
--rw-rw-rw-   0        0        0    10580 2023-07-16 19:09:18.000000 signmeup-0.0.1/accounts/tests.py
--rw-rw-rw-   0        0        0      634 2023-07-16 18:26:16.000000 signmeup-0.0.1/accounts/urls.py
--rw-rw-rw-   0        0        0     9366 2023-07-16 18:43:40.000000 signmeup-0.0.1/accounts/views.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.982040 signmeup-0.0.1/core/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-0.0.1/core/__init__.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-0.0.1/core/asgi.py
--rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-0.0.1/core/settings.py
--rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-0.0.1/core/urls.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-0.0.1/core/wsgi.py
--rw-rw-rw-   0        0        0       42 2023-07-17 12:29:51.011960 signmeup-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1364 2023-07-17 12:29:36.000000 signmeup-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.993010 signmeup-0.0.1/signmeup/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-0.0.1/signmeup/__init__.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-0.0.1/signmeup/asgi.py
--rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-0.0.1/signmeup/settings.py
--rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-0.0.1/signmeup/urls.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-0.0.1/signmeup/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:51.007971 signmeup-0.0.1/signmeup.egg-info/
--rw-rw-rw-   0        0        0     4789 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      205 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 12:12:12.373015 signmeup-1.0.1/
+-rw-rw-rw-   0        0        0       41 2023-07-17 11:11:18.000000 signmeup-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4789 2023-07-17 12:12:12.372017 signmeup-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4248 2023-06-27 18:55:07.000000 signmeup-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:12:12.329133 signmeup-1.0.1/accounts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 09:09:29.000000 signmeup-1.0.1/accounts/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-07-05 18:55:29.000000 signmeup-1.0.1/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2023-06-22 09:09:29.000000 signmeup-1.0.1/accounts/apps.py
+-rw-rw-rw-   0        0        0     2213 2023-07-16 18:29:42.000000 signmeup-1.0.1/accounts/middleware.py
+-rw-rw-rw-   0        0        0     4681 2023-07-12 13:39:25.000000 signmeup-1.0.1/accounts/models.py
+-rw-rw-rw-   0        0        0     2622 2023-07-12 13:43:59.000000 signmeup-1.0.1/accounts/serializers.py
+-rw-rw-rw-   0        0        0    10580 2023-07-16 19:09:18.000000 signmeup-1.0.1/accounts/tests.py
+-rw-rw-rw-   0        0        0      634 2023-07-16 18:26:16.000000 signmeup-1.0.1/accounts/urls.py
+-rw-rw-rw-   0        0        0     9366 2023-07-16 18:43:40.000000 signmeup-1.0.1/accounts/views.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:12:12.341132 signmeup-1.0.1/core/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-1.0.1/core/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-1.0.1/core/asgi.py
+-rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-1.0.1/core/settings.py
+-rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-1.0.1/core/urls.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-1.0.1/core/wsgi.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:12:12.374012 signmeup-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-07-17 12:12:07.000000 signmeup-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:12:12.352072 signmeup-1.0.1/signmeup/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-1.0.1/signmeup/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-1.0.1/signmeup/asgi.py
+-rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-1.0.1/signmeup/settings.py
+-rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-1.0.1/signmeup/urls.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-1.0.1/signmeup/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:12:12.369025 signmeup-1.0.1/signmeup.egg-info/
+-rw-rw-rw-   0        0        0     4789 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      205 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-17 12:12:12.000000 signmeup-1.0.1/signmeup.egg-info/top_level.txt
```

### Comparing `signmeup-0.0.1/PKG-INFO` & `signmeup-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signmeup
-Version: 0.0.1
+Version: 1.0.1
 Summary: Sign Me Up API Package
 Home-page: https://github.com/yourusername/signmeup
 Author: Your Name
 Author-email: yourname@example.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `signmeup-0.0.1/README.md` & `signmeup-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/middleware.py` & `signmeup-1.0.1/accounts/middleware.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/models.py` & `signmeup-1.0.1/accounts/models.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/serializers.py` & `signmeup-1.0.1/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/tests.py` & `signmeup-1.0.1/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/urls.py` & `signmeup-1.0.1/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/views.py` & `signmeup-1.0.1/accounts/views.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/core/settings.py` & `signmeup-1.0.1/core/settings.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/core/urls.py` & `signmeup-1.0.1/core/urls.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/setup.py` & `signmeup-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='signmeup',
-    version='0.0.1',
+    version='1.0.1',
     author='Your Name',
     author_email='yourname@example.com',
     description='Sign Me Up API Package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/signmeup',
     packages=find_packages(),
@@ -25,15 +25,15 @@
         'pytz==2023.3',
         'sqlparse==0.4.4',
         'typing_extensions==4.6.3',
         'tzdata==2023.3',
     ],
     entry_points={
         'console_scripts': [
-            'signmeup-postinstall = post_install.py:main',
+            'signmeup-postinstall = post_install:main',
         ],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         #'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `signmeup-0.0.1/signmeup/settings.py` & `signmeup-1.0.1/signmeup/settings.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/signmeup/urls.py` & `signmeup-1.0.1/signmeup/urls.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/signmeup.egg-info/PKG-INFO` & `signmeup-1.0.1/signmeup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signmeup
-Version: 0.0.1
+Version: 1.0.1
 Summary: Sign Me Up API Package
 Home-page: https://github.com/yourusername/signmeup
 Author: Your Name
 Author-email: yourname@example.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `signmeup-0.0.1/signmeup.egg-info/SOURCES.txt` & `signmeup-1.0.1/signmeup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

