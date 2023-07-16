# Comparing `tmp/django-extended-history-1.0.0.tar.gz` & `tmp/django-extended-history-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-extended-history-1.0.0.tar", last modified: Sat Apr  1 10:27:19 2023, max compression
+gzip compressed data, was "django-extended-history-1.1.0.tar", last modified: Sun Jul 16 21:41:24 2023, max compression
```

## Comparing `django-extended-history-1.0.0.tar` & `django-extended-history-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.934840 django-extended-history-1.0.0/
--rw-rw-rw-   0        0        0     1535 2023-03-31 15:50:16.000000 django-extended-history-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       76 2023-03-31 20:12:26.000000 django-extended-history-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2296 2023-04-01 10:27:19.934840 django-extended-history-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1575 2023-04-01 10:21:53.000000 django-extended-history-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.910903 django-extended-history-1.0.0/django_extended_history/
--rw-rw-rw-   0        0        0        0 2023-02-06 09:12:18.000000 django-extended-history-1.0.0/django_extended_history/__init__.py
--rw-rw-rw-   0        0        0     9187 2023-03-31 15:55:57.000000 django-extended-history-1.0.0/django_extended_history/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.928856 django-extended-history-1.0.0/django_extended_history/templates/
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.881989 django-extended-history-1.0.0/django_extended_history/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.932844 django-extended-history-1.0.0/django_extended_history/templates/admin/admin/
--rw-rw-rw-   0        0        0       84 2023-01-18 09:10:47.000000 django-extended-history-1.0.0/django_extended_history/templates/admin/admin/change_form.html
--rw-rw-rw-   0        0        0     1789 2023-03-17 16:58:22.000000 django-extended-history-1.0.0/django_extended_history/templates/object_history.html
--rw-rw-rw-   0        0        0       63 2023-02-06 09:12:18.000000 django-extended-history-1.0.0/django_extended_history/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-01 10:27:19.926860 django-extended-history-1.0.0/django_extended_history.egg-info/
--rw-rw-rw-   0        0        0     2296 2023-04-01 10:27:19.000000 django-extended-history-1.0.0/django_extended_history.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-04-01 10:27:19.000000 django-extended-history-1.0.0/django_extended_history.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 10:27:19.000000 django-extended-history-1.0.0/django_extended_history.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-01 10:27:19.000000 django-extended-history-1.0.0/django_extended_history.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-01 10:27:19.000000 django-extended-history-1.0.0/django_extended_history.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-31 16:36:21.000000 django-extended-history-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      939 2023-04-01 10:27:19.936835 django-extended-history-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.353337 django-extended-history-1.1.0/
+-rw-rw-rw-   0        0        0     1535 2023-03-31 15:50:16.000000 django-extended-history-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       76 2023-03-31 20:12:26.000000 django-extended-history-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2298 2023-07-16 21:41:24.354336 django-extended-history-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1577 2023-07-16 21:12:03.000000 django-extended-history-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.303469 django-extended-history-1.1.0/django_extended_history/
+-rw-rw-rw-   0        0        0        0 2023-02-06 09:12:18.000000 django-extended-history-1.1.0/django_extended_history/__init__.py
+-rw-rw-rw-   0        0        0     9365 2023-04-06 12:12:02.000000 django-extended-history-1.1.0/django_extended_history/admin.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.335383 django-extended-history-1.1.0/django_extended_history/templates/
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.236647 django-extended-history-1.1.0/django_extended_history/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.347353 django-extended-history-1.1.0/django_extended_history/templates/admin/admin/
+-rw-rw-rw-   0        0        0       84 2023-01-18 09:10:47.000000 django-extended-history-1.1.0/django_extended_history/templates/admin/admin/change_form.html
+-rw-rw-rw-   0        0        0     1789 2023-03-17 16:58:22.000000 django-extended-history-1.1.0/django_extended_history/templates/object_history.html
+-rw-rw-rw-   0        0        0       63 2023-02-06 09:12:18.000000 django-extended-history-1.1.0/django_extended_history/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:41:24.330398 django-extended-history-1.1.0/django_extended_history.egg-info/
+-rw-rw-rw-   0        0        0     2298 2023-07-16 21:41:24.000000 django-extended-history-1.1.0/django_extended_history.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-07-16 21:41:24.000000 django-extended-history-1.1.0/django_extended_history.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:41:24.000000 django-extended-history-1.1.0/django_extended_history.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-16 21:41:24.000000 django-extended-history-1.1.0/django_extended_history.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 21:41:24.000000 django-extended-history-1.1.0/django_extended_history.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-03-31 16:36:21.000000 django-extended-history-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      941 2023-07-16 21:41:24.363309 django-extended-history-1.1.0/setup.cfg
```

### Comparing `django-extended-history-1.0.0/LICENSE` & `django-extended-history-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-extended-history-1.0.0/PKG-INFO` & `django-extended-history-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extended-history
-Version: 1.0.0
+Version: 1.1.0
 Summary: Drop-in replacement for default Django history
 Home-page: https://github.com/HealthyFridge/django-extended-history
 Author: Rob Aben
 Author-email: rob@healthyfridge.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/HealthyFridge/django-extended-history/issues
 Project-URL: repository, https://github.com/HealthyFridge/django-extended-history
@@ -21,15 +21,15 @@
 
 **django-extended-history** is (IMHO) the simplest way to record all changes made in admin-screens.
 
 =============
 Requirements
 =============
 
-- Django 4.x
+- Django >=4.1
 
 =============
 Features
 =============
 
 -  Drop-in extension for Django history. No changes in any model, hence no migrations.
 -  Records all changes in JSON format, extending what Django stores by default.
```

### Comparing `django-extended-history-1.0.0/README.rst` & `django-extended-history-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 **django-extended-history** is (IMHO) the simplest way to record all changes made in admin-screens.
 
 =============
 Requirements
 =============
 
-- Django 4.x
+- Django >=4.1
 
 =============
 Features
 =============
 
 -  Drop-in extension for Django history. No changes in any model, hence no migrations.
 -  Records all changes in JSON format, extending what Django stores by default.
```

### Comparing `django-extended-history-1.0.0/django_extended_history/admin.py` & `django-extended-history-1.1.0/django_extended_history/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import json
 
 from django.contrib import admin
 from django.contrib.admin.models import LogEntry
 from django.contrib.admin.utils import construct_change_message
 from django.contrib.auth.models import Permission
 from django.db import models
@@ -110,22 +111,23 @@
                     deleted_form_list = []
                     for form in formset.initial_forms:
 
                         deleted_fields_list = []
                         if form.instance != deleted_object:
                             continue
 
-                        for field in form.initial:
-                            if form.initial[field] is not None and hasattr(form.fields[field], 'queryset'):
-                                old_value = str(form.fields[field].queryset.filter(pk=form.initial[field]).first())
-                            else:
-                                old_value = str(form.initial[field])
+                        for field in form.instance._meta.fields:
+                            if not isinstance(field, (models.AutoField, models.BigAutoField, models.SmallAutoField)):
+                                if isinstance(field, models.BinaryField):
+                                    old_value = base64.b64encode(getattr(deleted_object, field.name)).decode('utf-8') 
+                                else:
+                                    old_value = str(getattr(deleted_object, field.name))
 
-                            deleted_field_content = {"old": old_value}
-                            deleted_fields_list.append({field: deleted_field_content})
+                                deleted_field_content = {"old": old_value}
+                                deleted_fields_list.append({field.name: deleted_field_content})
 
                         deleted_form_list.append({str(deleted_object._meta.model_name): str(deleted_object), "fields": deleted_fields_list})
 
                     deleted_form_set.append(deleted_form_list)
 
                     change_message.append({"deleted related": deleted_form_set})
 
@@ -143,15 +145,15 @@
 
     def get_queryset(self, request):
         queryset = super(LogEntryAdmin, self).get_queryset(request)
         if request.user.is_superuser == False:  # type: ignore
             # List only those logentries to which to user has permission
             queryset = queryset.filter(Q(content_type__in=Permission.objects.filter(group__user=request.user).values('content_type')) |
                                        Q(content_type__in=Permission.objects.filter(user=request.user).values('content_type')))
-        return queryset.prefetch_related('content_type')
+        return queryset.prefetch_related('content_type').defer('change_message')
 
     @admin.display(description=_('change message'))
     def get_change_message(self, request):
         cm: str = request.change_message
         if cm and cm[0] == "[":
             try:
                 cm = json2html.convert(json=cm)  # type: ignore
```

### Comparing `django-extended-history-1.0.0/django_extended_history/templates/object_history.html` & `django-extended-history-1.1.0/django_extended_history/templates/object_history.html`

 * *Files identical despite different names*

### Comparing `django-extended-history-1.0.0/django_extended_history.egg-info/PKG-INFO` & `django-extended-history-1.1.0/django_extended_history.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extended-history
-Version: 1.0.0
+Version: 1.1.0
 Summary: Drop-in replacement for default Django history
 Home-page: https://github.com/HealthyFridge/django-extended-history
 Author: Rob Aben
 Author-email: rob@healthyfridge.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/HealthyFridge/django-extended-history/issues
 Project-URL: repository, https://github.com/HealthyFridge/django-extended-history
@@ -21,15 +21,15 @@
 
 **django-extended-history** is (IMHO) the simplest way to record all changes made in admin-screens.
 
 =============
 Requirements
 =============
 
-- Django 4.x
+- Django >=4.1
 
 =============
 Features
 =============
 
 -  Drop-in extension for Django history. No changes in any model, hence no migrations.
 -  Records all changes in JSON format, extending what Django stores by default.
```

### Comparing `django-extended-history-1.0.0/setup.cfg` & `django-extended-history-1.1.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6578 7465 6e64   = django-extend
 00000020: 6564 2d68 6973 746f 7279 0d0a 7665 7273  ed-history..vers
-00000030: 696f 6e20 3d20 312e 302e 300d 0a61 7574  ion = 1.0.0..aut
+00000030: 696f 6e20 3d20 312e 312e 300d 0a61 7574  ion = 1.1.0..aut
 00000040: 686f 7220 3d20 526f 6220 4162 656e 0d0a  hor = Rob Aben..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2072  author_email = r
 00000060: 6f62 4068 6561 6c74 6879 6672 6964 6765  ob@healthyfridge
 00000070: 2e6e 6c0d 0a64 6573 6372 6970 7469 6f6e  .nl..description
 00000080: 203d 2044 726f 702d 696e 2072 6570 6c61   = Drop-in repla
 00000090: 6365 6d65 6e74 2066 6f72 2064 6566 6175  cement for defau
 000000a0: 6c74 2044 6a61 6e67 6f20 6869 7374 6f72  lt Django histor
@@ -44,16 +44,16 @@
 000002b0: 0a70 6163 6b61 6765 7320 3d20 646a 616e  .packages = djan
 000002c0: 676f 5f65 7874 656e 6465 645f 6869 7374  go_extended_hist
 000002d0: 6f72 790d 0a69 6e63 6c75 6465 5f70 6163  ory..include_pac
 000002e0: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
 000002f0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
 00000300: 7320 3d20 3e3d 332e 380d 0a69 6e73 7461  s = >=3.8..insta
 00000310: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000320: 0964 6a61 6e67 6f20 3e3d 2034 0d0a 096a  .django >= 4...j
-00000330: 736f 6e32 6874 6d6c 203e 3d20 312e 332e  son2html >= 1.3.
-00000340: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  0....[options.pa
-00000350: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000360: 6572 6520 3d20 646a 616e 676f 5f65 7874  ere = django_ext
-00000370: 656e 6465 645f 6869 7374 6f72 790d 0a0d  ended_history...
-00000380: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000390: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000003a0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000320: 0964 6a61 6e67 6f20 3e3d 2034 2e31 0d0a  .django >= 4.1..
+00000330: 096a 736f 6e32 6874 6d6c 203e 3d20 312e  .json2html >= 1.
+00000340: 332e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  3.0....[options.
+00000350: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000360: 7768 6572 6520 3d20 646a 616e 676f 5f65  where = django_e
+00000370: 7874 656e 6465 645f 6869 7374 6f72 790d  xtended_history.
+00000380: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000390: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000003a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

