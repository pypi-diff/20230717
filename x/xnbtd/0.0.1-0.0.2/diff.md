# Comparing `tmp/xnbtd-0.0.1.tar.gz` & `tmp/xnbtd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.1.tar", max compression
+gzip compressed data, was "xnbtd-0.0.2.tar", max compression
```

## Comparing `xnbtd-0.0.1.tar` & `xnbtd-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.1/README.md
--rwxr-xr-x   0        0        0     3589 2023-07-17 15:07:07.840282 xnbtd-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.1/xnbtd/__init__.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.1/xnbtd/asgi.py
--rwxr-xr-x   0        0        0      584 2023-07-17 13:08:31.289429 xnbtd-0.0.1/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.1/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5530 2023-07-17 14:22:40.857352 xnbtd-0.0.1/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.1/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 13:08:31.300337 xnbtd-0.0.1/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.1/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0      290 2023-07-17 14:14:11.419116 xnbtd-0.0.1/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.1/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 xnbtd-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.2/README.md
+-rwxr-xr-x   0        0        0     3589 2023-07-17 17:03:02.397891 xnbtd-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.2/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.2/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0      591 2023-07-17 16:48:13.440460 xnbtd-0.0.2/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.2/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5530 2023-07-17 15:12:48.230236 xnbtd-0.0.2/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.2/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.2/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.2/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0      290 2023-07-17 14:14:11.419116 xnbtd-0.0.2/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.2/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2414 1970-01-01 00:00:00.000000 xnbtd-0.0.2/PKG-INFO
```

### Comparing `xnbtd-0.0.1/LICENSE` & `xnbtd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.1/README.md` & `xnbtd-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.1/pyproject.toml` & `xnbtd-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.1"
+version = "0.0.2"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
@@ -114,13 +114,13 @@
 ]
 
 [manageprojects.cookiecutter_context.cookiecutter]
 full_name = "André Théo LAURET"
 github_username = "eldertek"
 author_email = "andrelauret@eclipse-technology.eu"
 package_name = "xnbtd"
-package_version = "0.0.1"
+package_version = "0.0.2"
 package_description = "xnbtd is an open-source digital signage system for high schools."
 package_url = "https://github.com/eldertek/xnbtd"
 issues_url = "https://github.com/eldertek/xnbtd/issues"
 license = "GPL-3.0-or-later"
 _template = "https://github.com/jedie/cookiecutter_templates"
```

### Comparing `xnbtd-0.0.1/xnbtd/publish.py` & `xnbtd-0.0.2/xnbtd/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from poetry_publish.publish import poetry_publish
 from poetry_publish.utils.subprocess_utils import verbose_check_call
 
 import xnbtd
 
 
-PACKAGE_ROOT = Path(xnbtd.__file__).parent.parent
+PACKAGE_ROOT = Path(xnbtd.__file__).parent.parent.parent
 
 
 def publish():
     """
     Publish to PyPi
     Call this via:
         $ poetry run publish
```

### Comparing `xnbtd-0.0.1/xnbtd/settings/base.py` & `xnbtd-0.0.2/xnbtd/settings/base.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.1/xnbtd/settings/local.py` & `xnbtd-0.0.2/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.1/PKG-INFO` & `xnbtd-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.1
+Version: 0.0.2
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

