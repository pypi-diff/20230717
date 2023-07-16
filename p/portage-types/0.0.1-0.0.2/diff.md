# Comparing `tmp/portage_types-0.0.1.tar.gz` & `tmp/portage_types-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portage_types-0.0.1.tar", max compression
+gzip compressed data, was "portage_types-0.0.2.tar", max compression
```

## Comparing `portage_types-0.0.1.tar` & `portage_types-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-07-03 22:21:36.164437 portage_types-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      132 2023-07-03 22:20:07.696527 portage_types-0.0.1/README.md
--rw-r--r--   0        0        0     1556 2023-07-03 22:40:31.209893 portage_types-0.0.1/portage-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-07-03 22:23:05.282348 portage_types-0.0.1/portage-stubs/py.typed
--rw-r--r--   0        0        0      292 2023-07-03 23:47:56.999531 portage_types-0.0.1/portage-stubs/versions.pyi
--rw-r--r--   0        0        0      680 2023-07-03 22:22:10.123403 portage_types-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 portage_types-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-03 22:21:36.164437 portage_types-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      281 2023-07-07 01:34:26.833062 portage_types-0.0.2/README.md
+-rw-r--r--   0        0        0     1560 2023-07-16 22:37:27.034539 portage_types-0.0.2/portage-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 22:23:05.282348 portage_types-0.0.2/portage-stubs/py.typed
+-rw-r--r--   0        0        0      325 2023-07-16 22:37:27.034539 portage_types-0.0.2/portage-stubs/versions.pyi
+-rw-r--r--   0        0        0     4816 2023-07-16 22:37:31.608547 portage_types-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 portage_types-0.0.2/PKG-INFO
```

### Comparing `portage_types-0.0.1/LICENSE.txt` & `portage_types-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portage_types-0.0.1/portage-stubs/__init__.pyi` & `portage_types-0.0.2/portage-stubs/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Any, Literal, Mapping, Sequence, TypedDict
+# pylint: disable=too-few-public-methods,unused-argument
+from typing import Any, Literal, Mapping, TypedDict
 
 __all__ = ('db', 'root')
 
 
 class dbapi:
     def aux_get(self,
                 mycpv: str,
-                mylist: Sequence[Literal['DEFINED_PHASES', 'DEPEND', 'EAPI', 'HDEPEND', 'HOMEPAGE',
-                                         'INHERITED', 'IUSE', 'KEYWORDS', 'LICENSE', 'PDEPEND',
-                                         'PROPERTIES', 'PROVIDE', 'RDEPEND', 'REQUIRED_USE',
-                                         'repository', 'RESTRICT', 'SRC_URI', 'SLOT']],
+                mylist: list[Literal['DEFINED_PHASES', 'DEPEND', 'EAPI', 'HDEPEND', 'HOMEPAGE',
+                                     'INHERITED', 'IUSE', 'KEYWORDS', 'LICENSE', 'PDEPEND',
+                                     'PROPERTIES', 'PROVIDE', 'RDEPEND', 'REQUIRED_USE',
+                                     'repository', 'RESTRICT', 'SRC_URI', 'SLOT']],
                 mytree: str | None = ...,
-                myrepo: str | None = ...) -> Sequence[str]:
+                myrepo: str | None = ...) -> list[str]:
         ...
 
     def xmatch(self, level: Literal['bestmatch-visible', 'match-all-cpv-only', 'match-all',
                                     'match-visible', 'minimum-all', 'minimum-visible',
-                                    'minimum-all-ignore-profile'],
-               origdep: str) -> Sequence[str] | str:
+                                    'minimum-all-ignore-profile'], origdep: str) -> list[str] | str:
         ...
 
     def findname(self, mycpv: str, mytree: str | None = ..., myrepo: str | None = ...) -> str:
         ...
 
     def findname2(
             self,
             mycpv: str,
             mytree: str | None = ...,
             myrepo: str | None = ...
     ) -> tuple[None, Literal[0]] | tuple[str, str] | tuple[str, None]:
         ...
 
-    def match(self, mydep: str, use_cache: Literal[0, 1] = ...) -> Sequence[str] | str:
+    def match(self, mydep: str, use_cache: Literal[0, 1] = ...) -> list[str] | str:
         ...
 
 
 class PortageTree:
     dbapi: dbapi
```

### Comparing `portage_types-0.0.1/PKG-INFO` & `portage_types-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: portage-types
-Version: 0.0.1
+Version: 0.0.2
 Summary: Typing stubs for Portage
 License: MIT
 Author: Andrew Udvare
 Author-email: audvare@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 
 # Portage types
 
+[![QA](https://github.com/Tatsh/portage-types/actions/workflows/qa.yml/badge.svg)](https://github.com/Tatsh/portage-types/actions/workflows/qa.yml)
+
 Types for portage.
 
 ## Installation
 
 ```shell
 pip install portage-types
 ```
```

