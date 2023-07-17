# Comparing `tmp/df_config-1.1.8.tar.gz` & `tmp/df_config-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df_config-1.1.8.tar", last modified: Fri Feb 10 18:37:54 2023, max compression
+gzip compressed data, was "df_config-1.1.9.tar", last modified: Fri Feb 10 18:55:00 2023, max compression
```

## Comparing `df_config-1.1.8.tar` & `df_config-1.1.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.479901 df_config-1.1.8/
--rw-r--r--   0 flanker    (501) staff       (20)     3096 2022-12-29 22:09:02.000000 df_config-1.1.8/.gitignore
--rw-r--r--   0 flanker    (501) staff       (20)      558 2023-02-03 18:15:22.000000 df_config-1.1.8/.travis.yml
--rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-07-19 13:16:34.000000 df_config-1.1.8/LICENSE
--rw-r--r--   0 flanker    (501) staff       (20)      101 2020-07-19 13:16:34.000000 df_config-1.1.8/MANIFEST.in
--rw-r--r--   0 flanker    (501) staff       (20)    10409 2023-02-10 18:37:54.480108 df_config-1.1.8/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     9260 2022-11-27 10:59:47.000000 df_config-1.1.8/README.md
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.440742 df_config-1.1.8/df_config/
--rw-r--r--   0 flanker    (501) staff       (20)     1241 2023-02-10 18:34:32.000000 df_config-1.1.8/df_config/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1481 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/application.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.443457 df_config-1.1.8/df_config/apps/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/apps/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1599 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/apps/allauth.py
--rw-r--r--   0 flanker    (501) staff       (20)     3053 2022-11-27 11:33:48.000000 df_config-1.1.8/df_config/apps/backends.py
--rw-r--r--   0 flanker    (501) staff       (20)     6435 2022-11-27 09:10:35.000000 df_config-1.1.8/df_config/apps/middleware.py
--rw-r--r--   0 flanker    (501) staff       (20)     6607 2022-11-27 11:33:16.000000 df_config-1.1.8/df_config/apps/pipeline.py
--rw-r--r--   0 flanker    (501) staff       (20)     1198 2022-11-19 17:15:08.000000 df_config-1.1.8/df_config/checks.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.464265 df_config-1.1.8/df_config/config/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/config/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1539 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/config/base.py
--rw-r--r--   0 flanker    (501) staff       (20)    21514 2023-01-29 11:59:37.000000 df_config-1.1.8/df_config/config/defaults.py
--rw-r--r--   0 flanker    (501) staff       (20)    20396 2023-02-10 18:35:27.000000 df_config-1.1.8/df_config/config/dynamic_settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     8762 2023-01-06 22:10:37.000000 df_config-1.1.8/df_config/config/fields.py
--rw-r--r--   0 flanker    (501) staff       (20)     3068 2022-11-27 11:20:03.000000 df_config-1.1.8/df_config/config/fields_providers.py
--rw-r--r--   0 flanker    (501) staff       (20)    10562 2023-02-10 18:34:45.000000 df_config-1.1.8/df_config/config/merger.py
--rw-r--r--   0 flanker    (501) staff       (20)     7721 2023-01-06 19:23:43.000000 df_config-1.1.8/df_config/config/url.py
--rw-r--r--   0 flanker    (501) staff       (20)    10449 2023-02-03 22:19:05.000000 df_config-1.1.8/df_config/config/values_providers.py
--rw-r--r--   0 flanker    (501) staff       (20)     1605 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/context_processors.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.465035 df_config-1.1.8/df_config/extra/
--rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-10 21:42:06.000000 df_config-1.1.8/df_config/extra/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)      591 2023-01-15 09:27:42.000000 df_config-1.1.8/df_config/extra/loki.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.452927 df_config-1.1.8/df_config/guesses/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/guesses/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     8190 2023-02-03 22:24:53.000000 df_config-1.1.8/df_config/guesses/apps.py
--rw-r--r--   0 flanker    (501) staff       (20)     8425 2022-11-27 08:50:51.000000 df_config-1.1.8/df_config/guesses/auth.py
--rw-r--r--   0 flanker    (501) staff       (20)     8317 2022-11-26 21:49:09.000000 df_config-1.1.8/df_config/guesses/databases.py
--rw-r--r--   0 flanker    (501) staff       (20)     1217 2020-11-17 06:24:11.000000 df_config-1.1.8/df_config/guesses/djt.py
--rw-r--r--   0 flanker    (501) staff       (20)    26563 2023-01-20 21:31:12.000000 df_config-1.1.8/df_config/guesses/log.py
--rw-r--r--   0 flanker    (501) staff       (20)    14447 2023-01-14 15:24:13.000000 df_config-1.1.8/df_config/guesses/misc.py
--rw-r--r--   0 flanker    (501) staff       (20)     4473 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/guesses/pipeline.py
--rw-r--r--   0 flanker    (501) staff       (20)     9997 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/guesses/social_providers.py
--rw-r--r--   0 flanker    (501) staff       (20)     2312 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/guesses/staticfiles.py
--rw-r--r--   0 flanker    (501) staff       (20)    17408 2022-12-31 16:59:13.000000 df_config-1.1.8/df_config/iniconf.py
--rw-r--r--   0 flanker    (501) staff       (20)     5733 2023-02-10 18:35:27.000000 df_config-1.1.8/df_config/manage.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.458145 df_config-1.1.8/df_config/management/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/management/__init__.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.460535 df_config-1.1.8/df_config/management/commands/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/management/commands/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1626 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/management/commands/collectstatic.py
--rw-r--r--   0 flanker    (501) staff       (20)     8826 2023-02-03 22:24:53.000000 df_config-1.1.8/df_config/management/commands/config.py
--rw-r--r--   0 flanker    (501) staff       (20)     5130 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/management/commands/server.py
--rw-r--r--   0 flanker    (501) staff       (20)     2243 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/models.py
--rw-r--r--   0 flanker    (501) staff       (20)     3486 2022-09-04 06:52:40.000000 df_config-1.1.8/df_config/root_urls.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.431278 df_config-1.1.8/df_config/static/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.468622 df_config-1.1.8/df_config/static/favicon/
--rw-r--r--   0 flanker    (501) staff       (20)    33195 2020-07-19 13:16:34.000000 df_config-1.1.8/df_config/static/favicon/apple-touch-icon-precomposed.png
--rw-r--r--   0 flanker    (501) staff       (20)    33195 2020-07-19 13:16:34.000000 df_config-1.1.8/df_config/static/favicon/apple-touch-icon.png
--rw-r--r--   0 flanker    (501) staff       (20)     4286 2020-07-19 13:16:34.000000 df_config-1.1.8/df_config/static/favicon/favicon.ico
--rw-r--r--   0 flanker    (501) staff       (20)       31 2020-07-19 13:16:34.000000 df_config-1.1.8/df_config/static/favicon/robots.txt
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.469600 df_config-1.1.8/df_config/static/js/
--rw-r--r--   0 flanker    (501) staff       (20)     1193 2020-10-24 15:08:51.000000 df_config-1.1.8/df_config/static/js/df_config.min.js
--rw-r--r--   0 flanker    (501) staff       (20)     6674 2022-04-11 05:12:35.000000 df_config-1.1.8/df_config/static/js/df_config.min.js.map
--rw-r--r--   0 flanker    (501) staff       (20)       17 2022-11-27 09:10:35.000000 df_config-1.1.8/df_config/urls.py
--rw-r--r--   0 flanker    (501) staff       (20)    11160 2022-11-19 17:15:09.000000 df_config-1.1.8/df_config/utils.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.463279 df_config-1.1.8/df_config.egg-info/
--rw-r--r--   0 flanker    (501) staff       (20)    10409 2023-02-10 18:37:54.000000 df_config-1.1.8/df_config.egg-info/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     3408 2023-02-10 18:37:54.000000 df_config-1.1.8/df_config.egg-info/SOURCES.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2023-02-10 18:37:54.000000 df_config-1.1.8/df_config.egg-info/dependency_links.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2020-08-20 19:04:52.000000 df_config-1.1.8/df_config.egg-info/not-zip-safe
--rw-r--r--   0 flanker    (501) staff       (20)       12 2023-02-10 18:37:54.000000 df_config-1.1.8/df_config.egg-info/requires.txt
--rw-r--r--   0 flanker    (501) staff       (20)       10 2023-02-10 18:37:54.000000 df_config-1.1.8/df_config.egg-info/top_level.txt
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.472467 df_config-1.1.8/npm/
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.473087 df_config-1.1.8/npm/df_config/
--rw-r--r--   0 flanker    (501) staff       (20)     1763 2022-04-11 05:12:35.000000 df_config-1.1.8/npm/df_config/app.ts
--rw-r--r--   0 flanker    (501) staff       (20)   101575 2022-12-29 22:15:13.000000 df_config-1.1.8/npm/package-lock.json
--rw-r--r--   0 flanker    (501) staff       (20)      474 2022-12-29 22:14:40.000000 df_config-1.1.8/npm/package.json
--rw-r--r--   0 flanker    (501) staff       (20)      164 2020-07-19 13:16:34.000000 df_config-1.1.8/npm/tsconfig.json
--rw-r--r--   0 flanker    (501) staff       (20)     2192 2022-04-11 05:12:35.000000 df_config-1.1.8/npm/webpack.config.js
--rw-r--r--   0 flanker    (501) staff       (20)     2360 2023-02-10 18:37:54.481274 df_config-1.1.8/setup.cfg
--rw-r--r--   0 flanker    (501) staff       (20)     1257 2022-04-11 05:12:35.000000 df_config-1.1.8/setup.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.476903 df_config-1.1.8/test_df_config/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/__init__.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:37:54.479567 df_config-1.1.8/test_df_config/data/
--rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/data/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)       90 2020-07-19 13:16:34.000000 df_config-1.1.8/test_df_config/data/range_data.txt
--rw-r--r--   0 flanker    (501) staff       (20)     1682 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/data/sample_iniconf.py
--rw-r--r--   0 flanker    (501) staff       (20)     1254 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/data/sample_settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     1285 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/data/settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     6571 2023-02-10 18:35:27.000000 df_config-1.1.8/test_df_config/test_dynamic_settings.py
--rw-r--r--   0 flanker    (501) staff       (20)     6981 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/test_fields.py
--rw-r--r--   0 flanker    (501) staff       (20)     2280 2022-11-27 11:34:21.000000 df_config-1.1.8/test_df_config/test_fields_providers.py
--rw-r--r--   0 flanker    (501) staff       (20)     3488 2022-04-11 20:02:33.000000 df_config-1.1.8/test_df_config/test_manage.py
--rw-r--r--   0 flanker    (501) staff       (20)     6579 2023-02-10 18:35:27.000000 df_config-1.1.8/test_df_config/test_merger.py
--rw-r--r--   0 flanker    (501) staff       (20)     6599 2022-04-11 05:12:35.000000 df_config-1.1.8/test_df_config/test_utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     8694 2022-11-27 08:50:51.000000 df_config-1.1.8/test_df_config/test_values_providers.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.352053 df_config-1.1.9/
+-rw-r--r--   0 flanker    (501) staff       (20)     3096 2022-12-29 22:09:02.000000 df_config-1.1.9/.gitignore
+-rw-r--r--   0 flanker    (501) staff       (20)      558 2023-02-03 18:15:22.000000 df_config-1.1.9/.travis.yml
+-rw-r--r--   0 flanker    (501) staff       (20)    21393 2020-07-19 13:16:34.000000 df_config-1.1.9/LICENSE
+-rw-r--r--   0 flanker    (501) staff       (20)      101 2020-07-19 13:16:34.000000 df_config-1.1.9/MANIFEST.in
+-rw-r--r--   0 flanker    (501) staff       (20)    10409 2023-02-10 18:55:00.352246 df_config-1.1.9/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     9260 2022-11-27 10:59:47.000000 df_config-1.1.9/README.md
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.293375 df_config-1.1.9/df_config/
+-rw-r--r--   0 flanker    (501) staff       (20)     1241 2023-02-10 18:54:21.000000 df_config-1.1.9/df_config/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1481 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/application.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.296443 df_config-1.1.9/df_config/apps/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/apps/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1599 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/apps/allauth.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3053 2022-11-27 11:33:48.000000 df_config-1.1.9/df_config/apps/backends.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6435 2022-11-27 09:10:35.000000 df_config-1.1.9/df_config/apps/middleware.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6607 2022-11-27 11:33:16.000000 df_config-1.1.9/df_config/apps/pipeline.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1198 2022-11-19 17:15:08.000000 df_config-1.1.9/df_config/checks.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.321914 df_config-1.1.9/df_config/config/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/config/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1539 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/config/base.py
+-rw-r--r--   0 flanker    (501) staff       (20)    21514 2023-01-29 11:59:37.000000 df_config-1.1.9/df_config/config/defaults.py
+-rw-r--r--   0 flanker    (501) staff       (20)    20396 2023-02-10 18:35:27.000000 df_config-1.1.9/df_config/config/dynamic_settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8762 2023-01-06 22:10:37.000000 df_config-1.1.9/df_config/config/fields.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3068 2022-11-27 11:20:03.000000 df_config-1.1.9/df_config/config/fields_providers.py
+-rw-r--r--   0 flanker    (501) staff       (20)    10562 2023-02-10 18:34:45.000000 df_config-1.1.9/df_config/config/merger.py
+-rw-r--r--   0 flanker    (501) staff       (20)     7721 2023-01-06 19:23:43.000000 df_config-1.1.9/df_config/config/url.py
+-rw-r--r--   0 flanker    (501) staff       (20)    10449 2023-02-03 22:19:05.000000 df_config-1.1.9/df_config/config/values_providers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1605 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/context_processors.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.323291 df_config-1.1.9/df_config/extra/
+-rw-r--r--   0 flanker    (501) staff       (20)        0 2023-01-10 21:42:06.000000 df_config-1.1.9/df_config/extra/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)      591 2023-01-15 09:27:42.000000 df_config-1.1.9/df_config/extra/loki.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.312042 df_config-1.1.9/df_config/guesses/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/guesses/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8190 2023-02-03 22:24:53.000000 df_config-1.1.9/df_config/guesses/apps.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8425 2022-11-27 08:50:51.000000 df_config-1.1.9/df_config/guesses/auth.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8317 2022-11-26 21:49:09.000000 df_config-1.1.9/df_config/guesses/databases.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1217 2020-11-17 06:24:11.000000 df_config-1.1.9/df_config/guesses/djt.py
+-rw-r--r--   0 flanker    (501) staff       (20)    26563 2023-01-20 21:31:12.000000 df_config-1.1.9/df_config/guesses/log.py
+-rw-r--r--   0 flanker    (501) staff       (20)    14447 2023-01-14 15:24:13.000000 df_config-1.1.9/df_config/guesses/misc.py
+-rw-r--r--   0 flanker    (501) staff       (20)     4473 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/guesses/pipeline.py
+-rw-r--r--   0 flanker    (501) staff       (20)     9997 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/guesses/social_providers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2312 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/guesses/staticfiles.py
+-rw-r--r--   0 flanker    (501) staff       (20)    17408 2022-12-31 16:59:13.000000 df_config-1.1.9/df_config/iniconf.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5981 2023-02-10 18:54:34.000000 df_config-1.1.9/df_config/manage.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.312767 df_config-1.1.9/df_config/management/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/management/__init__.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.315754 df_config-1.1.9/df_config/management/commands/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/management/commands/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1626 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/management/commands/collectstatic.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8826 2023-02-03 22:24:53.000000 df_config-1.1.9/df_config/management/commands/config.py
+-rw-r--r--   0 flanker    (501) staff       (20)     5130 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/management/commands/server.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2243 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/models.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3486 2022-09-04 06:52:40.000000 df_config-1.1.9/df_config/root_urls.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.283740 df_config-1.1.9/df_config/static/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.328104 df_config-1.1.9/df_config/static/favicon/
+-rw-r--r--   0 flanker    (501) staff       (20)    33195 2020-07-19 13:16:34.000000 df_config-1.1.9/df_config/static/favicon/apple-touch-icon-precomposed.png
+-rw-r--r--   0 flanker    (501) staff       (20)    33195 2020-07-19 13:16:34.000000 df_config-1.1.9/df_config/static/favicon/apple-touch-icon.png
+-rw-r--r--   0 flanker    (501) staff       (20)     4286 2020-07-19 13:16:34.000000 df_config-1.1.9/df_config/static/favicon/favicon.ico
+-rw-r--r--   0 flanker    (501) staff       (20)       31 2020-07-19 13:16:34.000000 df_config-1.1.9/df_config/static/favicon/robots.txt
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.329764 df_config-1.1.9/df_config/static/js/
+-rw-r--r--   0 flanker    (501) staff       (20)     1193 2020-10-24 15:08:51.000000 df_config-1.1.9/df_config/static/js/df_config.min.js
+-rw-r--r--   0 flanker    (501) staff       (20)     6674 2022-04-11 05:12:35.000000 df_config-1.1.9/df_config/static/js/df_config.min.js.map
+-rw-r--r--   0 flanker    (501) staff       (20)       17 2022-11-27 09:10:35.000000 df_config-1.1.9/df_config/urls.py
+-rw-r--r--   0 flanker    (501) staff       (20)    11160 2022-11-19 17:15:09.000000 df_config-1.1.9/df_config/utils.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.320315 df_config-1.1.9/df_config.egg-info/
+-rw-r--r--   0 flanker    (501) staff       (20)    10409 2023-02-10 18:54:59.000000 df_config-1.1.9/df_config.egg-info/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     3408 2023-02-10 18:54:59.000000 df_config-1.1.9/df_config.egg-info/SOURCES.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2023-02-10 18:54:59.000000 df_config-1.1.9/df_config.egg-info/dependency_links.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-08-20 19:04:52.000000 df_config-1.1.9/df_config.egg-info/not-zip-safe
+-rw-r--r--   0 flanker    (501) staff       (20)       12 2023-02-10 18:54:59.000000 df_config-1.1.9/df_config.egg-info/requires.txt
+-rw-r--r--   0 flanker    (501) staff       (20)       10 2023-02-10 18:54:59.000000 df_config-1.1.9/df_config.egg-info/top_level.txt
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.340036 df_config-1.1.9/npm/
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.340910 df_config-1.1.9/npm/df_config/
+-rw-r--r--   0 flanker    (501) staff       (20)     1763 2022-04-11 05:12:35.000000 df_config-1.1.9/npm/df_config/app.ts
+-rw-r--r--   0 flanker    (501) staff       (20)   101575 2022-12-29 22:15:13.000000 df_config-1.1.9/npm/package-lock.json
+-rw-r--r--   0 flanker    (501) staff       (20)      474 2022-12-29 22:14:40.000000 df_config-1.1.9/npm/package.json
+-rw-r--r--   0 flanker    (501) staff       (20)      164 2020-07-19 13:16:34.000000 df_config-1.1.9/npm/tsconfig.json
+-rw-r--r--   0 flanker    (501) staff       (20)     2192 2022-04-11 05:12:35.000000 df_config-1.1.9/npm/webpack.config.js
+-rw-r--r--   0 flanker    (501) staff       (20)     2360 2023-02-10 18:55:00.353904 df_config-1.1.9/setup.cfg
+-rw-r--r--   0 flanker    (501) staff       (20)     1257 2022-04-11 05:12:35.000000 df_config-1.1.9/setup.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.347558 df_config-1.1.9/test_df_config/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/__init__.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2023-02-10 18:55:00.351568 df_config-1.1.9/test_df_config/data/
+-rw-r--r--   0 flanker    (501) staff       (20)     1218 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/data/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)       90 2020-07-19 13:16:34.000000 df_config-1.1.9/test_df_config/data/range_data.txt
+-rw-r--r--   0 flanker    (501) staff       (20)     1682 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/data/sample_iniconf.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1254 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/data/sample_settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1285 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/data/settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6571 2023-02-10 18:35:27.000000 df_config-1.1.9/test_df_config/test_dynamic_settings.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6981 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/test_fields.py
+-rw-r--r--   0 flanker    (501) staff       (20)     2280 2022-11-27 11:34:21.000000 df_config-1.1.9/test_df_config/test_fields_providers.py
+-rw-r--r--   0 flanker    (501) staff       (20)     3488 2022-04-11 20:02:33.000000 df_config-1.1.9/test_df_config/test_manage.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6579 2023-02-10 18:35:27.000000 df_config-1.1.9/test_df_config/test_merger.py
+-rw-r--r--   0 flanker    (501) staff       (20)     6599 2022-04-11 05:12:35.000000 df_config-1.1.9/test_df_config/test_utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)     8694 2022-11-27 08:50:51.000000 df_config-1.1.9/test_df_config/test_values_providers.py
```

### Comparing `df_config-1.1.8/.gitignore` & `df_config-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/.travis.yml` & `df_config-1.1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/LICENSE` & `df_config-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/PKG-INFO` & `df_config-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df_config
-Version: 1.1.8
+Version: 1.1.9
 Summary: Smart default settings for Django websites
 Home-page: https://github.com/d9pouces/df_config
 Author: Matthieu Gallet
 Author-email: df_config@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: df_config@19pouces.net
 License: CeCILL-B
```

### Comparing `df_config-1.1.8/README.md` & `df_config-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/__init__.py` & `df_config-1.1.9/df_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  You should have received a copy of the CeCILL-B license with                #
 #  this file. If not, please visit:                                            #
 #  https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt (English)           #
 #  or https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt (French)         #
 #                                                                              #
 # ##############################################################################
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
```

### Comparing `df_config-1.1.8/df_config/application.py` & `df_config-1.1.9/df_config/application.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/apps/__init__.py` & `df_config-1.1.9/df_config/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/apps/allauth.py` & `df_config-1.1.9/df_config/apps/allauth.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/apps/backends.py` & `df_config-1.1.9/df_config/apps/backends.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/apps/middleware.py` & `df_config-1.1.9/df_config/apps/middleware.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/apps/pipeline.py` & `df_config-1.1.9/df_config/apps/pipeline.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/checks.py` & `df_config-1.1.9/df_config/checks.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/__init__.py` & `df_config-1.1.9/df_config/config/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/base.py` & `df_config-1.1.9/df_config/config/base.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/defaults.py` & `df_config-1.1.9/df_config/config/defaults.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/dynamic_settings.py` & `df_config-1.1.9/df_config/config/dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/fields.py` & `df_config-1.1.9/df_config/config/fields.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/fields_providers.py` & `df_config-1.1.9/df_config/config/fields_providers.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/merger.py` & `df_config-1.1.9/df_config/config/merger.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/url.py` & `df_config-1.1.9/df_config/config/url.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/config/values_providers.py` & `df_config-1.1.9/df_config/config/values_providers.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/context_processors.py` & `df_config-1.1.9/df_config/context_processors.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/extra/loki.py` & `df_config-1.1.9/df_config/extra/loki.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/__init__.py` & `df_config-1.1.9/df_config/guesses/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/apps.py` & `df_config-1.1.9/df_config/guesses/apps.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/auth.py` & `df_config-1.1.9/df_config/guesses/auth.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/databases.py` & `df_config-1.1.9/df_config/guesses/databases.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/djt.py` & `df_config-1.1.9/df_config/guesses/djt.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/log.py` & `df_config-1.1.9/df_config/guesses/log.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/misc.py` & `df_config-1.1.9/df_config/guesses/misc.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/pipeline.py` & `df_config-1.1.9/df_config/guesses/pipeline.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/social_providers.py` & `df_config-1.1.9/df_config/guesses/social_providers.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/guesses/staticfiles.py` & `df_config-1.1.9/df_config/guesses/staticfiles.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/iniconf.py` & `df_config-1.1.9/df_config/iniconf.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/manage.py` & `df_config-1.1.9/df_config/manage.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,23 @@
     IniConfigProvider,
     PythonFileProvider,
     PythonModuleProvider,
 )
 
 PYCHARM_VARIABLE_NAME = "PYCHARM_DJANGO_MANAGE_MODULE"
 SETTINGS_VARIABLE_NAME = "DJANGO_SETTINGS_MODULE"
+DEFAULT_SETTINGS_MODULE = "df_config.config.base"
 MODULE_VARIABLE_NAME = "DF_CONF_NAME"
 
 
-def set_env(module_name: str = None, argv: List[str] = None):
+def set_env(
+    module_name: str = None,
+    argv: List[str] = None,
+    settings_module=DEFAULT_SETTINGS_MODULE,
+):
     """Set the environment variable `DF_CONF_NAME` with the main Python module name
     The value looks like "project_name".
     If `module_name` is not given, tries to infer it from the running script name
 
     """
     if MODULE_VARIABLE_NAME not in os.environ:
         script_re = re.compile(r"^([\w_\-.]+)-\w+(?:\.py|\.pyc|)$")
@@ -53,32 +58,34 @@
             if argv and argv[0]:
                 script_matcher = script_re.match(os.path.basename(argv[0]))
                 if script_matcher:
                     module_name = script_matcher.group(1)
         if not module_name:
             module_name = "df_config"
         os.environ[MODULE_VARIABLE_NAME] = module_name.replace("-", "_").lower()
-    os.environ.setdefault(SETTINGS_VARIABLE_NAME, "df_config.config.base")
+    os.environ.setdefault(SETTINGS_VARIABLE_NAME, settings_module)
     return os.environ[MODULE_VARIABLE_NAME]
 
 
-def get_merger_from_env(merger_class=SettingMerger) -> SettingMerger:
+def get_merger_from_env(
+    merger_class=SettingMerger, settings_module=DEFAULT_SETTINGS_MODULE
+) -> SettingMerger:
     """Return a settingmerger to determien all available settings, should be used after set_env().
     Settings are found in this order:
 
     * df_config.config.defaults
     * {project_name}.defaults (overrides df_config.config.defaults)
     * {root}/etc/{project_name}/settings.ini (overrides {project_name}.settings)
     * {root}/etc/{project_name}/settings.py (overrides {root}/etc/{project_name}/settings.ini)
     * ./local_settings.ini (overrides {root}/etc/{project_name}/settings.py)
     * ./local_settings.py (overrides ./local_settings.ini)
     * environment variables (overrides ./local_settings.py)
     """
     # required if set_env is not called
-    module_name = set_env()
+    module_name = set_env(settings_module=settings_module)
     prefix = os.path.abspath(sys.prefix)
     if prefix == "/usr":
         prefix = ""
     ini_mapping = f"{module_name}.iniconf:INI_MAPPING"
     config_providers = [
         DictProvider({"DF_MODULE_NAME": module_name}, name="default values"),
         PythonModuleProvider("df_config.config.defaults"),
@@ -103,16 +110,16 @@
     ]
     fields_provider = PythonConfigFieldsProvider(
         ini_mapping, fallback="df_config.iniconf:DEFAULT_INI_MAPPING"
     )
     return merger_class(fields_provider, config_providers)
 
 
-def manage(argv=None):
-    set_env()
+def manage(argv=None, settings_module=DEFAULT_SETTINGS_MODULE):
+    set_env(settings_module=settings_module)
     import django
 
     django.setup()
     from django.core.management import execute_from_command_line
 
     patch_commands()
     argv = argv or sys.argv
```

### Comparing `df_config-1.1.8/df_config/management/__init__.py` & `df_config-1.1.9/df_config/management/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/management/commands/__init__.py` & `df_config-1.1.9/df_config/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/management/commands/collectstatic.py` & `df_config-1.1.9/df_config/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/management/commands/config.py` & `df_config-1.1.9/df_config/management/commands/config.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/management/commands/server.py` & `df_config-1.1.9/df_config/management/commands/server.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/models.py` & `df_config-1.1.9/df_config/models.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/root_urls.py` & `df_config-1.1.9/df_config/root_urls.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/static/favicon/apple-touch-icon-precomposed.png` & `df_config-1.1.9/df_config/static/favicon/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/static/favicon/apple-touch-icon.png` & `df_config-1.1.9/df_config/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/static/favicon/favicon.ico` & `df_config-1.1.9/df_config/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/static/js/df_config.min.js` & `df_config-1.1.9/df_config/static/js/df_config.min.js`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/static/js/df_config.min.js.map` & `df_config-1.1.9/df_config/static/js/df_config.min.js.map`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config/utils.py` & `df_config-1.1.9/df_config/utils.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/df_config.egg-info/PKG-INFO` & `df_config-1.1.9/df_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-config
-Version: 1.1.8
+Version: 1.1.9
 Summary: Smart default settings for Django websites
 Home-page: https://github.com/d9pouces/df_config
 Author: Matthieu Gallet
 Author-email: df_config@19pouces.net
 Maintainer: Matthieu Gallet
 Maintainer-email: df_config@19pouces.net
 License: CeCILL-B
```

### Comparing `df_config-1.1.8/df_config.egg-info/SOURCES.txt` & `df_config-1.1.9/df_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/npm/df_config/app.ts` & `df_config-1.1.9/npm/df_config/app.ts`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/npm/package-lock.json` & `df_config-1.1.9/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/npm/webpack.config.js` & `df_config-1.1.9/npm/webpack.config.js`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/setup.cfg` & `df_config-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/setup.py` & `df_config-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/__init__.py` & `df_config-1.1.9/test_df_config/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/data/__init__.py` & `df_config-1.1.9/test_df_config/data/__init__.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/data/sample_iniconf.py` & `df_config-1.1.9/test_df_config/data/sample_iniconf.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/data/sample_settings.py` & `df_config-1.1.9/test_df_config/data/sample_settings.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/data/settings.py` & `df_config-1.1.9/test_df_config/data/settings.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_dynamic_settings.py` & `df_config-1.1.9/test_df_config/test_dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_fields.py` & `df_config-1.1.9/test_df_config/test_fields.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_fields_providers.py` & `df_config-1.1.9/test_df_config/test_fields_providers.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_manage.py` & `df_config-1.1.9/test_df_config/test_manage.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_merger.py` & `df_config-1.1.9/test_df_config/test_merger.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_utils.py` & `df_config-1.1.9/test_df_config/test_utils.py`

 * *Files identical despite different names*

### Comparing `df_config-1.1.8/test_df_config/test_values_providers.py` & `df_config-1.1.9/test_df_config/test_values_providers.py`

 * *Files identical despite different names*

