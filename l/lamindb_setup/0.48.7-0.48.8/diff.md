# Comparing `tmp/lamindb_setup-0.48.7.tar.gz` & `tmp/lamindb_setup-0.48.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.48.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.48.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.48.7.tar` & `lamindb_setup-0.48.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.7/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.7/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.7/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.7/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.7/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.7/README.md
--rw-r--r--   0        0        0    57445 2023-07-09 13:07:46.437615 lamindb_setup-0.48.7/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.7/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.48.7/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.48.7/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.7/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.7/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7799 2023-07-03 19:06:33.504770 lamindb_setup-0.48.7/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4418 2023-06-20 11:14:24.334197 lamindb_setup-0.48.7/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.7/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.48.7/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.7/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.7/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.7/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.7/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.7/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.7/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.7/lamin-project.yaml
--rw-r--r--   0        0        0     2757 2023-07-09 13:13:48.778611 lamindb_setup-0.48.7/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.7/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.48.7/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.48.7/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.7/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.7/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.7/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7408 2023-07-06 11:52:01.583053 lamindb_setup-0.48.7/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6628 2023-07-07 06:20:33.983236 lamindb_setup-0.48.7/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1413 2023-07-03 19:06:33.505992 lamindb_setup-0.48.7/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.48.7/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.7/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.7/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.7/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.7/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.7/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.7/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.7/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.48.7/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.7/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.48.7/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.7/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.48.7/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.7/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.7/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.7/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.7/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.7/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9365 2023-06-28 12:32:26.045930 lamindb_setup-0.48.7/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.7/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.7/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.7/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.7/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.7/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.7/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.48.7/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.7/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.7/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.7/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.7/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.7/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.7/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.7/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.7/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.7/lnschema-core/README.md
--rw-r--r--   0        0        0      617 2023-06-30 11:14:16.252662 lamindb_setup-0.48.7/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.7/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.7/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.7/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.7/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.7/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.7/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.7/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.7/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.7/noxfile.py
--rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.7/pyproject.toml
--rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.7/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.7/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.7/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.7/tests/test_bionty.py
--rw-r--r--   0        0        0     3102 2023-07-03 19:06:33.506273 lamindb_setup-0.48.7/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.7/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.7/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-03 19:06:33.506543 lamindb_setup-0.48.7/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.7/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.7/tests/test_signup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.7/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.8/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.8/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.8/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.8/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.8/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.8/README.md
+-rw-r--r--   0        0        0    57606 2023-07-17 14:59:34.334852 lamindb_setup-0.48.8/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.8/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.48.8/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.48.8/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.8/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.8/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.48.8/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.48.8/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.8/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.48.8/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.8/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.8/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.8/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.8/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.8/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.8/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.8/lamin-project.yaml
+-rw-r--r--   0        0        0     2757 2023-07-17 14:59:23.981072 lamindb_setup-0.48.8/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.8/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.48.8/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.48.8/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.8/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.8/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.8/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.48.8/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6599 2023-07-17 14:58:45.055228 lamindb_setup-0.48.8/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1413 2023-07-03 19:06:33.505992 lamindb_setup-0.48.8/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.48.8/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.8/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.8/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.8/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.8/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.8/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.8/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.8/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.48.8/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.8/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.48.8/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.8/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.48.8/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.8/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.8/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.8/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4583 2023-07-17 14:58:45.055809 lamindb_setup-0.48.8/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.8/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.8/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.8/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.8/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.8/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.8/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.8/lnschema-core/README.md
+-rw-r--r--   0        0        0      617 2023-06-30 11:14:16.252662 lamindb_setup-0.48.8/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.8/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.8/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.8/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.8/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.8/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.8/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.8/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.8/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.8/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.8/pyproject.toml
+-rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.8/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.8/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.8/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.8/tests/test_bionty.py
+-rw-r--r--   0        0        0     2974 2023-07-17 14:58:45.056044 lamindb_setup-0.48.8/tests/test_init_instance.py
+-rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.8/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.8/tests/test_login.py
+-rw-r--r--   0        0        0      457 2023-07-03 19:06:33.506543 lamindb_setup-0.48.8/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.8/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.8/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.8/PKG-INFO
```

### Comparing `lamindb_setup-0.48.7/.github/workflows/build.yml` & `lamindb_setup-0.48.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.8/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/.gitignore` & `lamindb_setup-0.48.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/.pre-commit-config.yaml` & `lamindb_setup-0.48.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/LICENSE` & `lamindb_setup-0.48.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/changelog.md` & `lamindb_setup-0.48.8/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Simplify `StorageSettings` | [439](https://github.com/laminlabs/lamindb-setup/pull/439) | [falexwolf](https://github.com/falexwolf) | 2023-07-17 | 0.48.8
 🔒️ Increase locker expiration time to 1 week | [437](https://github.com/laminlabs/lamindb-setup/pull/437) | [Koncopd](https://github.com/Koncopd) | 2023-07-08 | 0.48.7
 🚸 Import order of schema modules shouldn't matter | [436](https://github.com/laminlabs/lamindb-setup/pull/436) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.6
 🚸 Deal with legacy instances | [435](https://github.com/laminlabs/lamindb-setup/pull/435) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.5
 🚸 Raise more errors in API when instance is setup | [434](https://github.com/laminlabs/lamindb-setup/pull/434) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.48.3
 🚸 Silence loggers and close instance during init & load | [433](https://github.com/laminlabs/lamindb-setup/pull/433) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.48.2
 🐛 Fix sqlite file not existing in the bucket error | [432](https://github.com/laminlabs/lamindb-setup/pull/432) | [Koncopd](https://github.com/Koncopd) | 2023-06-28 | 0.48.1
 🩹 Do not register storage through `set.storage` on the hub | [430](https://github.com/laminlabs/lamindb-setup/pull/430) | [falexwolf](https://github.com/falexwolf) | 2023-06-28 |
```

### Comparing `lamindb_setup-0.48.7/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.48.8/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/faq/multi-session.ipynb` & `lamindb_setup-0.48.8/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.48.8/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.48.8/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.48.8/docs/guide/01-init-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999693627450981%*

 * *Differences: {"'cells'": "{9: {'source': {delete: [6]}}}"}*

```diff
@@ -94,15 +94,14 @@
             "source": [
                 "from pathlib import Path\n",
                 "\n",
                 "assert ln_setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle\n",
                 "assert ln_setup.settings.instance.name == \"mydata\"\n",
                 "assert ln_setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
-                "assert ln_setup.settings.storage.cache_dir is None\n",
                 "assert ln_setup.settings.storage.id is not None\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.db\n",
                 "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
                 ")"
             ]
         },
```

### Comparing `lamindb_setup-0.48.7/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.48.8/docs/guide/02-load-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999465811965812%*

 * *Differences: {"'cells'": "{7: {'source': {delete: [8]}}}"}*

```diff
@@ -97,15 +97,14 @@
                 "\n",
                 "assert ln_setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln_setup.settings.instance.name == \"mydata\"\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
                 ")\n",
-                "assert ln_setup.settings.instance.storage.cache_dir is None\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.db\n",
                 "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
                 ")"
             ]
         },
         {
```

### Comparing `lamindb_setup-0.48.7/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.48.8/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.48.8/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/docs/guide/setup-user.md` & `lamindb_setup-0.48.8/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/__init__.py` & `lamindb_setup-0.48.8/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.48.7"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.48.8"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.48.7/lamindb_setup/__main__.py` & `lamindb_setup-0.48.8/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.48.8/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_close.py` & `lamindb_setup-0.48.8/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_delete.py` & `lamindb_setup-0.48.8/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_docstrings.py` & `lamindb_setup-0.48.8/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_init_instance.py` & `lamindb_setup-0.48.8/lamindb_setup/_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,44 +11,50 @@
 from ._close import close as close_instance
 from ._docstrings import instance_description as description
 from ._settings import settings
 from ._silence_loggers import silence_loggers
 from .dev import InstanceSettings
 from .dev._docs import doc_args
 from .dev._setup_schema import get_schema_module_name, load_schema
-from .dev._storage import Storage
+from .dev._storage import StorageSettings
+
+
+def register_storage(ssettings: StorageSettings):
+    from lnschema_core.models import Storage
+
+    storage, created = Storage.objects.update_or_create(
+        root=ssettings.root_as_str,
+        defaults=dict(
+            root=ssettings.root_as_str,
+            type=ssettings.type,
+            region=ssettings.region,
+            created_by_id=settings.user.id,
+        ),
+    )
+    if created:
+        logger.success(f"Saved: {storage}")
 
 
 def register_user_and_storage(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
-    from lnschema_core.models import Storage, User
+    from lnschema_core.models import User
 
     try:
         user, created = User.objects.update_or_create(
             id=usettings.id,
             defaults=dict(
                 handle=usettings.handle,
                 name=usettings.name,
                 email=usettings.email,
             ),
         )
         if created:
             logger.success(f"Saved: {user}")
-        storage, created = Storage.objects.update_or_create(
-            root=isettings.storage.root_as_str,
-            defaults=dict(
-                root=isettings.storage.root_as_str,
-                type=isettings.storage.type,
-                region=isettings.storage.region,
-                created_by_id=usettings.id,
-            ),
-        )
-        if created:
-            logger.success(f"Saved: {storage}")
+        register_storage(isettings.storage)
     except OperationalError as error:
         logger.warning(f"Instance seems not set up ({error})")
 
 
 def reload_schema_modules(isettings: InstanceSettings):
     schema_names = ["core"] + list(isettings.schema)
     schema_module_names = [get_schema_module_name(n) for n in schema_names]
@@ -228,15 +234,15 @@
     if name is not None:
         return name
     if db is not None:
         # better way of accessing the database name?
         return str(db).split("/")[-1]
 
     if isinstance(storage, str):
-        storage_path = Storage._str_to_path(storage)
+        storage_path = StorageSettings._str_to_path(storage)
     else:
         storage_path = storage
 
     if isinstance(storage_path, UPath):
         name = storage_path._url.netloc
     else:
         name = str(storage_path.stem)
```

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_load_instance.py` & `lamindb_setup-0.48.8/lamindb_setup/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         name = identifier
     return owner, name
 
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
-    ssettings = StorageSettings(storage, instance_settings=isettings)
+    ssettings = StorageSettings(storage)
     if ssettings.is_cloud:
         try:  # triggering ssettings.id makes a lookup in the storage table
             logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
         except RuntimeError:
             raise RuntimeError(
                 "Storage not registered!\n"
                 "Load instance without the `storage` arg and register storage root: "
```

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_migrate.py` & `lamindb_setup-0.48.8/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_notebook.py` & `lamindb_setup-0.48.8/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_register_instance.py` & `lamindb_setup-0.48.8/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_schema.py` & `lamindb_setup-0.48.8/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_set.py` & `lamindb_setup-0.48.8/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_settings.py` & `lamindb_setup-0.48.8/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_setup_user.py` & `lamindb_setup-0.48.8/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.48.8/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_django.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         storage_region: Optional[str] = None,
         db: Optional[str] = None,  # DB URI
         schema: Optional[str] = None,  # comma-separated string of schema names
     ):
         self._owner: str = owner
         self._name: str = name
         self._storage: StorageSettings = StorageSettings(
-            storage_root, instance_settings=self, region=storage_region
+            storage_root, region=storage_region
         )
         self._db: Optional[str] = db
         self._schema_str: Optional[str] = schema
 
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current instance: {self.identifier}"
```

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,31 @@
 
 DIRS = AppDirs("lamindb", "laminlabs")
 
 
 class StorageSettings:
     """Manage cloud or local storage settings."""
 
-    # we can't type instance_settings if we keep it in this separate file
     def __init__(
         self,
         root: Union[str, Path, UPath],
-        instance_settings,
         region: Optional[str] = None,
     ):
         if isinstance(root, UPath):
             root_path = root
         elif isinstance(root, Path):
             root.mkdir(parents=True, exist_ok=True)  # resolve fails for nonexisting dir
             root_path = root.resolve()
         elif isinstance(root, str):
             root_path = Storage._str_to_path(root)
         else:
             raise ValueError("root should be of type Union[str, Path, UPath].")
         self._root = root_path
         self._region = region
         self._id: Optional[str] = None
-        self._instance_settings = instance_settings
 
     @staticmethod
     def _str_to_path(storage: str) -> Union[Path, UPath]:
         if storage.startswith("s3://"):
             # for new buckets there could be problems if the region is not specified
             storage_root = UPath(storage, cache_regions=True)
         elif storage.startswith("gs://"):
@@ -75,21 +72,18 @@
     def root_as_str(self) -> str:
         """Formatted root string."""
         return self.root.as_posix().rstrip("/")
 
     @property
     def cache_dir(
         self,
-    ) -> Union[Path, None]:
+    ) -> Path:
         """Cache root, a local directory to cache cloud files."""
-        if self.is_cloud:
-            cache_dir = Path(DIRS.user_cache_dir)
-            cache_dir.mkdir(parents=True, exist_ok=True)
-        else:
-            cache_dir = None
+        cache_dir = Path(DIRS.user_cache_dir)
+        cache_dir.mkdir(parents=True, exist_ok=True)
         return cache_dir
 
     @property
     def is_cloud(self) -> bool:
         """`True` if `storage_root` is in cloud, `False` otherwise."""
         return isinstance(self.root, UPath)
 
@@ -126,15 +120,15 @@
 
     # conversion to Path via cloud_to_local() would trigger download
     # of remote file to cache if there already is one
     # in pure write operations that update the cloud, we don't want this
     # hence, we manually construct the local file path
     # using the `.parts` attribute in the following line
     def cloud_to_local_no_update(self, filepath: Union[Path, UPath]) -> Path:
-        if self.is_cloud:
+        if isinstance(filepath, UPath):
             return self.cache_dir.joinpath(filepath._url.netloc, *filepath.parts[1:])  # type: ignore # noqa
         return filepath
 
     def local_filepath(self, filekey: Union[Path, UPath, str]) -> Path:
         """Local (cache) filepath from filekey: `local(filepath(...))`."""
         return self.cloud_to_local(self.key_to_filepath(filekey))
```

### Comparing `lamindb_setup-0.48.7/lamindb_setup/dev/upath.py` & `lamindb_setup-0.48.8/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.48.8/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/.gitignore` & `lamindb_setup-0.48.8/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.48.8/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.48.8/lnschema-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/LICENSE` & `lamindb_setup-0.48.8/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.48.8/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/lnschema-core/pyproject.toml` & `lamindb_setup-0.48.8/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/noxfile.py` & `lamindb_setup-0.48.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/pyproject.toml` & `lamindb_setup-0.48.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/tests/hub/test_instance.py` & `lamindb_setup-0.48.8/tests/hub/test_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/tests/hub/test_storage.py` & `lamindb_setup-0.48.8/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/tests/test_init_instance.py` & `lamindb_setup-0.48.8/tests/test_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,28 @@
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "postgresql"
     assert ln_setup.settings.instance.db == pgurl
     assert (
         ln_setup.settings.instance.storage.root.as_posix()
         == Path("mydatapg").absolute().as_posix()
     )
-    assert ln_setup.settings.instance.storage.cache_dir is None
     ln_setup.delete("pgtest")
 
 
 def test_init_instance_postgres_custom_name():
     ln_setup.init(storage="./mystorage", name="mydata2", db=pgurl, _test=True)
     assert ln_setup.settings.instance.name == "mydata2"
     assert not ln_setup.settings.instance.storage.is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "postgresql"
     assert ln_setup.settings.instance.db == pgurl
     assert (
         ln_setup.settings.instance.storage.root.as_posix()
         == Path("mystorage").absolute().as_posix()
     )
-    assert ln_setup.settings.instance.storage.cache_dir is None
     ln_setup.delete("mydata2")
 
 
 def test_init_instance_postgres_cloud_aws_us():
     ln_setup.init(storage="s3://lndb-setup-ci", _test=True)
     assert ln_setup.settings.storage.is_cloud
     assert str(ln_setup.settings.storage.root) == "s3://lndb-setup-ci/"
```

### Comparing `lamindb_setup-0.48.7/tests/test_load_instance.py` & `lamindb_setup-0.48.8/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.7/PKG-INFO` & `lamindb_setup-0.48.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.48.7
+Version: 0.48.8
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
```

