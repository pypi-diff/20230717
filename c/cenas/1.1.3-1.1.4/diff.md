# Comparing `tmp/cenas-1.1.3.tar.gz` & `tmp/cenas-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cenas-1.1.3.tar", last modified: Fri Jul 14 14:36:33 2023, max compression
+gzip compressed data, was "cenas-1.1.4.tar", last modified: Mon Jul 17 13:55:31 2023, max compression
```

## Comparing `cenas-1.1.3.tar` & `cenas-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 14:36:33.877823 cenas-1.1.3/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-14 14:36:33.877823 cenas-1.1.3/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1.3/README.md
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 14:36:33.877823 cenas-1.1.3/cenas/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.3/cenas/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1.3/cenas/admin.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1.3/cenas/apps.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 14:36:33.877823 cenas-1.1.3/cenas/migrations/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.3/cenas/migrations/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1.3/cenas/models.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1.3/cenas/tests.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1.3/cenas/urls.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      362 2023-07-14 12:10:33.000000 cenas-1.1.3/cenas/views.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 14:36:33.877823 cenas-1.1.3/cenas.egg-info/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      423 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/SOURCES.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/dependency_links.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/entry_points.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/requires.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-14 14:36:33.000000 cenas-1.1.3/cenas.egg-info/top_level.txt
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 14:36:33.877823 cenas-1.1.3/cenas1/
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1.3/cenas1/__init__.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.3/cenas1/asgi.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1.3/cenas1/settings.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1.3/cenas1/urls.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.3/cenas1/wsgi.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      192 2023-07-14 14:36:33.877823 cenas-1.1.3/setup.cfg
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      610 2023-07-14 14:31:09.000000 cenas-1.1.3/setup.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 13:55:31.710622 cenas-1.1.4/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 13:55:31.710622 cenas-1.1.4/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1.4/README.md
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 13:55:31.706622 cenas-1.1.4/cenas/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.4/cenas/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1.4/cenas/admin.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1.4/cenas/apps.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 13:55:31.706622 cenas-1.1.4/cenas/migrations/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.4/cenas/migrations/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1.4/cenas/models.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1.4/cenas/tests.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1.4/cenas/urls.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      500 2023-07-17 13:44:22.000000 cenas-1.1.4/cenas/views.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 13:55:31.706622 cenas-1.1.4/cenas.egg-info/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      423 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/entry_points.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/requires.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-17 13:55:31.000000 cenas-1.1.4/cenas.egg-info/top_level.txt
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 13:55:31.710622 cenas-1.1.4/cenas1/
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1.4/cenas1/__init__.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.4/cenas1/asgi.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1.4/cenas1/settings.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1.4/cenas1/urls.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.4/cenas1/wsgi.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      192 2023-07-17 13:55:31.710622 cenas-1.1.4/setup.cfg
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      610 2023-07-17 13:44:40.000000 cenas-1.1.4/setup.py
```

### Comparing `cenas-1.1.3/cenas1/settings.py` & `cenas-1.1.4/cenas1/settings.py`

 * *Files identical despite different names*

### Comparing `cenas-1.1.3/cenas1/urls.py` & `cenas-1.1.4/cenas1/urls.py`

 * *Files identical despite different names*

### Comparing `cenas-1.1.3/setup.py` & `cenas-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call(['python', 'post_install.py'])
 
 setup(
     name='cenas',
-    version='1.1.3',
+    version='1.1.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'django',
         # Add any other dependencies here
     ],
     cmdclass={
```

