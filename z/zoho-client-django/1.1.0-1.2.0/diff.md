# Comparing `tmp/zoho-client-django-1.1.0.tar.gz` & `tmp/zoho-client-django-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho-client-django-1.1.0.tar", last modified: Sun Jul 16 22:01:27 2023, max compression
+gzip compressed data, was "zoho-client-django-1.2.0.tar", last modified: Sun Jul 16 22:38:14 2023, max compression
```

## Comparing `zoho-client-django-1.1.0.tar` & `zoho-client-django-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.028766 zoho-client-django-1.1.0/
--rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.1.0/LICENSE
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:01:27.028608 zoho-client-django-1.1.0/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.1.0/README.md
--rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-16 22:01:27.028875 zoho-client-django-1.1.0/setup.cfg
--rw-r--r--   0 guy        (501) staff       (20)      768 2023-07-16 22:00:48.000000 zoho-client-django-1.1.0/setup.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.025140 zoho-client-django-1.1.0/zoho_client/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.1.0/zoho_client/admin.py
--rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.1.0/zoho_client/apps.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.025954 zoho-client-django-1.1.0/zoho_client/migrations/
--rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.1.0/zoho_client/migrations/0001_initial.py
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/migrations/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.1.0/zoho_client/models.py
--rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/tests.py
--rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.1.0/zoho_client/views.py
--rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.1.0/zoho_client/zoho.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.026708 zoho-client-django-1.1.0/zoho_client_django.egg-info/
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)      596 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/SOURCES.txt
--rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/dependency_links.txt
--rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/requires.txt
--rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-16 22:01:27.000000 zoho-client-django-1.1.0/zoho_client_django.egg-info/top_level.txt
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:01:27.028236 zoho-client-django-1.1.0/zoho_test_project/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.1.0/zoho_test_project/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/asgi.py
--rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.1.0/zoho_test_project/settings.py
--rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/urls.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.1.0/zoho_test_project/wsgi.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.876592 zoho-client-django-1.2.0/
+-rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.2.0/LICENSE
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:38:14.876447 zoho-client-django-1.2.0/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.2.0/README.md
+-rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-16 22:38:14.876640 zoho-client-django-1.2.0/setup.cfg
+-rw-r--r--   0 guy        (501) staff       (20)      867 2023-07-16 22:37:59.000000 zoho-client-django-1.2.0/setup.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.873652 zoho-client-django-1.2.0/zoho_client/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.0/zoho_client/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.2.0/zoho_client/admin.py
+-rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.2.0/zoho_client/apps.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.874122 zoho-client-django-1.2.0/zoho_client/migrations/
+-rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.2.0/zoho_client/migrations/0001_initial.py
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.0/zoho_client/migrations/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.2.0/zoho_client/models.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.871446 zoho-client-django-1.2.0/zoho_client/templates/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.871486 zoho-client-django-1.2.0/zoho_client/templates/admin/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.871525 zoho-client-django-1.2.0/zoho_client/templates/admin/zoho_client/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.874506 zoho-client-django-1.2.0/zoho_client/templates/admin/zoho_client/zohotoken/
+-rw-r--r--   0 guy        (501) staff       (20)      242 2023-07-15 11:22:51.000000 zoho-client-django-1.2.0/zoho_client/templates/admin/zoho_client/zohotoken/fetch_tokens.html
+-rw-r--r--   0 guy        (501) staff       (20)      320 2023-07-15 13:56:34.000000 zoho-client-django-1.2.0/zoho_client/templates/admin/zoho_client/zohotoken/zoho_token_change_list.html
+-rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.2.0/zoho_client/tests.py
+-rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.2.0/zoho_client/views.py
+-rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.2.0/zoho_client/zoho.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.875230 zoho-client-django-1.2.0/zoho_client_django.egg-info/
+-rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-16 22:38:14.000000 zoho-client-django-1.2.0/zoho_client_django.egg-info/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)      742 2023-07-16 22:38:14.000000 zoho-client-django-1.2.0/zoho_client_django.egg-info/SOURCES.txt
+-rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-16 22:38:14.000000 zoho-client-django-1.2.0/zoho_client_django.egg-info/dependency_links.txt
+-rw-r--r--   0 guy        (501) staff       (20)       41 2023-07-16 22:38:14.000000 zoho-client-django-1.2.0/zoho_client_django.egg-info/requires.txt
+-rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-16 22:38:14.000000 zoho-client-django-1.2.0/zoho_client_django.egg-info/top_level.txt
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-16 22:38:14.876124 zoho-client-django-1.2.0/zoho_test_project/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.2.0/zoho_test_project/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.0/zoho_test_project/asgi.py
+-rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.2.0/zoho_test_project/settings.py
+-rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.2.0/zoho_test_project/urls.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.0/zoho_test_project/wsgi.py
```

### Comparing `zoho-client-django-1.1.0/LICENSE` & `zoho-client-django-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/PKG-INFO` & `zoho-client-django-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.1.0
+Version: 1.2.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zoho-client-django-1.1.0/README.md` & `zoho-client-django-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/setup.py` & `zoho-client-django-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 # Read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="zoho-client-django",
-    version="1.1.0",  # Update this for new versions
+    version="1.2.0",  # Update this for new versions
     description="Django app which is a client for the Zoho CRM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Guy Moller",
     author_email="guy.moller@gmail.com",
     url="https://github.com/gosourcellc/zoho-client-django",
     packages=find_packages(),
+    package_data={
+        "zoho_client": ["templates/admin/zoho_client/zohotoken/*.html"],
+    },
     install_requires=[
         "Django>=4.2.3,<5.0",
         "requests>=2.31.0,<3.0",
     ],
 )
```

### Comparing `zoho-client-django-1.1.0/zoho_client/admin.py` & `zoho-client-django-1.2.0/zoho_client/admin.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/zoho_client/migrations/0001_initial.py` & `zoho-client-django-1.2.0/zoho_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/zoho_client/zoho.py` & `zoho-client-django-1.2.0/zoho_client/zoho.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/zoho_client_django.egg-info/PKG-INFO` & `zoho-client-django-1.2.0/zoho_client_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.1.0
+Version: 1.2.0
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `zoho-client-django-1.1.0/zoho_client_django.egg-info/SOURCES.txt` & `zoho-client-django-1.2.0/zoho_client_django.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 zoho_client/apps.py
 zoho_client/models.py
 zoho_client/tests.py
 zoho_client/views.py
 zoho_client/zoho.py
 zoho_client/migrations/0001_initial.py
 zoho_client/migrations/__init__.py
+zoho_client/templates/admin/zoho_client/zohotoken/fetch_tokens.html
+zoho_client/templates/admin/zoho_client/zohotoken/zoho_token_change_list.html
 zoho_client_django.egg-info/PKG-INFO
 zoho_client_django.egg-info/SOURCES.txt
 zoho_client_django.egg-info/dependency_links.txt
 zoho_client_django.egg-info/requires.txt
 zoho_client_django.egg-info/top_level.txt
 zoho_test_project/__init__.py
 zoho_test_project/asgi.py
```

### Comparing `zoho-client-django-1.1.0/zoho_test_project/settings.py` & `zoho-client-django-1.2.0/zoho_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.1.0/zoho_test_project/urls.py` & `zoho-client-django-1.2.0/zoho_test_project/urls.py`

 * *Files identical despite different names*

