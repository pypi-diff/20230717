# Comparing `tmp/arrangio-0.2.0.tar.gz` & `tmp/arrangio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrangio-0.2.0.tar", last modified: Mon Jul 10 10:26:14 2023, max compression
+gzip compressed data, was "arrangio-0.3.0.tar", last modified: Mon Jul 17 18:14:53 2023, max compression
```

## Comparing `arrangio-0.2.0.tar` & `arrangio-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.877805 arrangio-0.2.0/
--rw-r--r--   0 fscm       (501) staff       (20)     1089 2023-06-13 12:35:35.000000 arrangio-0.2.0/LICENSE
--rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-10 10:26:14.877240 arrangio-0.2.0/PKG-INFO
--rw-r--r--   0 fscm       (501) staff       (20)     2864 2023-06-21 15:52:17.000000 arrangio-0.2.0/README.md
--rw-r--r--   0 fscm       (501) staff       (20)     6616 2023-06-21 15:36:55.000000 arrangio-0.2.0/pyproject.toml
--rw-r--r--   0 fscm       (501) staff       (20)       38 2023-07-10 10:26:14.878100 arrangio-0.2.0/setup.cfg
--rw-r--r--   0 fscm       (501) staff       (20)      266 2023-06-13 12:35:00.000000 arrangio-0.2.0/setup.py
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.855676 arrangio-0.2.0/src/
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.866629 arrangio-0.2.0/src/arrangio/
--rw-r--r--   0 fscm       (501) staff       (20)     1647 2023-07-10 10:23:47.000000 arrangio-0.2.0/src/arrangio/__init__.py
--rw-r--r--   0 fscm       (501) staff       (20)      143 2023-06-20 17:04:15.000000 arrangio-0.2.0/src/arrangio/__init__.pyi
--rw-r--r--   0 fscm       (501) staff       (20)     1126 2023-06-21 15:36:11.000000 arrangio-0.2.0/src/arrangio/__main__.py
--rw-r--r--   0 fscm       (501) staff       (20)     1928 2023-06-21 15:39:17.000000 arrangio-0.2.0/src/arrangio/_parser_.py
--rw-r--r--   0 fscm       (501) staff       (20)      112 2023-06-20 17:04:08.000000 arrangio-0.2.0/src/arrangio/_parser_.pyi
--rw-r--r--   0 fscm       (501) staff       (20)     4588 2023-07-10 10:03:19.000000 arrangio-0.2.0/src/arrangio/_utils_.py
--rw-r--r--   0 fscm       (501) staff       (20)      203 2023-06-20 17:04:08.000000 arrangio-0.2.0/src/arrangio/_utils_.pyi
--rw-r--r--   0 fscm       (501) staff       (20)        0 2023-06-13 13:25:12.000000 arrangio-0.2.0/src/arrangio/py.typed
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.872349 arrangio-0.2.0/src/arrangio.egg-info/
--rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/PKG-INFO
--rw-r--r--   0 fscm       (501) staff       (20)      525 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/SOURCES.txt
--rw-r--r--   0 fscm       (501) staff       (20)        1 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/dependency_links.txt
--rw-r--r--   0 fscm       (501) staff       (20)       52 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/entry_points.txt
--rw-r--r--   0 fscm       (501) staff       (20)      177 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/requires.txt
--rw-r--r--   0 fscm       (501) staff       (20)        9 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/top_level.txt
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.875229 arrangio-0.2.0/tests/
--rw-r--r--   0 fscm       (501) staff       (20)     3282 2023-07-10 10:18:03.000000 arrangio-0.2.0/tests/test___main__.py
--rw-r--r--   0 fscm       (501) staff       (20)     1822 2023-06-21 13:59:31.000000 arrangio-0.2.0/tests/test__parser_.py
--rw-r--r--   0 fscm       (501) staff       (20)     4435 2023-07-10 10:09:47.000000 arrangio-0.2.0/tests/test__utils_.py
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-17 18:14:53.489432 arrangio-0.3.0/
+-rw-r--r--   0 fscm       (501) staff       (20)     1089 2023-06-13 12:35:35.000000 arrangio-0.3.0/LICENSE
+-rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-17 18:14:53.488743 arrangio-0.3.0/PKG-INFO
+-rw-r--r--   0 fscm       (501) staff       (20)     2864 2023-06-21 15:52:17.000000 arrangio-0.3.0/README.md
+-rw-r--r--   0 fscm       (501) staff       (20)     6616 2023-06-21 15:36:55.000000 arrangio-0.3.0/pyproject.toml
+-rw-r--r--   0 fscm       (501) staff       (20)       38 2023-07-17 18:14:53.489892 arrangio-0.3.0/setup.cfg
+-rw-r--r--   0 fscm       (501) staff       (20)      266 2023-06-13 12:35:00.000000 arrangio-0.3.0/setup.py
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-17 18:14:53.467102 arrangio-0.3.0/src/
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-17 18:14:53.478915 arrangio-0.3.0/src/arrangio/
+-rw-r--r--   0 fscm       (501) staff       (20)     1680 2023-07-17 18:13:12.000000 arrangio-0.3.0/src/arrangio/__init__.py
+-rw-r--r--   0 fscm       (501) staff       (20)      143 2023-06-20 17:04:15.000000 arrangio-0.3.0/src/arrangio/__init__.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)     1141 2023-07-17 17:36:30.000000 arrangio-0.3.0/src/arrangio/__main__.py
+-rw-r--r--   0 fscm       (501) staff       (20)     1928 2023-06-21 15:39:17.000000 arrangio-0.3.0/src/arrangio/_parser_.py
+-rw-r--r--   0 fscm       (501) staff       (20)      112 2023-06-20 17:04:08.000000 arrangio-0.3.0/src/arrangio/_parser_.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)     5131 2023-07-17 17:46:56.000000 arrangio-0.3.0/src/arrangio/_utils_.py
+-rw-r--r--   0 fscm       (501) staff       (20)      245 2023-07-17 17:37:41.000000 arrangio-0.3.0/src/arrangio/_utils_.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)        0 2023-06-13 13:25:12.000000 arrangio-0.3.0/src/arrangio/py.typed
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-17 18:14:53.484061 arrangio-0.3.0/src/arrangio.egg-info/
+-rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/PKG-INFO
+-rw-r--r--   0 fscm       (501) staff       (20)      525 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/SOURCES.txt
+-rw-r--r--   0 fscm       (501) staff       (20)        1 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/dependency_links.txt
+-rw-r--r--   0 fscm       (501) staff       (20)       52 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/entry_points.txt
+-rw-r--r--   0 fscm       (501) staff       (20)      177 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/requires.txt
+-rw-r--r--   0 fscm       (501) staff       (20)        9 2023-07-17 18:14:53.000000 arrangio-0.3.0/src/arrangio.egg-info/top_level.txt
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-17 18:14:53.487409 arrangio-0.3.0/tests/
+-rw-r--r--   0 fscm       (501) staff       (20)     3758 2023-07-17 18:11:19.000000 arrangio-0.3.0/tests/test___main__.py
+-rw-r--r--   0 fscm       (501) staff       (20)     1822 2023-06-21 13:59:31.000000 arrangio-0.3.0/tests/test__parser_.py
+-rw-r--r--   0 fscm       (501) staff       (20)     5957 2023-07-17 17:58:35.000000 arrangio-0.3.0/tests/test__utils_.py
```

### Comparing `arrangio-0.2.0/LICENSE` & `arrangio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrangio-0.2.0/PKG-INFO` & `arrangio-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrangio
-Version: 0.2.0
+Version: 0.3.0
 Summary: Arranges a set of songs in groups with similar total play time.
 Author: Frederico Martins
 License: MIT
 Project-URL: Documentation, http://electric-mass.github.io/arrangio
 Project-URL: Homepage, https://github.com/electric-mass//arrangio
 Project-URL: Source, https://github.com/electric-mass/arrangio
 Keywords: songs,grouping
```

### Comparing `arrangio-0.2.0/README.md` & `arrangio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arrangio-0.2.0/pyproject.toml` & `arrangio-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arrangio-0.2.0/src/arrangio/__init__.py` & `arrangio-0.3.0/src/arrangio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,17 @@
   -g [NUM], --groups [NUM]
                         number of groups to create (default: 2)
   -q, --quiet           quiet mode (default: False)
   -s LABEL:HHhMMmSSs [LABEL:HHhMMmSSs ...], --song LABEL:HHhMMmSSs [LABEL:HHhMMmSSs ...]
                         song information (e.g.: label:00h03m27s) (default: None)
   -v, --version         show program's version number and exit
 ```
-"""
+"""  # pylint: disable=line-too-long
 
 from typing import Final
 
 __all__: Final[tuple] = ()
 
 __author__: Final[str] = 'Electric Mass Records'
 __license__: Final[str] = 'MIT'
 __project__: Final[str] = __package__
-__version__: Final[str] = '0.2.0'
+__version__: Final[str] = '0.3.0'
```

### Comparing `arrangio-0.2.0/src/arrangio/_parser_.py` & `arrangio-0.3.0/src/arrangio/_parser_.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.2.0/src/arrangio/_utils_.py` & `arrangio-0.3.0/src/arrangio/_utils_.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 | get_subsets  | `list(tuple(int, list))`  | gets the subsets of songs |
 | show_results | `None`                    | shows the results         |
 
 All other resources in this module are considered implementation
 details.
 """
 
-from functools import lru_cache as cache
 from datetime import datetime as _datetime, timedelta as _timedelta
+from functools import lru_cache as cache
+from json import dumps as _dumps
 from re import compile as _compile
 from typing import Final
 
 
 REGXPR: Final[str] = (
     r'^(?P<label>\w+):'
     r'((?P<hours>\d+)h)?((?P<minutes>\d+)m)?(?P<seconds>\d+)s$')
@@ -133,14 +134,31 @@
     subsets = ((0, ()),) * num
     return __get_subsets(
         songs,
         songs_length,
         subsets)
 
 
+def show_json(result: tuple) -> None:
+    """Parses result of `get_subsets` and prints it to the screen as
+    json.
+
+    Args:
+        result (tuple(int, list()): the result from `get_subsets`.
+    """
+    _groups = []
+    for idx, subset in enumerate(result[1]):
+        _group = {
+            'id': idx,
+            'lenght': subset[0],
+            'songs': [{'name': n, 'lenght': l} for (l, n) in subset[1]]}
+        _groups.append(_group)
+    print(_dumps({'difference': result[0], 'groups': _groups}))
+
+
 def show_results(result: tuple) -> None:
     """Parses result of `get_subsets` and prints it to the screen.
 
     Args:
         result (tuple(int, list()): the result from `get_subsets`.
     """
     print('Difference (in seconds):', result[0])
```

### Comparing `arrangio-0.2.0/src/arrangio.egg-info/PKG-INFO` & `arrangio-0.3.0/src/arrangio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrangio
-Version: 0.2.0
+Version: 0.3.0
 Summary: Arranges a set of songs in groups with similar total play time.
 Author: Frederico Martins
 License: MIT
 Project-URL: Documentation, http://electric-mass.github.io/arrangio
 Project-URL: Homepage, https://github.com/electric-mass//arrangio
 Project-URL: Source, https://github.com/electric-mass/arrangio
 Keywords: songs,grouping
```

### Comparing `arrangio-0.2.0/src/arrangio.egg-info/SOURCES.txt` & `arrangio-0.3.0/src/arrangio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrangio-0.2.0/tests/test__parser_.py` & `arrangio-0.3.0/tests/test__parser_.py`

 * *Files identical despite different names*

