# Comparing `tmp/pdm_bump-0.7.1.tar.gz` & `tmp/pdm_bump-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_bump-0.7.1.tar", last modified: Fri Jun 16 19:21:29 2023, max compression
+gzip compressed data, was "pdm_bump-0.7.2.tar", last modified: Mon Jul 17 18:36:28 2023, max compression
```

## Comparing `pdm_bump-0.7.1.tar` & `pdm_bump-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1092 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/LICENSE
--rw-r--r--   0        0        0     2397 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/README.md
--rw-r--r--   0        0        0     6003 2023-06-16 19:21:29.162035 pdm_bump-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      869 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/src/pdm_bump/__init__.py
--rw-r--r--   0        0        0      542 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/__init__.py
--rw-r--r--   0        0        0     8508 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/base.py
--rw-r--r--   0        0        0     1954 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/explicit.py
--rw-r--r--   0        0        0     9966 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/increment.py
--rw-r--r--   0        0        0     8897 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/preview.py
--rw-r--r--   0        0        0     1558 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/vcs.py
--rw-r--r--   0        0        0     1378 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/cli.py
--rw-r--r--   0        0        0      259 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/__init__.py
--rw-r--r--   0        0        0     9465 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/config.py
--rw-r--r--   0        0        0     2293 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/loader.py
--rw-r--r--   0        0        0     7404 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/logging.py
--rw-r--r--   0        0        0     7593 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/version.py
--rw-r--r--   0        0        0     6592 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/dynamic.py
--rw-r--r--   0        0        0     6668 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/plugin.py
--rw-r--r--   0        0        0        0 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/py.typed
--rw-r--r--   0        0        0     2402 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/source.py
--rw-r--r--   0        0        0      792 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0        0        0     9907 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/core.py
--rw-r--r--   0        0        0     1103 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/git.py
--rw-r--r--   0        0        0     7356 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0        0        0     4906 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0        0        0    25464 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/action_test.py
--rw-r--r--   0        0        0     3743 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/plugin_test.py
--rw-r--r--   0        0        0    24207 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/version_test.py
--rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-17 18:35:12.758294 pdm_bump-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2397 2023-07-17 18:35:12.758294 pdm_bump-0.7.2/README.md
+-rw-r--r--   0        0        0     6003 2023-07-17 18:36:28.603353 pdm_bump-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      869 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      542 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     8508 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1954 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0     9966 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     8897 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     1558 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0     1378 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      259 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     9461 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     2293 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/loader.py
+-rw-r--r--   0        0        0     7404 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     7593 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     6596 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     6668 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2402 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      792 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0     9907 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0     1103 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     7356 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     4906 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    25464 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/action_test.py
+-rw-r--r--   0        0        0     3743 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/plugin_test.py
+-rw-r--r--   0        0        0    24207 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/version_test.py
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.2/PKG-INFO
```

### Comparing `pdm_bump-0.7.1/LICENSE` & `pdm_bump-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/README.md` & `pdm_bump-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/pyproject.toml` & `pdm_bump-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-bump"
-version = "0.7.1"
+version = "0.7.2"
 readme = "README.md"
 description = "A plugin for PDM providing the ability to modify the version according to PEP440"
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
 dependencies = [
     "pdm>=2.00",
```

### Comparing `pdm_bump-0.7.1/src/pdm_bump/__init__.py` & `pdm_bump-0.7.2/src/pdm_bump/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/__init__.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/base.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/base.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/explicit.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/explicit.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/increment.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/increment.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/preview.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/preview.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/actions/vcs.py` & `pdm_bump-0.7.2/src/pdm_bump/actions/vcs.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/cli.py` & `pdm_bump-0.7.2/src/pdm_bump/cli.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/core/config.py` & `pdm_bump-0.7.2/src/pdm_bump/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         section_key: Iterable[str] = ()
         if section in (
             _ConfigSection.TOOL_CONFIG,
             _ConfigSection.PLUGIN_CONFIG,
         ):
             section_key = ["tool", "pdm"]
             if _ConfigSection.PLUGIN_CONFIG == section:
-                section_key.extend(["plugins", "bump"])
+                section_key.extend(["bump-plugin"])
             section_key = tuple(section_key)
         elif _ConfigSection.BUILD_SYSTEM == section:
             section_key = ("build-system",)
         elif _ConfigSection.METADATA == section:
             section_key = ("project",)
         elif _ConfigSection.ROOT == section:
             return project_data or {}
```

### Comparing `pdm_bump-0.7.1/src/pdm_bump/core/loader.py` & `pdm_bump-0.7.2/src/pdm_bump/core/loader.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/core/logging.py` & `pdm_bump-0.7.2/src/pdm_bump/core/logging.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/core/version.py` & `pdm_bump-0.7.2/src/pdm_bump/core/version.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/dynamic.py` & `pdm_bump-0.7.2/src/pdm_bump/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE_FILE_PATH
             )
             return DynamicVersionConfig(
                 file_path=root_path / file_path,
                 pattern=DEFAULT_REGEX,
             )
         if (
-            project_config.get_pyproject_metadata(ConfigKeys.BUILD_BACKEND)
+            project_config.get_pyproject_build_system(ConfigKeys.BUILD_BACKEND)
             == ConfigValues.BUILD_BACKEND_PDM_BACKEND
         ):
             if (
                 project_config.get_pyproject_tool_config(
                     ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE
                 )
                 == ConfigValues.VERSION_SOURCE_SCM
```

### Comparing `pdm_bump-0.7.1/src/pdm_bump/plugin.py` & `pdm_bump-0.7.2/src/pdm_bump/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/source.py` & `pdm_bump-0.7.2/src/pdm_bump/source.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/vcs/__init__.py` & `pdm_bump-0.7.2/src/pdm_bump/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/vcs/core.py` & `pdm_bump-0.7.2/src/pdm_bump/vcs/core.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/vcs/git.py` & `pdm_bump-0.7.2/src/pdm_bump/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/vcs/gitcli.py` & `pdm_bump-0.7.2/src/pdm_bump/vcs/gitcli.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/src/pdm_bump/vcs/mixins.py` & `pdm_bump-0.7.2/src/pdm_bump/vcs/mixins.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/tests/action_test.py` & `pdm_bump-0.7.2/tests/action_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/tests/plugin_test.py` & `pdm_bump-0.7.2/tests/plugin_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/tests/version_test.py` & `pdm_bump-0.7.2/tests/version_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.1/PKG-INFO` & `pdm_bump-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-bump
-Version: 0.7.1
+Version: 0.7.2
 Summary: A plugin for PDM providing the ability to modify the version according to PEP440
 Home-page: https://github.com/carstencodes/pdm-bump
 Author-Email: Carsten Igel <cig@bite-that-bit.de>
 License: MIT
 Project-URL: Homepage, https://github.com/carstencodes/pdm-bump
 Requires-Python: >=3.9
 Requires-Dist: pdm>=2.00
```

