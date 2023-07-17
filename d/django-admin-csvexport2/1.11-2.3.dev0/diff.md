# Comparing `tmp/django-admin-csvexport2-1.11.tar.gz` & `tmp/django-admin-csvexport2-2.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-csvexport2-1.11.tar", last modified: Thu Aug 18 12:32:06 2022, max compression
+gzip compressed data, was "django-admin-csvexport2-2.3.dev0.tar", last modified: Mon Jul 17 16:43:09 2023, max compression
```

## Comparing `django-admin-csvexport2-1.11.tar` & `django-admin-csvexport2-2.3.dev0.tar`

### file list

```diff
@@ -1,27 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.519106 django-admin-csvexport2-1.11/
--rw-rw-rw-   0        0        0     1548 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/LICENCE
--rw-rw-rw-   0        0        0      116 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/MANIFEST.in
--rw-rw-rw-   0        0        0     5451 2022-08-18 12:32:06.518106 django-admin-csvexport2-1.11/PKG-INFO
--rw-rw-rw-   0        0        0     4235 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/README.rst
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.490105 django-admin-csvexport2-1.11/csvexport/
--rw-rw-rw-   0        0        0       62 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/__init__.py
--rw-rw-rw-   0        0        0     8937 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/actions.py
--rw-rw-rw-   0        0        0       98 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/apps.py
--rw-rw-rw-   0        0        0     3019 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/forms.py
--rw-rw-rw-   0        0        0      845 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/settings.py
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.477105 django-admin-csvexport2-1.11/csvexport/static/
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.491104 django-admin-csvexport2-1.11/csvexport/static/csvexport/
--rw-rw-rw-   0        0        0      386 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/static/csvexport/checkbox_select_all.js
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.478105 django-admin-csvexport2-1.11/csvexport/templates/
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.493103 django-admin-csvexport2-1.11/csvexport/templates/csvexport/
--rw-rw-rw-   0        0        0      229 2022-08-17 19:55:21.000000 django-admin-csvexport2-1.11/csvexport/templates/csvexport/checkbox_select_all.html
--rw-rw-rw-   0        0        0     1101 2022-08-17 20:02:32.000000 django-admin-csvexport2-1.11/csvexport/templates/csvexport/csvexport.html
-drwxrwxrwx   0        0        0        0 2022-08-18 12:32:06.517104 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/
--rw-rw-rw-   0        0        0     5451 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-08-18 12:32:06.000000 django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-08-18 12:32:06.519106 django-admin-csvexport2-1.11/setup.cfg
--rw-rw-rw-   0        0        0     1975 2022-08-17 19:59:04.000000 django-admin-csvexport2-1.11/setup.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.841411 django-admin-csvexport2-2.3.dev0/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1521 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/LICENCE
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      112 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/MANIFEST.in
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     5701 2023-07-17 16:43:09.841269 django-admin-csvexport2-2.3.dev0/PKG-INFO
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     4348 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/README.rst
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.836514 django-admin-csvexport2-2.3.dev0/csvexport/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)       66 2023-07-17 16:38:51.000000 django-admin-csvexport2-2.3.dev0/csvexport/__init__.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     7676 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/actions.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)       93 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/apps.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     2929 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/forms.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      829 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/settings.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.833521 django-admin-csvexport2-2.3.dev0/csvexport/static/
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.836688 django-admin-csvexport2-2.3.dev0/csvexport/static/csvexport/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      375 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/static/csvexport/checkbox_select_all.js
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.833651 django-admin-csvexport2-2.3.dev0/csvexport/templates/
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.837133 django-admin-csvexport2-2.3.dev0/csvexport/templates/csvexport/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      223 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/templates/csvexport/checkbox_select_all.html
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1067 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/csvexport/templates/csvexport/csvexport.html
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.838090 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     5701 2023-07-17 16:43:09.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/PKG-INFO
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1083 2023-07-17 16:43:09.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/SOURCES.txt
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        1 2023-07-17 16:43:09.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/dependency_links.txt
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)       34 2023-07-17 16:43:09.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/requires.txt
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)       21 2023-07-17 16:43:09.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/top_level.txt
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        1 2023-07-17 16:35:13.000000 django-admin-csvexport2-2.3.dev0/django_admin_csvexport2.egg-info/zip-safe
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)       38 2023-07-17 16:43:09.841456 django-admin-csvexport2-2.3.dev0/setup.cfg
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     2108 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/setup.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.833855 django-admin-csvexport2-2.3.dev0/tests/
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.839501 django-admin-csvexport2-2.3.dev0/tests/testapp/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/__init__.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1053 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/admin.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      114 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/apps.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.839730 django-admin-csvexport2-2.3.dev0/tests/testapp/management/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/management/__init__.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.839964 django-admin-csvexport2-2.3.dev0/tests/testapp/management/commands/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1933 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/management/commands/testapp.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.840525 django-admin-csvexport2-2.3.dev0/tests/testapp/migrations/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     5895 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     2620 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/migrations/0002_auto_20200831_1950.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     2150 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/models.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     3165 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/settings.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.840770 django-admin-csvexport2-2.3.dev0/tests/testapp/tests/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/tests/__init__.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)    10290 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/tests/test_export.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      758 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/urls.py
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)      391 2023-07-17 16:34:22.000000 django-admin-csvexport2-2.3.dev0/tests/testapp/wsgi.py
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.834463 django-admin-csvexport2-2.3.dev0/venv/
+drwxr-xr-x   0 brunomiglioretto   (501) staff       (20)        0 2023-07-17 16:43:09.840951 django-admin-csvexport2-2.3.dev0/venv/bin/
+-rw-r--r--   0 brunomiglioretto   (501) staff       (20)     1175 2023-07-17 16:34:59.000000 django-admin-csvexport2-2.3.dev0/venv/bin/activate_this.py
```

### Comparing `django-admin-csvexport2-1.11/LICENCE` & `django-admin-csvexport2-2.3.dev0/LICENCE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Copyright (c) 2020, Thomas Leichtfuß.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-    1. Redistributions of source code must retain the above copyright notice,
-       this list of conditions and the following disclaimer.
-
-    2. Redistributions in binary form must reproduce the above copyright
-       notice, this list of conditions and the following disclaimer in the
-       documentation and/or other materials provided with the distribution.
-
-    3. Neither the name of the author nor the names of contributors
-       may be used to endorse or promote products derived from this software
-       without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2020, Thomas Leichtfuß.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice,
+       this list of conditions and the following disclaimer.
+
+    2. Redistributions in binary form must reproduce the above copyright
+       notice, this list of conditions and the following disclaimer in the
+       documentation and/or other materials provided with the distribution.
+
+    3. Neither the name of the author nor the names of contributors
+       may be used to endorse or promote products derived from this software
+       without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django-admin-csvexport2-1.11/PKG-INFO` & `django-admin-csvexport2-2.3.dev0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,155 +1,135 @@
-Metadata-Version: 2.1
-Name: django-admin-csvexport2
-Version: 1.11
-Summary: Django-admin-action to export items as csv-formatted data.
-Home-page: https://github.com/brunomiglioretto/django-admin-csvexport
-Author: Bruno Miglioretto
-Author-email: brunomiglioretto@gmail.com
-License: BSD License
-Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-License-File: LICENCE
-
-=================================
-Welcome to django-admin-csvexport
-=================================
-
-.. image:: https://app.travis-ci.com/thomst/django-admin-csvexport.svg?branch=master
-   :target: https://app.travis-ci.com/github/thomst/django-admin-csvexport
-
-.. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
-   :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
-
-.. image:: https://img.shields.io/badge/python-3.4%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :target: https://img.shields.io/badge/python-3.4%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :alt: python: 3.4, 3.5, 3.6, 3.7, 3.8, 3.9
-
-.. image:: https://img.shields.io/badge/django-1.11%20%7C%202.0%20%7C%202.1%20%7C%202.2%20%7C%203.0%20%7C%203.1-orange
-   :target: https://img.shields.io/badge/django-1.11%20%7C%202.0%20%7C%202.1%20%7C%202.2%20%7C%203.0%20%7C%203.1-orange
-   :alt: django: 1.11, 2.0, 2.1, 2.2, 3.0, 3.1
-
-
-Description
-===========
-Django-admin-csvexport is a django-admin-action, that allows you to export the
-items of your django-admin changelist as csv-formatted data.
-
-
-Features
-========
-* selectable model-fields
-* related models included
-* customizable csv-format
-* view or download csv-data
-
-
-Installation
-============
-Install from pypi.org::
-
-    pip install django-admin-csvexport
-
-Add csvexport to your installed apps::
-
-    INSTALLED_APPS = [
-        'csvexport',
-        ...
-    ]
-
-Add csvexport to the actions of your modeladmin::
-
-    from csvexport.actions import csvexport
-
-    class MyModelAdmin(admin.ModelAdmin):
-        ...
-        actions = [csvexport]
-
-
-Configuration
-=============
-The following settings determine the depth of the model references and the
-value to display for empty fields::
-
-    CSV_EXPORT_REFERENCE_DEPTH = 3
-    CSV_EXPORT_EMPTY_VALUE = ''
-
-The following settings define the csv-format to be used. The default values meet
-the unix standard csv-format::
-
-    CSV_EXPORT_DELIMITER = ','
-    CSV_EXPORT_ESCAPECHAR = ''
-    CSV_EXPORT_QUOTECHAR = '"'
-    CSV_EXPORT_DOUBLEQUOTE = True
-    CSV_EXPORT_LINETERMINATOR = r'\n'
-    CSV_EXPORT_QUOTING = 'QUOTE_ALL'
-
-For the newline escape sequence use a raw-string.
-
-For :code:`CSV_EXPORT_QUOTING` use the name of one of these csv_ module
-constants:
-
-* QUOTE_ALL_
-* QUOTE_MINIMAL_
-* QUOTE_NONNUMERIC_
-* QUOTE_NONE_
-
-.. _csv: https://docs.python.org/3/library/csv.html
-.. _QUOTE_ALL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_MINIMAL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_NONNUMERIC: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_NONE: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-
-The csv-format can also be adjusted by the formular rendered by the csvexport
-admin-action. If there is no need to adjust the csv-format on each export use::
-
-    CSV_EXPORT_FORMAT_FORM = False
-
-The formular can also be extended by a checkbox which allows to filter the
-resulting csv rows to be unique. Therefore use::
-
-    CSV_EXPORT_UNIQUE_FORM = True
-
-With the following additional parameters for your ModelAdmin you could limit the
-fields offered by the export form and choose them to be preselected::
-
-    class MyModelAdmin(admin.ModelAdmin):
-        csvexport_export_fields = [
-            'field_a',
-            'field_b,
-            'relational_field.field_a_on_related_model',
-            ...
-        ]
-        csvexport_selected_fields = [
-            'field_a',
-            'field_b,
-            'relational_field.field_a_on_related_model',
-            ...
-        ]
-
-Fields of related models could be referenced by using a dot between the
-relational fields and the fields to be exported:
-:code:`'relation_a.relation_b.any_field'`. Not defining
-:code:`csvexport_export_fields` means all possible fields will be regarded.
-
-
-Usage
-=====
-Just use it as any django-admin-action: Select your items, choose csvexport
-from the admin-action-bar and go. You will be led to a formular that allows
-you to view or download your items as csv-data.
+=================================
+Welcome to django-admin-csvexport
+=================================
+
+.. image:: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml
+   :alt: Run tests for django-admin-csvexport
+
+.. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
+   :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
+   :alt: coveralls badge
+
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.7, 3.8, 3.9,3.9,3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
+
+
+Description
+===========
+Django-admin-csvexport is a django-admin-action, that allows you to export the
+items of your django-admin changelist as csv-formatted data.
+
+
+Features
+========
+* selectable model-fields
+* related models included
+* customizable csv-format
+* view or download csv-data
+
+
+Installation
+============
+Install from pypi.org::
+
+    pip install django-admin-csvexport
+
+Add csvexport to your installed apps::
+
+    INSTALLED_APPS = [
+        'csvexport',
+        ...
+    ]
+
+Add csvexport to the actions of your modeladmin::
+
+    from csvexport.actions import csvexport
+
+    class MyModelAdmin(admin.ModelAdmin):
+        ...
+        actions = [csvexport]
+
+
+Configuration
+=============
+The following settings determine the depth of the model references and the
+value to display for empty fields::
+
+    CSV_EXPORT_REFERENCE_DEPTH = 3
+    CSV_EXPORT_EMPTY_VALUE = ''
+
+The following settings define the csv-format to be used. The default values meet
+the unix standard csv-format::
+
+    CSV_EXPORT_DELIMITER = ','
+    CSV_EXPORT_ESCAPECHAR = ''
+    CSV_EXPORT_QUOTECHAR = '"'
+    CSV_EXPORT_DOUBLEQUOTE = True
+    CSV_EXPORT_LINETERMINATOR = r'\n'
+    CSV_EXPORT_QUOTING = 'QUOTE_ALL'
+
+For the newline escape sequence use a raw-string.
+
+For :code:`CSV_EXPORT_QUOTING` use the name of one of these csv_ module
+constants:
+
+* QUOTE_ALL_
+* QUOTE_MINIMAL_
+* QUOTE_NONNUMERIC_
+* QUOTE_NONE_
+
+.. _csv: https://docs.python.org/3/library/csv.html
+.. _QUOTE_ALL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_MINIMAL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_NONNUMERIC: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_NONE: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+
+The csv-format can also be adjusted by the formular rendered by the csvexport
+admin-action. If there is no need to adjust the csv-format on each export use::
+
+    CSV_EXPORT_FORMAT_FORM = False
+
+The formular can also be extended by a checkbox which allows to filter the
+resulting csv rows to be unique. Therefore use::
+
+    CSV_EXPORT_UNIQUE_FORM = True
+
+With the following additional parameters for your ModelAdmin you could limit the
+fields offered by the export form and choose them to be preselected::
+
+    class MyModelAdmin(admin.ModelAdmin):
+        csvexport_export_fields = [
+            'field_a',
+            'field_b,
+            'relational_field.field_a_on_related_model',
+            ...
+        ]
+        csvexport_selected_fields = [
+            'field_a',
+            'field_b,
+            'relational_field.field_a_on_related_model',
+            ...
+        ]
+
+Fields of related models could be referenced by using a dot between the
+relational fields and the fields to be exported:
+:code:`'relation_a.relation_b.any_field'`. Not defining
+:code:`csvexport_export_fields` means all possible fields will be regarded.
+
+The CSV_EXPORT_REFERENCE_DEPTH value could also be adjusted in modeladmin specific
+manner::
+
+    class MyModelAdmin(admin.ModelAdmin):
+        csvexport_reference_depth = 2
+
+
+Usage
+=====
+Just use it as any django-admin-action: Select your items, choose csvexport
+from the admin-action-bar and go. You will be led to a formular that allows
+you to view or download your items as csv-data.
```

### Comparing `django-admin-csvexport2-1.11/csvexport/actions.py` & `django-admin-csvexport2-2.3.dev0/csvexport/actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,241 +1,206 @@
-# -*- coding: utf-8 -*-
-import csv
-import codecs
-from anytree import AnyNode
-from anytree import LevelOrderGroupIter
-from anytree import LevelOrderIter
-from django.core.exceptions import ObjectDoesNotExist
-from django.utils.translation import gettext_lazy as _
-from django.contrib import messages
-from django.http import HttpResponse
-from django.shortcuts import render
-from django.db.models.manager import BaseManager
-from django import forms
-from django.db import models
-
-from csvexport import settings
-from .forms import CSVFormatForm
-from .forms import UniqueForm
-from .forms import CSVFieldsForm
-from .forms import CheckboxSelectAll
-
-
-RELATION_TYPES = (
-    models.OneToOneField,
-    models.OneToOneRel,
-    models.ForeignKey,
-    models.ManyToOneRel,
-    models.ManyToManyField,
-    models.ManyToManyRel
-)
-SUPPORTED_RELATION_TYPES = (
-    models.ForeignKey,
-    models.OneToOneField,
-    models.OneToOneRel
-)
-
-
-class ModelNode(AnyNode):
-    """
-    A node per model to map their relations and access their fields.
-    """
-    export_fields = list()
-    selected_fields = list()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.choices = list()
-        self.initial = list()
-        self.build_choices()
-
-    @classmethod
-    def setup(cls, modeladmin):
-        cls.export_fields = getattr(modeladmin, 'csvexport_export_fields', list())
-        cls.selected_fields = getattr(modeladmin, 'csvexport_selected_fields', list())
-
-    @property
-    def key(self):
-        return '_'.join(n.model.__name__ for n in self.path)
-
-    def build_choices(self):
-        """
-        Get choice-tuples for a given model.
-        """
-        path = '.'.join(n.field.name for n in self.path[1:])
-        fields = self.get_fields()
-        for field in fields:
-            choice = '{}.{}'.format(path, field.name).lstrip('.')
-            if not self.export_fields or choice in self.export_fields:
-                self.choices.append((choice, field.name))
-                if self.selected_fields and choice in self.selected_fields:
-                    self.initial.append(choice)
-
-    def get_fields(self):
-        """
-        Get all model fields that are not relations.
-        """
-        fields = self.model._meta.get_fields()
-        check_type = lambda f: all(not issubclass(type(f), r) for r in RELATION_TYPES)
-        fields = [f for f in fields if check_type(f)]
-        return fields
-
-    def get_rel_fields(self):
-        """
-        Get model fields that are subclasses of ForeignKey.
-        """
-        fields = self.model._meta.get_fields()
-        check_type = lambda f: any(issubclass(type(f), r) for r in SUPPORTED_RELATION_TYPES)
-        fields = [f for f in fields if check_type(f)]
-        return fields
-
-    def get_form_field(self):
-        if self.choices:
-            label = ' -> '.join(str(n.model._meta.verbose_name) for n in self.path)
-            help_text = _('Which fields do you want to export?')
-            return forms.MultipleChoiceField(
-                label=label,
-                help_text=help_text,
-                widget=CheckboxSelectAll,
-                choices=self.choices,
-                initial=self.initial,
-                required=False)
-
-
-class IterNodesWithChoices(LevelOrderIter):
-    """
-    Only iter over Nodes with choices.
-    """
-    def __next__(self):
-        node = super().__next__()
-        if node.choices:
-            return node
-        else:
-            return next(self)
-
-
-class CSVData:
-    """
-    Simple replacement for the filelike-object passed to the csv-writer.
-    """
-    def __init__(self, unique=False):
-        self.data = list()
-        self.unique = unique
-
-    def write(self, data):
-        if not self.unique or data not in self.data:
-            self.data.append(data)
-
-    def __str__(self):
-        return ''.join(self.data)
-
-
-def csvexport(modeladmin, request, queryset):
-    """
-    Admin-action to export items as csv-formatted data.
-    """
-    # initiate the format-form
-    if 'csvexport' in request.POST and settings.CSV_EXPORT_FORMAT_FORM:
-        format_form = CSVFormatForm(request.POST)
-    else:
-        format_form = CSVFormatForm(dict(
-            delimiter=settings.CSV_EXPORT_DELIMITER,
-            escapechar=settings.CSV_EXPORT_ESCAPECHAR,
-            quotechar=settings.CSV_EXPORT_QUOTECHAR,
-            doublequote=settings.CSV_EXPORT_DOUBLEQUOTE,
-            quoting=settings.CSV_EXPORT_QUOTING,
-            lineterminator=settings.CSV_EXPORT_LINETERMINATOR,
-        ))
-
-    # initiate unique-form
-    if 'csvexport' in request.POST and settings.CSV_EXPORT_UNIQUE_FORM:
-        unique_form = UniqueForm(request.POST)
-    else:
-        unique_form = UniqueForm(dict(uniq=False))
-
-    # initiate field-form
-    if 'csvexport' in request.POST:
-        fields_form = CSVFieldsForm(request.POST)
-    else:
-        fields_form = CSVFieldsForm()
-
-    # Build up the node-tree
-    ModelNode.setup(modeladmin)
-    root_node = ModelNode(model=modeladmin.model)
-
-    n = 0
-    while n < settings.CSV_EXPORT_REFERENCE_DEPTH:
-        n += 1
-        for node in tuple(LevelOrderGroupIter(root_node))[-1]:
-            for field in node.get_rel_fields():
-                try:
-                    # Do we have a OneToOneField OneToOneRel cycle?
-                    # Then we just continue.
-                    assert field.remote_field == node.field
-                except (AttributeError, AssertionError):
-                    # Otherwise we build a new Node.
-                    current_node = ModelNode(model=field.related_model, field=field, parent=node)
-                else:
-                    continue
-
-    # Add form-fields to form
-    for node in IterNodesWithChoices(root_node):
-        fields_form.fields[node.key] = node.get_form_field()
-
-    # Write and return csv-data
-    if format_form.is_valid() and fields_form.is_valid() and unique_form.is_valid():
-        # get csv-format
-        csv_format = dict()
-        csv_format['delimiter'] = format_form.cleaned_data['delimiter']
-        csv_format['escapechar'] = format_form.cleaned_data['escapechar']
-        csv_format['quotechar'] = format_form.cleaned_data['quotechar']
-        csv_format['doublequote'] = format_form.cleaned_data['doublequote']
-        csv_format['quoting'] = getattr(csv, format_form.cleaned_data['quoting'])
-        newline = format_form.cleaned_data['lineterminator']
-        csv_format['lineterminator'] = codecs.decode(newline, 'unicode_escape')
-
-        # use select-options as csv-header
-        header = list()
-        for node in IterNodesWithChoices(root_node):
-            header += list(fields_form.cleaned_data[node.key])
-
-        csv_data = CSVData(unique_form.cleaned_data['unique'])
-        header_fields = [f.replace('.', '__') for f in header]
-        related_fields = ['__'.join(f.split('__')[:-1]) for f in header_fields if '__' in f]
-        if related_fields:
-            queryset = queryset.select_related(*related_fields)
-
-        # write csv-header and -data and return csv-data as view or download
-        try:
-            writer = csv.writer(csv_data, **csv_format)
-            writer.writerow(tuple(f for f in header))
-            for item in queryset.values_list(*header_fields):
-                row = tuple(f if f is not None and f != '' else settings.CSV_EXPORT_EMPTY_VALUE for f in item)
-                writer.writerow(row)
-        except (csv.Error, TypeError) as exc:
-            messages.error(request, 'Could not write csv-file: {}'.format(exc))
-        else:
-            if 'csvexport_view' in request.POST:
-                content_type = "text/plain;charset=utf-8"
-                response = HttpResponse(csv_data, content_type=content_type)
-            elif 'csvexport_download' in request.POST:
-                content_type = "text/csv"
-                response = HttpResponse(csv_data, content_type=content_type)
-                filename = modeladmin.model._meta.label_lower + '.csv'
-                content_disposition = 'attachment; filename="{}"'.format(filename)
-                response['Content-Disposition'] = content_disposition
-            return response
-
-    # If forms are invalid or csv-data couldn't be written return to the form
-    format_form = format_form if settings.CSV_EXPORT_FORMAT_FORM else None
-    unique_form = unique_form if settings.CSV_EXPORT_UNIQUE_FORM else None
-
-    context = modeladmin.admin_site.each_context(request)
-    context.update({
-        'objects': queryset.order_by('pk'),
-        'format_form': format_form,
-        'unique_form': unique_form,
-        'fields_form': fields_form,
-        'title': _('CSV-Export')
-        })
-
-    return render(request, 'csvexport/csvexport.html', context)
+# -*- coding: utf-8 -*-
+import csv
+import codecs
+from anytree import LevelOrderIter
+from modeltree import ModelTree
+from django.utils.translation import gettext_lazy as _
+from django.contrib import messages
+from django.http import HttpResponse
+from django.shortcuts import render
+from django import forms
+
+from csvexport import settings
+from .forms import CSVFormatForm
+from .forms import UniqueForm
+from .forms import CSVFieldsForm
+from .forms import CheckboxSelectAll
+
+
+class BaseModelTree(ModelTree):
+    """
+    A node per model to map their relations and access their fields.
+    """
+    export_fields = list()
+    selected_fields = list()
+
+    FOLLOW_ACROSS_APPS = True
+
+    RELATION_TYPES = [
+        'one_to_one',
+        'many_to_one',
+    ]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.choices = list()
+        self.initial = list()
+        self.build_choices()
+
+    @classmethod
+    def setup(cls, modeladmin, request):
+        params = dict(
+            request = request,
+            export_fields=getattr(modeladmin, 'csvexport_export_fields', list()),
+            selected_fields=getattr(modeladmin, 'csvexport_selected_fields', list()),
+            MAX_DEPTH=getattr(modeladmin, 'csvexport_reference_depth', settings.CSV_EXPORT_REFERENCE_DEPTH),
+        )
+        return type('ExportModelTree', (cls,), params)
+
+    @property
+    def key(self):
+        return '_'.join(n.model.__name__ for n in self.path)
+
+    @property
+    def user_has_view_permission(self):
+        perm = f'{self.model._meta.app_label}.view_{self.model._meta.model_name}'
+        return self.request.user.has_perm(perm)
+
+    def build_choices(self):
+        """
+        Get choice-tuples for a given model.
+        """
+        path = '.'.join(n.field.name for n in self.path[1:])
+        fields = [f for f in self.model._meta.get_fields() if not f.is_relation]
+        for field in fields:
+            choice = '{}.{}'.format(path, field.name).lstrip('.')
+            if not self.export_fields or choice in self.export_fields:
+                self.choices.append((choice, field.name))
+                if self.selected_fields and choice in self.selected_fields:
+                    self.initial.append(choice)
+
+    def get_form_field(self):
+        if self.choices:
+            label = ' -> '.join(str(n.model._meta.verbose_name) for n in self.path)
+            help_text = _('Which fields do you want to export?')
+            return forms.MultipleChoiceField(
+                label=label,
+                help_text=help_text,
+                widget=CheckboxSelectAll,
+                choices=self.choices,
+                initial=self.initial,
+                required=False)
+
+
+class IterNodesWithChoicesAndPermission(LevelOrderIter):
+    """
+    Only iter over Nodes with choices and where the user has view permission.
+    """
+    def __next__(self):
+        node = super().__next__()
+        if node.choices and node.user_has_view_permission:
+            return node
+        else:
+            return next(self)
+
+
+class CSVData:
+    """
+    Simple replacement for the filelike-object passed to the csv-writer.
+    """
+    def __init__(self, unique=False):
+        self.data = list()
+        self.unique = unique
+
+    def write(self, data):
+        if not self.unique or data not in self.data:
+            self.data.append(data)
+
+    def __str__(self):
+        return ''.join(self.data)
+
+
+def csvexport(modeladmin, request, queryset):
+    """
+    Admin-action to export items as csv-formatted data.
+    """
+    # initiate the format-form
+    if 'csvexport' in request.POST and settings.CSV_EXPORT_FORMAT_FORM:
+        format_form = CSVFormatForm(request.POST)
+    else:
+        format_form = CSVFormatForm(dict(
+            delimiter=settings.CSV_EXPORT_DELIMITER,
+            escapechar=settings.CSV_EXPORT_ESCAPECHAR,
+            quotechar=settings.CSV_EXPORT_QUOTECHAR,
+            doublequote=settings.CSV_EXPORT_DOUBLEQUOTE,
+            quoting=settings.CSV_EXPORT_QUOTING,
+            lineterminator=settings.CSV_EXPORT_LINETERMINATOR,
+        ))
+
+    # initiate unique-form
+    if 'csvexport' in request.POST and settings.CSV_EXPORT_UNIQUE_FORM:
+        unique_form = UniqueForm(request.POST)
+    else:
+        unique_form = UniqueForm(dict(uniq=False))
+
+    # initiate field-form
+    if 'csvexport' in request.POST:
+        fields_form = CSVFieldsForm(request.POST)
+    else:
+        fields_form = CSVFieldsForm()
+
+    # Build up the node-tree
+    tree_class = BaseModelTree.setup(modeladmin, request)
+    root_node = tree_class(modeladmin.model)
+
+    # Add form-fields to form
+    for node in IterNodesWithChoicesAndPermission(root_node):
+        fields_form.fields[node.key] = node.get_form_field()
+
+    # Write and return csv-data
+    if format_form.is_valid() and fields_form.is_valid() and unique_form.is_valid():
+        # get csv-format
+        csv_format = dict()
+        csv_format['delimiter'] = format_form.cleaned_data['delimiter']
+        csv_format['escapechar'] = format_form.cleaned_data['escapechar']
+        csv_format['quotechar'] = format_form.cleaned_data['quotechar']
+        csv_format['doublequote'] = format_form.cleaned_data['doublequote']
+        csv_format['quoting'] = getattr(csv, format_form.cleaned_data['quoting'])
+        newline = format_form.cleaned_data['lineterminator']
+        csv_format['lineterminator'] = codecs.decode(newline, 'unicode_escape')
+
+        # use select-options as csv-header
+        header = list()
+        for node in IterNodesWithChoicesAndPermission(root_node):
+            header += list(fields_form.cleaned_data[node.key])
+
+        csv_data = CSVData(unique_form.cleaned_data['unique'])
+        header_fields = [f.replace('.', '__') for f in header]
+        related_fields = ['__'.join(f.split('__')[:-1]) for f in header_fields if '__' in f]
+        if related_fields:
+            queryset = queryset.select_related(*related_fields)
+
+        # write csv-header and -data and return csv-data as view or download
+        try:
+            writer = csv.writer(csv_data, **csv_format)
+            writer.writerow(tuple(f for f in header))
+            for item in queryset.values_list(*header_fields):
+                row = tuple(f if f is not None and f != '' else settings.CSV_EXPORT_EMPTY_VALUE for f in item)
+                writer.writerow(row)
+        except (csv.Error, TypeError) as exc:
+            messages.error(request, 'Could not write csv-file: {}'.format(exc))
+        else:
+            if 'csvexport_view' in request.POST:
+                content_type = "text/plain;charset=utf-8"
+                response = HttpResponse(csv_data, content_type=content_type)
+            elif 'csvexport_download' in request.POST:
+                content_type = "text/csv"
+                response = HttpResponse(csv_data, content_type=content_type)
+                filename = modeladmin.model._meta.label_lower + '.csv'
+                content_disposition = 'attachment; filename="{}"'.format(filename)
+                response['Content-Disposition'] = content_disposition
+            return response
+
+    # If forms are invalid or csv-data couldn't be written return to the form
+    format_form = format_form if settings.CSV_EXPORT_FORMAT_FORM else None
+    unique_form = unique_form if settings.CSV_EXPORT_UNIQUE_FORM else None
+
+    context = modeladmin.admin_site.each_context(request)
+    context.update({
+        'objects': queryset.order_by('pk'),
+        'format_form': format_form,
+        'unique_form': unique_form,
+        'fields_form': fields_form,
+        'title': _('CSV-Export')
+        })
+
+    return render(request, 'csvexport/csvexport.html', context)
```

### Comparing `django-admin-csvexport2-1.11/csvexport/settings.py` & `django-admin-csvexport2-2.3.dev0/csvexport/settings.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from django.conf import settings
-
-
-
-# Set the unix standard csv-format as default
-CSV_EXPORT_DELIMITER = getattr(settings, 'CSV_EXPORT_DELIMITER', ',')
-CSV_EXPORT_ESCAPECHAR = getattr(settings, 'CSV_EXPORT_ESCAPECHAR', '')
-CSV_EXPORT_QUOTECHAR = getattr(settings, 'CSV_EXPORT_QUOTECHAR', '"')
-CSV_EXPORT_DOUBLEQUOTE = getattr(settings, 'CSV_EXPORT_DOUBLEQUOTE', True)
-CSV_EXPORT_LINETERMINATOR = getattr(settings, 'CSV_EXPORT_LINETERMINATOR', r'\n')
-CSV_EXPORT_QUOTING = getattr(settings, 'CSV_EXPORT_QUOTING', 'QUOTE_ALL')
-
-CSV_EXPORT_FORMAT_FORM = getattr(settings, 'CSV_EXPORT_FORMAT_FORM', True)
-CSV_EXPORT_UNIQUE_FORM = getattr(settings, 'CSV_EXPORT_UNIQUE_FORM', False)
-CSV_EXPORT_EMPTY_VALUE = getattr(settings, 'CSV_EXPORT_EMPTY_VALUE', '')
-CSV_EXPORT_REFERENCE_DEPTH = getattr(settings, 'CSV_EXPORT_REFERENCE_DEPTH', 3)
+from django.conf import settings
+
+
+
+# Set the unix standard csv-format as default
+CSV_EXPORT_DELIMITER = getattr(settings, 'CSV_EXPORT_DELIMITER', ',')
+CSV_EXPORT_ESCAPECHAR = getattr(settings, 'CSV_EXPORT_ESCAPECHAR', '')
+CSV_EXPORT_QUOTECHAR = getattr(settings, 'CSV_EXPORT_QUOTECHAR', '"')
+CSV_EXPORT_DOUBLEQUOTE = getattr(settings, 'CSV_EXPORT_DOUBLEQUOTE', True)
+CSV_EXPORT_LINETERMINATOR = getattr(settings, 'CSV_EXPORT_LINETERMINATOR', r'\n')
+CSV_EXPORT_QUOTING = getattr(settings, 'CSV_EXPORT_QUOTING', 'QUOTE_ALL')
+
+CSV_EXPORT_FORMAT_FORM = getattr(settings, 'CSV_EXPORT_FORMAT_FORM', True)
+CSV_EXPORT_UNIQUE_FORM = getattr(settings, 'CSV_EXPORT_UNIQUE_FORM', False)
+CSV_EXPORT_EMPTY_VALUE = getattr(settings, 'CSV_EXPORT_EMPTY_VALUE', '')
+CSV_EXPORT_REFERENCE_DEPTH = getattr(settings, 'CSV_EXPORT_REFERENCE_DEPTH', 3)
```

### Comparing `django-admin-csvexport2-1.11/django_admin_csvexport2.egg-info/PKG-INFO` & `django-admin-csvexport2-2.3.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,168 @@
-Metadata-Version: 2.1
-Name: django-admin-csvexport2
-Version: 1.11
-Summary: Django-admin-action to export items as csv-formatted data.
-Home-page: https://github.com/brunomiglioretto/django-admin-csvexport
-Author: Bruno Miglioretto
-Author-email: brunomiglioretto@gmail.com
-License: BSD License
-Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-License-File: LICENCE
-
-=================================
-Welcome to django-admin-csvexport
-=================================
-
-.. image:: https://app.travis-ci.com/thomst/django-admin-csvexport.svg?branch=master
-   :target: https://app.travis-ci.com/github/thomst/django-admin-csvexport
-
-.. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
-   :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
-
-.. image:: https://img.shields.io/badge/python-3.4%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :target: https://img.shields.io/badge/python-3.4%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :alt: python: 3.4, 3.5, 3.6, 3.7, 3.8, 3.9
-
-.. image:: https://img.shields.io/badge/django-1.11%20%7C%202.0%20%7C%202.1%20%7C%202.2%20%7C%203.0%20%7C%203.1-orange
-   :target: https://img.shields.io/badge/django-1.11%20%7C%202.0%20%7C%202.1%20%7C%202.2%20%7C%203.0%20%7C%203.1-orange
-   :alt: django: 1.11, 2.0, 2.1, 2.2, 3.0, 3.1
-
-
-Description
-===========
-Django-admin-csvexport is a django-admin-action, that allows you to export the
-items of your django-admin changelist as csv-formatted data.
-
-
-Features
-========
-* selectable model-fields
-* related models included
-* customizable csv-format
-* view or download csv-data
-
-
-Installation
-============
-Install from pypi.org::
-
-    pip install django-admin-csvexport
-
-Add csvexport to your installed apps::
-
-    INSTALLED_APPS = [
-        'csvexport',
-        ...
-    ]
-
-Add csvexport to the actions of your modeladmin::
-
-    from csvexport.actions import csvexport
-
-    class MyModelAdmin(admin.ModelAdmin):
-        ...
-        actions = [csvexport]
-
-
-Configuration
-=============
-The following settings determine the depth of the model references and the
-value to display for empty fields::
-
-    CSV_EXPORT_REFERENCE_DEPTH = 3
-    CSV_EXPORT_EMPTY_VALUE = ''
-
-The following settings define the csv-format to be used. The default values meet
-the unix standard csv-format::
-
-    CSV_EXPORT_DELIMITER = ','
-    CSV_EXPORT_ESCAPECHAR = ''
-    CSV_EXPORT_QUOTECHAR = '"'
-    CSV_EXPORT_DOUBLEQUOTE = True
-    CSV_EXPORT_LINETERMINATOR = r'\n'
-    CSV_EXPORT_QUOTING = 'QUOTE_ALL'
-
-For the newline escape sequence use a raw-string.
-
-For :code:`CSV_EXPORT_QUOTING` use the name of one of these csv_ module
-constants:
-
-* QUOTE_ALL_
-* QUOTE_MINIMAL_
-* QUOTE_NONNUMERIC_
-* QUOTE_NONE_
-
-.. _csv: https://docs.python.org/3/library/csv.html
-.. _QUOTE_ALL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_MINIMAL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_NONNUMERIC: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-.. _QUOTE_NONE: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
-
-The csv-format can also be adjusted by the formular rendered by the csvexport
-admin-action. If there is no need to adjust the csv-format on each export use::
-
-    CSV_EXPORT_FORMAT_FORM = False
-
-The formular can also be extended by a checkbox which allows to filter the
-resulting csv rows to be unique. Therefore use::
-
-    CSV_EXPORT_UNIQUE_FORM = True
-
-With the following additional parameters for your ModelAdmin you could limit the
-fields offered by the export form and choose them to be preselected::
-
-    class MyModelAdmin(admin.ModelAdmin):
-        csvexport_export_fields = [
-            'field_a',
-            'field_b,
-            'relational_field.field_a_on_related_model',
-            ...
-        ]
-        csvexport_selected_fields = [
-            'field_a',
-            'field_b,
-            'relational_field.field_a_on_related_model',
-            ...
-        ]
-
-Fields of related models could be referenced by using a dot between the
-relational fields and the fields to be exported:
-:code:`'relation_a.relation_b.any_field'`. Not defining
-:code:`csvexport_export_fields` means all possible fields will be regarded.
-
-
-Usage
-=====
-Just use it as any django-admin-action: Select your items, choose csvexport
-from the admin-action-bar and go. You will be led to a formular that allows
-you to view or download your items as csv-data.
+Metadata-Version: 2.1
+Name: django-admin-csvexport2
+Version: 2.3.dev0
+Summary: Django-admin-action to export items as csv-formatted data.
+Home-page: https://github.com/brunomiglioretto/django-admin-csvexport
+Author: Bruno Miglioretto
+Author-email: brunomiglioretto@gmail.com
+License: BSD License
+Platform: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENCE
+
+=================================
+Welcome to django-admin-csvexport
+=================================
+
+.. image:: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/thomst/django-admin-csvexport/actions/workflows/ci.yml
+   :alt: Run tests for django-admin-csvexport
+
+.. image:: https://coveralls.io/repos/github/thomst/django-admin-csvexport/badge.svg?branch=master
+   :target: https://coveralls.io/github/thomst/django-admin-csvexport?branch=master
+   :alt: coveralls badge
+
+.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.7, 3.8, 3.9,3.9,3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
+
+
+Description
+===========
+Django-admin-csvexport is a django-admin-action, that allows you to export the
+items of your django-admin changelist as csv-formatted data.
+
+
+Features
+========
+* selectable model-fields
+* related models included
+* customizable csv-format
+* view or download csv-data
+
+
+Installation
+============
+Install from pypi.org::
+
+    pip install django-admin-csvexport
+
+Add csvexport to your installed apps::
+
+    INSTALLED_APPS = [
+        'csvexport',
+        ...
+    ]
+
+Add csvexport to the actions of your modeladmin::
+
+    from csvexport.actions import csvexport
+
+    class MyModelAdmin(admin.ModelAdmin):
+        ...
+        actions = [csvexport]
+
+
+Configuration
+=============
+The following settings determine the depth of the model references and the
+value to display for empty fields::
+
+    CSV_EXPORT_REFERENCE_DEPTH = 3
+    CSV_EXPORT_EMPTY_VALUE = ''
+
+The following settings define the csv-format to be used. The default values meet
+the unix standard csv-format::
+
+    CSV_EXPORT_DELIMITER = ','
+    CSV_EXPORT_ESCAPECHAR = ''
+    CSV_EXPORT_QUOTECHAR = '"'
+    CSV_EXPORT_DOUBLEQUOTE = True
+    CSV_EXPORT_LINETERMINATOR = r'\n'
+    CSV_EXPORT_QUOTING = 'QUOTE_ALL'
+
+For the newline escape sequence use a raw-string.
+
+For :code:`CSV_EXPORT_QUOTING` use the name of one of these csv_ module
+constants:
+
+* QUOTE_ALL_
+* QUOTE_MINIMAL_
+* QUOTE_NONNUMERIC_
+* QUOTE_NONE_
+
+.. _csv: https://docs.python.org/3/library/csv.html
+.. _QUOTE_ALL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_MINIMAL: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_NONNUMERIC: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+.. _QUOTE_NONE: https://docs.python.org/3/library/csv.html#csv.QUOTE_ALL
+
+The csv-format can also be adjusted by the formular rendered by the csvexport
+admin-action. If there is no need to adjust the csv-format on each export use::
+
+    CSV_EXPORT_FORMAT_FORM = False
+
+The formular can also be extended by a checkbox which allows to filter the
+resulting csv rows to be unique. Therefore use::
+
+    CSV_EXPORT_UNIQUE_FORM = True
+
+With the following additional parameters for your ModelAdmin you could limit the
+fields offered by the export form and choose them to be preselected::
+
+    class MyModelAdmin(admin.ModelAdmin):
+        csvexport_export_fields = [
+            'field_a',
+            'field_b,
+            'relational_field.field_a_on_related_model',
+            ...
+        ]
+        csvexport_selected_fields = [
+            'field_a',
+            'field_b,
+            'relational_field.field_a_on_related_model',
+            ...
+        ]
+
+Fields of related models could be referenced by using a dot between the
+relational fields and the fields to be exported:
+:code:`'relation_a.relation_b.any_field'`. Not defining
+:code:`csvexport_export_fields` means all possible fields will be regarded.
+
+The CSV_EXPORT_REFERENCE_DEPTH value could also be adjusted in modeladmin specific
+manner::
+
+    class MyModelAdmin(admin.ModelAdmin):
+        csvexport_reference_depth = 2
+
+
+Usage
+=====
+Just use it as any django-admin-action: Select your items, choose csvexport
+from the admin-action-bar and go. You will be led to a formular that allows
+you to view or download your items as csv-data.
```

