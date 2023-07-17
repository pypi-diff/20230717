# Comparing `tmp/recurtx-0.0.8.tar.gz` & `tmp/recurtx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.8.tar", last modified: Tue Jul  4 13:18:58 2023, max compression
+gzip compressed data, was "recurtx-0.0.9.tar", last modified: Tue Jul  4 14:11:03 2023, max compression
```

## Comparing `recurtx-0.0.8.tar` & `recurtx-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-30 15:42:22.000000 recurtx-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 13:18:58.720000 recurtx-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5703 2023-06-30 15:42:22.000000 recurtx-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-01 00:45:28.000000 recurtx-0.0.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 15:42:22.000000 recurtx-0.0.8/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-07-01 15:45:17.000000 recurtx-0.0.8/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-07-04 12:47:23.000000 recurtx-0.0.8/recurtx/ll.py
--rw-r--r--   0 root         (0) root         (0)     7134 2023-06-30 15:42:22.000000 recurtx-0.0.8/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     5003 2023-07-01 15:43:03.000000 recurtx-0.0.8/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-07-04 13:12:02.000000 recurtx-0.0.8/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-06-30 15:42:23.000000 recurtx-0.0.8/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-07-04 12:47:05.000000 recurtx-0.0.8/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-04 13:18:58.730000 recurtx-0.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1547 2023-06-30 15:42:23.000000 recurtx-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:11:03.650000 recurtx-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-04 13:20:08.000000 recurtx-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 14:11:03.650000 recurtx-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-07-04 13:20:08.000000 recurtx-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-04 13:20:08.000000 recurtx-0.0.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:11:03.650000 recurtx-0.0.9/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/ll.py
+-rw-r--r--   0 root         (0) root         (0)     7134 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2023-07-04 14:03:26.000000 recurtx-0.0.9/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-07-04 13:20:09.000000 recurtx-0.0.9/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:11:03.650000 recurtx-0.0.9/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 14:11:03.000000 recurtx-0.0.9/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-04 14:11:03.650000 recurtx-0.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1547 2023-07-04 13:20:09.000000 recurtx-0.0.9/setup.py
```

### Comparing `recurtx-0.0.8/LICENSE` & `recurtx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/PKG-INFO` & `recurtx-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.8/README.md` & `recurtx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/pyproject.toml` & `recurtx-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/__main__.py` & `recurtx-0.0.9/recurtx/__main__.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/ll.py` & `recurtx-0.0.9/recurtx/ll.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/pandas.py` & `recurtx-0.0.9/recurtx/pandas.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/polars.py` & `recurtx-0.0.9/recurtx/polars.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/recur.py` & `recurtx-0.0.9/recurtx/recur.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx/search.py` & `recurtx-0.0.9/recurtx/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 from pathlib import Path
 from typing import List, Optional, Set, Tuple, Union
 
+from .utils import subprocess_run
+
 
 def run_search(
     text: str,
     target: Union[str, List, Tuple, Set],
     path: Path,
     sub: Optional[Union[str, List, Tuple, Set]] = None,
     wildcard: str = "*",
@@ -114,9 +116,11 @@
         path=_path,
         sub=sub,
         wildcard=wildcard,
         separator=separator,
         verbose=verbose,
     )
 
-    if sub is not None:
-        _path.rename(text)
+    if (sub is not None) and _path.exists():
+        sub_path = Path(text)
+        sub_path.parent.mkdir(parents=True, exist_ok=True)
+        subprocess_run(["mv", str(_path), str(sub_path)], verbose=False)
```

### Comparing `recurtx-0.0.8/recurtx/utils.py` & `recurtx-0.0.9/recurtx/utils.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.8/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.9/recurtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.8/setup.py` & `recurtx-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

