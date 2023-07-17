# Comparing `tmp/unearth-0.9.2.tar.gz` & `tmp/unearth-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unearth-0.9.2.tar", last modified: Tue Jul  4 02:02:53 2023, max compression
+gzip compressed data, was "unearth-0.9.3.tar", last modified: Mon Jul 17 16:04:53 2023, max compression
```

## Comparing `unearth-0.9.2.tar` & `unearth-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1059 2023-07-04 02:02:38.374191 unearth-0.9.2/LICENSE
--rw-r--r--   0        0        0     2885 2023-07-04 02:02:38.374191 unearth-0.9.2/README.md
--rw-r--r--   0        0        0     1919 2023-07-04 02:02:38.374191 unearth-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      616 2023-07-04 02:02:38.374191 unearth-0.9.2/src/unearth/__init__.py
--rw-r--r--   0        0        0     5993 2023-07-04 02:02:38.374191 unearth-0.9.2/src/unearth/__main__.py
--rw-r--r--   0        0        0    13606 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/auth.py
--rw-r--r--   0        0        0     7965 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/collector.py
--rw-r--r--   0        0        0      970 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/errors.py
--rw-r--r--   0        0        0    10775 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/evaluator.py
--rw-r--r--   0        0        0    15178 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/finder.py
--rw-r--r--   0        0        0     5526 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/link.py
--rw-r--r--   0        0        0     5406 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/pep425tags.py
--rw-r--r--   0        0        0    11520 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/preparer.py
--rw-r--r--   0        0        0        0 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/py.typed
--rw-r--r--   0        0        0     6687 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/session.py
--rw-r--r--   0        0        0     6405 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/utils.py
--rw-r--r--   0        0        0      258 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/__init__.py
--rw-r--r--   0        0        0     8415 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/base.py
--rw-r--r--   0        0        0     2589 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/bazaar.py
--rw-r--r--   0        0        0     4813 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/git.py
--rw-r--r--   0        0        0     2006 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/hg.py
--rw-r--r--   0        0        0     6238 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/svn.py
--rw-r--r--   0        0        0      132 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     2581 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2173 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/app.py
--rw-r--r--   0        0        0    96588 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/files/click-8.1.3-py3-none-any.whl
--rw-r--r--   0        0        0   133101 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
--rw-r--r--   0        0        0      816 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/findlinks/index.html
--rw-r--r--   0        0        0     1860 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/black.html
--rw-r--r--   0        0        0      876 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/click.html
--rw-r--r--   0        0        0      461 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/first.html
--rw-r--r--   0        0        0      964 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/pipenv.html
--rw-r--r--   0        0        0     2345 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/black.json
--rw-r--r--   0        0        0     1081 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/click.json
--rw-r--r--   0        0        0      521 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/first.json
--rw-r--r--   0        0        0     1178 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/pipenv.json
--rw-r--r--   0        0        0     2628 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_collector.py
--rw-r--r--   0        0        0     8267 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_evaluator.py
--rw-r--r--   0        0        0     6341 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_finder.py
--rw-r--r--   0        0        0     4044 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_link.py
--rw-r--r--   0        0        0     3380 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_session.py
--rw-r--r--   0        0        0      558 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_utils.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 unearth-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-17 16:04:39.541082 unearth-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2885 2023-07-17 16:04:39.541082 unearth-0.9.3/README.md
+-rw-r--r--   0        0        0     1917 2023-07-17 16:04:53.573293 unearth-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/__init__.py
+-rw-r--r--   0        0        0     5993 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/__main__.py
+-rw-r--r--   0        0        0    13606 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/auth.py
+-rw-r--r--   0        0        0     7965 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/collector.py
+-rw-r--r--   0        0        0      970 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/errors.py
+-rw-r--r--   0        0        0    10878 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/evaluator.py
+-rw-r--r--   0        0        0    15178 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/finder.py
+-rw-r--r--   0        0        0     5526 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/link.py
+-rw-r--r--   0        0        0     5406 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/pep425tags.py
+-rw-r--r--   0        0        0    11520 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/preparer.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/py.typed
+-rw-r--r--   0        0        0     6687 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/session.py
+-rw-r--r--   0        0        0     7756 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/utils.py
+-rw-r--r--   0        0        0      258 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/__init__.py
+-rw-r--r--   0        0        0     8415 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/base.py
+-rw-r--r--   0        0        0     2589 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/bazaar.py
+-rw-r--r--   0        0        0     4813 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/git.py
+-rw-r--r--   0        0        0     2006 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/hg.py
+-rw-r--r--   0        0        0     6238 2023-07-17 16:04:39.541082 unearth-0.9.3/src/unearth/vcs/svn.py
+-rw-r--r--   0        0        0      132 2023-07-17 16:04:39.541082 unearth-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     2581 2023-07-17 16:04:39.541082 unearth-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:04:39.541082 unearth-0.9.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2173 2023-07-17 16:04:39.541082 unearth-0.9.3/tests/fixtures/app.py
+-rw-r--r--   0        0        0    96588 2023-07-17 16:04:39.541082 unearth-0.9.3/tests/fixtures/files/click-8.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0   133101 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0      816 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/findlinks/index.html
+-rw-r--r--   0        0        0     1860 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/index/black.html
+-rw-r--r--   0        0        0      876 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/index/click.html
+-rw-r--r--   0        0        0      461 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/index/first.html
+-rw-r--r--   0        0        0      964 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/index/pipenv.html
+-rw-r--r--   0        0        0     2345 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/json/black.json
+-rw-r--r--   0        0        0     1081 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/json/click.json
+-rw-r--r--   0        0        0      521 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/json/first.json
+-rw-r--r--   0        0        0     1178 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/fixtures/json/pipenv.json
+-rw-r--r--   0        0        0     2628 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_collector.py
+-rw-r--r--   0        0        0     8510 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_evaluator.py
+-rw-r--r--   0        0        0     6341 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_finder.py
+-rw-r--r--   0        0        0     4044 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_link.py
+-rw-r--r--   0        0        0     3380 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_session.py
+-rw-r--r--   0        0        0      558 2023-07-17 16:04:39.545082 unearth-0.9.3/tests/test_utils.py
+-rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 unearth-0.9.3/PKG-INFO
```

### Comparing `unearth-0.9.2/LICENSE` & `unearth-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/README.md` & `unearth-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/pyproject.toml` & `unearth-0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "unearth"
 description = "A utility to fetch and download python packages"
 authors = [
     { name = "Frost Ming", email = "me@frostming.com" },
 ]
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.9.2"
+version = "0.9.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/unearth"
 Documentation = "https://unearth.readthedocs.io"
```

### Comparing `unearth-0.9.2/src/unearth/__init__.py` & `unearth-0.9.3/src/unearth/__init__.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/__main__.py` & `unearth-0.9.3/src/unearth/__main__.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/auth.py` & `unearth-0.9.3/src/unearth/auth.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/collector.py` & `unearth-0.9.3/src/unearth/collector.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/errors.py` & `unearth-0.9.3/src/unearth/errors.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/evaluator.py` & `unearth-0.9.3/src/unearth/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,20 @@
     parse_wheel_filename,
 )
 from packaging.version import InvalidVersion, Version
 from requests import Session
 
 from unearth.link import Link
 from unearth.pep425tags import get_supported
-from unearth.utils import ARCHIVE_EXTENSIONS, splitext, strip_extras
+from unearth.utils import (
+    ARCHIVE_EXTENSIONS,
+    fix_legacy_specifier,
+    splitext,
+    strip_extras,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def is_equality_specifier(specifier: SpecifierSet) -> bool:
     return any(s.operator in ("==", "===") for s in specifier)
 
@@ -147,15 +152,17 @@
             raise LinkMismatchError(f"Yanked {yank_reason}")
 
     def _check_requires_python(self, link: Link) -> None:
         if not self.ignore_compatibility and link.requires_python:
             py_ver = self.target_python.py_ver or sys.version_info[:2]
             py_version = ".".join(str(v) for v in py_ver)
             try:
-                requires_python = SpecifierSet(link.requires_python)
+                requires_python = SpecifierSet(
+                    fix_legacy_specifier(link.requires_python)
+                )
             except InvalidSpecifier:
                 raise LinkMismatchError(
                     f"Invalid requires-python: {link.requires_python}"
                 )
             if not requires_python.contains(py_version, True):
                 raise LinkMismatchError(
                     "The target python version({}) doesn't match "
```

### Comparing `unearth-0.9.2/src/unearth/finder.py` & `unearth-0.9.3/src/unearth/finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/link.py` & `unearth-0.9.3/src/unearth/link.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/pep425tags.py` & `unearth-0.9.3/src/unearth/pep425tags.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/preparer.py` & `unearth-0.9.3/src/unearth/preparer.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/session.py` & `unearth-0.9.3/src/unearth/session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/utils.py` & `unearth-0.9.3/src/unearth/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """A package should contain a link to the actual file."""
 from __future__ import annotations
 
 import functools
 import itertools
 import os
+import re
 import sys
 import urllib.parse as parse
+import warnings
 from pathlib import Path
 from typing import Iterable, Iterator, Sequence, TypeVar
 from urllib.request import pathname2url, url2pathname
 
 WINDOWS = sys.platform == "win32"
 
 
@@ -213,7 +215,43 @@
     def __getitem__(self, index: int) -> T:  # type: ignore[override]
         if index < 0:
             raise IndexError("Negative indices are not supported")
         for i, item in enumerate(self):
             if i == index:
                 return item
         raise IndexError("Index out of range")
+
+
+_legacy_specifier_re = re.compile(r"(==|!=|<=|>=|<|>)(\s*)([^,;\s)]*)")
+
+
+@functools.lru_cache()
+def fix_legacy_specifier(specifier: str) -> str:
+    """Since packaging 22.0, legacy specifiers like '>=4.*' are no longer
+    supported. We try to normalize them to the new format.
+    """
+
+    def fix_wildcard(match: re.Match[str]) -> str:
+        operator, _, version = match.groups()
+        if operator in ("==", "!="):
+            return match.group(0)
+        if ".*" in version:
+            warnings.warn(
+                ".* suffix can only be used with `==` or `!=` operators",
+                FutureWarning,
+                stacklevel=4,
+            )
+            version = version.replace(".*", ".0")
+            if operator in ("<", "<="):  # <4.* and <=4.* are equivalent to <4.0
+                operator = "<"
+            elif operator in (">", ">="):  # >4.* and >=4.* are equivalent to >=4.0
+                operator = ">="
+        elif "+" in version:  # Drop the local version
+            warnings.warn(
+                "Local version label can only be used with `==` or `!=` operators",
+                FutureWarning,
+                stacklevel=4,
+            )
+            version = version.split("+")[0]
+        return f"{operator}{version}"
+
+    return _legacy_specifier_re.sub(fix_wildcard, specifier)
```

### Comparing `unearth-0.9.2/src/unearth/vcs/base.py` & `unearth-0.9.3/src/unearth/vcs/base.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/vcs/bazaar.py` & `unearth-0.9.3/src/unearth/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/vcs/git.py` & `unearth-0.9.3/src/unearth/vcs/git.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/vcs/hg.py` & `unearth-0.9.3/src/unearth/vcs/hg.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/src/unearth/vcs/svn.py` & `unearth-0.9.3/src/unearth/vcs/svn.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/conftest.py` & `unearth-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/app.py` & `unearth-0.9.3/tests/fixtures/app.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/files/click-8.1.3-py3-none-any.whl` & `unearth-0.9.3/tests/fixtures/files/click-8.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl` & `unearth-0.9.3/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/findlinks/index.html` & `unearth-0.9.3/tests/fixtures/findlinks/index.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/index/black.html` & `unearth-0.9.3/tests/fixtures/index/black.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/index/click.html` & `unearth-0.9.3/tests/fixtures/index/click.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/index/pipenv.html` & `unearth-0.9.3/tests/fixtures/index/pipenv.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/json/black.json` & `unearth-0.9.3/tests/fixtures/json/black.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/json/click.json` & `unearth-0.9.3/tests/fixtures/json/click.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/json/first.json` & `unearth-0.9.3/tests/fixtures/json/first.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/fixtures/json/pipenv.json` & `unearth-0.9.3/tests/fixtures/json/pipenv.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/test_collector.py` & `unearth-0.9.3/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/test_evaluator.py` & `unearth-0.9.3/tests/test_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
     assert evaluator.evaluate_link(link) is not None
     assert link.hash_name == "sha256"
     assert (
         link.hash == "bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
     )
 
 
+@pytest.mark.filterwarnings("ignore::FutureWarning")
 @pytest.mark.parametrize(
     "link,expected",
     [
         (Link("https://test.pypi.org/files/click-8.1.3-py3-none-any.whl"), True),
         (Link("https://test.pypi.org/files/click-8.1.3-cp39-cp39-win_amd64.whl"), True),
         (
             Link("https://test.pypi.org/files/click-8.1.3-cp310-cp310-win_amd64.whl"),
@@ -222,14 +223,21 @@
         (
             Link(
                 "https://test.pypi.org/files/click-8.1.3-cp39-cp39-"
                 "macosx_11_0_arm64.whl"
             ),
             False,
         ),
+        (
+            Link(
+                "https://test.pypi.org/files/click-8.1.3-py3-none-any.whl",
+                requires_python=">3.6.*",
+            ),
+            True,
+        ),
     ],
 )
 @pytest.mark.parametrize("ignore_compatibility", (True, False))
 def test_evaluate_compatibility_tags(link, expected, ignore_compatibility, session):
     evaluator = Evaluator(
         "click",
         session,
```

### Comparing `unearth-0.9.2/tests/test_finder.py` & `unearth-0.9.3/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/test_link.py` & `unearth-0.9.3/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/test_session.py` & `unearth-0.9.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/tests/test_utils.py` & `unearth-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.2/PKG-INFO` & `unearth-0.9.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: unearth
-Version: 0.9.2
+Version: 0.9.3
 Summary: A utility to fetch and download python packages
+Author-Email: Frost Ming <me@frostming.com>
 License: MIT
-Author-email: Frost Ming <me@frostming.com>
-Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: keyring
-Project-URL: Changelog, https://github.com/frostming/unearth/releases
-Project-URL: Documentation, https://unearth.readthedocs.io
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/frostming/unearth
+Project-URL: Documentation, https://unearth.readthedocs.io
+Project-URL: Changelog, https://github.com/frostming/unearth/releases
+Requires-Python: >=3.7
+Requires-Dist: packaging>=20
+Requires-Dist: requests>=2.25
+Requires-Dist: cached-property>=1.5.2; python_version < "3.8"
+Requires-Dist: keyring; extra == "keyring"
+Provides-Extra: keyring
 Description-Content-Type: text/markdown
 
 # unearth
 
 <!--index start-->
 
 [![Tests](https://github.com/frostming/unearth/workflows/Tests/badge.svg)](https://github.com/frostming/unearth/actions?query=workflow%3Aci)
@@ -88,8 +92,7 @@
 ```
 
 <!--index end-->
 
 ## Documentation
 
 [Read the docs](https://unearth.readthedocs.io/en/latest/)
-
```

