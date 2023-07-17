# Comparing `tmp/hyperfocus-1.0.0a2.tar.gz` & `tmp/hyperfocus-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfocus-1.0.0a2.tar", max compression
+gzip compressed data, was "hyperfocus-1.0.0b0.tar", max compression
```

## Comparing `hyperfocus-1.0.0a2.tar` & `hyperfocus-1.0.0b0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0     1646 2022-09-14 06:48:11.909343 hyperfocus-1.0.0a2/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-06-23 11:42:18.275923 hyperfocus-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     1189 2022-07-20 07:13:16.892584 hyperfocus-1.0.0a2/README.md
--rw-r--r--   0        0        0      142 2022-07-20 07:13:16.002585 hyperfocus-1.0.0a2/hyperfocus/__init__.py
--rw-r--r--   0        0        0        0 2022-07-20 07:13:14.872584 hyperfocus-1.0.0a2/hyperfocus/config/__init__.py
--rw-r--r--   0        0        0     3991 2022-09-06 07:21:55.536223 hyperfocus-1.0.0a2/hyperfocus/config/config.py
--rw-r--r--   0        0        0      152 2022-07-20 07:13:14.622584 hyperfocus-1.0.0a2/hyperfocus/config/exceptions.py
--rw-r--r--   0        0        0     1068 2022-07-20 07:13:14.942585 hyperfocus-1.0.0a2/hyperfocus/config/file.py
--rw-r--r--   0        0        0     2364 2022-09-06 06:49:46.106269 hyperfocus-1.0.0a2/hyperfocus/config/policy.py
--rw-r--r--   0        0        0        0 2022-07-28 09:20:05.005389 hyperfocus-1.0.0a2/hyperfocus/console/__init__.py
--rw-r--r--   0        0        0      836 2022-08-30 15:38:46.261098 hyperfocus-1.0.0a2/hyperfocus/console/cli.py
--rw-r--r--   0        0        0        0 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/commands/__init__.py
--rw-r--r--   0        0        0     3779 2022-09-02 07:25:35.329098 hyperfocus-1.0.0a2/hyperfocus/console/commands/_shortcodes.py
--rw-r--r--   0        0        0      765 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/commands/add.py
--rw-r--r--   0        0        0     1328 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/commands/config.py
--rw-r--r--   0        0        0      941 2022-09-02 07:23:47.269101 hyperfocus-1.0.0a2/hyperfocus/console/commands/copy.py
--rw-r--r--   0        0        0     1335 2022-09-02 07:23:56.539101 hyperfocus-1.0.0a2/hyperfocus/console/commands/delete.py
--rw-r--r--   0        0        0      602 2022-09-02 07:24:01.189101 hyperfocus-1.0.0a2/hyperfocus/console/commands/done.py
--rw-r--r--   0        0        0      939 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/commands/init.py
--rw-r--r--   0        0        0      404 2022-08-30 15:38:22.851098 hyperfocus-1.0.0a2/hyperfocus/console/commands/log.py
--rw-r--r--   0        0        0     1103 2022-09-06 07:10:27.926239 hyperfocus-1.0.0a2/hyperfocus/console/commands/main.py
--rw-r--r--   0        0        0      595 2022-09-02 07:24:08.599100 hyperfocus-1.0.0a2/hyperfocus/console/commands/reset.py
--rw-r--r--   0        0        0      674 2022-09-02 07:24:11.959100 hyperfocus-1.0.0a2/hyperfocus/console/commands/show.py
--rw-r--r--   0        0        0     3124 2022-09-02 07:28:58.589093 hyperfocus-1.0.0a2/hyperfocus/console/commands/stash.py
--rw-r--r--   0        0        0      526 2022-08-30 14:08:00.021230 hyperfocus-1.0.0a2/hyperfocus/console/commands/status.py
--rw-r--r--   0        0        0        0 2022-07-28 09:20:05.015389 hyperfocus-1.0.0a2/hyperfocus/console/core/__init__.py
--rw-r--r--   0        0        0     2290 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/core/error_handler.py
--rw-r--r--   0        0        0     2144 2022-09-06 07:14:46.336233 hyperfocus-1.0.0a2/hyperfocus/console/core/group.py
--rw-r--r--   0        0        0      882 2022-09-06 07:14:46.326233 hyperfocus-1.0.0a2/hyperfocus/console/core/hyperfocus.py
--rw-r--r--   0        0        0     1595 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/core/parameters.py
--rw-r--r--   0        0        0      173 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/console/exceptions.py
--rw-r--r--   0        0        0       75 2022-07-20 07:13:16.022585 hyperfocus-1.0.0a2/hyperfocus/database/__init__.py
--rw-r--r--   0        0        0      749 2022-09-06 07:32:54.676206 hyperfocus-1.0.0a2/hyperfocus/database/_database.py
--rw-r--r--   0        0        0      649 2022-09-01 07:38:19.445315 hyperfocus-1.0.0a2/hyperfocus/database/error_handler.py
--rw-r--r--   0        0        0      143 2022-07-20 07:13:15.122584 hyperfocus-1.0.0a2/hyperfocus/database/exceptions.py
--rw-r--r--   0        0        0     1729 2022-09-01 07:34:36.085320 hyperfocus-1.0.0a2/hyperfocus/database/models.py
--rw-r--r--   0        0        0      241 2022-09-01 06:56:03.095376 hyperfocus-1.0.0a2/hyperfocus/exceptions.py
--rw-r--r--   0        0        0      224 2022-07-20 07:13:16.432584 hyperfocus-1.0.0a2/hyperfocus/locations.py
--rw-r--r--   0        0        0        0 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/services/__init__.py
--rw-r--r--   0        0        0     4390 2022-09-01 07:28:27.335329 hyperfocus-1.0.0a2/hyperfocus/services/daily_tracker.py
--rw-r--r--   0        0        0      195 2022-08-30 14:23:15.181208 hyperfocus-1.0.0a2/hyperfocus/services/exceptions.py
--rw-r--r--   0        0        0     1318 2022-09-01 07:27:33.345331 hyperfocus-1.0.0a2/hyperfocus/services/history.py
--rw-r--r--   0        0        0     2068 2022-09-02 07:29:15.619093 hyperfocus-1.0.0a2/hyperfocus/services/session.py
--rw-r--r--   0        0        0     1953 2022-09-01 07:00:20.045370 hyperfocus-1.0.0a2/hyperfocus/services/stash_box.py
--rw-r--r--   0        0        0        0 2022-07-20 07:13:16.022585 hyperfocus-1.0.0a2/hyperfocus/termui/__init__.py
--rw-r--r--   0        0        0     5689 2022-09-01 07:37:13.555317 hyperfocus-1.0.0a2/hyperfocus/termui/components.py
--rw-r--r--   0        0        0      105 2022-07-28 09:20:05.015389 hyperfocus-1.0.0a2/hyperfocus/termui/exceptions.py
--rw-r--r--   0        0        0     1894 2022-09-01 07:37:33.805316 hyperfocus-1.0.0a2/hyperfocus/termui/formatter.py
--rw-r--r--   0        0        0      279 2022-08-31 06:53:00.399845 hyperfocus-1.0.0a2/hyperfocus/termui/icons.py
--rw-r--r--   0        0        0     7161 2022-09-01 06:56:03.265376 hyperfocus-1.0.0a2/hyperfocus/termui/markup.py
--rw-r--r--   0        0        0      839 2022-09-01 07:37:43.525316 hyperfocus-1.0.0a2/hyperfocus/termui/printer.py
--rw-r--r--   0        0        0     1028 2022-09-01 07:37:52.075316 hyperfocus-1.0.0a2/hyperfocus/termui/prompt.py
--rw-r--r--   0        0        0      282 2022-08-19 14:00:12.890399 hyperfocus-1.0.0a2/hyperfocus/termui/style.py
--rw-r--r--   0        0        0      383 2022-09-01 06:56:03.105376 hyperfocus-1.0.0a2/hyperfocus/utils.py
--rw-r--r--   0        0        0     1330 2022-09-14 06:45:03.929344 hyperfocus-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     2188 2022-09-14 06:51:59.208184 hyperfocus-1.0.0a2/setup.py
--rw-r--r--   0        0        0     2039 2022-09-14 06:51:59.208414 hyperfocus-1.0.0a2/PKG-INFO
+-rwxr-xr-x   0        0        0     1737 2023-07-17 17:33:59.871807 hyperfocus-1.0.0b0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1071 2023-02-10 16:31:14.841918 hyperfocus-1.0.0b0/LICENSE
+-rwxr-xr-x   0        0        0     1196 2023-07-16 16:38:16.319771 hyperfocus-1.0.0b0/README.md
+-rwxr-xr-x   0        0        0      142 2023-02-10 16:31:14.845259 hyperfocus-1.0.0b0/hyperfocus/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.845731 hyperfocus-1.0.0b0/hyperfocus/config/__init__.py
+-rwxr-xr-x   0        0        0     3991 2023-02-10 16:31:14.846381 hyperfocus-1.0.0b0/hyperfocus/config/config.py
+-rwxr-xr-x   0        0        0      152 2023-02-10 16:31:14.846884 hyperfocus-1.0.0b0/hyperfocus/config/exceptions.py
+-rwxr-xr-x   0        0        0     1068 2023-02-10 16:31:14.846884 hyperfocus-1.0.0b0/hyperfocus/config/file.py
+-rwxr-xr-x   0        0        0     2364 2023-02-10 16:31:14.847383 hyperfocus-1.0.0b0/hyperfocus/config/policy.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.847882 hyperfocus-1.0.0b0/hyperfocus/console/__init__.py
+-rwxr-xr-x   0        0        0      836 2023-02-10 16:31:14.848530 hyperfocus-1.0.0b0/hyperfocus/console/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.849030 hyperfocus-1.0.0b0/hyperfocus/console/commands/__init__.py
+-rwxr-xr-x   0        0        0     3779 2023-02-10 16:31:14.849546 hyperfocus-1.0.0b0/hyperfocus/console/commands/_shortcodes.py
+-rwxr-xr-x   0        0        0      765 2023-02-10 16:31:14.850046 hyperfocus-1.0.0b0/hyperfocus/console/commands/add.py
+-rwxr-xr-x   0        0        0     1328 2023-02-10 16:31:14.850712 hyperfocus-1.0.0b0/hyperfocus/console/commands/config.py
+-rwxr-xr-x   0        0        0      941 2023-02-10 16:31:14.851187 hyperfocus-1.0.0b0/hyperfocus/console/commands/copy.py
+-rwxr-xr-x   0        0        0     1335 2023-02-10 16:31:14.851843 hyperfocus-1.0.0b0/hyperfocus/console/commands/delete.py
+-rwxr-xr-x   0        0        0      602 2023-02-10 16:31:14.852593 hyperfocus-1.0.0b0/hyperfocus/console/commands/done.py
+-rwxr-xr-x   0        0        0      939 2023-02-10 16:31:14.853095 hyperfocus-1.0.0b0/hyperfocus/console/commands/init.py
+-rwxr-xr-x   0        0        0      404 2023-02-10 16:31:14.853594 hyperfocus-1.0.0b0/hyperfocus/console/commands/log.py
+-rwxr-xr-x   0        0        0     1103 2023-02-10 16:31:14.854094 hyperfocus-1.0.0b0/hyperfocus/console/commands/main.py
+-rwxr-xr-x   0        0        0      595 2023-02-10 16:31:14.854595 hyperfocus-1.0.0b0/hyperfocus/console/commands/reset.py
+-rwxr-xr-x   0        0        0      674 2023-02-10 16:31:14.855095 hyperfocus-1.0.0b0/hyperfocus/console/commands/show.py
+-rwxr-xr-x   0        0        0     3124 2023-02-10 16:31:14.855594 hyperfocus-1.0.0b0/hyperfocus/console/commands/stash.py
+-rwxr-xr-x   0        0        0      526 2023-02-10 16:31:14.856094 hyperfocus-1.0.0b0/hyperfocus/console/commands/status.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.856595 hyperfocus-1.0.0b0/hyperfocus/console/core/__init__.py
+-rwxr-xr-x   0        0        0     2290 2023-02-10 16:31:14.857096 hyperfocus-1.0.0b0/hyperfocus/console/core/error_handler.py
+-rwxr-xr-x   0        0        0     2144 2023-02-10 16:31:14.858095 hyperfocus-1.0.0b0/hyperfocus/console/core/group.py
+-rwxr-xr-x   0        0        0      882 2023-02-10 16:31:14.858594 hyperfocus-1.0.0b0/hyperfocus/console/core/hyperfocus.py
+-rwxr-xr-x   0        0        0     1595 2023-02-10 16:31:14.859515 hyperfocus-1.0.0b0/hyperfocus/console/core/parameters.py
+-rwxr-xr-x   0        0        0      173 2023-02-10 16:31:14.860017 hyperfocus-1.0.0b0/hyperfocus/console/exceptions.py
+-rwxr-xr-x   0        0        0       75 2023-02-10 16:31:14.860517 hyperfocus-1.0.0b0/hyperfocus/database/__init__.py
+-rwxr-xr-x   0        0        0      749 2023-02-10 16:31:14.861074 hyperfocus-1.0.0b0/hyperfocus/database/_database.py
+-rwxr-xr-x   0        0        0      649 2023-02-10 16:31:14.861725 hyperfocus-1.0.0b0/hyperfocus/database/error_handler.py
+-rwxr-xr-x   0        0        0      143 2023-02-10 16:31:14.862543 hyperfocus-1.0.0b0/hyperfocus/database/exceptions.py
+-rwxr-xr-x   0        0        0     1729 2023-02-10 16:31:14.862543 hyperfocus-1.0.0b0/hyperfocus/database/models.py
+-rwxr-xr-x   0        0        0      241 2023-02-10 16:31:14.862543 hyperfocus-1.0.0b0/hyperfocus/exceptions.py
+-rwxr-xr-x   0        0        0      224 2023-02-10 16:31:14.863753 hyperfocus-1.0.0b0/hyperfocus/locations.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.863753 hyperfocus-1.0.0b0/hyperfocus/services/__init__.py
+-rwxr-xr-x   0        0        0     4390 2023-02-10 16:31:14.863753 hyperfocus-1.0.0b0/hyperfocus/services/daily_tracker.py
+-rwxr-xr-x   0        0        0      195 2023-02-10 16:31:14.864906 hyperfocus-1.0.0b0/hyperfocus/services/exceptions.py
+-rwxr-xr-x   0        0        0     1327 2023-07-16 15:50:44.373335 hyperfocus-1.0.0b0/hyperfocus/services/history.py
+-rwxr-xr-x   0        0        0     2068 2023-02-10 16:31:14.865242 hyperfocus-1.0.0b0/hyperfocus/services/session.py
+-rwxr-xr-x   0        0        0     1953 2023-02-10 16:31:14.865242 hyperfocus-1.0.0b0/hyperfocus/services/stash_box.py
+-rwxr-xr-x   0        0        0        0 2023-02-10 16:31:14.866658 hyperfocus-1.0.0b0/hyperfocus/termui/__init__.py
+-rwxr-xr-x   0        0        0     5689 2023-02-10 16:31:14.866658 hyperfocus-1.0.0b0/hyperfocus/termui/components.py
+-rwxr-xr-x   0        0        0      105 2023-02-10 16:31:14.867136 hyperfocus-1.0.0b0/hyperfocus/termui/exceptions.py
+-rwxr-xr-x   0        0        0     1894 2023-02-10 16:31:14.867902 hyperfocus-1.0.0b0/hyperfocus/termui/formatter.py
+-rwxr-xr-x   0        0        0      279 2023-02-10 16:31:14.868158 hyperfocus-1.0.0b0/hyperfocus/termui/icons.py
+-rwxr-xr-x   0        0        0     7161 2023-02-10 16:31:14.868660 hyperfocus-1.0.0b0/hyperfocus/termui/markup.py
+-rwxr-xr-x   0        0        0      839 2023-02-10 16:31:14.868660 hyperfocus-1.0.0b0/hyperfocus/termui/printer.py
+-rwxr-xr-x   0        0        0     1028 2023-02-10 16:31:14.868660 hyperfocus-1.0.0b0/hyperfocus/termui/prompt.py
+-rwxr-xr-x   0        0        0      282 2023-02-10 16:31:14.869977 hyperfocus-1.0.0b0/hyperfocus/termui/style.py
+-rwxr-xr-x   0        0        0      383 2023-02-10 16:31:14.870458 hyperfocus-1.0.0b0/hyperfocus/utils.py
+-rwxr-xr-x   0        0        0     1329 2023-07-17 17:31:40.023308 hyperfocus-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 hyperfocus-1.0.0b0/PKG-INFO
```

### Comparing `hyperfocus-1.0.0a2/CHANGELOG.md` & `hyperfocus-1.0.0b0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 1.0.0-beta.0 (2023-07-17)
+
+### Fixed:
+
+* Log command must not show empty working days.
+
 ## 1.0.0-alpha.2 (2022-09-14)
 
 ### Added:
 
 * Add `-h` option for help.
 * Add `log` command to show task log history.
```

### Comparing `hyperfocus-1.0.0a2/LICENSE` & `hyperfocus-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/README.md` & `hyperfocus-1.0.0b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <a href="#readme">
         <img alt="HyperFocus logo" src="https://raw.githubusercontent.com/u8slvn/hyperfocus/main/_statics/logo.png">
     </a>
 </p>
 <p align="center">
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/v/hyperfocus.svg" alt="Pypi Version"></a>
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/pyversions/hyperfocus" alt="Python Version"></a>
-    <a href="https://github.com/u8slvn/hyperfocus/actions/workflows/ci.yml"><img src="https://img.shields.io/github/workflow/status/u8slvn/hyperfocus/CI/main" alt="CI"></a>
+    <a href="https://github.com/u8slvn/hyperfocus/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/u8slvn/hyperfocus/ci.yml" alt="CI"></a>
     <a href="https://coveralls.io/github/u8slvn/hyperfocus?branch=main"><img src="https://coveralls.io/repos/github/u8slvn/hyperfocus/badge.svg?branch=main" alt="Coverage Status"></a>
     <a href="https://app.codacy.com/gh/u8slvn/hyperfocus/dashboard"><img src="https://img.shields.io/codacy/grade/01ddd5668dbf4fc09f20ef215d0eec0b" alt="Code Quality"></a>
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/l/hyperfocus" alt="Project license"></a>
 </p>
 
 ---
```

### Comparing `hyperfocus-1.0.0a2/hyperfocus/config/config.py` & `hyperfocus-1.0.0b0/hyperfocus/config/config.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/config/file.py` & `hyperfocus-1.0.0b0/hyperfocus/config/file.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/config/policy.py` & `hyperfocus-1.0.0b0/hyperfocus/config/policy.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/cli.py` & `hyperfocus-1.0.0b0/hyperfocus/console/cli.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/_shortcodes.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/_shortcodes.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/add.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/add.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/config.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/config.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/copy.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/copy.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/delete.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/delete.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/done.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/done.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/init.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/init.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/main.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/main.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/reset.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/reset.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/show.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/show.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/stash.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/stash.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/commands/status.py` & `hyperfocus-1.0.0b0/hyperfocus/console/commands/status.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/core/error_handler.py` & `hyperfocus-1.0.0b0/hyperfocus/console/core/error_handler.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/core/group.py` & `hyperfocus-1.0.0b0/hyperfocus/console/core/group.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/core/hyperfocus.py` & `hyperfocus-1.0.0b0/hyperfocus/console/core/hyperfocus.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/console/core/parameters.py` & `hyperfocus-1.0.0b0/hyperfocus/console/core/parameters.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/database/_database.py` & `hyperfocus-1.0.0b0/hyperfocus/database/_database.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/database/error_handler.py` & `hyperfocus-1.0.0b0/hyperfocus/database/error_handler.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/database/models.py` & `hyperfocus-1.0.0b0/hyperfocus/database/models.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/services/daily_tracker.py` & `hyperfocus-1.0.0b0/hyperfocus/services/daily_tracker.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/services/history.py` & `hyperfocus-1.0.0b0/hyperfocus/services/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Generator
 
-from hyperfocus.database.models import WorkingDay
+from hyperfocus.database.models import Task, WorkingDay
 from hyperfocus.services.daily_tracker import DailyTracker
 
 
 if TYPE_CHECKING:
     import datetime
 
-    from hyperfocus.database.models import Task
-
 
 class History:
     """
     Retrieve all tasks from the past days as history log.
     """
 
     def __init__(self, daily_tracker: DailyTracker) -> None:
@@ -29,14 +27,17 @@
         query = WorkingDay.select()
         query = query.where(WorkingDay.date < self.start)
         query = query.order_by(WorkingDay.date.desc())
         previous_days = query.execute()
 
         for previous_day in previous_days:
             daily_tracker = DailyTracker(previous_day)
-            yield False, previous_day.date
-
             tasks = daily_tracker.get_tasks()
 
+            if not tasks:
+                continue
+
+            yield False, previous_day.date
+
             for i, task in enumerate(tasks):
                 last_element = i == len(tasks) - 1
                 yield last_element, task
```

### Comparing `hyperfocus-1.0.0a2/hyperfocus/services/session.py` & `hyperfocus-1.0.0b0/hyperfocus/services/session.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/services/stash_box.py` & `hyperfocus-1.0.0b0/hyperfocus/services/stash_box.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/termui/components.py` & `hyperfocus-1.0.0b0/hyperfocus/termui/components.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/termui/formatter.py` & `hyperfocus-1.0.0b0/hyperfocus/termui/formatter.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/termui/markup.py` & `hyperfocus-1.0.0b0/hyperfocus/termui/markup.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/termui/printer.py` & `hyperfocus-1.0.0b0/hyperfocus/termui/printer.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/hyperfocus/termui/prompt.py` & `hyperfocus-1.0.0b0/hyperfocus/termui/prompt.py`

 * *Files identical despite different names*

### Comparing `hyperfocus-1.0.0a2/pyproject.toml` & `hyperfocus-1.0.0b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfocus"
-version = "1.0.0-alpha.2"
+version = "1.0.0-beta.0"
 description = "Minimalist daily task manager."
 authors = ["u8slvn <u8slvn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/u8slvn/hyperfocus"
 homepage = "https://github.com/u8slvn/hyperfocus"
 keywords = [
```

### Comparing `hyperfocus-1.0.0a2/PKG-INFO` & `hyperfocus-1.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hyperfocus
-Version: 1.0.0a2
+Version: 1.0.0b0
 Summary: Minimalist daily task manager.
 Home-page: https://github.com/u8slvn/hyperfocus
 License: MIT
 Keywords: cli,todo,todolist,todo-list,task-list,productivity
 Author: u8slvn
 Author-email: u8slvn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: peewee (>=3.15.1,<4.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Project-URL: Changelog, https://github.com/u8slvn/hyperfocus/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/u8slvn/hyperfocus
 Description-Content-Type: text/markdown
 
@@ -24,15 +25,15 @@
     <a href="#readme">
         <img alt="HyperFocus logo" src="https://raw.githubusercontent.com/u8slvn/hyperfocus/main/_statics/logo.png">
     </a>
 </p>
 <p align="center">
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/v/hyperfocus.svg" alt="Pypi Version"></a>
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/pyversions/hyperfocus" alt="Python Version"></a>
-    <a href="https://github.com/u8slvn/hyperfocus/actions/workflows/ci.yml"><img src="https://img.shields.io/github/workflow/status/u8slvn/hyperfocus/CI/main" alt="CI"></a>
+    <a href="https://github.com/u8slvn/hyperfocus/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/u8slvn/hyperfocus/ci.yml" alt="CI"></a>
     <a href="https://coveralls.io/github/u8slvn/hyperfocus?branch=main"><img src="https://coveralls.io/repos/github/u8slvn/hyperfocus/badge.svg?branch=main" alt="Coverage Status"></a>
     <a href="https://app.codacy.com/gh/u8slvn/hyperfocus/dashboard"><img src="https://img.shields.io/codacy/grade/01ddd5668dbf4fc09f20ef215d0eec0b" alt="Code Quality"></a>
     <a href="https://pypi.org/project/hyperfocus/"><img src="https://img.shields.io/pypi/l/hyperfocus" alt="Project license"></a>
 </p>
 
 ---
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: hyperfocus Version: 1.0.0a2 Summary: Minimalist
+Metadata-Version: 2.1 Name: hyperfocus Version: 1.0.0b0 Summary: Minimalist
 daily task manager. Home-page: https://github.com/u8slvn/hyperfocus License:
 MIT Keywords: cli,todo,todolist,todo-list,task-list,productivity Author: u8slvn
 Author-email: u8slvn@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: peewee (>=3.15.1,<4.0.0)
-Requires-Dist: pyperclip (>=1.8.2,<2.0.0) Project-URL: Changelog, https://
-github.com/u8slvn/hyperfocus/blob/main/CHANGELOG.md Project-URL: Repository,
-https://github.com/u8slvn/hyperfocus Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: peewee (>=3.15.1,<4.0.0) Requires-Dist:
+pyperclip (>=1.8.2,<2.0.0) Project-URL: Changelog, https://github.com/u8slvn/
+hyperfocus/blob/main/CHANGELOG.md Project-URL: Repository, https://github.com/
+u8slvn/hyperfocus Description-Content-Type: text/markdown
                                [HyperFocus_logo]
 [Pypi_Version] [Python_Version] [CI] [Coverage_Status] [Code_Quality] [Project
                                    license]
 --- ```shell $ pipx install hyperfocus --pip-args="--pre" ```
```

