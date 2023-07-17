# Comparing `tmp/Flask-BigApp-2023.1.9.6.tar.gz` & `tmp/Flask-BigApp-2023.1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.9.6.tar", last modified: Thu Jun 29 08:02:27 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.7.tar", last modified: Thu Jul  6 20:58:57 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.9.6.tar` & `Flask-BigApp-2023.1.9.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-29 08:02:23.000000 Flask-BigApp-2023.1.9.6/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-15 10:09:07.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11409 2023-06-29 07:26:28.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-29 07:12:39.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     5172 2023-06-29 07:59:44.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/registeries.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3630 2023-06-29 07:52:15.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.9.7/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.9.7/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-05-04 14:17:25.000000 Flask-BigApp-2023.1.9.7/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.9.7/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-07-06 20:58:40.000000 Flask-BigApp-2023.1.9.7/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.910463 Flask-BigApp-2023.1.9.7/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-07-06 20:58:57.000000 Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-10 15:02:44.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11409 2023-07-06 20:58:04.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-05-18 10:09:34.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5172 2023-07-06 20:58:04.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-05-18 10:27:54.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9106 2023-07-06 20:58:04.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3630 2023-07-06 20:58:04.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.910463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.910463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.914463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.910463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.910463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-06 20:58:57.918463 Flask-BigApp-2023.1.9.7/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-05-18 12:04:01.000000 Flask-BigApp-2023.1.9.7/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.9.6/LICENSE` & `Flask-BigApp-2023.1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/PKG-INFO` & `Flask-BigApp-2023.1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.6
+Version: 2023.1.9.7
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.6/README.md` & `Flask-BigApp-2023.1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/setup.py` & `Flask-BigApp-2023.1.9.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.9.6',
+    version=f'2023.1.9.7',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
```

### Comparing `Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.6
+Version: 2023.1.9.7
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9.7/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/bigapp.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/registeries.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/registeries.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/security.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,59 @@
             return func(*args, **kwargs)
 
         return inner
 
     return login_check_wrapper
 
 
+def api_login_check(
+        bool_session_key: str,
+        fail_if_session_value_is: bool = False,
+        json_to_return: t.Optional[t.Dict[str, t.Any]] = None,
+):
+    """
+    A decorator that checks if the specified session key exists, shows a 401 error if it does not
+
+    Example of a route that requires a user to be logged in:
+
+    @bp.route("/api/resource", methods=["GET"])
+    @api_login_check('logged_in')
+    def api_page():
+        ...
+
+    Can also supply your own failed return JSON:
+
+    @bp.route("/api/resource", methods=["GET"])
+    @api_login_check('logged_in', json_to_return={"error": "You are not logged in."})
+    def api_page():
+        ...
+
+    Default json_to_return is {"error": "You are not logged in."}
+
+    :param bool_session_key: The session key to check for.
+    :param fail_if_session_value_is: The boolean value to check the session key against.
+    :param json_to_return: the json that will be returned if login has failed.
+    """
+
+    def login_check_wrapper(func):
+        @wraps(func)
+        def inner(*args, **kwargs):
+            if bool_session_key not in session:
+                return json_to_return or {"error": "You are not logged in."}, 401
+
+            if session[bool_session_key] == fail_if_session_value_is:
+                return json_to_return or {"error": "You are not logged in."}, 401
+
+            return func(*args, **kwargs)
+
+        return inner
+
+    return login_check_wrapper
+
+
 def permission_check(
         iter_session_key: str,
         endpoint_redirect: str,
         redirect_if_no_match: t.Optional[list] = None,
         endpoint_kwargs: t.Optional[t.Dict[str, t.Union[str, int]]] = None,
         message: t.Optional[str] = None,
         message_category: str = "message"
```

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp/utilities.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9.7/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.6/tests/test_group.py` & `Flask-BigApp-2023.1.9.7/tests/test_group.py`

 * *Files identical despite different names*

