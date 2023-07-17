# Comparing `tmp/odoo-configurator-3.0.0.tar.gz` & `tmp/odoo-configurator-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-configurator-3.0.0.tar", last modified: Mon Jul 17 13:40:57 2023, max compression
+gzip compressed data, was "odoo-configurator-3.0.1.tar", last modified: Mon Jul 17 18:44:57 2023, max compression
```

## Comparing `odoo-configurator-3.0.0.tar` & `odoo-configurator-3.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     7652 2023-01-26 16:07:11.000000 odoo-configurator-3.0.0/LICENCE
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       69 2023-07-17 10:53:28.000000 odoo-configurator-3.0.0/MANIFEST.in
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     7183 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/PKG-INFO
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     6552 2023-07-17 13:31:27.000000 odoo-configurator-3.0.0/README.md
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     1066 2023-07-17 13:39:36.000000 odoo-configurator-3.0.0/pyproject.toml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     1467 2023-07-17 08:45:12.000000 odoo-configurator-3.0.0/requirements.txt
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       38 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/setup.cfg
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.692376 odoo-configurator-3.0.0/src/
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.692376 odoo-configurator-3.0.0/src/odoo_configurator/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      208 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/__init__.py
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     1080 2023-07-17 08:53:03.000000 odoo-configurator-3.0.0/src/odoo_configurator/__main__.py
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/src/odoo_configurator/apps/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      562 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/__init__.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     7008 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/account.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     5058 2023-04-04 15:58:31.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/base.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     2079 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/call.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     2649 2023-04-05 15:04:35.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/config.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)      293 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/connection.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)    10062 2023-03-29 15:23:19.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/datas.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1439 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/defaults.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     7236 2023-07-17 08:27:51.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/import_configurator.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     2238 2023-06-14 07:42:15.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/imports.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1519 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/mattermost.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     5425 2023-04-24 15:17:32.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/modules.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1940 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/roles.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1780 2023-02-14 10:19:48.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/translations.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1312 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/users.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)      513 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/apps/website.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     6808 2023-07-17 11:15:53.000000 odoo-configurator-3.0.0/src/odoo_configurator/configurator.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     8694 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/import_manager.py
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      497 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/logging.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     8821 2023-06-14 07:43:13.000000 odoo-configurator-3.0.0/src/odoo_configurator/odoo_connection.py
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     2211 2023-01-26 16:01:21.000000 odoo-configurator-3.0.0/src/odoo_configurator/password_manager.py
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.692376 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     7183 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/PKG-INFO
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     1897 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/SOURCES.txt
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)        1 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/dependency_links.txt
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       70 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/entry_points.txt
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      111 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/requires.txt
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       28 2023-07-17 13:40:57.000000 odoo-configurator-3.0.0/src/odoo_configurator.egg-info/top_level.txt
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/src/templates/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      429 2023-01-26 16:05:11.000000 odoo-configurator-3.0.0/src/templates/0_base.yml
-drwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)        0 2023-07-17 13:40:57.696376 odoo-configurator-3.0.0/src/templates/14.0/
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      113 2023-01-26 16:04:08.000000 odoo-configurator-3.0.0/src/templates/14.0/0_base.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     3245 2020-06-10 08:22:02.000000 odoo-configurator-3.0.0/src/templates/1_base_auto_entreprise.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       37 2020-06-10 08:22:02.000000 odoo-configurator-3.0.0/src/templates/1_base_entreprise.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      753 2023-02-28 09:13:02.000000 odoo-configurator-3.0.0/src/templates/2_base_account.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      827 2023-01-26 16:05:11.000000 odoo-configurator-3.0.0/src/templates/2_base_account_14.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      171 2020-10-08 14:39:36.000000 odoo-configurator-3.0.0/src/templates/2_base_account_entreprise.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       39 2020-11-26 09:38:01.000000 odoo-configurator-3.0.0/src/templates/2_base_crm.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      123 2021-06-16 14:12:49.000000 odoo-configurator-3.0.0/src/templates/2_base_event.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       41 2022-11-15 14:59:54.000000 odoo-configurator-3.0.0/src/templates/2_base_expense.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       47 2021-05-19 07:06:22.000000 odoo-configurator-3.0.0/src/templates/2_base_ged.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       40 2023-02-28 09:13:02.000000 odoo-configurator-3.0.0/src/templates/2_base_hr.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       75 2023-02-28 09:13:02.000000 odoo-configurator-3.0.0/src/templates/2_base_maintenance.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       57 2020-11-26 09:38:01.000000 odoo-configurator-3.0.0/src/templates/2_base_marketing.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       35 2020-06-10 10:38:22.000000 odoo-configurator-3.0.0/src/templates/2_base_mrp.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      345 2021-10-25 13:35:17.000000 odoo-configurator-3.0.0/src/templates/2_base_purchase.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)     1296 2023-04-05 15:29:16.000000 odoo-configurator-3.0.0/src/templates/2_base_sale.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       52 2020-09-10 14:44:32.000000 odoo-configurator-3.0.0/src/templates/2_base_sale_subscription.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)       42 2023-01-12 08:58:27.000000 odoo-configurator-3.0.0/src/templates/2_base_sign.yml
--rw-rw-r--   0 mperrocheau  (1000) mperrocheau  (1000)      201 2023-01-12 08:58:27.000000 odoo-configurator-3.0.0/src/templates/2_base_website.yml
--rwxrwxr-x   0 mperrocheau  (1000) mperrocheau  (1000)     1063 2023-07-17 08:27:51.000000 odoo-configurator-3.0.0/start_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.266245 odoo-configurator-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.270245 odoo-configurator-3.0.1/src/odoo_configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.278245 odoo-configurator-3.0.1/src/odoo_configurator/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5058 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/call.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10062 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/datas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7236 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/import_configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/mattermost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1312 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/website.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6763 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8694 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/import_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8821 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/odoo_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/password_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.270245 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.282245 odoo-configurator-3.0.1/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/0_base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.282245 odoo-configurator-3.0.1/src/templates/14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/14.0/0_base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/1_base_auto_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/1_base_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account_14.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_crm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_event.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_expense.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_ged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_hr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_maintenance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_marketing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_mrp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_purchase.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sale_subscription.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_website.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/start_config.py
```

### Comparing `odoo-configurator-3.0.0/LICENCE` & `odoo-configurator-3.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/PKG-INFO` & `odoo-configurator-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.0.0
+Version: 3.0.1
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 Project-URL: Homepage, https://github.com/TeclibERP/odoo-configurator
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 odoo-configurator
 =================
 
 Update Odoo database with YAML files
 
 ## Installation
-    sudo pip install odoo-configurator
+    pip install odoo-configurator
 
 ## Usage
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
```

### Comparing `odoo-configurator-3.0.0/README.md` & `odoo-configurator-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 odoo-configurator
 =================
 
 Update Odoo database with YAML files
 
 ## Installation
-    sudo pip install odoo-configurator
+    pip install odoo-configurator
 
 ## Usage
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
```

### Comparing `odoo-configurator-3.0.0/pyproject.toml` & `odoo-configurator-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "odoo-configurator"
-version = "3.0.0"
+version = "3.0.1"
 description = "Configure and update Odoo database with YAML files"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "myrrkel@gmail.com" },
 { name = "David Halgand", email = "david@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

### Comparing `odoo-configurator-3.0.0/requirements.txt` & `odoo-configurator-3.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/__main__.py` & `odoo-configurator-3.0.1/src/odoo_configurator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (C) 2023 - Teclib'ERP (<https://www.teclib-erp.com>).
 # License LGPL-3.0 or later (https://www.gnu.org/licenses/lgpl.html).
 
 from .configurator import Configurator
 import argparse
 
+
 def main():
     parser = argparse.ArgumentParser(description='Odoo Configurator')
     parser.add_argument('files', metavar='files', type=open, nargs='+', help='Config Files To load')
     parser.add_argument('--update', action='store_true', help='Update Mode')
     parser.add_argument('--install', action='store_true', help='Install Mode')
     parser.add_argument('--debug', action='store_true', help='Debug log')
     parser.add_argument('--debug_xmlrpc', action='store_true', help='Debug log xmlrpc')
```

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/__init__.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/account.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/account.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/base.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/base.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/call.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/call.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/config.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/config.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/datas.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/datas.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/defaults.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/defaults.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/import_configurator.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/import_configurator.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/imports.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/imports.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/mattermost.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/mattermost.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/modules.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/modules.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/roles.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/roles.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/translations.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/translations.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/users.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/users.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/apps/website.py` & `odoo-configurator-3.0.1/src/odoo_configurator/apps/website.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/configurator.py` & `odoo-configurator-3.0.1/src/odoo_configurator/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 logger = get_logger(__name__)
 
 
 class Configurator:
     mode = ["config"]
     debug = False
 
-    def __init__(self, paths, install, update, debug, debug_xmlrpc, keepass):
+    def __init__(self, paths, install=False, update=False, debug=False, debug_xmlrpc=False, keepass=''):
         self.password_manager = PasswordManager(keepass)
         self.paths = paths
         self.configurator_dir = os.path.dirname(sys.argv[0])
         if install:
             self.mode.append('install')
         if update:
             self.mode.append('update')
@@ -83,15 +83,14 @@
             pre_update_config = hiyapyco.load(config_files, method=hiyapyco.METHOD_MERGE, interpolate=True,
                                               failonmissingfiles=True, loglevel='INFO')
             pre_update_config['auth'] = parsed_config['auth']
 
         while len(parsed_config.get("inherits", [])) != count_inherit:
             count_inherit = len(parsed_config.get("inherits", []))
             config_files = self.paths + self.get_files_path(parsed_config['inherits']) + self.paths
-            logger.info("Configurator path %s" % self.configurator_dir)
             logger.info("Configuration Loading %s" % (",".join(config_files)))
             parsed_config = hiyapyco.load(config_files, method=hiyapyco.METHOD_MERGE, interpolate=True,
                                           failonmissingfiles=True, loglevel='INFO')
 
         parsed_config['scripts'] = []
         count_script = 0
         while len(parsed_config.get("script_files", [])) != count_script:
```

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/import_manager.py` & `odoo-configurator-3.0.1/src/odoo_configurator/import_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/odoo_connection.py` & `odoo-configurator-3.0.1/src/odoo_configurator/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator/password_manager.py` & `odoo-configurator-3.0.1/src/odoo_configurator/password_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator.egg-info/PKG-INFO` & `odoo-configurator-3.0.1/src/odoo_configurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.0.0
+Version: 3.0.1
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 Project-URL: Homepage, https://github.com/TeclibERP/odoo-configurator
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 odoo-configurator
 =================
 
 Update Odoo database with YAML files
 
 ## Installation
-    sudo pip install odoo-configurator
+    pip install odoo-configurator
 
 ## Usage
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
```

### Comparing `odoo-configurator-3.0.0/src/odoo_configurator.egg-info/SOURCES.txt` & `odoo-configurator-3.0.1/src/odoo_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/templates/1_base_auto_entreprise.yml` & `odoo-configurator-3.0.1/src/templates/1_base_auto_entreprise.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/templates/2_base_account.yml` & `odoo-configurator-3.0.1/src/templates/2_base_account.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/templates/2_base_account_14.yml` & `odoo-configurator-3.0.1/src/templates/2_base_account_14.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.0/src/templates/2_base_sale.yml` & `odoo-configurator-3.0.1/src/templates/2_base_sale.yml`

 * *Files identical despite different names*

