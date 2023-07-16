# Comparing `tmp/reflex_nexus-0.0.12.tar.gz` & `tmp/reflex_nexus-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_nexus-0.0.12.tar", max compression
+gzip compressed data, was "reflex_nexus-0.0.22.tar", max compression
```

## Comparing `reflex_nexus-0.0.12.tar` & `reflex_nexus-0.0.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/LICENSE
--rw-r--r--   0        0        0     5656 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/README.md
--rw-r--r--   0        0        0     1564 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     1150 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/application.py
--rw-r--r--   0        0        0        0 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/device_registry.py
--rw-r--r--   0        0        0      541 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/logger.py
--rw-r--r--   0        0        0      732 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/main_window.py
--rw-r--r--   0        0        0      931 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/menu_bar.py
--rw-r--r--   0        0        0      369 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/stylesheet.qss
--rw-r--r--   0        0        0      938 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/widget_registry.py
--rw-r--r--   0        0        0     1327 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/devices/reflex_v2.py
--rw-r--r--   0        0        0      117 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/drivers/usb_hid.py
--rw-r--r--   0        0        0      380 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/widgets/log_viewer.py
--rw-r--r--   0        0        0      883 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/widgets/pad_interface.py
--rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 reflex_nexus-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-16 22:32:02.846619 reflex_nexus-0.0.22/LICENSE
+-rw-r--r--   0        0        0     5687 2023-07-16 22:32:02.846619 reflex_nexus-0.0.22/README.md
+-rw-r--r--   0        0        0     1564 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     1150 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/application.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/device_registry.py
+-rw-r--r--   0        0        0      541 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/logger.py
+-rw-r--r--   0        0        0      732 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/main_window.py
+-rw-r--r--   0        0        0      931 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/menu_bar.py
+-rw-r--r--   0        0        0      369 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/stylesheet.qss
+-rw-r--r--   0        0        0      938 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/app/widget_registry.py
+-rw-r--r--   0        0        0     1327 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/devices/reflex_v2.py
+-rw-r--r--   0        0        0      117 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/drivers/usb_hid.py
+-rw-r--r--   0        0        0      380 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/widgets/log_viewer.py
+-rw-r--r--   0        0        0      883 2023-07-16 22:32:02.850619 reflex_nexus-0.0.22/src/widgets/pad_interface.py
+-rw-r--r--   0        0        0     6392 1970-01-01 00:00:00.000000 reflex_nexus-0.0.22/PKG-INFO
```

### Comparing `reflex_nexus-0.0.12/LICENSE` & `reflex_nexus-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/README.md` & `reflex_nexus-0.0.22/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,25 @@
 - [Sphinx-Rtd-Theme] - Read the Docs Sphinx theme
 
 *RE:Flex Nexus is released under the MIT License, more details in [LICENSE]
 file.*
 
 <!--- Site links -->
 
-[coverage]: https://coveralls.io/github/ReflexCreations/Nexus
+[coverage]: https://coveralls.io/github/ReflexCreations/Nexus?branch=main
 [discord]: https://discord.gg/TCn3emnwZU
 [Documentation]: https://reflex-nexus.readthedocs.io/
 [Git]: https://git-scm.com/downloads/
-[LICENSE]: https://github.com/ReflexCreations/Nexus/LICENSE
-[lint]: https://github.com/ReflexCreations/Nexus/actions/workflows/lint.yml
+[LICENSE]: https://github.com/ReflexCreations/Nexus/blob/master/LICENSE
+[lint]: https://github.com/ReflexCreations/Nexus/actions
 [Python]: https://python.org/downloads/
 [pypi]: https://pypi.org/project/reflex-nexus
 [Releases]: https://github.com/ReflexCreations/Nexus/releases/
 [tag]: https://github.com/ReflexCreations/Nexus/tags
-[test]: https://github.com/ReflexCreations/Nexus/actions/workflows/test.yml
+[test]: https://github.com/ReflexCreations/Nexus/actions
 
 <!--- Runtime dependency links -->
 
 [libusb-package]: https://pypi.org/project/libusb-package/
 [PyQtDarkTheme]: https://pypi.org/project/pyqtdarktheme/
 [PySide6]: https://pypi.org/project/PySide6/
 [PyUSB]: https://pypi.org/project/pyusb/
@@ -122,20 +122,21 @@
 [PyInstaller]: https://pypi.org/project/pyinstaller/
 [pytest]: https://pypi.org/project/pytest/
 [pytest-cov]: https://pypi.org/project/pytest-cov/
 [Ruff]: https://pypi.org/project/ruff/
 [Sphinx]: https://pypi.org/project/Sphinx/
 [Sphinx-Rtd-Theme]: https://pypi.org/project/sphinx-rtd-theme/
 
+
 <!--- Badge images -->
 
-[coverage-badge]: https://img.shields.io/coverallsCoverage/github/ReflexCreations/Nexus
+[coverage-badge]: https://coveralls.io/repos/github/ReflexCreations/Nexus/badge.svg?branch=main
 [discord-badge]: https://img.shields.io/discord/738700768147669088?label=discord
-[docs-badge]: https://img.shields.io/readthedocs/reflex-nexus
+[docs-badge]: https://readthedocs.org/projects/reflex-nexus/badge/?version=latest
 [license-badge]: https://img.shields.io/github/license/ReflexCreations/Nexus
-[lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/lint.yml?label=linting
+[lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/project-lint.yml?label=linting
 [linux-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-linux.yml?label=linux%20build
 [macos-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-macos.yml?label=macos%20build
 [pypi-badge]: https://img.shields.io/pypi/v/reflex-nexus
 [tag-badge]: https://img.shields.io/github/v/tag/ReflexCreations/Nexus
-[test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/test.yml?label=tests
+[test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/project-test.yml?label=tests
 [windows-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-windows.yml?label=windows%20build
```

### Comparing `reflex_nexus-0.0.12/pyproject.toml` & `reflex_nexus-0.0.22/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [metadata]
 title = "RE:Flex Nexus"
 copyright = "2023, Impulse Creations, Ltd"
 logo = "assets/favicon.ico"
 
 [tool.poetry]
 name = "reflex-nexus"
-version = "0.0.12"
+version = "0.0.22"
 description = "RE:Flex Nexus - Universal Dance Pad Utilities"
 authors = ["Brittany Barrett <brittany.l.barrett@gmail.com>"]
 packages = [{include = "src"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://reflex.dance"
 repository = "https://github.com/ReflexCreations/Nexus"
```

### Comparing `reflex_nexus-0.0.12/src/app/application.py` & `reflex_nexus-0.0.22/src/app/application.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/app/logger.py` & `reflex_nexus-0.0.22/src/app/logger.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/app/main_window.py` & `reflex_nexus-0.0.22/src/app/main_window.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/app/menu_bar.py` & `reflex_nexus-0.0.22/src/app/menu_bar.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/app/widget_registry.py` & `reflex_nexus-0.0.22/src/app/widget_registry.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/devices/reflex_v2.py` & `reflex_nexus-0.0.22/src/devices/reflex_v2.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/src/widgets/pad_interface.py` & `reflex_nexus-0.0.22/src/widgets/pad_interface.py`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.12/PKG-INFO` & `reflex_nexus-0.0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-nexus
-Version: 0.0.12
+Version: 0.0.22
 Summary: RE:Flex Nexus - Universal Dance Pad Utilities
 Home-page: https://reflex.dance
 License: MIT
 Author: Brittany Barrett
 Author-email: brittany.l.barrett@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -113,25 +113,25 @@
 - [Sphinx-Rtd-Theme] - Read the Docs Sphinx theme
 
 *RE:Flex Nexus is released under the MIT License, more details in [LICENSE]
 file.*
 
 <!--- Site links -->
 
-[coverage]: https://coveralls.io/github/ReflexCreations/Nexus
+[coverage]: https://coveralls.io/github/ReflexCreations/Nexus?branch=main
 [discord]: https://discord.gg/TCn3emnwZU
 [Documentation]: https://reflex-nexus.readthedocs.io/
 [Git]: https://git-scm.com/downloads/
-[LICENSE]: https://github.com/ReflexCreations/Nexus/LICENSE
-[lint]: https://github.com/ReflexCreations/Nexus/actions/workflows/lint.yml
+[LICENSE]: https://github.com/ReflexCreations/Nexus/blob/master/LICENSE
+[lint]: https://github.com/ReflexCreations/Nexus/actions
 [Python]: https://python.org/downloads/
 [pypi]: https://pypi.org/project/reflex-nexus
 [Releases]: https://github.com/ReflexCreations/Nexus/releases/
 [tag]: https://github.com/ReflexCreations/Nexus/tags
-[test]: https://github.com/ReflexCreations/Nexus/actions/workflows/test.yml
+[test]: https://github.com/ReflexCreations/Nexus/actions
 
 <!--- Runtime dependency links -->
 
 [libusb-package]: https://pypi.org/project/libusb-package/
 [PyQtDarkTheme]: https://pypi.org/project/pyqtdarktheme/
 [PySide6]: https://pypi.org/project/PySide6/
 [PyUSB]: https://pypi.org/project/pyusb/
@@ -143,21 +143,22 @@
 [PyInstaller]: https://pypi.org/project/pyinstaller/
 [pytest]: https://pypi.org/project/pytest/
 [pytest-cov]: https://pypi.org/project/pytest-cov/
 [Ruff]: https://pypi.org/project/ruff/
 [Sphinx]: https://pypi.org/project/Sphinx/
 [Sphinx-Rtd-Theme]: https://pypi.org/project/sphinx-rtd-theme/
 
+
 <!--- Badge images -->
 
-[coverage-badge]: https://img.shields.io/coverallsCoverage/github/ReflexCreations/Nexus
+[coverage-badge]: https://coveralls.io/repos/github/ReflexCreations/Nexus/badge.svg?branch=main
 [discord-badge]: https://img.shields.io/discord/738700768147669088?label=discord
-[docs-badge]: https://img.shields.io/readthedocs/reflex-nexus
+[docs-badge]: https://readthedocs.org/projects/reflex-nexus/badge/?version=latest
 [license-badge]: https://img.shields.io/github/license/ReflexCreations/Nexus
-[lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/lint.yml?label=linting
+[lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/project-lint.yml?label=linting
 [linux-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-linux.yml?label=linux%20build
 [macos-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-macos.yml?label=macos%20build
 [pypi-badge]: https://img.shields.io/pypi/v/reflex-nexus
 [tag-badge]: https://img.shields.io/github/v/tag/ReflexCreations/Nexus
-[test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/test.yml?label=tests
+[test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/project-test.yml?label=tests
 [windows-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-windows.yml?label=windows%20build
```

