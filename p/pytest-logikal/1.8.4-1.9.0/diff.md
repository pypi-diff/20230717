# Comparing `tmp/pytest-logikal-1.8.4.tar.gz` & `tmp/pytest-logikal-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-1.8.4.tar", last modified: Mon May 15 20:09:18 2023, max compression
+gzip compressed data, was "pytest-logikal-1.9.0.tar", last modified: Sat May 27 22:00:57 2023, max compression
```

## Comparing `pytest-logikal-1.8.4.tar` & `pytest-logikal-1.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.226343 pytest-logikal-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 20:09:18.000000 pytest-logikal-1.8.4/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2903 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:09:18.222343 pytest-logikal-1.8.4/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-15 20:08:55.000000 pytest-logikal-1.8.4/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 20:09:18.226343 pytest-logikal-1.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:57.823762 pytest-logikal-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-27 22:00:57.823762 pytest-logikal-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:57.819762 pytest-logikal-1.9.0/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12931 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8232 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6081 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4412 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:57.819762 pytest-logikal-1.9.0/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-27 22:00:57.000000 pytest-logikal-1.9.0/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:57.819762 pytest-logikal-1.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 22:00:57.823762 pytest-logikal-1.9.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-27 22:00:31.000000 pytest-logikal-1.9.0/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-27 22:00:57.823762 pytest-logikal-1.9.0/setup.cfg
```

### Comparing `pytest-logikal-1.8.4/LICENSE.txt` & `pytest-logikal-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/PKG-INFO` & `pytest-logikal-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.4
+Version: 1.9.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.4/entry_points.ini` & `pytest-logikal-1.9.0/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pyproject.toml` & `pytest-logikal-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/bandit.py` & `pytest-logikal-1.9.0/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/browser.py` & `pytest-logikal-1.9.0/pytest_logikal/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import inspect
 import logging
 import re
 from contextlib import contextmanager
 from importlib import import_module
 from operator import itemgetter
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterable, Iterator, Optional, TypeVar, Union, cast
+from typing import Any, Dict, Iterable, Iterator, Optional, TypeVar, Union, cast
 
 import pytest
 from selenium.common.exceptions import SessionNotCreatedException
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.webdriver import WebDriver as Chrome
 
 from pytest_logikal.core import PYPROJECT
-from pytest_logikal.utils import Function, assert_image_equal
+from pytest_logikal.utils import Fixture, Function, assert_image_equal
 
 logger = logging.getLogger(__name__)
 
-Fixture = Callable[[Function], Function]
 Setting = TypeVar('Setting')
 
 
 class BrowserSettings:  # pylint: disable=too-many-instance-attributes
     UNLIMITED_HEIGHT = 'unlimited'
     FRAME_HEIGHT = 'frame'
```

### Comparing `pytest-logikal-1.8.4/pytest_logikal/build.py` & `pytest-logikal-1.9.0/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/core.py` & `pytest-logikal-1.9.0/pytest_logikal/core.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/css.py` & `pytest-logikal-1.9.0/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/css_config.yml` & `pytest-logikal-1.9.0/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/docker.py` & `pytest-logikal-1.9.0/pytest_logikal/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/docs.py` & `pytest-logikal-1.9.0/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/file_checker.py` & `pytest-logikal-1.9.0/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/html.py` & `pytest-logikal-1.9.0/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/isort.py` & `pytest-logikal-1.9.0/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/js.py` & `pytest-logikal-1.9.0/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/js_config.yml` & `pytest-logikal-1.9.0/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/licenses.py` & `pytest-logikal-1.9.0/pytest_logikal/licenses.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/package-lock.json` & `pytest-logikal-1.9.0/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/plugin.py` & `pytest-logikal-1.9.0/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/pylint.py` & `pytest-logikal-1.9.0/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/requirements.py` & `pytest-logikal-1.9.0/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/style.py` & `pytest-logikal-1.9.0/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/svg.py` & `pytest-logikal-1.9.0/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal/utils.py` & `pytest-logikal-1.9.0/pytest_logikal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from PIL import Image, ImageChops
 
 from pytest_logikal.core import DEFAULT_INI_OPTIONS, PYPROJECT
 
 logger = getLogger(__name__)
 
 Function = TypeVar('Function', bound=Callable[..., Any])
+Fixture = Callable[[Function], Function]
 
 
 def get_ini_option(name: str) -> Any:
     ini_options = PYPROJECT.get('tool', {}).get('pytest', {}).get('ini_options', {})
     default = DEFAULT_INI_OPTIONS[name]['value']
     return type(default)(ini_options.get(name, default))
```

### Comparing `pytest-logikal-1.8.4/pytest_logikal/validator.py` & `pytest-logikal-1.9.0/pytest_logikal/validator.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal.egg-info/PKG-INFO` & `pytest-logikal-1.9.0/pytest_logikal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.8.4
+Version: 1.9.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.8.4/pytest_logikal.egg-info/SOURCES.txt` & `pytest-logikal-1.9.0/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal.egg-info/entry_points.txt` & `pytest-logikal-1.9.0/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/pytest_logikal.egg-info/requires.txt` & `pytest-logikal-1.9.0/pytest_logikal.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 bandit==1.7.5
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
 isort[colors]==5.12.0
 mypy==1.3.0
-pip-licenses==4.3.1
+pip-licenses==4.3.2
 pycodestyle==2.10.0
 pydocstyle[toml]==6.3.0
 pylint==2.17.4
 pytest==7.3.1
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist[psutil]==3.3.0
-Pillow~=9.4
+pytest-xdist[psutil]==3.3.1
+Pillow~=9.5
 Pygments~=2.15
 docker~=6.1
 pyorbs~=2.0
 termcolor~=2.3
 tomli~=2.0
 
 [browser]
 selenium==4.9.1
 
 [django]
 Django~=4.2
 django-stubs~=4.2
 django-migration-linter~=4.1
-djlint==1.27.2
+djlint==1.29.0
 pylint-django==2.5.3
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 requests~=2.28
 types-requests~=2.28
```

### Comparing `pytest-logikal-1.8.4/requirements/build.txt.lock` & `pytest-logikal-1.9.0/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.8.4/requirements/dev.txt.lock` & `pytest-logikal-1.9.0/requirements/dev.txt.lock`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 0e455408c9c56e0a39bdb8aacd526635799e910415fdf1a72a6ed693a7454a65
+##  Requirements hash: dece568bc168a75c88ff894b8f452cf8fa0a42c59b4e08b4c9abc5eb952bd936
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
-asgiref==3.6.0
+asgiref==3.7.2
 astroid==2.15.5
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 bleach==6.0.0
 build==0.10.0
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
-coverage==7.2.5
+coverage==7.2.6
 cryptography==40.0.2
 cssbeautifier==1.14.7
 dill==0.3.6
 Django==4.2.1
 django-migration-linter==4.1.0
 django-stubs==4.2.0
 django-stubs-ext==4.2.0
-djlint==1.27.2
+djlint==1.29.0
 docker==6.1.2
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==18.7.0
+Faker==18.9.0
 filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 idna==3.4
@@ -69,49 +69,49 @@
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
-pip-licenses==4.3.1
+pip-licenses==4.3.2
 pkginfo==1.9.6
 platformdirs==3.5.1
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
-pylint-plugin-utils==0.8.1
+pylint-plugin-utils==0.8.2
 pyorbs==2.0.0
 pyproject_hooks==1.0.0
 PySocks==1.7.1
 pytest==7.3.1
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.3.0
+pytest-xdist==3.3.1
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
 readme-renderer==37.3
 regex==2023.5.5
-requests==2.30.0
+requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.3.5
 SecretStorage==3.3.3
 selenium==4.9.1
-setuptools==67.7.2
+setuptools==67.8.0
 six==1.16.0
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
@@ -128,19 +128,19 @@
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
 twine==4.0.2
 types-pytz==2023.3.0.0
-types-PyYAML==6.0.12.9
-types-requests==2.30.0.0
+types-PyYAML==6.0.12.10
+types-requests==2.31.0.0
 types-urllib3==1.26.25.13
-typing_extensions==4.5.0
+typing_extensions==4.6.2
 urllib3==2.0.2
 wcwidth==0.2.6
 webencodings==0.5.1
-websocket-client==1.5.1
+websocket-client==1.5.2
 wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

### Comparing `pytest-logikal-1.8.4/requirements/docs.txt.lock` & `pytest-logikal-1.9.0/requirements/docs.txt.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: d7e5b7eb5d25fb787135d9a9cd3f8e57d6592a677f77275b1a41f8a7d293f5d1
+##  Requirements hash: 096d2ffc0e6aca1b4cdb4e36f00f1e4af366c87b42c13ad65768c961cbcd1028
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
-asgiref==3.6.0
+asgiref==3.7.2
 astroid==2.15.5
 async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
-coverage==7.2.5
+coverage==7.2.6
 cssbeautifier==1.14.7
 dill==0.3.6
 Django==4.2.1
 django-migration-linter==4.1.0
 django-stubs==4.2.0
 django-stubs-ext==4.2.0
-djlint==1.27.2
+djlint==1.29.0
 docker==6.1.2
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==18.7.0
+Faker==18.9.0
 filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 idna==3.4
@@ -60,42 +60,42 @@
 mypy-extensions==1.0.0
 outcome==1.2.0
 packaging==23.1
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
-pip-licenses==4.3.1
+pip-licenses==4.3.2
 platformdirs==3.5.1
 pluggy==1.0.0
 prettytable==3.7.0
 psutil==5.9.5
 pycodestyle==2.10.0
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
-pylint-plugin-utils==0.8.1
+pylint-plugin-utils==0.8.2
 pyorbs==2.0.0
 PySocks==1.7.1
 pytest==7.3.1
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.3.0
+pytest-xdist==3.3.1
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
 regex==2023.5.5
-requests==2.30.0
+requests==2.31.0
 rich==13.3.5
 selenium==4.9.1
-setuptools==67.7.2
+setuptools==67.8.0
 six==1.16.0
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
@@ -111,18 +111,18 @@
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
 trio==0.22.0
 trio-websocket==0.10.2
 types-pytz==2023.3.0.0
-types-PyYAML==6.0.12.9
-types-requests==2.30.0.0
+types-PyYAML==6.0.12.10
+types-requests==2.31.0.0
 types-urllib3==1.26.25.13
-typing_extensions==4.5.0
+typing_extensions==4.6.2
 urllib3==2.0.2
 wcwidth==0.2.6
-websocket-client==1.5.1
+websocket-client==1.5.2
 wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

