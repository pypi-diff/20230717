# Comparing `tmp/xnbtd-0.0.2.tar.gz` & `tmp/xnbtd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.2.tar", max compression
+gzip compressed data, was "xnbtd-0.0.3.tar", max compression
```

## Comparing `xnbtd-0.0.2.tar` & `xnbtd-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,32 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.2/README.md
--rwxr-xr-x   0        0        0     3589 2023-07-17 17:03:02.397891 xnbtd-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.2/xnbtd/__init__.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.2/xnbtd/asgi.py
--rwxr-xr-x   0        0        0      591 2023-07-17 16:48:13.440460 xnbtd-0.0.2/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.2/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5530 2023-07-17 15:12:48.230236 xnbtd-0.0.2/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.2/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.2/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.2/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0      290 2023-07-17 14:14:11.419116 xnbtd-0.0.2/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.2/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 xnbtd-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.3/README.md
+-rwxr-xr-x   0        0        0     3589 2023-07-17 17:29:42.819210 xnbtd-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.3/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.3/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.314243 xnbtd-0.0.3/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.3/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.3/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-07-17 11:37:10.000000 xnbtd-0.0.3/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      980 2023-07-17 11:37:06.366946 xnbtd-0.0.3/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.3/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.3/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.3/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.3/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.3/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.3/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5542 2023-07-17 17:18:11.522098 xnbtd-0.0.3/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.3/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.3/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.3/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.188792 xnbtd-0.0.3/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0     1720 2023-07-17 14:22:40.776230 xnbtd-0.0.3/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.3/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.3/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     2230 2023-07-17 11:37:10.000000 xnbtd-0.0.3/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     4015 2023-07-17 11:36:58.456118 xnbtd-0.0.3/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.3/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.3/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.3/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      290 2023-07-17 14:14:11.419116 xnbtd-0.0.3/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.3/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 xnbtd-0.0.3/PKG-INFO
```

### Comparing `xnbtd-0.0.2/LICENSE` & `xnbtd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.2/README.md` & `xnbtd-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.2/pyproject.toml` & `xnbtd-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.2"
+version = "0.0.3"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-0.0.2/xnbtd/publish.py` & `xnbtd-0.0.3/xnbtd/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from poetry_publish.publish import poetry_publish
 from poetry_publish.utils.subprocess_utils import verbose_check_call
 
 import xnbtd
 
 
-PACKAGE_ROOT = Path(xnbtd.__file__).parent.parent.parent
+PACKAGE_ROOT = Path(xnbtd.__file__).parent.parent
 
 
 def publish():
     """
     Publish to PyPi
     Call this via:
         $ poetry run publish
```

### Comparing `xnbtd-0.0.2/xnbtd/settings/base.py` & `xnbtd-0.0.3/xnbtd/settings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
-    'tours.apps.ToursConfig',
-    'plannings.apps.PlanningsConfig',
+    'xnbtd.tours.apps.ToursConfig',
+    'xnbtd.plannings.apps.PlanningsConfig',
 ]
 
 ROOT_URLCONF = 'xnbtd.urls'
 WSGI_APPLICATION = 'xnbtd.wsgi.application'
 
 
 MIDDLEWARE = [
```

### Comparing `xnbtd-0.0.2/xnbtd/settings/local.py` & `xnbtd-0.0.3/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.2/PKG-INFO` & `xnbtd-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.2
+Version: 0.0.3
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

