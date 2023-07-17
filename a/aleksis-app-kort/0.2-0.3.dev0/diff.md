# Comparing `tmp/aleksis_app_kort-0.2.tar.gz` & `tmp/aleksis_app_kort-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_kort-0.2.tar", max compression
+gzip compressed data, was "aleksis_app_kort-0.3.dev0.tar", max compression
```

## Comparing `aleksis_app_kort-0.2.tar` & `aleksis_app_kort-0.3.dev0.tar`

### file list

```diff
@@ -1,88 +1,93 @@
--rw-r--r--   0        0        0      844 2023-05-15 19:45:26.471295 aleksis_app_kort-0.2/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/LICENCE.rst
--rw-r--r--   0        0        0      888 2022-12-04 11:35:00.665707 aleksis_app_kort-0.2/README.rst
--rw-r--r--   0        0        0      150 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/aleksis/apps/kort/__init__.py
--rw-r--r--   0        0        0      193 2022-03-10 18:37:05.158053 aleksis_app_kort-0.2/aleksis/apps/kort/admin.py
--rw-r--r--   0        0        0     7107 2022-12-04 12:04:32.510414 aleksis_app_kort-0.2/aleksis/apps/kort/api.py
--rw-r--r--   0        0        0     1449 2022-12-04 12:00:14.657517 aleksis_app_kort-0.2/aleksis/apps/kort/apps.py
--rw-r--r--   0        0        0     5311 2022-08-14 13:54:09.409675 aleksis_app_kort-0.2/aleksis/apps/kort/forms.py
--rw-r--r--   0        0        0     5751 2023-03-20 15:59:14.764294 aleksis_app_kort-0.2/aleksis/apps/kort/frontend/index.js
--rw-r--r--   0        0        0      231 2023-03-19 14:58:24.454538 aleksis_app_kort-0.2/aleksis/apps/kort/frontend/messages/de.json
--rw-r--r--   0        0        0      228 2023-03-19 14:47:27.272460 aleksis_app_kort-0.2/aleksis/apps/kort/frontend/messages/en.json
--rw-r--r--   0        0        0        3 2023-03-19 14:58:24.458538 aleksis_app_kort-0.2/aleksis/apps/kort/frontend/messages/ru.json
--rw-r--r--   0        0        0      295 2023-04-14 09:25:50.833116 aleksis_app_kort-0.2/aleksis/apps/kort/frontend/messages/uk.json
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/aleksis/apps/kort/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-03-19 20:34:24.461191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18993 2023-03-19 14:48:32.328267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13124 2023-03-19 20:34:24.461191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24175 2023-03-19 14:48:32.316267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-19 20:34:24.465191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18909 2023-03-19 14:48:32.252267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.465191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.236267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.296267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2023-03-19 20:34:24.465191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19053 2023-03-19 14:48:32.212267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-19 20:34:24.461191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18863 2023-03-19 14:48:32.276267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2023-03-19 20:34:24.465191 aleksis_app_kort-0.2/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19140 2023-03-19 14:48:32.240267 aleksis_app_kort-0.2/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1459 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0001_initial.py
--rw-r--r--   0        0        0     2334 2021-11-30 20:07:19.626067 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0002_card_printer.py
--rw-r--r--   0        0        0     1544 2022-03-08 19:23:37.637527 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py
--rw-r--r--   0        0        0      428 2022-03-08 19:32:45.096219 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0004_alter_card_chip_number.py
--rw-r--r--   0        0        0      538 2022-03-10 16:48:40.401048 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0005_card_pdf_file.py
--rw-r--r--   0        0        0     1218 2022-03-10 19:03:08.179322 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py
--rw-r--r--   0        0        0     2418 2022-05-29 10:47:02.293945 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py
--rw-r--r--   0        0        0     1052 2022-05-29 10:47:02.293945 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py
--rw-r--r--   0        0        0      455 2022-05-29 10:47:02.293945 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0009_cardprinter_generate_number_on_server.py
--rw-r--r--   0        0        0      778 2022-05-29 10:47:02.293945 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py
--rw-r--r--   0        0        0      437 2022-05-29 10:47:02.293945 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0011_cardprinter_card_detector.py
--rw-r--r--   0        0        0     2071 2022-07-29 13:47:52.820053 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py
--rw-r--r--   0        0        0      906 2022-07-29 13:47:52.820053 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py
--rw-r--r--   0        0        0      754 2022-08-02 22:25:04.075075 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py
--rw-r--r--   0        0        0      575 2022-12-04 11:45:56.812937 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0015_migrate_scopes.py
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/aleksis/apps/kort/migrations/__init__.py
--rw-r--r--   0        0        0    11630 2022-12-04 12:00:14.781516 aleksis_app_kort-0.2/aleksis/apps/kort/models.py
--rw-r--r--   0        0        0     3515 2022-08-29 10:20:09.797130 aleksis_app_kort-0.2/aleksis/apps/kort/rules.py
--rw-r--r--   0        0        0       32 2022-09-04 10:38:46.745643 aleksis_app_kort-0.2/aleksis/apps/kort/settings.py
--rw-r--r--   0        0        0        0 2021-11-29 18:36:49.876779 aleksis_app_kort-0.2/aleksis/apps/kort/static/.keepdir
--rw-r--r--   0        0        0     5184 2022-08-04 09:05:10.177572 aleksis_app_kort-0.2/aleksis/apps/kort/tables.py
--rw-r--r--   0        0        0      634 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/tasks.py
--rw-r--r--   0        0        0     2126 2022-08-10 14:27:45.460767 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/actions.html
--rw-r--r--   0        0        0     1345 2022-03-12 21:12:55.899447 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/delete.html
--rw-r--r--   0        0        0      399 2023-01-27 18:23:26.937618 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/detail.html
--rw-r--r--   0        0        0     2307 2022-08-10 14:26:18.376009 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/detail_content.html
--rw-r--r--   0        0        0      641 2022-03-08 19:29:07.431134 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/edit.html
--rw-r--r--   0        0        0     3295 2022-08-04 09:04:47.167728 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/issue.html
--rw-r--r--   0        0        0     1177 2023-01-27 18:23:26.937618 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/list.html
--rw-r--r--   0        0        0      787 2022-08-10 14:27:45.448768 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/print_form.html
--rw-r--r--   0        0        0      292 2022-03-10 16:04:46.741747 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/short.html
--rw-r--r--   0        0        0      203 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/status.html
--rw-r--r--   0        0        0     1344 2022-08-10 14:27:45.472767 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/actions.html
--rw-r--r--   0        0        0      896 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/create.html
--rw-r--r--   0        0        0     1273 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/delete.html
--rw-r--r--   0        0        0     1291 2022-08-10 14:27:45.488766 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/detail.html
--rw-r--r--   0        0        0     1851 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/detail_content.html
--rw-r--r--   0        0        0      892 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/edit.html
--rw-r--r--   0        0        0     1276 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/instructions.html
--rw-r--r--   0        0        0      699 2022-08-10 14:27:45.456767 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/list.html
--rw-r--r--   0        0        0      115 2022-07-29 13:47:52.824052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/short.html
--rw-r--r--   0        0        0      470 2022-08-03 17:35:59.880270 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/person_status.html
--rw-r--r--   0        0        0      385 2022-08-03 17:25:48.418519 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/picture.html
--rw-r--r--   0        0        0     1312 2022-08-10 14:27:45.480766 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/actions.html
--rw-r--r--   0        0        0      645 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/create.html
--rw-r--r--   0        0        0     1303 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/delete.html
--rw-r--r--   0        0        0     1292 2022-08-10 14:27:45.476766 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/detail.html
--rw-r--r--   0        0        0     3776 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/detail_content.html
--rw-r--r--   0        0        0      657 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/edit.html
--rw-r--r--   0        0        0      706 2022-08-10 14:27:45.468767 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/list.html
--rw-r--r--   0        0        0      317 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/short.html
--rw-r--r--   0        0        0      228 2022-05-29 10:47:02.297945 aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/status.html
--rw-r--r--   0        0        0     1232 2022-07-29 13:47:52.828052 aleksis_app_kort-0.2/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html
--rw-r--r--   0        0        0      760 2022-03-11 22:36:47.959342 aleksis_app_kort-0.2/aleksis/apps/kort/templatetags/barcode.py
--rw-r--r--   0        0        0     2537 2023-03-19 14:47:27.272460 aleksis_app_kort-0.2/aleksis/apps/kort/urls.py
--rw-r--r--   0        0        0    14858 2022-08-12 16:41:36.393225 aleksis_app_kort-0.2/aleksis/apps/kort/views.py
--rw-r--r--   0        0        0     1361 2023-05-15 19:44:27.239009 aleksis_app_kort-0.2/pyproject.toml
--rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 aleksis_app_kort-0.2/PKG-INFO
+-rw-r--r--   0        0        0      844 2023-07-17 10:18:52.689002 aleksis_app_kort-0.3.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/LICENCE.rst
+-rw-r--r--   0        0        0      952 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/README.rst
+-rw-r--r--   0        0        0      150 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-17 10:18:52.689002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/admin.py
+-rw-r--r--   0        0        0     7107 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/api.py
+-rw-r--r--   0        0        0     1515 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/apps.py
+-rw-r--r--   0        0        0     5311 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/forms.py
+-rw-r--r--   0        0        0     5751 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/index.js
+-rw-r--r--   0        0        0      231 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/messages/de.json
+-rw-r--r--   0        0        0      228 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/messages/en.json
+-rw-r--r--   0        0        0      290 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/messages/ru.json
+-rw-r--r--   0        0        0      302 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/messages/uk.json
+-rw-r--r--   0        0        0        0 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18993 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13124 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24175 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18909 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1545 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19486 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18863 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16278 2023-07-17 10:20:03.697057 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27175 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1459 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2334 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0002_card_printer.py
+-rw-r--r--   0        0        0     1544 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py
+-rw-r--r--   0        0        0      428 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0004_alter_card_chip_number.py
+-rw-r--r--   0        0        0      538 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0005_card_pdf_file.py
+-rw-r--r--   0        0        0     1218 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py
+-rw-r--r--   0        0        0     2418 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py
+-rw-r--r--   0        0        0     1052 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py
+-rw-r--r--   0        0        0      455 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0009_cardprinter_generate_number_on_server.py
+-rw-r--r--   0        0        0      778 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py
+-rw-r--r--   0        0        0      437 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0011_cardprinter_card_detector.py
+-rw-r--r--   0        0        0     2071 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py
+-rw-r--r--   0        0        0      906 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py
+-rw-r--r--   0        0        0      754 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py
+-rw-r--r--   0        0        0      575 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0015_migrate_scopes.py
+-rw-r--r--   0        0        0      499 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0016_card_last_read_counter.py
+-rw-r--r--   0        0        0      534 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0017_cardprinter_oauth2_client_secret.py
+-rw-r--r--   0        0        0        0 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/models/__init__.py
+-rw-r--r--   0        0        0    12148 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/models/cards.py
+-rw-r--r--   0        0        0     1638 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/models/sdm.py
+-rw-r--r--   0        0        0      853 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/preferences.py
+-rw-r--r--   0        0        0     3515 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/rules.py
+-rw-r--r--   0        0        0       32 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/settings.py
+-rw-r--r--   0        0        0        0 2022-01-08 20:03:03.940172 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/static/.keepdir
+-rw-r--r--   0        0        0     5230 2023-07-17 10:19:13.781018 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/tables.py
+-rw-r--r--   0        0        0      634 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/tasks.py
+-rw-r--r--   0        0        0     2126 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/actions.html
+-rw-r--r--   0        0        0     1345 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/delete.html
+-rw-r--r--   0        0        0      399 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/detail.html
+-rw-r--r--   0        0        0     2307 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/detail_content.html
+-rw-r--r--   0        0        0      641 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/edit.html
+-rw-r--r--   0        0        0     3295 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/issue.html
+-rw-r--r--   0        0        0     1177 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/list.html
+-rw-r--r--   0        0        0      787 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/print_form.html
+-rw-r--r--   0        0        0      292 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/short.html
+-rw-r--r--   0        0        0      203 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/status.html
+-rw-r--r--   0        0        0     1344 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/actions.html
+-rw-r--r--   0        0        0      896 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/create.html
+-rw-r--r--   0        0        0     1273 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/delete.html
+-rw-r--r--   0        0        0     1291 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/detail.html
+-rw-r--r--   0        0        0     1851 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/detail_content.html
+-rw-r--r--   0        0        0      892 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/edit.html
+-rw-r--r--   0        0        0     1276 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/instructions.html
+-rw-r--r--   0        0        0      699 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/list.html
+-rw-r--r--   0        0        0      115 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/short.html
+-rw-r--r--   0        0        0      470 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/person_status.html
+-rw-r--r--   0        0        0      385 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/picture.html
+-rw-r--r--   0        0        0     1312 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/actions.html
+-rw-r--r--   0        0        0      645 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/create.html
+-rw-r--r--   0        0        0     1303 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/delete.html
+-rw-r--r--   0        0        0     1292 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/detail.html
+-rw-r--r--   0        0        0     3776 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/detail_content.html
+-rw-r--r--   0        0        0      657 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/edit.html
+-rw-r--r--   0        0        0      706 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/list.html
+-rw-r--r--   0        0        0      317 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/short.html
+-rw-r--r--   0        0        0      228 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/status.html
+-rw-r--r--   0        0        0     1232 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html
+-rw-r--r--   0        0        0      760 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templatetags/barcode.py
+-rw-r--r--   0        0        0     2537 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/urls.py
+-rw-r--r--   0        0        0    14856 2023-07-17 10:18:52.693002 aleksis_app_kort-0.3.dev0/aleksis/apps/kort/views.py
+-rw-r--r--   0        0        0     2404 2023-07-17 10:19:19.889022 aleksis_app_kort-0.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 aleksis_app_kort-0.3.dev0/PKG-INFO
```

### Comparing `aleksis_app_kort-0.2/CHANGELOG.rst` & `aleksis_app_kort-0.3.dev0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/LICENCE.rst` & `aleksis_app_kort-0.3.dev0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/README.rst` & `aleksis_app_kort-0.3.dev0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Licence
 -------
 
 ::
 
   Copyright © 2021, 2022 Jonathan Weth <dev@jonathanweth.de>
   Copyright © 2021 Margarete Grassl <grasslma@katharineum.de>
+  Copyright © 2023 Dominik George <dominik.george@teckids.org>
 
   Licenced under the EUPL, version 1.2 or later
 
 Please see the LICENCE.rst file accompanying this distribution for the
 full licence text or on the `European Union Public Licence`_ website
 https://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers
 (including all other official language versions).
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/api.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/api.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/apps.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     copyright_info = (
         (
             [2021, 2022],
             "Jonathan Weth",
             "dev@jonathanweth.de",
         ),
         ([2021], "Margarete Grassl", "grasslma@katharineum.de"),
+        ([2023], "Dominik George", "dominik.george@teckids.org"),
     )
 
     @classmethod
     def get_all_scopes(cls) -> dict[str, str]:
         """Return all OAuth scopes and their descriptions for this app."""
         CardPrinter = apps.get_model("kort", "CardPrinter")
         label_prefix = _("Access and manage printer status and print jobs")
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/forms.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/frontend/index.js` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
 #: aleksis/apps/kort/apps.py:31
 msgid "Access and manage printer status and print jobs"
 msgstr ""
 
 #: aleksis/apps/kort/forms.py:15
 msgid "Select person(s) or group(s)"
 msgstr ""
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/locale/ru/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-19 15:48+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2023-05-26 04:37+0000\n"
+"Last-Translator: Serhii Horichenko <m@sgg.im>\n"
+"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/aleksis-app-kort/ru/>\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/kort/apps.py:31
 msgid "Access and manage printer status and print jobs"
 msgstr ""
 
 #: aleksis/apps/kort/forms.py:15
 msgid "Select person(s) or group(s)"
@@ -44,30 +45,30 @@
 
 #: aleksis/apps/kort/forms.py:23
 msgid "Select a printer to directly print the newly issued card."
 msgstr ""
 
 #: aleksis/apps/kort/forms.py:28
 msgid "Persons"
-msgstr ""
+msgstr "Люди"
 
 #: aleksis/apps/kort/forms.py:41
 msgid "Groups"
-msgstr ""
+msgstr "Группы"
 
 #: aleksis/apps/kort/forms.py:51 aleksis/apps/kort/models.py:191
 msgid "Card layout"
 msgstr ""
 
 #: aleksis/apps/kort/forms.py:53 aleksis/apps/kort/models.py:263
 #: aleksis/apps/kort/tables.py:30
 #: aleksis/apps/kort/templates/kort/card/detail_content.html:24
 #: aleksis/apps/kort/templates/kort/card/short.html:12
 msgid "Valid until"
-msgstr ""
+msgstr "Действует до"
 
 #: aleksis/apps/kort/forms.py:63
 msgid "You must select at least one person or group."
 msgstr ""
 
 #: aleksis/apps/kort/forms.py:71
 msgid "The selected groups don't have any members."
@@ -119,35 +120,35 @@
 
 #: aleksis/apps/kort/models.py:64 aleksis/apps/kort/models.py:223
 #: aleksis/apps/kort/templates/kort/card_layout/detail_content.html:11
 #: aleksis/apps/kort/templates/kort/card_layout/short.html:4
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:11
 #: aleksis/apps/kort/templates/kort/printer/short.html:4
 msgid "Name"
-msgstr ""
+msgstr "Полное имя"
 
 #: aleksis/apps/kort/models.py:65
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:24
 msgid "Description"
-msgstr ""
+msgstr "Описание"
 
 #: aleksis/apps/kort/models.py:66
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:17
 #: aleksis/apps/kort/templates/kort/printer/short.html:8
 msgid "Location"
-msgstr ""
+msgstr "Нас.пункт"
 
 #: aleksis/apps/kort/models.py:70 aleksis/apps/kort/models.py:336
 #: aleksis/apps/kort/tables.py:95
 #: aleksis/apps/kort/templates/kort/card/detail_content.html:38
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:38
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:90
 #: aleksis/apps/kort/templates/kort/printer/short.html:12
 msgid "Status"
-msgstr ""
+msgstr "Состояние"
 
 #: aleksis/apps/kort/models.py:74 aleksis/apps/kort/models.py:340
 msgid "Status text"
 msgstr ""
 
 #: aleksis/apps/kort/models.py:75 aleksis/apps/kort/tables.py:58
 #: aleksis/apps/kort/templates/kort/printer/detail_content.html:31
@@ -228,27 +229,27 @@
 msgid "Card Layouts"
 msgstr ""
 
 #: aleksis/apps/kort/models.py:260
 #: aleksis/apps/kort/templates/kort/card/detail_content.html:11
 #: aleksis/apps/kort/templates/kort/card/short.html:4
 msgid "Person"
-msgstr ""
+msgstr "Физлицо"
 
 #: aleksis/apps/kort/models.py:262
 msgid "Chip Number"
 msgstr ""
 
 #: aleksis/apps/kort/models.py:264 aleksis/apps/kort/tables.py:31
 msgid "Deactivated"
 msgstr ""
 
 #: aleksis/apps/kort/models.py:270
 msgid "PDF file"
-msgstr ""
+msgstr "Файл PDF"
 
 #: aleksis/apps/kort/models.py:303
 msgid "There is no layout provided for the card."
 msgstr ""
 
 #: aleksis/apps/kort/models.py:322 aleksis/apps/kort/models.py:331
 #: aleksis/apps/kort/templates/kort/card/detail.html:8
@@ -283,15 +284,15 @@
 #: aleksis/apps/kort/tables.py:29 aleksis/apps/kort/tables.py:57
 msgid "Current status"
 msgstr ""
 
 #: aleksis/apps/kort/tables.py:32 aleksis/apps/kort/tables.py:61
 #: aleksis/apps/kort/tables.py:85
 msgid "Actions"
-msgstr ""
+msgstr "Действия"
 
 #: aleksis/apps/kort/tables.py:54
 msgid "Printer name"
 msgstr ""
 
 #: aleksis/apps/kort/tables.py:55
 msgid "Printer location"
@@ -318,15 +319,15 @@
 msgid "Close"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/actions.html:20
 #: aleksis/apps/kort/templates/kort/card_layout/actions.html:17
 #: aleksis/apps/kort/templates/kort/printer/actions.html:17
 msgid "Show"
-msgstr ""
+msgstr "Показать"
 
 #: aleksis/apps/kort/templates/kort/card/actions.html:25
 msgid "Do you really want to deactivate the following card?"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/actions.html:35
 #: aleksis/apps/kort/templates/kort/card/actions.html:41
@@ -338,15 +339,15 @@
 #: aleksis/apps/kort/templates/kort/card_layout/actions.html:33
 #: aleksis/apps/kort/templates/kort/card_layout/delete.html:29
 #: aleksis/apps/kort/templates/kort/card_layout/detail.html:31
 #: aleksis/apps/kort/templates/kort/printer/actions.html:33
 #: aleksis/apps/kort/templates/kort/printer/delete.html:29
 #: aleksis/apps/kort/templates/kort/printer/detail.html:31
 msgid "Delete"
-msgstr ""
+msgstr "Удалить"
 
 #: aleksis/apps/kort/templates/kort/card/delete.html:8
 msgid "Delete Card"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/delete.html:12
 msgid "Do you really want to delete the following card?"
@@ -361,15 +362,15 @@
 "    "
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/delete.html:26
 #: aleksis/apps/kort/templates/kort/card_layout/delete.html:25
 #: aleksis/apps/kort/templates/kort/printer/delete.html:25
 msgid "Go back"
-msgstr ""
+msgstr "Назад"
 
 #: aleksis/apps/kort/templates/kort/card/detail_content.html:6
 msgid "Card details"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/detail_content.html:19
 msgid "not set yet"
@@ -420,15 +421,15 @@
 
 #: aleksis/apps/kort/templates/kort/card/issue.html:77
 msgid "Next step"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/issue.html:83
 msgid "Cancel"
-msgstr ""
+msgstr "Отменить"
 
 #: aleksis/apps/kort/templates/kort/card/list.html:17
 msgid "Issue new card(s)"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card/print_form.html:8
 #: aleksis/apps/kort/templates/kort/card/print_form.html:16
@@ -444,15 +445,15 @@
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card_layout/actions.html:26
 #: aleksis/apps/kort/templates/kort/card_layout/detail.html:24
 #: aleksis/apps/kort/templates/kort/printer/actions.html:27
 #: aleksis/apps/kort/templates/kort/printer/detail.html:24
 msgid "Edit"
-msgstr ""
+msgstr "Редактировать"
 
 #: aleksis/apps/kort/templates/kort/card_layout/create.html:12
 #: aleksis/apps/kort/templates/kort/card_layout/create.html:13
 msgid "Create card layout"
 msgstr ""
 
 #: aleksis/apps/kort/templates/kort/card_layout/create.html:23
@@ -655,23 +656,23 @@
 
 #: aleksis/apps/kort/views.py:232
 msgid "Progress: Generate card layout as PDF file"
 msgstr ""
 
 #: aleksis/apps/kort/views.py:233
 msgid "Generating PDF file …"
-msgstr ""
+msgstr "Создание файла PDF …"
 
 #: aleksis/apps/kort/views.py:234
 msgid "The PDF file with the card layout has been generated successfully."
 msgstr ""
 
 #: aleksis/apps/kort/views.py:235
 msgid "There was a problem while generating the PDF file."
-msgstr ""
+msgstr "Во время создания файла PDF возникла проблема."
 
 #: aleksis/apps/kort/views.py:237
 msgid "Show card"
 msgstr ""
 
 #: aleksis/apps/kort/views.py:275
 msgid "The card printer has been created successfully."
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0001_initial.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0002_card_printer.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0002_card_printer.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0003_auto_20220308_2023.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0005_card_pdf_file.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0005_card_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0006_auto_20220310_2003.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0007_auto_20220315_1957.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0008_auto_20220319_2018.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0010_auto_20220326_2123.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0012_auto_20220529_1435.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0013_auto_20220530_1939.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0014_auto_20220803_0025.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/migrations/0015_migrate_scopes.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/migrations/0015_migrate_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/models.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/models/cards.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.db.models import Q
 from django.template import Context, Template
 from django.utils import timezone
 from django.utils.translation import gettext as _
 
 from celery.result import AsyncResult
 from model_utils.models import TimeStampedModel
+from oauth2_provider.generators import generate_client_secret
 
 from aleksis.core.mixins import ExtensibleModel
 from aleksis.core.models import OAuthApplication, Person
 from aleksis.core.util.pdf import process_context_for_pdf
 
 
 class CardPrinterStatus(models.TextChoices):
@@ -78,35 +79,49 @@
         to=OAuthApplication,
         on_delete=models.CASCADE,
         verbose_name=_("OAuth2 application"),
         blank=True,
         null=True,
         related_name="card_printers",
     )
+    oauth2_client_secret = models.CharField(
+        max_length=255,
+        blank=True,
+        verbose_name=_("OAuth2 client secret"),
+    )
 
     # Settings
-    cups_printer = models.CharField(max_length=255, verbose_name=_("CUPS printer"), blank=True)
+    cups_printer = models.CharField(
+        max_length=255,
+        verbose_name=_("CUPS printer"),
+        blank=True,
+        help_text=_("Leave blank to deactivate CUPS printing"),
+    )
     generate_number_on_server = models.BooleanField(
         default=True, verbose_name=_("Generate card number on server")
     )
     card_detector = models.CharField(max_length=255, verbose_name=_("Card detector"), blank=True)
 
     def save(self, *args, **kwargs):
+        super().save(*args, **kwargs)
+
         if not self.oauth2_application:
+            client_secret = generate_client_secret()
             application = OAuthApplication(
                 client_type=OAuthApplication.CLIENT_CONFIDENTIAL,
                 authorization_grant_type=OAuthApplication.GRANT_CLIENT_CREDENTIALS,
                 name=f"Card printer: {self.name}",
-                redirect_uris="urn:ietf:wg:oauth:2.0:oob",
                 allowed_scopes=[self.scope],
+                client_secret=client_secret,
             )
             application.save()
             self.oauth2_application = application
+            self.oauth2_client_secret = client_secret
 
-        super().save(*args, **kwargs)
+            super().save(*args, **kwargs)
 
     def __str__(self):
         return self.name
 
     @property
     def status_label(self) -> str:
         """Return the verbose name of the status."""
@@ -123,15 +138,15 @@
         return CardPrinterStatus.get_icon(self.status)
 
     def generate_config(self) -> dict[str, Any]:
         """Generate the configuration for the printer client."""
         config = {
             "base_url": settings.BASE_URL,
             "client_id": self.oauth2_application.client_id,
-            "client_secret": self.oauth2_application.client_secret,
+            "client_secret": self.oauth2_client_secret,
         }
         return config
 
     @property
     def config_filename(self) -> str:
         """Return the filename for the printer client configuration."""
         return f"card-printer-config-{self.pk}.json"
@@ -259,14 +274,16 @@
     person = models.ForeignKey(
         Person, models.CASCADE, verbose_name=_("Person"), related_name="cards"
     )
     chip_number = models.CharField(verbose_name=_("Chip Number"), blank=True, max_length=255)
     valid_until = models.DateField(verbose_name=_("Valid until"))
     deactivated = models.BooleanField(verbose_name=_("Deactivated"), default=False)
 
+    last_read_counter = models.IntegerField(verbose_name=_("Last read counter"), default=0)
+
     layout = models.ForeignKey(
         CardLayout, on_delete=models.SET_NULL, blank=True, null=True, verbose_name=_("Card Layout")
     )
     pdf_file = models.FileField(
         verbose_name=_("PDF file"),
         blank=True,
         upload_to="cards/",
@@ -288,15 +305,15 @@
             "person": self.person,
             "chip_number": self.chip_number,
             "valid_until": self.valid_until,
             "media_files": self.layout.media_files.all(),
         }
 
     def generate_pdf(self) -> Union[bool, AsyncResult]:
-        from .tasks import generate_card_pdf
+        from ..tasks import generate_card_pdf
 
         if self.pdf_file:
             return True
         return generate_card_pdf.delay(self.pk)
 
     def print_card(self, printer: CardPrinter):
         if not self.layout:
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/rules.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/tables.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class CardTable(Table):
     """Table to list cards."""
 
     class Meta:
         attrs = {"class": "highlight"}
 
-    person = RelatedLinkColumn()
+    person = LinkColumn("card", verbose_name=_("Chip number"), args=[A("pk")])
     chip_number = LinkColumn("card", verbose_name=_("Chip number"), args=[A("pk")])
     current_status = Column(verbose_name=_("Current status"), accessor=A("pk"))
     valid_until = Column(verbose_name=_("Valid until"))
     deactivated = BooleanColumn(verbose_name=_("Deactivated"))
     actions = Column(verbose_name=_("Actions"), accessor=A("pk"))
 
     def render_current_status(self, value, record):
```

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/tasks.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/actions.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/delete.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/detail_content.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/edit.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/issue.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/issue.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/list.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card/print_form.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card/print_form.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/actions.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/create.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/delete.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/detail.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/detail_content.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/edit.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/instructions.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/instructions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/card_layout/list.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/card_layout/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/actions.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/create.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/delete.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/detail.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/detail_content.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/detail_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/edit.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/kort/printer/list.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/kort/printer/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templates/material/fields/django_ace_acewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/templatetags/barcode.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/templatetags/barcode.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/urls.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kort-0.2/aleksis/apps/kort/views.py` & `aleksis_app_kort-0.3.dev0/aleksis/apps/kort/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     def get(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
         self.object = self.get_object()
 
         if not self.object.chip_number:
             messages.error(request, _("The chip number is missing."))
             return redirect("cards")
 
-        redirect_url = reverse("card", args=[self.object.pk])
+        redirect_url = f"/app/kort/cards/{self.object.pk}/"
         result = self.object.generate_pdf()
 
         if result is True:
             return redirect(redirect_url)
 
         return render_progress_page(
             request,
```

### Comparing `aleksis_app_kort-0.2/PKG-INFO` & `aleksis_app_kort-0.3.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: aleksis-app-kort
-Version: 0.2
+Version: 0.3.dev0
 Summary: AlekSIS (School Information System) — App Kort (manage student IDs)
 Home-page: https://aleksis.org
-License: EUPL-1.2
+License: EUPL-1.2-or-later
 Author: Margarete Grassl
 Author-email: grasslma@katharineum.de
+Maintainer: Jonathan Weth
+Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Requires-Dist: aleksis-core (>=3.0,<4.0)
 Requires-Dist: django-ace (>=1.0.12,<2.0.0)
-Requires-Dist: django-formtools (>=2.3,<3.0)
-Requires-Dist: python-barcode (>=0.14.0,<0.15.0)
+Requires-Dist: django-formtools (==2.2)
+Requires-Dist: pylibsdm (>=1.0.0a0.dev2,<2.0.0)
+Requires-Dist: python-barcode (>=0.15.0,<0.16.0)
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding/AlekSIS-App-Kort
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Kort (manage student IDs)
 ==================================================================================================
 
 AlekSIS
@@ -38,14 +41,15 @@
 Licence
 -------
 
 ::
 
   Copyright © 2021, 2022 Jonathan Weth <dev@jonathanweth.de>
   Copyright © 2021 Margarete Grassl <grasslma@katharineum.de>
+  Copyright © 2023 Dominik George <dominik.george@teckids.org>
 
   Licenced under the EUPL, version 1.2 or later
 
 Please see the LICENCE.rst file accompanying this distribution for the
 full licence text or on the `European Union Public Licence`_ website
 https://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers
 (including all other official language versions).
```

