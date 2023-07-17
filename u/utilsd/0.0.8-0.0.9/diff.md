# Comparing `tmp/utilsd-0.0.8.tar.gz` & `tmp/utilsd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsd-0.0.8.tar", last modified: Tue Jun  8 08:06:24 2021, max compression
+gzip compressed data, was "utilsd-0.0.9.tar", last modified: Wed Jun  9 09:55:32 2021, max compression
```

## Comparing `utilsd-0.0.8.tar` & `utilsd-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.488604 utilsd-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-06-08 08:06:24.484604 utilsd-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-06-08 08:06:13.000000 utilsd-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-08 08:06:24.488604 utilsd-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-06-08 08:06:13.000000 utilsd-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/avgmeter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/config/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/config/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/config/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    14878 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/config/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/earlystop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5097 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/fileio/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23935 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4754 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/fileio/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd/search/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/search/confext.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/search/confgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-06-08 08:06:13.000000 utilsd-0.0.8/utilsd/search/space.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-08 08:06:24.484604 utilsd-0.0.8/utilsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-06-08 08:06:24.000000 utilsd-0.0.8/utilsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-08 08:06:24.000000 utilsd-0.0.8/utilsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-08 08:06:24.000000 utilsd-0.0.8/utilsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-06-08 08:06:24.000000 utilsd-0.0.8/utilsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-08 08:06:24.000000 utilsd-0.0.8/utilsd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.535794 utilsd-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-06-09 09:55:32.535794 utilsd-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-06-09 09:55:22.000000 utilsd-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-09 09:55:32.535794 utilsd-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-06-09 09:55:22.000000 utilsd-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.515794 utilsd-0.0.9/utilsd/
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.519794 utilsd-0.0.9/utilsd/analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/avgmeter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.523794 utilsd-0.0.9/utilsd/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/config/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/config/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15060 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/config/python.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2664 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/earlystop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5097 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.523794 utilsd-0.0.9/utilsd/fileio/
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24129 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.535794 utilsd-0.0.9/utilsd/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4754 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/fileio/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3800 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.535794 utilsd-0.0.9/utilsd/search/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/search/confext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/search/confgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-06-09 09:55:22.000000 utilsd-0.0.9/utilsd/search/space.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 09:55:32.519794 utilsd-0.0.9/utilsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-06-09 09:55:32.000000 utilsd-0.0.9/utilsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-09 09:55:32.000000 utilsd-0.0.9/utilsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 09:55:32.000000 utilsd-0.0.9/utilsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-06-09 09:55:32.000000 utilsd-0.0.9/utilsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-09 09:55:32.000000 utilsd-0.0.9/utilsd.egg-info/top_level.txt
```

### Comparing `utilsd-0.0.8/PKG-INFO` & `utilsd-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsd
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common utils for deep learning.
 Home-page: https://github.com/ultmaster/utilsd
 Author: Yuge Zhang
 Author-email: scottyugochang@gmail.com
 License: UNKNOWN
 Description: # Common utils for deep learning
```

### Comparing `utilsd-0.0.8/README.md` & `utilsd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/setup.py` & `utilsd-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/analysis/__main__.py` & `utilsd-0.0.9/utilsd/analysis/__main__.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/analysis/pattern.py` & `utilsd-0.0.9/utilsd/analysis/pattern.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/analysis/pipeline.py` & `utilsd-0.0.9/utilsd/analysis/pipeline.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/analysis/utils.py` & `utilsd-0.0.9/utilsd/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/avgmeter.py` & `utilsd-0.0.9/utilsd/avgmeter.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/config/python.py` & `utilsd-0.0.9/utilsd/config/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 The second part of this file defines how `PythonConfig` can be written in yaml and command line arguments.
 """
 
 import dataclasses
 import inspect
 import json
 import os
+import warnings
 from argparse import SUPPRESS, ArgumentParser, ArgumentTypeError
 from dataclasses import fields, is_dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, TypeVar, Tuple, Union, Type, Generic
 
 from ..fileio.config import Config
@@ -374,11 +375,15 @@
 
         def type_fn(self): return t
         def build_fn(self, **kwargs):
             result = {f.name: getattr(self, f.name) for f in dataclasses.fields(self)}
             for k in kwargs:
                 # silently overwrite the arguments with given ones.
                 result[k] = kwargs[k]
-            return self.type()(**result)
+            try:
+                return self.type()(**result)
+            except:
+                warnings.warn(f'Error when constructing {self.type()} with {result}.', RuntimeWarning)
+                raise
 
         return dataclasses.make_dataclass(class_name, fields, bases=(cls,), init=False,
                                           namespace={'type': type_fn, 'build': build_fn})
```

### Comparing `utilsd-0.0.8/utilsd/config/registry.py` & `utilsd-0.0.9/utilsd/config/registry.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/earlystop.py` & `utilsd-0.0.9/utilsd/earlystop.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/experiment.py` & `utilsd-0.0.9/utilsd/experiment.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/config.py` & `utilsd-0.0.9/utilsd/fileio/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from addict import Dict
 from yapf.yapflib.yapf_api import FormatCode
 
 from .io import load as mmcv_load, dump as mmcv_dump
 
 BASE_KEY = '_base_'
 DELETE_KEY = '_delete_'
+CUSTOM_IMPORT_KEY = '_custom_imports_'
 RESERVED_KEYS = ['filename', 'text', 'pretty_text']
 
 
 def check_file_exist(filename, msg_tmpl='file "{}" does not exist'):
     if not osp.isfile(filename):
         raise FileNotFoundError(msg_tmpl.format(filename))
 
@@ -280,16 +281,18 @@
 
     @staticmethod
     def fromfile(filename,
                  use_predefined_variables=True,
                  import_custom_modules=True):
         cfg_dict, cfg_text = Config._file2dict(filename,
                                                use_predefined_variables)
-        if import_custom_modules and cfg_dict.get('custom_imports', None):
-            import_modules_from_strings(**cfg_dict['custom_imports'])
+        if import_custom_modules and cfg_dict.get(CUSTOM_IMPORT_KEY, None):
+            if not isinstance(cfg_dict[CUSTOM_IMPORT_KEY], list):
+                raise ValueError('_custom_imports_ must be a list of import paths.')
+            import_modules_from_strings(cfg_dict.pop(CUSTOM_IMPORT_KEY))
         return Config(cfg_dict, cfg_text=cfg_text, filename=filename)
 
     @staticmethod
     def fromstring(cfg_str, file_format):
         """Generate config from config str.
         Args:
             cfg_str (str): Config str.
```

### Comparing `utilsd-0.0.8/utilsd/fileio/handlers/base.py` & `utilsd-0.0.9/utilsd/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/handlers/json_handler.py` & `utilsd-0.0.9/utilsd/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/handlers/pickle_handler.py` & `utilsd-0.0.9/utilsd/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/handlers/yaml_handler.py` & `utilsd-0.0.9/utilsd/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/io.py` & `utilsd-0.0.9/utilsd/fileio/io.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/fileio/parse.py` & `utilsd-0.0.9/utilsd/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/logging.py` & `utilsd-0.0.9/utilsd/logging.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/search/confext.py` & `utilsd-0.0.9/utilsd/search/confext.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/search/confgen.py` & `utilsd-0.0.9/utilsd/search/confgen.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd/search/space.py` & `utilsd-0.0.9/utilsd/search/space.py`

 * *Files identical despite different names*

### Comparing `utilsd-0.0.8/utilsd.egg-info/PKG-INFO` & `utilsd-0.0.9/utilsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsd
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common utils for deep learning.
 Home-page: https://github.com/ultmaster/utilsd
 Author: Yuge Zhang
 Author-email: scottyugochang@gmail.com
 License: UNKNOWN
 Description: # Common utils for deep learning
```

### Comparing `utilsd-0.0.8/utilsd.egg-info/SOURCES.txt` & `utilsd-0.0.9/utilsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

