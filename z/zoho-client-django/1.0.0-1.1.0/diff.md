# Comparing `tmp/zoho-client-django-1.0.0.tar.gz` & `tmp/zoho-client-django-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho-client-django-1.0.0.tar", last modified: Sat Jul 15 15:25:51 2023, max compression
+gzip compressed data, was "zoho-client-django-1.1.0.tar", last modified: Sun Jul 16 22:01:27 2023, max compression
```

## Comparing `zoho-client-django-1.0.0.tar` & `zoho-client-django-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.325658 zoho-client-django-1.0.0/
--rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.0.0/LICENSE
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-15 15:25:51.325521 zoho-client-django-1.0.0/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.0.0/README.md
--rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-15 15:25:51.325697 zoho-client-django-1.0.0/setup.cfg
--rw-r--r--   0 guy        (501) staff       (20)      768 2023-07-15 15:25:06.000000 zoho-client-django-1.0.0/setup.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.322791 zoho-client-django-1.0.0/zoho_client/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.0.0/zoho_client/admin.py
--rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.0.0/zoho_client/apps.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.323560 zoho-client-django-1.0.0/zoho_client/migrations/
--rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.0.0/zoho_client/migrations/0001_initial.py
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/migrations/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.0.0/zoho_client/models.py
--rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/tests.py
--rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.0.0/zoho_client/views.py
--rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.0.0/zoho_client/zoho.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.324264 zoho-client-django-1.0.0/zoho_client_django.egg-info/
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)      596 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/SOURCES.txt
--rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/dependency_links.txt
--rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/requires.txt
--rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-15 15:25:51.000000 zoho-client-django-1.0.0/zoho_client_django.egg-info/top_level.txt
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-15 15:25:51.325184 zoho-client-django-1.0.0/zoho_test_project/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.0.0/zoho_test_project/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/asgi.py
--rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.0.0/zoho_test_project/settings.py
--rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/urls.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.0.0/zoho_test_project/wsgi.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.028766 zoho-client-django-1.1.0/
+-rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.1.0/LICENSE
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:01:27.028608 zoho-client-django-1.1.0/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.1.0/README.md
+-rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-16 22:01:27.028875 zoho-client-django-1.1.0/setup.cfg
+-rw-r--r--   0 guy        (501) staff       (20)      768 2023-07-16 22:00:48.000000 zoho-client-django-1.1.0/setup.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.025140 zoho-client-django-1.1.0/zoho_client/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.1.0/zoho_client/admin.py
+-rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.1.0/zoho_client/apps.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.025954 zoho-client-django-1.1.0/zoho_client/migrations/
+-rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.1.0/zoho_client/migrations/0001_initial.py
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/migrations/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.1.0/zoho_client/models.py
+-rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/tests.py
+-rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/views.py
+-rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.1.0/zoho_client/zoho.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.026708 zoho-client-django-1.1.0/zoho_client_django.egg-info/
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)      596 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/SOURCES.txt
+-rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/dependency_links.txt
+-rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/requires.txt
+-rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/top_level.txt
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.028236 zoho-client-django-1.1.0/zoho_test_project/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.1.0/zoho_test_project/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/asgi.py
+-rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.1.0/zoho_test_project/settings.py
+-rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/urls.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/wsgi.py
```

### Comparing `zoho-client-django-1.0.0/LICENSE` & `zoho-client-django-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/PKG-INFO` & `zoho-client-django-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.0.0
+Version: 1.1.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zoho-client-django-1.0.0/README.md` & `zoho-client-django-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/setup.py` & `zoho-client-django-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="zoho-client-django",
-    version="1.0.0",  # Update this for new versions
+    version="1.1.0",  # Update this for new versions
     description="Django app which is a client for the Zoho CRM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Guy Moller",
     author_email="guy.moller@gmail.com",
     url="https://github.com/gosourcellc/zoho-client-django",
     packages=find_packages(),
```

### Comparing `zoho-client-django-1.0.0/zoho_client/admin.py` & `zoho-client-django-1.1.0/zoho_client/admin.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/zoho_client/migrations/0001_initial.py` & `zoho-client-django-1.1.0/zoho_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/zoho_client/zoho.py` & `zoho-client-django-1.1.0/zoho_client/zoho.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/zoho_client_django.egg-info/PKG-INFO` & `zoho-client-django-1.1.0/zoho_client_django.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.0.0
+Version: 1.1.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zoho-client-django-1.0.0/zoho_client_django.egg-info/SOURCES.txt` & `zoho-client-django-1.1.0/zoho_client_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/zoho_test_project/settings.py` & `zoho-client-django-1.1.0/zoho_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.0.0/zoho_test_project/urls.py` & `zoho-client-django-1.1.0/zoho_test_project/urls.py`

 * *Files identical despite different names*

