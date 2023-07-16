# Comparing `tmp/django-errors-1.5.5.tar.gz` & `tmp/django-errors-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-1.5.5.tar", last modified: Fri Jun 23 19:34:52 2023, max compression
+gzip compressed data, was "django-errors-1.6.6.tar", last modified: Sun Jul 16 22:40:12 2023, max compression
```

## Comparing `django-errors-1.5.5.tar` & `django-errors-1.6.6.tar`

### file list

```diff
@@ -1,89 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 19:34:36.000000 django-errors-1.5.5/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-23 19:34:36.000000 django-errors-1.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 19:34:36.000000 django-errors-1.5.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 19:34:36.000000 django-errors-1.5.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-23 19:34:36.000000 django-errors-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-23 19:34:36.000000 django-errors-1.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-23 19:34:52.665191 django-errors-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-23 19:34:36.000000 django-errors-1.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-23 19:34:36.000000 django-errors-1.5.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 19:34:36.000000 django-errors-1.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 19:34:36.000000 django-errors-1.5.5/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 19:34:36.000000 django-errors-1.5.5/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 19:34:52.665191 django-errors-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 19:34:36.000000 django-errors-1.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.653191 django-errors-1.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/cn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.657191 django-errors-1.5.5/src/django_errors/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-23 19:34:36.000000 django-errors-1.5.5/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.661191 django-errors-1.5.5/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:34:51.000000 django-errors-1.5.5/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 19:34:52.000000 django-errors-1.5.5/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:52.665191 django-errors-1.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:34:36.000000 django-errors-1.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-23 19:34:36.000000 django-errors-1.5.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-23 19:34:36.000000 django-errors-1.5.5/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 19:34:36.000000 django-errors-1.5.5/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-23 19:34:36.000000 django-errors-1.5.5/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 19:34:36.000000 django-errors-1.5.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-16 22:39:59.000000 django-errors-1.6.6/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-16 22:39:59.000000 django-errors-1.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 22:39:59.000000 django-errors-1.6.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 22:39:59.000000 django-errors-1.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-16 22:39:59.000000 django-errors-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 22:39:59.000000 django-errors-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-16 22:40:12.637911 django-errors-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-16 22:39:59.000000 django-errors-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-16 22:39:59.000000 django-errors-1.6.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-16 22:39:59.000000 django-errors-1.6.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-16 22:39:59.000000 django-errors-1.6.6/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-16 22:40:12.637911 django-errors-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-16 22:39:59.000000 django-errors-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-16 22:39:59.000000 django-errors-1.6.6/tox.ini
```

### Comparing `django-errors-1.5.5/.pre-commit-config.yaml` & `django-errors-1.6.6/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-toml
   - id: end-of-file-fixer
   - id: trailing-whitespace
     exclude: .bumpversion.cfg
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.7.0
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/asottile/blacken-docs
-  rev: 1.14.0
+  rev: 1.15.0
   hooks:
   - id: blacken-docs
     additional_dependencies:
     - black>=22.12.0
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
```

### Comparing `django-errors-1.5.5/LICENSE` & `django-errors-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/PKG-INFO` & `django-errors-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.5.5
-Summary: django-errors is a Django application for handling server errors.
+Version: 1.6.6
+Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-errors-1.5.5/README.md` & `django-errors-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/mkdocs.yml` & `django-errors-1.6.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/pyproject.toml` & `django-errors-1.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django_find_project = false
 
 [tool.towncrier]
 package = "django_errors"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "news/"
-version = "1.5.5"
+version = "1.6.6"
 
 # For rendering properly for this project
 issue_format = "`#{issue} <https://github.com/DLRSP/django-errors/issues/{issue}>`_"
 # template = "tools/news/template.rst"
 
 # Grouping of entries, within our changelog
 type = [
```

### Comparing `django-errors-1.5.5/requirements/docs.txt` & `django-errors-1.6.6/requirements/docs.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/docs.txt requirements/docs.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/docs.txt requirements/docs.in
 #
 certifi==2023.5.7 \
     --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
     --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via requests
-charset-normalizer==3.1.0 \
-    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
-    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
-    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
-    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
-    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
-    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
-    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
-    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
-    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
-    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
-    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
-    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
-    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
-    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
-    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
-    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
-    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
-    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
-    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
-    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
-    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
-    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
-    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
-    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
-    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
-    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
-    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
-    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
-    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
-    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
-    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
-    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
-    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
-    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
-    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
-    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
-    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
-    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
-    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
-    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
-    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
-    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
-    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
-    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
-    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
-    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
-    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
-    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
-    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
-    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
-    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
-    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
-    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
-    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
-    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
-    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
-    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
-    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
-    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
-    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
-    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
-    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
-    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
-    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
-    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
-    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
-    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
-    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
-    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
-    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
-    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
-    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
-    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
-    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
-    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
+charset-normalizer==3.2.0 \
+    --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
+    --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
+    --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
+    --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
+    --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
+    --hash=sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252 \
+    --hash=sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad \
+    --hash=sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329 \
+    --hash=sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a \
+    --hash=sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f \
+    --hash=sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6 \
+    --hash=sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4 \
+    --hash=sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a \
+    --hash=sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46 \
+    --hash=sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2 \
+    --hash=sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23 \
+    --hash=sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace \
+    --hash=sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd \
+    --hash=sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982 \
+    --hash=sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10 \
+    --hash=sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2 \
+    --hash=sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea \
+    --hash=sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09 \
+    --hash=sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5 \
+    --hash=sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149 \
+    --hash=sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489 \
+    --hash=sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9 \
+    --hash=sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80 \
+    --hash=sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592 \
+    --hash=sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3 \
+    --hash=sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6 \
+    --hash=sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed \
+    --hash=sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c \
+    --hash=sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200 \
+    --hash=sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a \
+    --hash=sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e \
+    --hash=sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d \
+    --hash=sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6 \
+    --hash=sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623 \
+    --hash=sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669 \
+    --hash=sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3 \
+    --hash=sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa \
+    --hash=sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9 \
+    --hash=sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2 \
+    --hash=sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f \
+    --hash=sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1 \
+    --hash=sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4 \
+    --hash=sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a \
+    --hash=sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8 \
+    --hash=sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3 \
+    --hash=sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029 \
+    --hash=sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f \
+    --hash=sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959 \
+    --hash=sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22 \
+    --hash=sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7 \
+    --hash=sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952 \
+    --hash=sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346 \
+    --hash=sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e \
+    --hash=sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d \
+    --hash=sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299 \
+    --hash=sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd \
+    --hash=sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a \
+    --hash=sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3 \
+    --hash=sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037 \
+    --hash=sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94 \
+    --hash=sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c \
+    --hash=sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858 \
+    --hash=sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a \
+    --hash=sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449 \
+    --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
+    --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
+    --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
+    --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
+    --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
+    --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
     # via requests
-click==8.1.3 \
-    --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
-    --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
+click==8.1.5 \
+    --hash=sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367 \
+    --hash=sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548
     # via mkdocs
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via mkdocs-material
 ghp-import==2.1.0 \
     --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
     --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
     # via mkdocs
 gitdb==4.0.10 \
     --hash=sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a \
     --hash=sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7
     # via gitpython
-gitpython==3.1.31 \
-    --hash=sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573 \
-    --hash=sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d
+gitpython==3.1.32 \
+    --hash=sha256:8d9b8cb1e80b9735e8717c9362079d3ce4c6e5ddeebedd0361b228c3a67a62f6 \
+    --hash=sha256:e3d59b1c2c6ebb9dfa7a184daf3b6dd4914237e7488a1730a6d8f6f5d0b4187f
     # via mkdocs-git-revision-date-plugin
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
-importlib-metadata==6.7.0 \
-    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
-    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via
     #   markdown
     #   mkdocs
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via
@@ -191,33 +191,33 @@
     # via
     #   -r requirements/docs.in
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
 mkdocs-git-revision-date-plugin==0.3.2 \
     --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
     # via -r requirements/docs.in
-mkdocs-material==9.1.16 \
-    --hash=sha256:1021bfea20f00a9423530c8c2ae9be3c78b80f5a527b3f822e6de3d872e5ab79 \
-    --hash=sha256:f9e62558a6b01ffac314423cbc223d970c25fbc78999860226245b64e64d6751
+mkdocs-material==9.1.18 \
+    --hash=sha256:5bcf8fb79ac2f253c0ffe93fa181cba87718c6438f459dc4180ac7418cc9a450 \
+    --hash=sha256:981dd39979723d4cda7cfc77bbbe5e54922d5761a7af23fb8ba9edb52f114b13
     # via -r requirements/docs.in
 mkdocs-material-extensions==1.1.1 \
     --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
     --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
     # via mkdocs-material
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via mkdocs
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via mkdocs-material
-pymdown-extensions==10.0.1 \
-    --hash=sha256:ae66d84013c5d027ce055693e09a4628b67e9dec5bce05727e45b0918e36f274 \
-    --hash=sha256:b44e1093a43b8a975eae17b03c3a77aad4681b3b56fce60ce746dbef1944c8cb
+pymdown-extensions==10.1 \
+    --hash=sha256:508009b211373058debb8247e168de4cbcb91b1bff7b5e961b2c3e864e00b195 \
+    --hash=sha256:ef25dbbae530e8f67575d222b75ff0649b1e841e22c2ae9a20bad9472c2207dc
     # via mkdocs-material
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via ghp-import
 pyyaml==6.0 \
     --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
@@ -399,11 +399,11 @@
     --hash=sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96 \
     --hash=sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d \
     --hash=sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a \
     --hash=sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64 \
     --hash=sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44 \
     --hash=sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33
     # via mkdocs
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
```

### Comparing `django-errors-1.5.5/requirements/py310-django32.txt` & `django-errors-1.6.6/requirements/py310-django32.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,58 +66,58 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==3.2.19 \
-    --hash=sha256:031365bae96814da19c10706218c44dff3b654cc4de20a98bd2d29b9bde469f0 \
-    --hash=sha256:21cc991466245d659ab79cb01204f9515690f8dae00e5eabde307f14d24d4d7d
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 pytz==2023.3 \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
```

### Comparing `django-errors-1.5.5/requirements/py310-django42.txt` & `django-errors-1.6.6/requirements/py311-django42.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,54 +66,42 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.2 \
-    --hash=sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf \
-    --hash=sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5
+django==4.2.3 \
+    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
+    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
-    # via pytest
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-tomli==2.0.1 \
-    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
-    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-    # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
-    # via asgiref
```

### Comparing `django-errors-1.5.5/requirements/py311-django32.txt` & `django-errors-1.6.6/requirements/py311-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,44 +66,44 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==3.2.19 \
-    --hash=sha256:031365bae96814da19c10706218c44dff3b654cc4de20a98bd2d29b9bde469f0 \
-    --hash=sha256:21cc991466245d659ab79cb01204f9515690f8dae00e5eabde307f14d24d4d7d
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
     # via -r requirements/requirements.in
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 pytz==2023.3 \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
```

### Comparing `django-errors-1.5.5/requirements/py311-django42.txt` & `django-errors-1.6.6/requirements/py310-django42.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,42 +66,54 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.2 \
-    --hash=sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf \
-    --hash=sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5
+django==4.2.3 \
+    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
+    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
     # via -r requirements/requirements.in
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
+    # via pytest
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via pytest
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
+    # via asgiref
```

### Comparing `django-errors-1.5.5/requirements/py38-django32.txt` & `django-errors-1.6.6/requirements/py39-django32.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,66 +66,66 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==3.2.19 \
-    --hash=sha256:031365bae96814da19c10706218c44dff3b654cc4de20a98bd2d29b9bde469f0 \
-    --hash=sha256:21cc991466245d659ab79cb01204f9515690f8dae00e5eabde307f14d24d4d7d
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
-importlib-metadata==6.7.0 \
-    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
-    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 pytz==2023.3 \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
```

### Comparing `django-errors-1.5.5/requirements/py38-django42.txt` & `django-errors-1.6.6/requirements/py38-django42.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 backports-zoneinfo==0.2.1 \
     --hash=sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf \
@@ -84,62 +84,62 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.2 \
-    --hash=sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf \
-    --hash=sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5
+django==4.2.3 \
+    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
+    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
-importlib-metadata==6.7.0 \
-    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
-    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
```

### Comparing `django-errors-1.5.5/requirements/py39-django32.txt` & `django-errors-1.6.6/requirements/py38-django32.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,66 +66,66 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==3.2.19 \
-    --hash=sha256:031365bae96814da19c10706218c44dff3b654cc4de20a98bd2d29b9bde469f0 \
-    --hash=sha256:21cc991466245d659ab79cb01204f9515690f8dae00e5eabde307f14d24d4d7d
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
-importlib-metadata==6.7.0 \
-    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
-    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 pytz==2023.3 \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
```

### Comparing `django-errors-1.5.5/requirements/py39-django42.txt` & `django-errors-1.6.6/requirements/py39-django42.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,62 +66,62 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.2 \
-    --hash=sha256:2a6b6fbff5b59dd07bef10bcb019bee2ea97a30b2a656d51346596724324badf \
-    --hash=sha256:672b3fa81e1f853bb58be1b51754108ab4ffa12a77c06db86aa8df9ed0c46fe5
+django==4.2.3 \
+    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
+    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
     # via -r requirements/requirements.in
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
-importlib-metadata==6.7.0 \
-    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
-    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
 pluggy==1.2.0 \
     --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
     --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pytest==7.3.2 \
-    --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
-    --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/requirements.in
     #   pytest-django
     #   pytest-randomly
 pytest-django==4.5.2 \
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
-pytest-randomly==3.12.0 \
-    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
-    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
-typing-extensions==4.6.3 \
-    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
-    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
```

### Comparing `django-errors-1.5.5/runtests.py` & `django-errors-1.6.6/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/setup.cfg` & `django-errors-1.6.6/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 1.5.5
+version = 1.6.6
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
-description = django-errors is a Django application for handling server errors.
+description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE
 keywords = 
 	django
 	errors
```

### Comparing `django-errors-1.5.5/setup.py` & `django-errors-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/middleware/handler.py` & `django-errors-1.6.6/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors/views.py` & `django-errors-1.6.6/src/django_errors/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/src/django_errors.egg-info/PKG-INFO` & `django-errors-1.6.6/src/django_errors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.5.5
-Summary: django-errors is a Django application for handling server errors.
+Version: 1.6.6
+Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-errors-1.5.5/src/django_errors.egg-info/SOURCES.txt` & `django-errors-1.6.6/src/django_errors.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,29 +28,21 @@
 src/django_errors/views.py
 src/django_errors.egg-info/PKG-INFO
 src/django_errors.egg-info/SOURCES.txt
 src/django_errors.egg-info/dependency_links.txt
 src/django_errors.egg-info/not-zip-safe
 src/django_errors.egg-info/requires.txt
 src/django_errors.egg-info/top_level.txt
-src/django_errors/locale/cn/LC_MESSAGES/django.mo
 src/django_errors/locale/cn/LC_MESSAGES/django.po
-src/django_errors/locale/de/LC_MESSAGES/django.mo
 src/django_errors/locale/de/LC_MESSAGES/django.po
-src/django_errors/locale/en/LC_MESSAGES/django.mo
 src/django_errors/locale/en/LC_MESSAGES/django.po
-src/django_errors/locale/es/LC_MESSAGES/django.mo
 src/django_errors/locale/es/LC_MESSAGES/django.po
-src/django_errors/locale/fr/LC_MESSAGES/django.mo
 src/django_errors/locale/fr/LC_MESSAGES/django.po
-src/django_errors/locale/it/LC_MESSAGES/django.mo
 src/django_errors/locale/it/LC_MESSAGES/django.po
-src/django_errors/locale/lt/LC_MESSAGES/django.mo
 src/django_errors/locale/lt/LC_MESSAGES/django.po
-src/django_errors/locale/ru/LC_MESSAGES/django.mo
 src/django_errors/locale/ru/LC_MESSAGES/django.po
 src/django_errors/middleware/__init__.py
 src/django_errors/middleware/handler.py
 src/django_errors/templates/errors/400.html
 src/django_errors/templates/errors/403.html
 src/django_errors/templates/errors/404.html
 src/django_errors/templates/errors/405.html
```

### Comparing `django-errors-1.5.5/tests/test_errors.py` & `django-errors-1.6.6/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/tests/views.py` & `django-errors-1.6.6/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.5.5/tox.ini` & `django-errors-1.6.6/tox.ini`

 * *Files identical despite different names*

