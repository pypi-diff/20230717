# Comparing `tmp/cenas-1.1.8.tar.gz` & `tmp/cenas-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cenas-1.1.8.tar", last modified: Mon Jul 17 15:06:09 2023, max compression
+gzip compressed data, was "cenas-1.1.9.tar", last modified: Mon Jul 17 15:14:42 2023, max compression
```

## Comparing `cenas-1.1.8.tar` & `cenas-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:06:09.909928 cenas-1.1.8/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 15:06:09.909928 cenas-1.1.8/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1.8/README.md
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:06:09.905928 cenas-1.1.8/cenas/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.8/cenas/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1.8/cenas/admin.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1.8/cenas/apps.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:06:09.909928 cenas-1.1.8/cenas/migrations/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.8/cenas/migrations/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1.8/cenas/models.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1.8/cenas/tests.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1.8/cenas/urls.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      676 2023-07-17 15:00:52.000000 cenas-1.1.8/cenas/views.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:06:09.909928 cenas-1.1.8/cenas.egg-info/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      423 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/SOURCES.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/dependency_links.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/entry_points.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/requires.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-17 15:06:09.000000 cenas-1.1.8/cenas.egg-info/top_level.txt
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:06:09.909928 cenas-1.1.8/cenas1/
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1.8/cenas1/__init__.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.8/cenas1/asgi.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1.8/cenas1/settings.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1.8/cenas1/urls.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.8/cenas1/wsgi.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      192 2023-07-17 15:06:09.909928 cenas-1.1.8/setup.cfg
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      347 2023-07-17 15:05:58.000000 cenas-1.1.8/setup.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:14:42.939103 cenas-1.1.9/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 15:14:42.939103 cenas-1.1.9/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1.9/README.md
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:14:42.939103 cenas-1.1.9/cenas/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.9/cenas/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1.9/cenas/admin.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1.9/cenas/apps.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:14:42.939103 cenas-1.1.9/cenas/migrations/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.9/cenas/migrations/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1.9/cenas/models.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1.9/cenas/tests.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1.9/cenas/urls.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      764 2023-07-17 15:14:18.000000 cenas-1.1.9/cenas/views.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:14:42.939103 cenas-1.1.9/cenas.egg-info/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      423 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/entry_points.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/requires.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-17 15:14:42.000000 cenas-1.1.9/cenas.egg-info/top_level.txt
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-17 15:14:42.939103 cenas-1.1.9/cenas1/
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1.9/cenas1/__init__.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.9/cenas1/asgi.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1.9/cenas1/settings.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1.9/cenas1/urls.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.9/cenas1/wsgi.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      192 2023-07-17 15:14:42.939103 cenas-1.1.9/setup.cfg
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      347 2023-07-17 15:14:38.000000 cenas-1.1.9/setup.py
```

### Comparing `cenas-1.1.8/cenas/views.py` & `cenas-1.1.9/cenas/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from django.shortcuts import render
 from django.core.management import call_command
 from django.core.wsgi import get_wsgi_application
 import subprocess
 import os
 
+# Set up Django settings
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'cenas.settings')
+application = get_wsgi_application()
+
 def home(request):
     return render(request, 'home.html')
 
 def upload_form(request):
     return render(request, 'upload_form.html')
 
 def run():
@@ -15,12 +19,11 @@
     project_root = os.path.dirname(os.path.abspath(__file__))
     os.chdir(project_root)
 
     # Run the migrations
     call_command('migrate')
 
     # Start the Django development server
-    application = get_wsgi_application()
     subprocess.Popen(['python', 'manage.py', 'runserver'])
 
 if __name__ == '__main__':
     run()
```

### Comparing `cenas-1.1.8/cenas1/settings.py` & `cenas-1.1.9/cenas1/settings.py`

 * *Files identical despite different names*

### Comparing `cenas-1.1.8/cenas1/urls.py` & `cenas-1.1.9/cenas1/urls.py`

 * *Files identical despite different names*

