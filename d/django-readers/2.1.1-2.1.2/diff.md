# Comparing `tmp/django-readers-2.1.1.tar.gz` & `tmp/django-readers-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-readers-2.1.1.tar", last modified: Tue Mar 21 16:32:59 2023, max compression
+gzip compressed data, was "django-readers-2.1.2.tar", last modified: Mon Jul 17 12:57:52 2023, max compression
```

## Comparing `django-readers-2.1.1.tar` & `django-readers-2.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:32:59.029585 django-readers-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-21 16:32:44.000000 django-readers-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-21 16:32:59.029585 django-readers-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-21 16:32:44.000000 django-readers-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:32:59.029585 django-readers-2.1.1/django_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/producers.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/projectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/qs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-21 16:32:44.000000 django-readers-2.1.1/django_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:32:59.029585 django-readers-2.1.1/django_readers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-21 16:32:58.000000 django-readers-2.1.1/django_readers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-21 16:32:58.000000 django-readers-2.1.1/django_readers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:32:58.000000 django-readers-2.1.1/django_readers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 16:32:58.000000 django-readers-2.1.1/django_readers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 16:32:58.000000 django-readers-2.1.1/django_readers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-21 16:32:59.029585 django-readers-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-21 16:32:44.000000 django-readers-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:57:52.740948 django-readers-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 12:57:36.000000 django-readers-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-17 12:57:52.740948 django-readers-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-17 12:57:36.000000 django-readers-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:57:52.740948 django-readers-2.1.2/django_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/producers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/projectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-17 12:57:36.000000 django-readers-2.1.2/django_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:57:52.740948 django-readers-2.1.2/django_readers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-17 12:57:52.000000 django-readers-2.1.2/django_readers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-17 12:57:52.000000 django-readers-2.1.2/django_readers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:57:52.000000 django-readers-2.1.2/django_readers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:57:52.000000 django-readers-2.1.2/django_readers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 12:57:52.000000 django-readers-2.1.2/django_readers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 12:57:52.740948 django-readers-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-17 12:57:36.000000 django-readers-2.1.2/setup.py
```

### Comparing `django-readers-2.1.1/LICENSE` & `django-readers-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/PKG-INFO` & `django-readers-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-readers
-Version: 2.1.1
+Version: 2.1.2
 Summary: A lightweight function-oriented toolkit for better organisation of business logic and efficient selection and projection of data in Django projects.
 Home-page: https://www.django-readers.org
 Author: DabApps
 Author-email: hello@dabapps.com
 License: BSD
 Project-URL: Changelog, https://github.com/dabapps/django-readers/releases
 Project-URL: Issues, https://github.com/dabapps/django-readers/issues
```

### Comparing `django-readers-2.1.1/README.md` & `django-readers-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/pairs.py` & `django-readers-2.1.2/django_readers/pairs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/producers.py` & `django-readers-2.1.2/django_readers/producers.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/projectors.py` & `django-readers-2.1.2/django_readers/projectors.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/qs.py` & `django-readers-2.1.2/django_readers/qs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/rest_framework.py` & `django-readers-2.1.2/django_readers/rest_framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,17 @@
                     return self(result)
 
                 wrapper.out = field_or_dict
                 return wrapper
             else:
                 if isinstance(item, str):
                     item = StringWithOutAttribute(item)
+                    item.out = field_or_dict
                 if isinstance(item, tuple):
                     item = PairWithOutAttribute(item)
-                item.out = field_or_dict
+                    item.out = field_or_dict
                 return item
 
         def __rrshift__(self, other):
             return self(other)
 
     return ShiftableDecorator()
```

### Comparing `django-readers-2.1.1/django_readers/specs.py` & `django-readers-2.1.2/django_readers/specs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers/utils.py` & `django-readers-2.1.2/django_readers/utils.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.1.1/django_readers.egg-info/PKG-INFO` & `django-readers-2.1.2/django_readers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-readers
-Version: 2.1.1
+Version: 2.1.2
 Summary: A lightweight function-oriented toolkit for better organisation of business logic and efficient selection and projection of data in Django projects.
 Home-page: https://www.django-readers.org
 Author: DabApps
 Author-email: hello@dabapps.com
 License: BSD
 Project-URL: Changelog, https://github.com/dabapps/django-readers/releases
 Project-URL: Issues, https://github.com/dabapps/django-readers/issues
```

### Comparing `django-readers-2.1.1/setup.py` & `django-readers-2.1.2/setup.py`

 * *Files identical despite different names*

