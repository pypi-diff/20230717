# Comparing `tmp/django-followit-0.5.0.tar.gz` & `tmp/django-followit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-followit-0.5.0.tar", last modified: Mon Apr  4 00:26:29 2022, max compression
+gzip compressed data, was "django-followit-0.6.0.tar", last modified: Mon Jul 17 19:45:21 2023, max compression
```

## Comparing `django-followit-0.5.0.tar` & `django-followit-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2022-04-04 00:26:29.000000 django-followit-0.5.0/
--rw-r--r--   0 evgeny     (501) staff       (20)     2666 2022-04-04 00:26:29.000000 django-followit-0.5.0/PKG-INFO
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2022-04-04 00:26:29.000000 django-followit-0.5.0/django_followit.egg-info/
--rw-r--r--   0 evgeny     (501) staff       (20)     2666 2022-04-04 00:26:29.000000 django-followit-0.5.0/django_followit.egg-info/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)      595 2022-04-04 00:26:29.000000 django-followit-0.5.0/django_followit.egg-info/SOURCES.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        9 2022-04-04 00:26:29.000000 django-followit-0.5.0/django_followit.egg-info/top_level.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        1 2022-04-04 00:26:29.000000 django-followit-0.5.0/django_followit.egg-info/dependency_links.txt
--rw-r--r--   0 evgeny     (501) staff       (20)      284 2022-04-04 00:12:13.000000 django-followit-0.5.0/MANIFEST.in
--rw-r--r--   0 evgeny     (501) staff       (20)     1142 2022-04-04 00:17:09.000000 django-followit-0.5.0/setup.py
--rw-r--r--   0 evgeny     (501) staff       (20)       38 2022-04-04 00:26:29.000000 django-followit-0.5.0/setup.cfg
--rw-r--r--   0 evgeny     (501) staff       (20)    12537 2022-04-04 00:12:13.000000 django-followit-0.5.0/ez_setup.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1909 2022-04-04 00:16:51.000000 django-followit-0.5.0/README.rst
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2022-04-04 00:26:29.000000 django-followit-0.5.0/followit/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2022-04-04 00:26:29.000000 django-followit-0.5.0/followit/migrations/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/migrations/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)      971 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/migrations/0001_initial.py
--rw-r--r--   0 evgeny     (501) staff       (20)     2435 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/compat.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1519 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/LICENSE
--rw-r--r--   0 evgeny     (501) staff       (20)      540 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/models.py
--rw-r--r--   0 evgeny     (501) staff       (20)       73 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/TODO.rst
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2022-04-04 00:26:29.000000 django-followit-0.5.0/followit/tests/
--rw-r--r--   0 evgeny     (501) staff       (20)      225 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/models.py
--rw-r--r--   0 evgeny     (501) staff       (20)      473 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)      455 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/settings.py
--rwxr-xr-x   0 evgeny     (501) staff       (20)      257 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/manage.py
--rw-r--r--   0 evgeny     (501) staff       (20)      242 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/README.rst
--rw-r--r--   0 evgeny     (501) staff       (20)     1314 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/tests.py
--rw-r--r--   0 evgeny     (501) staff       (20)      553 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/tests/runtests.py
--rw-r--r--   0 evgeny     (501) staff       (20)     6020 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1610 2022-04-04 00:17:33.000000 django-followit-0.5.0/followit/utils.py
--rw-r--r--   0 evgeny     (501) staff       (20)      549 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1818 2022-04-04 00:12:13.000000 django-followit-0.5.0/followit/views.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-17 19:45:21.096167 django-followit-0.6.0/
+-rw-r--r--   0 evgeny     (501) staff       (20)      284 2022-04-04 00:12:13.000000 django-followit-0.6.0/MANIFEST.in
+-rw-r--r--   0 evgeny     (501) staff       (20)     2690 2023-07-17 19:45:21.095711 django-followit-0.6.0/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     1953 2023-07-15 19:15:16.000000 django-followit-0.6.0/README.rst
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-17 19:45:21.084684 django-followit-0.6.0/django_followit.egg-info/
+-rw-r--r--   0 evgeny     (501) staff       (20)     2690 2023-07-17 19:45:20.000000 django-followit-0.6.0/django_followit.egg-info/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)      595 2023-07-17 19:45:21.000000 django-followit-0.6.0/django_followit.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-17 19:45:20.000000 django-followit-0.6.0/django_followit.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        9 2023-07-17 19:45:20.000000 django-followit-0.6.0/django_followit.egg-info/top_level.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)    12537 2022-04-04 00:12:13.000000 django-followit-0.6.0/ez_setup.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-17 19:45:21.090077 django-followit-0.6.0/followit/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1519 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/LICENSE
+-rw-r--r--   0 evgeny     (501) staff       (20)       73 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/TODO.rst
+-rw-r--r--   0 evgeny     (501) staff       (20)     6020 2023-07-14 21:44:21.000000 django-followit-0.6.0/followit/__init__.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     2435 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/compat.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-17 19:45:21.091357 django-followit-0.6.0/followit/migrations/
+-rw-r--r--   0 evgeny     (501) staff       (20)      971 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/migrations/0001_initial.py
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/migrations/__init__.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      540 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/models.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-17 19:45:21.095177 django-followit-0.6.0/followit/tests/
+-rw-r--r--   0 evgeny     (501) staff       (20)      242 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/README.rst
+-rw-r--r--   0 evgeny     (501) staff       (20)      473 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/__init__.py
+-rwxr-xr-x   0 evgeny     (501) staff       (20)      257 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/manage.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      225 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/models.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      553 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/runtests.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      455 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/settings.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1314 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/tests/tests.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      651 2023-07-15 19:13:17.000000 django-followit-0.6.0/followit/urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1610 2022-04-04 00:31:36.000000 django-followit-0.6.0/followit/utils.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1818 2022-04-04 00:12:13.000000 django-followit-0.6.0/followit/views.py
+-rw-r--r--   0 evgeny     (501) staff       (20)       38 2023-07-17 19:45:21.096293 django-followit-0.6.0/setup.cfg
+-rw-r--r--   0 evgeny     (501) staff       (20)     1142 2023-07-16 17:26:35.000000 django-followit-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-followit-0.5.0/PKG-INFO` & `django-followit-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-followit
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Django application that allows users to follow django model objects
 Home-page: https://github.com/ASKBOT/django-followit
 Author: Evgeny.Fadeev
 Author-email: evgeny.fadeev@gmail.com
 License: BSD License
 Keywords: follow,database,django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
@@ -28,19 +27,20 @@
 
 Release Notes
 =============
 
 The list below shows compatibility of `django-followit` with versions of Django and Python.
 Python version compatibility was thoroughly tested only with release `0.4.0`::
 
-  * ``0.5.x`` supports django versions 1.10 and up.
-  * ``0.4.x`` django 1.7(**) - 1.9. Python 2 and 3.
-  * ``0.3.x`` - django 1.9 - 1.11
-  * ``0.2.x`` - django 1.8
-  * ``0.1.x`` - django 1.7
+  * ``0.6.x`` supports Django 1.10 to 4.x
+  * ``0.5.x`` supports Django versions 1.10 up to 3.2
+  * ``0.4.x`` Django 1.7(**) - 1.9. Python 2 and 3.
+  * ``0.3.x`` - Django 1.9 - 1.11
+  * ``0.2.x`` - Django 1.8
+  * ``0.1.x`` - Django 1.7
   * ``0.0.9`` can be used for the earlier versions
 
 (**) versions ``0.4.x`` do not support Django 1.7 with Python 3.
 
 Setup
 =====
 
@@ -75,9 +75,7 @@
     {% url follow_object "somemodel" item_id %} #model name lower case
 
     /unfollow/<model_name>/<item_id>/
     {% url unfollow_object "somemodel" item_id %} #lower case model name
 
     /toggle-follow/<model_name>/<item_id>/
     {% url toggle_follow_object "somemodel" item_id %} #lower case model name
-
-
```

### Comparing `django-followit-0.5.0/django_followit.egg-info/PKG-INFO` & `django-followit-0.6.0/django_followit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-followit
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Django application that allows users to follow django model objects
 Home-page: https://github.com/ASKBOT/django-followit
 Author: Evgeny.Fadeev
 Author-email: evgeny.fadeev@gmail.com
 License: BSD License
 Keywords: follow,database,django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
@@ -28,19 +27,20 @@
 
 Release Notes
 =============
 
 The list below shows compatibility of `django-followit` with versions of Django and Python.
 Python version compatibility was thoroughly tested only with release `0.4.0`::
 
-  * ``0.5.x`` supports django versions 1.10 and up.
-  * ``0.4.x`` django 1.7(**) - 1.9. Python 2 and 3.
-  * ``0.3.x`` - django 1.9 - 1.11
-  * ``0.2.x`` - django 1.8
-  * ``0.1.x`` - django 1.7
+  * ``0.6.x`` supports Django 1.10 to 4.x
+  * ``0.5.x`` supports Django versions 1.10 up to 3.2
+  * ``0.4.x`` Django 1.7(**) - 1.9. Python 2 and 3.
+  * ``0.3.x`` - Django 1.9 - 1.11
+  * ``0.2.x`` - Django 1.8
+  * ``0.1.x`` - Django 1.7
   * ``0.0.9`` can be used for the earlier versions
 
 (**) versions ``0.4.x`` do not support Django 1.7 with Python 3.
 
 Setup
 =====
 
@@ -75,9 +75,7 @@
     {% url follow_object "somemodel" item_id %} #model name lower case
 
     /unfollow/<model_name>/<item_id>/
     {% url unfollow_object "somemodel" item_id %} #lower case model name
 
     /toggle-follow/<model_name>/<item_id>/
     {% url toggle_follow_object "somemodel" item_id %} #lower case model name
-
-
```

### Comparing `django-followit-0.5.0/django_followit.egg-info/SOURCES.txt` & `django-followit-0.6.0/django_followit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/setup.py` & `django-followit-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import ez_setup
 ez_setup.use_setuptools()
 
 setup(
     name="django-followit",
-    version='0.5.0',
+    version='0.6.0',
     description='A Django application that allows users to follow django model objects',
     packages=find_packages(),
     author='Evgeny.Fadeev',
     author_email='evgeny.fadeev@gmail.com',
     license='BSD License',
     keywords='follow, database, django',
     url='https://github.com/ASKBOT/django-followit',
```

### Comparing `django-followit-0.5.0/ez_setup.py` & `django-followit-0.6.0/ez_setup.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/README.rst` & `django-followit-0.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 Release Notes
 =============
 
 The list below shows compatibility of `django-followit` with versions of Django and Python.
 Python version compatibility was thoroughly tested only with release `0.4.0`::
 
-  * ``0.5.x`` supports django versions 1.10 and up.
-  * ``0.4.x`` django 1.7(**) - 1.9. Python 2 and 3.
-  * ``0.3.x`` - django 1.9 - 1.11
-  * ``0.2.x`` - django 1.8
-  * ``0.1.x`` - django 1.7
+  * ``0.6.x`` supports Django 1.10 to 4.x
+  * ``0.5.x`` supports Django versions 1.10 up to 3.2
+  * ``0.4.x`` Django 1.7(**) - 1.9. Python 2 and 3.
+  * ``0.3.x`` - Django 1.9 - 1.11
+  * ``0.2.x`` - Django 1.8
+  * ``0.1.x`` - Django 1.7
   * ``0.0.9`` can be used for the earlier versions
 
 (**) versions ``0.4.x`` do not support Django 1.7 with Python 3.
 
 Setup
 =====
```

### Comparing `django-followit-0.5.0/followit/migrations/0001_initial.py` & `django-followit-0.6.0/followit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/compat.py` & `django-followit-0.6.0/followit/compat.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/LICENSE` & `django-followit-0.6.0/followit/LICENSE`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/models.py` & `django-followit-0.6.0/followit/models.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/tests/tests.py` & `django-followit-0.6.0/followit/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/tests/runtests.py` & `django-followit-0.6.0/followit/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/__init__.py` & `django-followit-0.6.0/followit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 if django.VERSION[:2] == (1, 7) and sys.version_info.major == 3:
     msg = """\n\nThis version of django-followit does not Django 1.7 with Python 3
 Either use Python 2.7 or upgrade Django to version from 1.8 up to 3.
 """
     raise ImproperlyConfigured(msg)
 
-if django.VERSION < (1, 7) or django.VERSION >= (4, 0):
+if django.VERSION < (1, 7) or django.VERSION >= (5, 0):
     msg = "\n\nThis version of django-followit supports Django 1.7 - 3."
 
     if django.VERSION < (1, 7):
         msg += "\nFor earlier Django versions try django-followit 0.0.9"
 
     raise ImproperlyConfigured(msg)
```

### Comparing `django-followit-0.5.0/followit/utils.py` & `django-followit-0.6.0/followit/utils.py`

 * *Files identical despite different names*

### Comparing `django-followit-0.5.0/followit/urls.py` & `django-followit-0.6.0/followit/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from django.conf.urls import url
+try:
+    from django.conf.urls import url as re_path # Django 1.11
+except ImportError:
+    from django.urls import re_path
 
 from . import views as FollowitViews
 
 urlpatterns = [
-    url(
+    re_path(
         r'^follow/(?P<model_name>\w+)/(?P<object_id>\d+)/$',
         FollowitViews.follow_object,
         name = 'follow_object'
     ),
-    url(
+    re_path(
         r'^unfollow/(?P<model_name>\w+)/(?P<object_id>\d+)/$',
         FollowitViews.unfollow_object,
         name = 'unfollow_object'
     ),
-    url(
+    re_path(
         r'^toggle-follow/(?P<model_name>\w+)/(?P<object_id>\d+)/$',
         FollowitViews.toggle_follow_object,
         name='toggle_follow_object'
     )
 ]
```

### Comparing `django-followit-0.5.0/followit/views.py` & `django-followit-0.6.0/followit/views.py`

 * *Files identical despite different names*

