# Comparing `tmp/keras_pbar-0.0.1.dev2.tar.gz` & `tmp/keras_pbar-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_pbar-0.0.1.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "keras_pbar-0.0.1.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `keras_pbar-0.0.1.dev2.tar` & `keras_pbar-0.0.1.dev3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      502 2023-06-30 22:22:03.854543 keras_pbar-0.0.1.dev2/Readme.md
--rw-r--r--   0        0        0       45 2023-06-30 22:22:03.854543 keras_pbar-0.0.1.dev2/keras_pbar/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-30 22:22:03.854543 keras_pbar-0.0.1.dev2/keras_pbar/keras_pbar.py
--rw-r--r--   0        0        0       64 2023-06-30 22:22:03.854543 keras_pbar-0.0.1.dev2/keras_pbar/py.typed
--rw-r--r--   0        0        0      731 2023-06-30 22:22:03.854543 keras_pbar-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 keras_pbar-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-07-17 17:05:16.855727 keras_pbar-0.0.1.dev3/Readme.md
+-rw-r--r--   0        0        0       47 2023-07-17 17:05:16.855727 keras_pbar-0.0.1.dev3/keras_pbar/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-17 17:05:16.855727 keras_pbar-0.0.1.dev3/keras_pbar/keras_pbar.py
+-rw-r--r--   0        0        0       64 2023-07-17 17:05:16.855727 keras_pbar-0.0.1.dev3/keras_pbar/py.typed
+-rw-r--r--   0        0        0      643 2023-07-17 17:05:16.855727 keras_pbar-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 keras_pbar-0.0.1.dev3/PKG-INFO
```

### Comparing `keras_pbar-0.0.1.dev2/keras_pbar/keras_pbar.py` & `keras_pbar-0.0.1.dev3/keras_pbar/keras_pbar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 
 from typing import Sized, Iterable, TypeVar
-from keras.utils import Progbar
+from keras_core.utils import Progbar
 
 T = TypeVar("T")
 
 
-def keras_pbar(iterable: Iterable[T], n: int | None = None) -> Iterable[T]:
+def pbar(iterable: Iterable[T], n: int | None = None) -> Iterable[T]:
     """
     Prints Keras progress bar to stdout and updates it on every iteration.
 
     Parameters
     ----------
     iterable:
         The iterable for which progress bar should be displayed.
     n:
         If iterable is not sized, must explicitly provide the length.
 
-    Returns
+    Returns2
     -------
 
     it:
         Iterable, which updates progress bar on every step.
 
 
     Examples
     -------
     >>> import time
     >>> import pandas as pd
-    >>> from keras_pbar import keras_pbar
+    >>> from keras_pbar import pbar
     >>> df = pd.read_csv("data.csv")
-    >>> for identifier, sliced in keras_pbar(df.group_by("id")):
-    >>>     # Do some time consuming processing.
+    >>> for identifier, sliced in pbar(df.group_by("id")):
+    >>>     # Do some time-consuming processing.
     >>>     time.sleep(2)
 
     """
     if n is None:
         if not isinstance(iterable, Sized):
             raise ValueError("Must provide n, for not sized iterable.")
         n = len(iterable)
```

### Comparing `keras_pbar-0.0.1.dev2/pyproject.toml` & `keras_pbar-0.0.1.dev3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [project]
 name = "keras_pbar"
-version = "0.0.1dev2"
+version = "0.0.1dev3"
 description = "TQDM-like API for Keras Progressbar."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
 ]
 dependencies = [
-    "keras"
+    "keras_core"
 ]
 [project.optional-dependencies]
 dev = [
-    "tensorflow; sys_platform == 'linux'",
-    "tensorflow_macos; sys_platform == 'darwin'",
     "black",
     "pytest",
     "tox"
 ]
 [project.urls]
 "Homepage" = "https://github.com/aaarrti/keras_pbar"
 [build-system]
```

### Comparing `keras_pbar-0.0.1.dev2/PKG-INFO` & `keras_pbar-0.0.1.dev3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: keras_pbar
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: TQDM-like API for Keras Progressbar.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
-Requires-Dist: keras
-Requires-Dist: tensorflow ; extra == "dev" and ( sys_platform == 'linux')
-Requires-Dist: tensorflow_macos ; extra == "dev" and ( sys_platform == 'darwin')
+Requires-Dist: keras_core
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: tox ; extra == "dev"
 Project-URL: Homepage, https://github.com/aaarrti/keras_pbar
 Provides-Extra: dev
 
 # Keras Progressbar with TQDM-like API.
@@ -22,15 +20,18 @@
 So, I published this tiny module, in order to avoid copy-pasting it
 in every my project.
 
 ### Example usage
 ```python
 import time
 import pandas as pd
-from keras_pbar import keras_pbar
+from keras_pbar import pbar
 
 df = pd.read_csv("data.csv")
-for identifier, sliced in keras_pbar(df.group_by("id")):
+for identifier, sliced in pbar(df.group_by("id")):
     # Do some time consuming processing.
     time.sleep(2)
 ```
+### Notes
+It does not directly depend on `tensorflow`, so you can install it without.
+But probably during import time, it will fail, when `keras` tries to import `tensorlfow`.
```

