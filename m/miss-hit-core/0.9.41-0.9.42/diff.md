# Comparing `tmp/miss_hit_core-0.9.41.tar.gz` & `tmp/miss_hit_core-0.9.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miss_hit_core-0.9.41.tar", last modified: Fri May 26 10:11:38 2023, max compression
+gzip compressed data, was "miss_hit_core-0.9.42.tar", last modified: Mon Jul 17 08:47:04 2023, max compression
```

## Comparing `miss_hit_core-0.9.41.tar` & `miss_hit_core-0.9.42.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-26 10:11:38.884103 miss_hit_core-0.9.41/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.41/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.41/LICENSE.AGPL
--rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-05-26 10:11:38.884103 miss_hit_core-0.9.41/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     6162 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-26 10:11:38.880103 miss_hit_core-0.9.41/miss_hit_core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.41/miss_hit_core/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.41/miss_hit_core/cfg_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21634 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/cfg_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.41/miss_hit_core/cfg_tree.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18768 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/command_line.py
--rw-r--r--   0 florian   (1000) florian   (1000)    19019 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/config.py
--rw-r--r--   0 florian   (1000) florian   (1000)    28905 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)   112073 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/m_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.41/miss_hit_core/m_entity_root.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.41/miss_hit_core/m_language.py
--rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.41/miss_hit_core/m_language_builtins.py
--rw-r--r--   0 florian   (1000) florian   (1000)    63636 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/m_lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.41/miss_hit_core/m_parse_utils.py
--rw-r--r--   0 florian   (1000) florian   (1000)    81645 2023-05-26 10:11:20.000000 miss_hit_core-0.9.41/miss_hit_core/m_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.41/miss_hit_core/m_types.py
--rw-r--r--   0 florian   (1000) florian   (1000)    43130 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/mh_metric.py
--rw-r--r--   0 florian   (1000) florian   (1000)    52197 2023-05-19 08:46:33.000000 miss_hit_core-0.9.41/miss_hit_core/mh_style.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.41/miss_hit_core/pathutil.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-26 10:11:38.880103 miss_hit_core-0.9.41/miss_hit_core/resources/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-26 10:11:38.884103 miss_hit_core-0.9.41/miss_hit_core/resources/assets/
--rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/alert-triangle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/bar-chart-2.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/check-square.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/download.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/edit.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/external-link.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/file-text.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/help-circle.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/package.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/settings.svg
--rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/assets/terminal.svg
--rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core/resources/style.css
--rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.41/miss_hit_core/resources.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10267 2023-05-16 12:34:12.000000 miss_hit_core-0.9.41/miss_hit_core/s_ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)    24582 2023-05-26 08:33:33.000000 miss_hit_core-0.9.41/miss_hit_core/s_parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-05-26 10:11:27.000000 miss_hit_core-0.9.41/miss_hit_core/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8074 2023-03-23 13:17:08.000000 miss_hit_core-0.9.41/miss_hit_core/work_package.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-26 10:11:38.880103 miss_hit_core-0.9.41/miss_hit_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/miss_hit_core.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-26 10:11:38.884103 miss_hit_core-0.9.41/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-05-26 10:11:38.000000 miss_hit_core-0.9.41/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:47:04.884966 miss_hit_core-0.9.42/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2019-11-17 11:29:52.000000 miss_hit_core-0.9.42/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)    34523 2020-08-01 08:20:05.000000 miss_hit_core-0.9.42/LICENSE.AGPL
+-rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-07-17 08:47:04.884966 miss_hit_core-0.9.42/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     6162 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:47:04.880967 miss_hit_core-0.9.42/miss_hit_core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-08-16 07:52:19.000000 miss_hit_core-0.9.42/miss_hit_core/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    17465 2022-08-21 10:31:44.000000 miss_hit_core-0.9.42/miss_hit_core/cfg_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21634 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/cfg_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16418 2022-08-21 10:17:29.000000 miss_hit_core-0.9.42/miss_hit_core/cfg_tree.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18768 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/command_line.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    19019 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/config.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    28905 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)   112073 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/m_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2182 2021-03-18 19:12:14.000000 miss_hit_core-0.9.42/miss_hit_core/m_entity_root.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11754 2022-09-18 09:26:58.000000 miss_hit_core-0.9.42/miss_hit_core/m_language.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    33495 2020-08-16 07:52:19.000000 miss_hit_core-0.9.42/miss_hit_core/m_language_builtins.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    63636 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/m_lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4033 2022-08-13 12:46:59.000000 miss_hit_core-0.9.42/miss_hit_core/m_parse_utils.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    81645 2023-05-26 10:11:20.000000 miss_hit_core-0.9.42/miss_hit_core/m_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4413 2020-09-12 11:41:10.000000 miss_hit_core-0.9.42/miss_hit_core/m_types.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    43130 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/mh_metric.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    52197 2023-05-19 08:46:33.000000 miss_hit_core-0.9.42/miss_hit_core/mh_style.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2450 2021-10-30 16:34:20.000000 miss_hit_core-0.9.42/miss_hit_core/pathutil.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:47:04.884966 miss_hit_core-0.9.42/miss_hit_core/resources/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:47:04.884966 miss_hit_core-0.9.42/miss_hit_core/resources/assets/
+-rw-r--r--   0 florian   (1000) florian   (1000)      424 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/alert-triangle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      355 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/bar-chart-2.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      345 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/check-square.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      370 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/download.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/edit.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      388 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/external-link.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      473 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/file-text.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      365 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/help-circle.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      517 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/package.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1011 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/settings.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)      310 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/assets/terminal.svg
+-rw-r--r--   0 florian   (1000) florian   (1000)     3101 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core/resources/style.css
+-rw-r--r--   0 florian   (1000) florian   (1000)     3518 2020-11-30 09:06:20.000000 miss_hit_core-0.9.42/miss_hit_core/resources.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10328 2023-07-17 08:46:42.000000 miss_hit_core-0.9.42/miss_hit_core/s_ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    24582 2023-05-26 08:33:33.000000 miss_hit_core-0.9.42/miss_hit_core/s_parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2150 2023-07-17 08:46:50.000000 miss_hit_core-0.9.42/miss_hit_core/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8073 2023-07-17 08:46:42.000000 miss_hit_core-0.9.42/miss_hit_core/work_package.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-17 08:47:04.880967 miss_hit_core-0.9.42/miss_hit_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     7254 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1391 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       98 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       14 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/miss_hit_core.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-07-17 08:47:04.884966 miss_hit_core-0.9.42/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1662 2023-07-17 08:47:04.000000 miss_hit_core-0.9.42/setup.py
```

### Comparing `miss_hit_core-0.9.41/LICENSE` & `miss_hit_core-0.9.42/LICENSE`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/LICENSE.AGPL` & `miss_hit_core-0.9.42/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/PKG-INFO` & `miss_hit_core-0.9.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss_hit_core
-Version: 0.9.41
+Version: 0.9.42
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
```

### Comparing `miss_hit_core-0.9.41/README.md` & `miss_hit_core-0.9.42/README.md`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/cfg_ast.py` & `miss_hit_core-0.9.42/miss_hit_core/cfg_ast.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/cfg_parser.py` & `miss_hit_core-0.9.42/miss_hit_core/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/cfg_tree.py` & `miss_hit_core-0.9.42/miss_hit_core/cfg_tree.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/command_line.py` & `miss_hit_core-0.9.42/miss_hit_core/command_line.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/config.py` & `miss_hit_core-0.9.42/miss_hit_core/config.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/errors.py` & `miss_hit_core-0.9.42/miss_hit_core/errors.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_ast.py` & `miss_hit_core-0.9.42/miss_hit_core/m_ast.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_entity_root.py` & `miss_hit_core-0.9.42/miss_hit_core/m_entity_root.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_language.py` & `miss_hit_core-0.9.42/miss_hit_core/m_language.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_language_builtins.py` & `miss_hit_core-0.9.42/miss_hit_core/m_language_builtins.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_lexer.py` & `miss_hit_core-0.9.42/miss_hit_core/m_lexer.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_parse_utils.py` & `miss_hit_core-0.9.42/miss_hit_core/m_parse_utils.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_parser.py` & `miss_hit_core-0.9.42/miss_hit_core/m_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/m_types.py` & `miss_hit_core-0.9.42/miss_hit_core/m_types.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/mh_metric.py` & `miss_hit_core-0.9.42/miss_hit_core/mh_metric.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/mh_style.py` & `miss_hit_core-0.9.42/miss_hit_core/mh_style.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/pathutil.py` & `miss_hit_core-0.9.42/miss_hit_core/pathutil.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/resources/assets/package.svg` & `miss_hit_core-0.9.42/miss_hit_core/resources/assets/package.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/resources/assets/settings.svg` & `miss_hit_core-0.9.42/miss_hit_core/resources/assets/settings.svg`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/resources/style.css` & `miss_hit_core-0.9.42/miss_hit_core/resources/style.css`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/resources.py` & `miss_hit_core-0.9.42/miss_hit_core/resources.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/s_ast.py` & `miss_hit_core-0.9.42/miss_hit_core/s_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,18 @@
 
     def full_name(self):
         # Gets the full name for this block, including the model's
         # name. E.g. Test1/SubSystem/MyBlock
         name_stack = []
         ptr = self
         while ptr:
-            if isinstance(ptr, Container):
+            if isinstance(ptr, Model):
                 name_stack.append(ptr.name)
+            elif isinstance(ptr, Library):
+                break
             elif isinstance(ptr, Block):
                 name_stack.append(ptr.name)
             ptr = ptr.n_parent
         return "/".join(reversed(name_stack))
 
     def local_name(self):
         # Gets the name for this block, local to the
```

### Comparing `miss_hit_core-0.9.41/miss_hit_core/s_parser.py` & `miss_hit_core-0.9.42/miss_hit_core/s_parser.py`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/miss_hit_core/version.py` & `miss_hit_core-0.9.42/miss_hit_core/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 ##                                                                          ##
 ##############################################################################
 
 # Some constants we use for tool version and URLs
 
 GITHUB_ISSUES = "https://github.com/florianschanda/miss_hit/issues"
 
-VERSION_TUPLE = (0, 9, 41)
+VERSION_TUPLE = (0, 9, 42)
 VERSION_SUFFIX = ""
 
 VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
           ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "MISS_HIT %s" % VERSION
```

### Comparing `miss_hit_core-0.9.41/miss_hit_core/work_package.py` & `miss_hit_core-0.9.42/miss_hit_core/work_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         assert isinstance(simulink_wp, SIMULINK_File_WP)
         assert isinstance(simulink_block, s_ast.Matlab_Function)
 
         n_container = simulink_block.get_container()
 
         super().__init__(simulink_wp.in_test_dir,
                          n_container.filename,
-                         simulink_block.local_name(),
+                         simulink_block.full_name(),
                          simulink_block.get_encoding(),
                          simulink_wp.mh.fork(),
                          simulink_wp.options,
                          simulink_wp.extra_options)
 
         self.cfg         = simulink_wp.cfg
         self.block       = simulink_block
```

### Comparing `miss_hit_core-0.9.41/miss_hit_core.egg-info/PKG-INFO` & `miss_hit_core-0.9.42/miss_hit_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miss-hit-core
-Version: 0.9.41
+Version: 0.9.42
 Summary: Code formatting and code metrics for programs written in the MATLAB/Simulink and Octave languages.
 Home-page: https://misshit.org
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/miss_hit/issues
 Project-URL: Documentation, https://florianschanda.github.io/miss_hit/
```

### Comparing `miss_hit_core-0.9.41/miss_hit_core.egg-info/SOURCES.txt` & `miss_hit_core-0.9.42/miss_hit_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miss_hit_core-0.9.41/setup.py` & `miss_hit_core-0.9.42/setup.py`

 * *Files identical despite different names*

