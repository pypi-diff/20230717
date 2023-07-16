# Comparing `tmp/textframe-0.0.4.tar.gz` & `tmp/textframe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textframe-0.0.4.tar", last modified: Sun Jul 16 22:05:13 2023, max compression
+gzip compressed data, was "textframe-0.0.5.tar", last modified: Sun Jul 16 23:52:23 2023, max compression
```

## Comparing `textframe-0.0.4.tar` & `textframe-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:05:13.439645 textframe-0.0.4/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.4/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17390 2023-07-16 22:05:13.439645 textframe-0.0.4/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 textframe-0.0.4/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      586 2023-07-16 22:05:07.000000 textframe-0.0.4/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 22:05:13.439645 textframe-0.0.4/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:05:13.437645 textframe-0.0.4/textframe/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8989 2023-07-16 22:00:12.000000 textframe-0.0.4/textframe/TableString.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 21:34:02.000000 textframe-0.0.4/textframe/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:05:13.438645 textframe-0.0.4/textframe/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.4/textframe/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3935 2023-07-16 13:10:40.000000 textframe-0.0.4/textframe/chars/border_chars.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:05:13.438645 textframe-0.0.4/textframe/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.4/textframe/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1562 2023-07-16 21:34:02.000000 textframe-0.0.4/textframe/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.4/textframe/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2740 2023-07-16 21:34:02.000000 textframe-0.0.4/textframe/helpers/row_cross_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      490 2023-07-16 21:34:02.000000 textframe-0.0.4/textframe/helpers/row_outer_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       45 2023-07-16 22:04:44.000000 textframe-0.0.4/textframe/helpers/sanitize_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1300 2023-07-16 22:00:59.000000 textframe-0.0.4/textframe/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 textframe-0.0.4/textframe/type.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:05:13.437645 textframe-0.0.4/textframe.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17390 2023-07-16 22:05:13.000000 textframe-0.0.4/textframe.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      518 2023-07-16 22:05:13.000000 textframe-0.0.4/textframe.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 22:05:13.000000 textframe-0.0.4/textframe.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-16 22:05:13.000000 textframe-0.0.4/textframe.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.462437 textframe-0.0.5/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.5/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 23:52:23.461437 textframe-0.0.5/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    16877 2023-07-16 06:49:58.000000 textframe-0.0.5/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-16 22:50:19.000000 textframe-0.0.5/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-16 23:52:23.462437 textframe-0.0.5/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.459437 textframe-0.0.5/textframe/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 22:43:09.000000 textframe-0.0.5/textframe/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.460436 textframe-0.0.5/textframe/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9056 2023-07-16 23:20:46.000000 textframe-0.0.5/textframe/api/TextFrame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 textframe-0.0.5/textframe/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.460436 textframe-0.0.5/textframe/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.5/textframe/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 textframe-0.0.5/textframe/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 textframe-0.0.5/textframe/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 textframe-0.0.5/textframe/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-16 22:19:15.000000 textframe-0.0.5/textframe/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 textframe-0.0.5/textframe/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.461437 textframe-0.0.5/textframe/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.5/textframe/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2094 2023-07-16 23:08:04.000000 textframe-0.0.5/textframe/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.5/textframe/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3159 2023-07-16 23:45:46.000000 textframe-0.0.5/textframe/helpers/row_cross_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      535 2023-07-16 22:38:57.000000 textframe-0.0.5/textframe/helpers/row_outer_border.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.461437 textframe-0.0.5/textframe/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 textframe-0.0.5/textframe/tests/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2737 2023-07-16 23:48:25.000000 textframe-0.0.5/textframe/tests/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-16 10:37:16.000000 textframe-0.0.5/textframe/typing.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 23:52:23.459437 textframe-0.0.5/textframe.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    17392 2023-07-16 23:52:23.000000 textframe-0.0.5/textframe.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      687 2023-07-16 23:52:23.000000 textframe-0.0.5/textframe.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-16 23:52:23.000000 textframe-0.0.5/textframe.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-16 23:52:23.000000 textframe-0.0.5/textframe.egg-info/top_level.txt
```

### Comparing `textframe-0.0.4/LICENCE` & `textframe-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `textframe-0.0.4/PKG-INFO` & `textframe-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.4
-Summary: An ASCII text table renderer.
+Version: 0.0.5
+Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
-Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
-Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
+Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
+Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `textframe-0.0.4/README.md` & `textframe-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `textframe-0.0.4/pyproject.toml` & `textframe-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textframe"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
-description = "An ASCII text table renderer."
+description = "An ASCII plain text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.urls]
-"Homepage" = "https://gitlab.com/guydewinton/tablestring"
-"Bug Tracker" = "https://gitlab.com/guydewinton/tablestring/issues"
+"Homepage" = "https://gitlab.com/guydewinton/textframe"
+"Bug Tracker" = "https://gitlab.com/guydewinton/textframe/issues"
```

### Comparing `textframe-0.0.4/textframe/TableString.py` & `textframe-0.0.5/textframe/api/TextFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import math
 import shutil
 from typing import List, Dict
 
-from textframe.chars.border_chars import v_line, top_left, top_right, bottom_left, bottom_right
+from textframe.characters.corners import top_left, top_right, bottom_left, bottom_right
+from textframe.characters.line_v import v_line
 from textframe.helpers.is_last_element import is_last_element
 from textframe.helpers.row_cross_border import row_cross_line
 from textframe.helpers.row_outer_border import row_outer_border
 from textframe.helpers.cell_string import cell_string_single_line
-from textframe.type import BorderType, TableFrameColumnDict, TableFrameOption
+from textframe.typing import BorderType, TableFrameColumnDict, TableFrameOption
 
 
-class TableString:
+class TextFrame:
 
     _border: BorderType
     _left_padding: int
     _outer_width: 1
     _frame_divider: BorderType
 
     _output_frame_list = []
@@ -29,15 +30,15 @@
         self._left_padding = left_padding
         self._frame_divider = frame_divider
 
     def add_text_frame(self, text: str, multiline: bool = True, options=None):
         text_row = cell_string_single_line(text, self._outer_width - 2, 1, "left", "truncate")
 
         self._output_frame_list.append({
-            "v_lines": [],
+            "v_lines": [[self._outer_width - 2, "blank"]],
             "line_strings": [row_outer_border(text_row, self._border)],
             "base_divider": self._frame_divider,
         })
 
     # def add_grid_frame(self, text: str, multiline: bool, options):
     #     raise NotImplemented
 
@@ -79,21 +80,21 @@
                 if column_index in calculated_width_columns:
                     column_item["width"] = calculated_column_width
                 total_column_width += column_item["width"]
         else:
             total_column_width = total_defined_column_width
 
         if total_column_width + len(columns) + 1 > self._outer_width:
-            raise Exception(f"Table width exceeds '{TableString.__name__}' width by {total_column_width - self._outer_width}.")
+            raise Exception(f"Table width exceeds '{TextFrame.__name__}' width by {total_column_width - self._outer_width}.")
         if total_column_width + len(columns) + 1 < self._outer_width:
             if len(calculated_width_columns) > 0:
                 columns[calculated_width_columns[0]]["width"] += (self._outer_width - total_column_width) - (len(columns) + 1)
             else:
                 raise Exception(
-                    f"Table width exceeds '{TableString.__name__}' width by {total_column_width - self._outer_width}.")
+                    f"Table width exceeds '{TextFrame.__name__}' width by {total_column_width - self._outer_width}.")
 
         header_v_lines = []
         row_v_lines = []
         width_tally = 0
 
         for column_index, column_item in enumerate(columns):
             if column_index < len(columns):
```

### Comparing `textframe-0.0.4/textframe/helpers/cell_string.py` & `textframe-0.0.5/textframe/helpers/cell_string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import math
 from typing import Literal, List
 
-from textframe.type import Alignment
+from textframe.typing import Alignment
 
 
-def cell_string_single_line(string: str, width: int, padding: int, align: Alignment, resolve_excess_length: Literal["truncate", "raise"] = "truncate", truc_value: str = "...") -> str:
+def cell_string_single_line(string: str,
+                            width: int,
+                            padding: int,
+                            align: Alignment,
+                            resolve_excess_length: Literal["truncate", "raise"] = "truncate",
+                            truc_value: str = "...") -> str:
+
+    string = string.split("\n")[0]
+    string = " ".join(string.split("\t"))
 
     if len(string) + (padding * 2) > width:
         if resolve_excess_length == "raise":
             raise Exception(
                 f"The length of string '{string}' (+ padding of ({padding})) exceeds column width ({width}).")
         if resolve_excess_length == "truncate":
             slice_outer_index = width - ((padding * 2) + len(truc_value))
@@ -38,10 +46,21 @@
         return_string += string
 
     return_string += " " * padding
 
     return return_string
 
 
-def cell_string_multi_line(string: str, width: int, padding: int) -> List[str]:
+def cell_string_multi_line(string: str,
+                           width: int,
+                           padding: int,
+                           max_lines: int | None = None,
+                           resolve_excess_length: Literal["truncate", "raise"] = "truncate",
+                           truc_value: str = "...") -> List[str]:
+
+    # parse embedded new lines... => initial array
+
+
+
+
     pass
```

### Comparing `textframe-0.0.4/textframe/helpers/row_cross_border.py` & `textframe-0.0.5/textframe/helpers/row_cross_border.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from textframe.chars.border_chars import cross_matrix, h_line
-from textframe.type import BorderType
+from textframe.characters.line_h import h_line
+from textframe.characters.matrix_cross import cross_matrix
+from textframe.typing import BorderType
 
 
 def row_cross_line(divider: BorderType, v_line_list_top: list, v_line_list_bottom: list) -> str:
 
     """
     :param divider: BorderType
     :param v_line_list_top: [[col_width, BorderType]]
@@ -27,28 +28,35 @@
     cumulative_bottom.reverse()
 
     current_v_line_index = len(v_line_list_top) + len(v_line_list_bottom)
 
     while current_v_line_index > 0:
         if len(cumulative_top) > 0 and len(cumulative_bottom) > 0:
             if cumulative_top[-1][1] > cumulative_bottom[-1][1]:
+                # return_string += "one"
                 return_string += f"{h_line[divider] * cumulative_bottom[-1][0]}{cross_matrix['blank'][divider][cumulative_bottom[-1][2]]}"
                 cumulative_top[-1][0] = cumulative_top[-1][0] - cumulative_bottom[-1][0] - 1
                 cumulative_bottom.pop()
             elif cumulative_top[-1][1] == cumulative_bottom[-1][1]:
+                # return_string += "two"
                 return_string += f"{h_line[divider] * cumulative_bottom[-1][0]}{cross_matrix[cumulative_top[-1][2]][divider][cumulative_bottom[-1][2]]}"
                 cumulative_top.pop()
                 cumulative_bottom.pop()
             elif cumulative_top[-1][1] < cumulative_bottom[-1][1]:
+                # return_string += "three"
                 return_string += f"{h_line[divider] * cumulative_top[-1][0]}{cross_matrix[cumulative_top[-1][2]][divider]['blank']}"
                 cumulative_bottom[-1][0] = cumulative_bottom[-1][0] - cumulative_top[-1][0] - 1
                 cumulative_top.pop()
         else:
             if len(cumulative_top) > 0:
                 return_string += f"{h_line[divider] * cumulative_top[-1][0]}{cross_matrix[cumulative_top[-1][2]][divider]['blank']}"
+                if cumulative_top[-1][0] < 0:
+                    return_string = return_string[0:cumulative_top[-1][0]]
                 cumulative_top.pop()
             if len(cumulative_bottom) > 0:
                 return_string += f"{h_line[divider] * cumulative_bottom[-1][0]}{cross_matrix['blank'][divider][cumulative_bottom[-1][2]]}"
+                if cumulative_bottom[-1][0] < 0:
+                    return_string = return_string[0:cumulative_bottom[-1][0]]
                 cumulative_bottom.pop()
         current_v_line_index -= 1
     return return_string[0:-1]
```

### Comparing `textframe-0.0.4/textframe/test.py` & `textframe-0.0.5/textframe/tests/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from textframe.TableString import TableString
+import textframe as tf
 
-
-x = TableString(width=150, border="double")
+x = tf.TextFrame(width=150, border="double")
 
 column_list = [
     {
         "key": "Key One",
         "width":  20
     },
     {
@@ -20,22 +19,22 @@
     {
         "Key One": "Blah",
         "Key Two": "Blah",
         "Key Three": "Blah"
 
     },
     {
-        "Key One": "Blah",
+        "Key One": "Bla\nh",
         "Key Two": "Blah",
         "Key Three": "Blah"
 
     },
     {
-        "Key One": "Blah dfsdfsdfsdfkksdlfkjsdljflsdkjflsdkjflsdkjflksdjflsdkjflsdkjflsdkjflksdjflkdsjflksdjflkdsjfs",
-        "Key Two": "Blah",
+        "Key One": "Blah dfsdfsdfsdfkksdlfkjsdljflsdkjf\t\t\t\tlsdkjflsdkjflksdjflsdkjflsdkjflsdkjflksdjflkdsjflksdjflkdsjfs",
+        "Key Two": "B\nlah",
         "Key Three": "Blah s.kflsdjlsdkjflsdkjf;lskdjf;lkdjfls;kdjfl;skdjfsl;kdjflds;kfjsl;kdjfl;sdkjflsd;kjf;slkdjf;sdlkjf"
 
     },
 ]
 
 options = {
     "header_base_divider": "thick",
@@ -43,26 +42,99 @@
     "column_divider": "thin",
     "header_column_divider": "none",
     "frame_base_divider": "thick",
     # "header_align": "center"
 }
 
 x.add_table_frame(column_list, row_list, options)
-x.add_text_frame("This is my test", True, {})
+x.add_text_frame("This is my test")
+
 
+really_long_string = "kjslkjslkj\t dslkjlskdjf lkjl sdfklj sdklslk  ljlk lkdfjd\t slk kl lkfkds lk ds lkdslkj lk lk dslkjf\tdslkfslkfl kkl sdkldsfkljdsfkds lsdksdlkfs kll\tks  sdfkldskljdsfkls lskdfkl d"
+
+x.add_text_frame(really_long_string)
+x.add_text_frame(really_long_string)
 column_list2 = [
     {
         "key": "Key One",
         "width": 60,
         "align": "right"
     },
     {
         "key": "Key Two"
     },
     {
         "key": "Key Three"
     }
 ]
-x.add_table_frame(column_list2, row_list, options)
+
+options2 = {
+    "header_base_divider": "thick",
+    "row_line_divider": "blank",
+    "column_divider": "thin",
+    "header_column_divider": "none",
+    "frame_base_divider": "thick",
+    # "header_align": "center"
+}
+x.add_table_frame(column_list2, row_list, options2)
 
 x.print()
 
+column_list3 = [
+    {
+        "key": "Key One",
+        "align": "left"
+    },
+]
+
+options3 = {
+    "header_base_divider": "thick",
+    "row_line_divider": "thin",
+    "column_divider": "thin",
+    "header_column_divider": "thick",
+    "frame_base_divider": "thick",
+    # "header_align": "center"
+}
+
+x.add_table_frame(column_list3, row_list, options3)
+
+column_list4 = [
+    {
+        "key": "Key One",
+        "width": 60,
+        "align": "right"
+    },
+    {
+        "key": "Key Two"
+    },
+]
+x.add_table_frame(column_list4, row_list, options3)
+
+column_list5 = [
+    {
+        "key": "Key One",
+        "width": 60,
+        "align": "right"
+    },
+    {
+        "key": "Key Two"
+    },
+    {
+        "key": "Key One",
+        "align": "right"
+    },
+    {
+        "key": "Key Two"
+    },
+    {
+        "key": "Key One",
+        "align": "right"
+    },
+    {
+        "key": "Key Two"
+    },
+]
+
+x.add_table_frame(column_list5, row_list, options3)
+
+
+x.print()
```

### Comparing `textframe-0.0.4/textframe/type.py` & `textframe-0.0.5/textframe/typing.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.4/textframe.egg-info/PKG-INFO` & `textframe-0.0.5/textframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.4
-Summary: An ASCII text table renderer.
+Version: 0.0.5
+Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
-Project-URL: Homepage, https://gitlab.com/guydewinton/tablestring
-Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablestring/issues
+Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
+Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `textframe-0.0.4/textframe.egg-info/SOURCES.txt` & `textframe-0.0.5/textframe.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 LICENCE
 README.md
 pyproject.toml
-textframe/TableString.py
 textframe/__init__.py
-textframe/test.py
-textframe/type.py
+textframe/typing.py
 textframe.egg-info/PKG-INFO
 textframe.egg-info/SOURCES.txt
 textframe.egg-info/dependency_links.txt
 textframe.egg-info/top_level.txt
-textframe/chars/__init__.py
-textframe/chars/border_chars.py
+textframe/api/TextFrame.py
+textframe/api/__init__.py
+textframe/characters/__init__.py
+textframe/characters/corners.py
+textframe/characters/line_h.py
+textframe/characters/line_v.py
+textframe/characters/matrix_cross.py
+textframe/characters/matrix_side.py
 textframe/helpers/__init__.py
 textframe/helpers/cell_string.py
 textframe/helpers/is_last_element.py
 textframe/helpers/row_cross_border.py
 textframe/helpers/row_outer_border.py
-textframe/helpers/sanitize_text.py
+textframe/tests/__init__.py
+textframe/tests/test.py
```

