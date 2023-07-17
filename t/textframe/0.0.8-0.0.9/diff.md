# Comparing `tmp/textframe-0.0.8.tar.gz` & `tmp/textframe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textframe-0.0.8.tar", last modified: Mon Jul 17 19:50:53 2023, max compression
+gzip compressed data, was "textframe-0.0.9.tar", last modified: Mon Jul 17 19:54:10 2023, max compression
```

## Comparing `textframe-0.0.8.tar` & `textframe-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.312926 textframe-0.0.8/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.8/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 19:50:53.311926 textframe-0.0.8/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 textframe-0.0.8/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-17 19:50:43.000000 textframe-0.0.8/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-17 19:50:53.312926 textframe-0.0.8/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.307926 textframe-0.0.8/textframe/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 22:43:09.000000 textframe-0.0.8/textframe/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.309926 textframe-0.0.8/textframe/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    15426 2023-07-17 17:48:39.000000 textframe-0.0.8/textframe/api/TextFrame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 textframe-0.0.8/textframe/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.309926 textframe-0.0.8/textframe/characters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.8/textframe/characters/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 textframe-0.0.8/textframe/characters/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 textframe-0.0.8/textframe/characters/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 textframe-0.0.8/textframe/characters/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-16 22:19:15.000000 textframe-0.0.8/textframe/characters/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 textframe-0.0.8/textframe/characters/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.311926 textframe-0.0.8/textframe/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.8/textframe/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4177 2023-07-17 19:49:53.000000 textframe-0.0.8/textframe/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3520 2023-07-17 09:40:41.000000 textframe-0.0.8/textframe/helpers/grid_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.8/textframe/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3051 2023-07-17 17:48:39.000000 textframe-0.0.8/textframe/helpers/row_frame_divider.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      536 2023-07-17 01:05:28.000000 textframe-0.0.8/textframe/helpers/row_outer_border.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.311926 textframe-0.0.8/textframe/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 textframe-0.0.8/textframe/tests/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6964 2023-07-17 17:57:53.000000 textframe-0.0.8/textframe/tests/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      823 2023-07-17 09:25:26.000000 textframe-0.0.8/textframe/typing.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:50:53.308926 textframe-0.0.8/textframe.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 19:50:53.000000 textframe-0.0.8/textframe.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      720 2023-07-17 19:50:53.000000 textframe-0.0.8/textframe.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-17 19:50:53.000000 textframe-0.0.8/textframe.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-17 19:50:53.000000 textframe-0.0.8/textframe.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.419393 textframe-0.0.9/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.9/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 19:54:10.419393 textframe-0.0.9/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 textframe-0.0.9/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-17 19:52:51.000000 textframe-0.0.9/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-17 19:54:10.419393 textframe-0.0.9/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.416393 textframe-0.0.9/textframe/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 22:43:09.000000 textframe-0.0.9/textframe/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.417393 textframe-0.0.9/textframe/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    15439 2023-07-17 19:54:04.000000 textframe-0.0.9/textframe/api/TextFrame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 textframe-0.0.9/textframe/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.418393 textframe-0.0.9/textframe/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.9/textframe/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 textframe-0.0.9/textframe/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 textframe-0.0.9/textframe/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 textframe-0.0.9/textframe/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-16 22:19:15.000000 textframe-0.0.9/textframe/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 textframe-0.0.9/textframe/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.418393 textframe-0.0.9/textframe/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.9/textframe/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4177 2023-07-17 19:49:53.000000 textframe-0.0.9/textframe/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3520 2023-07-17 09:40:41.000000 textframe-0.0.9/textframe/helpers/grid_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.9/textframe/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3051 2023-07-17 17:48:39.000000 textframe-0.0.9/textframe/helpers/row_frame_divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      536 2023-07-17 01:05:28.000000 textframe-0.0.9/textframe/helpers/row_outer_border.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.419393 textframe-0.0.9/textframe/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 textframe-0.0.9/textframe/tests/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6964 2023-07-17 17:57:53.000000 textframe-0.0.9/textframe/tests/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      823 2023-07-17 09:25:26.000000 textframe-0.0.9/textframe/typing.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 19:54:10.417393 textframe-0.0.9/textframe.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 19:54:10.000000 textframe-0.0.9/textframe.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      720 2023-07-17 19:54:10.000000 textframe-0.0.9/textframe.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-17 19:54:10.000000 textframe-0.0.9/textframe.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-17 19:54:10.000000 textframe-0.0.9/textframe.egg-info/top_level.txt
```

### Comparing `textframe-0.0.8/LICENCE` & `textframe-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/PKG-INFO` & `textframe-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `textframe-0.0.8/README.md` & `textframe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/pyproject.toml` & `textframe-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textframe"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII plain text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `textframe-0.0.8/textframe/api/TextFrame.py` & `textframe-0.0.9/textframe/api/TextFrame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import shutil
 import time
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 from textframe.characters.corners import top_left, top_right, bottom_left, bottom_right
 from textframe.characters.line_v import v_line
 from textframe.helpers.is_last_element import is_last_element
 from textframe.helpers.row_frame_divider import row_frame_divider
 from textframe.helpers.row_outer_border import row_outer_border
 from textframe.helpers.cell_string import cell_string_single_line, cell_string_multi_line
@@ -27,15 +27,15 @@
                  left_padding: int = 1,
                  frame_divider: BorderType = "thick"):
         self._border = border if border != 'none' else 'blank'
         self._outer_width = width if width else shutil.get_terminal_size((120 + (left_padding * 2), 0))[0] - (left_padding * 2)
         self._left_padding = left_padding
         self._frame_divider = frame_divider
 
-    def add_text_frame(self, text: str, multiline: bool = True, max_lines: int | None = None, options=None):
+    def add_text_frame(self, text: str, multiline: bool = True, max_lines: Optional[int] = None, options=None):
         line_strings_array = []
         if multiline:
             multiline_array = cell_string_multi_line(string=text,
                                                      width=self._outer_width - 2,
                                                      padding=1,
                                                      max_lines=max_lines)
             for multiline_item in multiline_array:
```

### Comparing `textframe-0.0.8/textframe/characters/matrix_cross.py` & `textframe-0.0.9/textframe/characters/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/characters/matrix_side.py` & `textframe-0.0.9/textframe/characters/matrix_side.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/helpers/cell_string.py` & `textframe-0.0.9/textframe/helpers/cell_string.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/helpers/grid_frame.py` & `textframe-0.0.9/textframe/helpers/grid_frame.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/helpers/row_frame_divider.py` & `textframe-0.0.9/textframe/helpers/row_frame_divider.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/helpers/row_outer_border.py` & `textframe-0.0.9/textframe/helpers/row_outer_border.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/tests/test.py` & `textframe-0.0.9/textframe/tests/test.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe/typing.py` & `textframe-0.0.9/textframe/typing.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.8/textframe.egg-info/PKG-INFO` & `textframe-0.0.9/textframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `textframe-0.0.8/textframe.egg-info/SOURCES.txt` & `textframe-0.0.9/textframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

