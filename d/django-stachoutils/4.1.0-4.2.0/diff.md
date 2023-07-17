# Comparing `tmp/django-stachoutils-4.1.0.tar.gz` & `tmp/django-stachoutils-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stachoutils-4.1.0.tar", last modified: Wed Jul 12 12:02:22 2023, max compression
+gzip compressed data, was "django-stachoutils-4.2.0.tar", last modified: Mon Jul 17 07:57:43 2023, max compression
```

## Comparing `django-stachoutils-4.1.0.tar` & `django-stachoutils-4.2.0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1488 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/LICENSE
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      199 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1256 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/README.rst
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3892 2023-07-12 11:35:32.000000 django-stachoutils-4.1.0/django_stachoutils/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      277 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/csv_utf8.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1799 2020-11-30 15:48:58.000000 django-stachoutils-4.1.0/django_stachoutils/decorators.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/forms/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      347 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/forms/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      666 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/forms/fields.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6062 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/forms/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4062 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/forms/nested.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6331 2023-07-12 12:00:59.000000 django-stachoutils-4.1.0/django_stachoutils/forms/widgets.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3674 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/log.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/management/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/management/__init__.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/management/commands/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/management/commands/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10369 2020-06-10 12:58:56.000000 django-stachoutils-4.1.0/django_stachoutils/management/commands/dumpdata_related.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1132 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/management/commands/hotspot_report.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      747 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/management/commands/sync_permissions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      585 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/middlewares.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      185 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3437 2022-04-04 12:34:34.000000 django-stachoutils-4.1.0/django_stachoutils/options.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/profiler.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2254 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/shortcuts.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1836 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/sql.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/css/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      191 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/css/admin_extras.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      331 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/css/commons.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1797 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/css/forms.css
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      517 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/filters.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      206 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-no.gif
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      197 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-yes.gif
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      176 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/icon-no.gif
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      299 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/icon-yes.gif
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      710 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/processing.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6826 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/sprites.png
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1693 2022-02-25 16:39:28.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2193 2022-02-24 14:12:10.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/change_list.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2022 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/editeur.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1964 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/forms.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1589 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2878 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1793 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19113 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11435 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1599 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5199 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1261 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1312 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      118 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green_arrows.gif
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1421 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4729 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      896 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1539 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       87 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter_arrows.gif
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1556 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4916 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1409 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1557 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5069 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1402 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1617 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      107 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple_arrows.gif
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      378 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/storage.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/templates/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/forms/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/forms/widgets/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      319 2023-07-12 11:23:41.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/forms/widgets/textarea_counter_simple.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      505 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/forms/widgets/texte_editeur.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      456 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/pagination.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      523 2022-02-28 14:16:20.000000 django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/templatetags/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/templatetags/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12315 2022-02-28 14:16:20.000000 django-stachoutils-4.1.0/django_stachoutils/templatetags/stachoutils_extras.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils/views/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/views/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      591 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/django_stachoutils/views/actions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15931 2023-07-12 11:35:32.000000 django-stachoutils-4.1.0/django_stachoutils/views/generic.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6614 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        7 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       19 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/django_stachoutils.egg-info/top_level.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2162 2023-07-12 11:35:57.000000 django-stachoutils-4.1.0/setup.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/tests/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      374 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/Makefile
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       34 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/coveragerc
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/tests/forms/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/forms/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1060 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/forms/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5125 2021-12-20 11:10:00.000000 django-stachoutils-4.1.0/tests/forms/test_fields.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4219 2021-12-20 11:10:00.000000 django-stachoutils-4.1.0/tests/forms/test_fields_with_thumbor.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19278 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/forms/test_models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5168 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/forms/test_nested.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9488 2023-07-12 11:35:32.000000 django-stachoutils-4.1.0/tests/forms/test_widgets.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/tests/javascript/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/javascript/demo_texte_editeur.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      674 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/javascript/runtests.html
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/javascript/tests/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7440 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/javascript/tests/test_widgets.js
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/log/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/log/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1325 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/log/test_smtp_handler.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2244 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/log/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/media/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206420 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/media/1st_Saab_9-3_SE.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   384780 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/media/Saab_9-3_Vector_sedan.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   736699 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/media/home_1.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    65868 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/media/jardin.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30317 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/media/terrasse.jpg
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/middlewares/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/middlewares/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1807 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/middlewares/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/models/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/models/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      545 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/models/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      660 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/models/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/options/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/options/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      380 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/options/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4578 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/options/test_logs.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2262 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/options/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:21.000000 django-stachoutils-4.1.0/tests/projects/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/projects/django_project/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/projects/django_project/django_project/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/django_project/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5635 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/django_project/settings.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      124 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/django_project/urls.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1443 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/django_project/wsgi.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2683 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/initial_data.json
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      257 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/manage.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      849 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/admin.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/migrations/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2362 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/migrations/0001_initial.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      450 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/migrations/0002_musicgenre_history.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/migrations/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2667 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/tests.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/projects/django_project/my_app/views.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5225 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/runtests.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2235 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/settings.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/shortcuts/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/shortcuts/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      252 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/shortcuts/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4004 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/shortcuts/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/sql/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/sql/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      384 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/sql/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2527 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/sql/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/storage/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/storage/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      453 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/storage/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1222 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/storage/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/templates/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      332 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templates/generic_list_filters_test.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      815 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templates/generic_list_test.html
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/templatetags/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      566 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5940 2020-06-15 16:55:20.000000 django-stachoutils-4.1.0/tests/templatetags/test_filters.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6017 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/test_pagination_tags.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7707 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/test_tags.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4390 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/tests.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      877 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/templatetags/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       17 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/urls.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/utils/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/utils/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3546 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/utils/tests.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-12 12:02:22.000000 django-stachoutils-4.1.0/tests/views/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      127 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/actions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      136 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/admin.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1546 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/models.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/test_actions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    24400 2020-06-10 10:53:26.000000 django-stachoutils-4.1.0/tests/views/test_generic_view.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1488 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      199 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1256 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3892 2023-07-12 11:35:32.000000 django-stachoutils-4.2.0/django_stachoutils/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      277 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/csv_utf8.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1799 2020-11-30 15:48:58.000000 django-stachoutils-4.2.0/django_stachoutils/decorators.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/forms/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      347 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/forms/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      666 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/forms/fields.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6062 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/forms/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4062 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/forms/nested.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6331 2023-07-12 12:00:59.000000 django-stachoutils-4.2.0/django_stachoutils/forms/widgets.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3674 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/log.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/management/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/management/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/management/commands/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/management/commands/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10369 2020-06-10 12:58:56.000000 django-stachoutils-4.2.0/django_stachoutils/management/commands/dumpdata_related.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1132 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/management/commands/hotspot_report.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      747 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/management/commands/sync_permissions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      585 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/middlewares.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      185 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3437 2022-04-04 12:34:34.000000 django-stachoutils-4.2.0/django_stachoutils/options.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/profiler.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2254 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/shortcuts.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1836 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/sql.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/css/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      191 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/css/admin_extras.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      331 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/css/commons.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1797 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/css/forms.css
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      517 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/filters.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      206 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-no.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      197 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-yes.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      176 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/icon-no.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      299 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/icon-yes.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      710 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/processing.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6826 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/sprites.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1693 2022-02-25 16:39:28.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2193 2022-02-24 14:12:10.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/change_list.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2060 2023-07-17 07:55:39.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/editeur.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1964 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/forms.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1589 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2878 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1793 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19113 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11435 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1599 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5199 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1261 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1312 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      118 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green_arrows.gif
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1421 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4729 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      896 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1539 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       87 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter_arrows.gif
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1556 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4916 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1409 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1557 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5069 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1402 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1617 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      107 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple_arrows.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      378 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/storage.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/templates/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/forms/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/forms/widgets/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      319 2023-07-12 11:23:41.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/forms/widgets/textarea_counter_simple.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      505 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/forms/widgets/texte_editeur.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      456 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/pagination.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      523 2022-02-28 14:16:20.000000 django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/django_stachoutils/templatetags/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/templatetags/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12315 2022-02-28 14:16:20.000000 django-stachoutils-4.2.0/django_stachoutils/templatetags/stachoutils_extras.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/django_stachoutils/views/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/views/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      591 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/django_stachoutils/views/actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15931 2023-07-12 11:35:32.000000 django-stachoutils-4.2.0/django_stachoutils/views/generic.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6614 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        7 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       19 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/django_stachoutils.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2162 2023-07-17 07:55:39.000000 django-stachoutils-4.2.0/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      374 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/Makefile
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       34 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/coveragerc
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/forms/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/forms/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1060 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/forms/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5125 2021-12-20 11:10:00.000000 django-stachoutils-4.2.0/tests/forms/test_fields.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4219 2021-12-20 11:10:00.000000 django-stachoutils-4.2.0/tests/forms/test_fields_with_thumbor.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19278 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/forms/test_models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5168 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/forms/test_nested.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9488 2023-07-12 11:35:32.000000 django-stachoutils-4.2.0/tests/forms/test_widgets.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/javascript/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/javascript/demo_texte_editeur.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      674 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/javascript/runtests.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/javascript/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7440 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/javascript/tests/test_widgets.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/log/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/log/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1325 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/log/test_smtp_handler.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2244 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/log/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/media/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206420 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/media/1st_Saab_9-3_SE.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   384780 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/media/Saab_9-3_Vector_sedan.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   736699 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/media/home_1.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    65868 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/media/jardin.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30317 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/media/terrasse.jpg
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/middlewares/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/middlewares/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1807 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/middlewares/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/models/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/models/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      545 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/models/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      660 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/models/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/options/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/options/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      380 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/options/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4578 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/options/test_logs.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2262 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/options/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:42.000000 django-stachoutils-4.2.0/tests/projects/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/projects/django_project/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/projects/django_project/django_project/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/django_project/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5635 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/django_project/settings.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      124 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/django_project/urls.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1443 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/django_project/wsgi.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2683 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/initial_data.json
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      257 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/manage.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      849 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/admin.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/migrations/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2362 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/migrations/0001_initial.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      450 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/migrations/0002_musicgenre_history.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/migrations/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2667 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/tests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/projects/django_project/my_app/views.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5225 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/runtests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2235 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/settings.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/shortcuts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/shortcuts/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      252 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/shortcuts/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4004 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/shortcuts/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/sql/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/sql/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      384 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/sql/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2527 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/sql/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/storage/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/storage/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      453 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/storage/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1222 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/storage/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/templates/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      332 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templates/generic_list_filters_test.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      815 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templates/generic_list_test.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/templatetags/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      566 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5940 2020-06-15 16:55:20.000000 django-stachoutils-4.2.0/tests/templatetags/test_filters.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6017 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/test_pagination_tags.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7707 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/test_tags.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4390 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/tests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      877 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/templatetags/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       17 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/urls.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/utils/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/utils/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3546 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/utils/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-07-17 07:57:43.000000 django-stachoutils-4.2.0/tests/views/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      127 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      136 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/admin.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1546 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/test_actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    24400 2020-06-10 10:53:26.000000 django-stachoutils-4.2.0/tests/views/test_generic_view.py
```

### Comparing `django-stachoutils-4.1.0/LICENSE` & `django-stachoutils-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/PKG-INFO` & `django-stachoutils-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-stachoutils
-Version: 4.1.0
+Version: 4.2.0
 Summary: Commons for Django
 Home-page: https://github.com/Starou/django-stachoutils
 Author: Stanislas Guerra
 Author-email: stan@slashdev.me
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-stachoutils
 Project-URL: Issue Tracker, https://github.com/Starou/django-stachoutils/issues
```

### Comparing `django-stachoutils-4.1.0/README.rst` & `django-stachoutils-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/__init__.py` & `django-stachoutils-4.2.0/django_stachoutils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/decorators.py` & `django-stachoutils-4.2.0/django_stachoutils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/forms/fields.py` & `django-stachoutils-4.2.0/django_stachoutils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/forms/models.py` & `django-stachoutils-4.2.0/django_stachoutils/forms/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/forms/nested.py` & `django-stachoutils-4.2.0/django_stachoutils/forms/nested.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/forms/widgets.py` & `django-stachoutils-4.2.0/django_stachoutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/log.py` & `django-stachoutils-4.2.0/django_stachoutils/log.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/management/commands/dumpdata_related.py` & `django-stachoutils-4.2.0/django_stachoutils/management/commands/dumpdata_related.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/management/commands/hotspot_report.py` & `django-stachoutils-4.2.0/django_stachoutils/management/commands/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/management/commands/sync_permissions.py` & `django-stachoutils-4.2.0/django_stachoutils/management/commands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/middlewares.py` & `django-stachoutils-4.2.0/django_stachoutils/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/options.py` & `django-stachoutils-4.2.0/django_stachoutils/options.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/profiler.py` & `django-stachoutils-4.2.0/django_stachoutils/profiler.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/shortcuts.py` & `django-stachoutils-4.2.0/django_stachoutils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/sql.py` & `django-stachoutils-4.2.0/django_stachoutils/sql.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/css/forms.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/filters.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/filters.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/processing.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/processing.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/img/sprites.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/img/sprites.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/change_list.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/change_list.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/editeur.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/editeur.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -35,13 +35,14 @@
         });
         $(this).children(".toolbar").children("button.bas").click(function() {
             var selection = textArea.getSelection().text;
             textArea.replaceSelection(selection.toLowerCase(), true);
         });
     });
 
-    $(".titre-box button.bas").click(function() {
-        var input = $(this).parent().find("input:text");
+    /* Button and input in 2 cols. */
+    $("button.bas-de-casse").click(function() {
+        var input = $(this).parent().prev().find('input');
         var selection = input.getSelection().text;
         input.replaceSelection(selection.toLowerCase(), true);
     });
 });
```

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/forms.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/forms.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css` & `django-stachoutils-4.2.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html` & `django-stachoutils-4.2.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/templatetags/stachoutils_extras.py` & `django-stachoutils-4.2.0/django_stachoutils/templatetags/stachoutils_extras.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/views/actions.py` & `django-stachoutils-4.2.0/django_stachoutils/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils/views/generic.py` & `django-stachoutils-4.2.0/django_stachoutils/views/generic.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/django_stachoutils.egg-info/PKG-INFO` & `django-stachoutils-4.2.0/django_stachoutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-stachoutils
-Version: 4.1.0
+Version: 4.2.0
 Summary: Commons for Django
 Home-page: https://github.com/Starou/django-stachoutils
 Author: Stanislas Guerra
 Author-email: stan@slashdev.me
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-stachoutils
 Project-URL: Issue Tracker, https://github.com/Starou/django-stachoutils/issues
```

### Comparing `django-stachoutils-4.1.0/django_stachoutils.egg-info/SOURCES.txt` & `django-stachoutils-4.2.0/django_stachoutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/setup.py` & `django-stachoutils-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name="django-stachoutils",
-    version="4.1.0",
+    version="4.2.0",
     license='BSD Licence',
     author='Stanislas Guerra',
     author_email='stan@slashdev.me',
     description='Commons for Django',
     url='https://github.com/Starou/django-stachoutils',
     project_urls={
         'Source Code': 'https://github.com/Starou/django-stachoutils',
```

### Comparing `django-stachoutils-4.1.0/tests/forms/models.py` & `django-stachoutils-4.2.0/tests/forms/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/forms/test_fields.py` & `django-stachoutils-4.2.0/tests/forms/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/forms/test_fields_with_thumbor.py` & `django-stachoutils-4.2.0/tests/forms/test_fields_with_thumbor.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/forms/test_models.py` & `django-stachoutils-4.2.0/tests/forms/test_models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/forms/test_nested.py` & `django-stachoutils-4.2.0/tests/forms/test_nested.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/forms/test_widgets.py` & `django-stachoutils-4.2.0/tests/forms/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/javascript/demo_texte_editeur.html` & `django-stachoutils-4.2.0/tests/javascript/demo_texte_editeur.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/javascript/runtests.html` & `django-stachoutils-4.2.0/tests/javascript/runtests.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/javascript/tests/test_widgets.js` & `django-stachoutils-4.2.0/tests/javascript/tests/test_widgets.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/log/test_smtp_handler.py` & `django-stachoutils-4.2.0/tests/log/test_smtp_handler.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/log/tests.py` & `django-stachoutils-4.2.0/tests/log/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/media/1st_Saab_9-3_SE.jpg` & `django-stachoutils-4.2.0/tests/media/1st_Saab_9-3_SE.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/media/Saab_9-3_Vector_sedan.jpg` & `django-stachoutils-4.2.0/tests/media/Saab_9-3_Vector_sedan.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/media/home_1.jpg` & `django-stachoutils-4.2.0/tests/media/home_1.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/media/jardin.jpg` & `django-stachoutils-4.2.0/tests/media/jardin.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/media/terrasse.jpg` & `django-stachoutils-4.2.0/tests/media/terrasse.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/middlewares/tests.py` & `django-stachoutils-4.2.0/tests/middlewares/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/models/models.py` & `django-stachoutils-4.2.0/tests/models/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/models/tests.py` & `django-stachoutils-4.2.0/tests/models/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/options/test_logs.py` & `django-stachoutils-4.2.0/tests/options/test_logs.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/options/tests.py` & `django-stachoutils-4.2.0/tests/options/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/django_project/settings.py` & `django-stachoutils-4.2.0/tests/projects/django_project/django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/django_project/wsgi.py` & `django-stachoutils-4.2.0/tests/projects/django_project/django_project/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/initial_data.json` & `django-stachoutils-4.2.0/tests/projects/django_project/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/my_app/admin.py` & `django-stachoutils-4.2.0/tests/projects/django_project/my_app/admin.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/my_app/migrations/0001_initial.py` & `django-stachoutils-4.2.0/tests/projects/django_project/my_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/projects/django_project/my_app/models.py` & `django-stachoutils-4.2.0/tests/projects/django_project/my_app/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/runtests.py` & `django-stachoutils-4.2.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/settings.py` & `django-stachoutils-4.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/shortcuts/tests.py` & `django-stachoutils-4.2.0/tests/shortcuts/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/sql/tests.py` & `django-stachoutils-4.2.0/tests/sql/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/storage/tests.py` & `django-stachoutils-4.2.0/tests/storage/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templates/generic_list_test.html` & `django-stachoutils-4.2.0/tests/templates/generic_list_test.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/models.py` & `django-stachoutils-4.2.0/tests/templatetags/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/test_filters.py` & `django-stachoutils-4.2.0/tests/templatetags/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/test_pagination_tags.py` & `django-stachoutils-4.2.0/tests/templatetags/test_pagination_tags.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/test_tags.py` & `django-stachoutils-4.2.0/tests/templatetags/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/tests.py` & `django-stachoutils-4.2.0/tests/templatetags/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/templatetags/utils.py` & `django-stachoutils-4.2.0/tests/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/utils/tests.py` & `django-stachoutils-4.2.0/tests/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/views/models.py` & `django-stachoutils-4.2.0/tests/views/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/views/test_actions.py` & `django-stachoutils-4.2.0/tests/views/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-4.1.0/tests/views/test_generic_view.py` & `django-stachoutils-4.2.0/tests/views/test_generic_view.py`

 * *Files identical despite different names*

