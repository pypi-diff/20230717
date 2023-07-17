# Comparing `tmp/textframe-0.0.6.tar.gz` & `tmp/textframe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textframe-0.0.6.tar", last modified: Mon Jul 17 17:44:10 2023, max compression
+gzip compressed data, was "textframe-0.0.7.tar", last modified: Mon Jul 17 17:48:49 2023, max compression
```

## Comparing `textframe-0.0.6.tar` & `textframe-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.797460 textframe-0.0.6/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.6/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 17:44:10.797460 textframe-0.0.6/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 textframe-0.0.6/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-17 17:43:45.000000 textframe-0.0.6/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-17 17:44:10.797460 textframe-0.0.6/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.793460 textframe-0.0.6/textframe/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 22:43:09.000000 textframe-0.0.6/textframe/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.794460 textframe-0.0.6/textframe/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    15824 2023-07-17 17:10:41.000000 textframe-0.0.6/textframe/api/TextFrame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 textframe-0.0.6/textframe/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.795460 textframe-0.0.6/textframe/characters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.6/textframe/characters/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 textframe-0.0.6/textframe/characters/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 textframe-0.0.6/textframe/characters/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 textframe-0.0.6/textframe/characters/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-16 22:19:15.000000 textframe-0.0.6/textframe/characters/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 textframe-0.0.6/textframe/characters/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.797460 textframe-0.0.6/textframe/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.6/textframe/helpers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4164 2023-07-17 09:25:26.000000 textframe-0.0.6/textframe/helpers/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3520 2023-07-17 09:40:41.000000 textframe-0.0.6/textframe/helpers/grid_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.6/textframe/helpers/is_last_element.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3196 2023-07-17 16:16:26.000000 textframe-0.0.6/textframe/helpers/row_frame_divider.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      536 2023-07-17 01:05:28.000000 textframe-0.0.6/textframe/helpers/row_outer_border.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.797460 textframe-0.0.6/textframe/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 textframe-0.0.6/textframe/tests/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6965 2023-07-17 17:12:00.000000 textframe-0.0.6/textframe/tests/test.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      823 2023-07-17 09:25:26.000000 textframe-0.0.6/textframe/typing.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:44:10.794460 textframe-0.0.6/textframe.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 17:44:10.000000 textframe-0.0.6/textframe.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      720 2023-07-17 17:44:10.000000 textframe-0.0.6/textframe.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-17 17:44:10.000000 textframe-0.0.6/textframe.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-17 17:44:10.000000 textframe-0.0.6/textframe.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.505621 textframe-0.0.7/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 textframe-0.0.7/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 17:48:49.504621 textframe-0.0.7/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 textframe-0.0.7/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-17 17:48:39.000000 textframe-0.0.7/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-17 17:48:49.505621 textframe-0.0.7/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.500621 textframe-0.0.7/textframe/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       47 2023-07-16 22:43:09.000000 textframe-0.0.7/textframe/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.502621 textframe-0.0.7/textframe/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    15426 2023-07-17 17:48:39.000000 textframe-0.0.7/textframe/api/TextFrame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 textframe-0.0.7/textframe/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.502621 textframe-0.0.7/textframe/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.7/textframe/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 textframe-0.0.7/textframe/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 textframe-0.0.7/textframe/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 textframe-0.0.7/textframe/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-16 22:19:15.000000 textframe-0.0.7/textframe/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 textframe-0.0.7/textframe/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.504621 textframe-0.0.7/textframe/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 textframe-0.0.7/textframe/helpers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4164 2023-07-17 09:25:26.000000 textframe-0.0.7/textframe/helpers/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3520 2023-07-17 09:40:41.000000 textframe-0.0.7/textframe/helpers/grid_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 textframe-0.0.7/textframe/helpers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3051 2023-07-17 17:48:39.000000 textframe-0.0.7/textframe/helpers/row_frame_divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      536 2023-07-17 01:05:28.000000 textframe-0.0.7/textframe/helpers/row_outer_border.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.504621 textframe-0.0.7/textframe/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 textframe-0.0.7/textframe/tests/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6965 2023-07-17 17:12:00.000000 textframe-0.0.7/textframe/tests/test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      823 2023-07-17 09:25:26.000000 textframe-0.0.7/textframe/typing.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-17 17:48:49.501621 textframe-0.0.7/textframe.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-17 17:48:49.000000 textframe-0.0.7/textframe.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      720 2023-07-17 17:48:49.000000 textframe-0.0.7/textframe.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-17 17:48:49.000000 textframe-0.0.7/textframe.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-17 17:48:49.000000 textframe-0.0.7/textframe.egg-info/top_level.txt
```

### Comparing `textframe-0.0.6/LICENCE` & `textframe-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/PKG-INFO` & `textframe-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.6
+Version: 0.0.7
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `textframe-0.0.6/README.md` & `textframe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/pyproject.toml` & `textframe-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textframe"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII plain text table renderer."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `textframe-0.0.6/textframe/api/TextFrame.py` & `textframe-0.0.7/textframe/api/TextFrame.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,17 +214,14 @@
 
         self._output_frame_list.append({
             "v_lines": header_v_lines,
             "line_strings": [row_outer_border(row_string=header_line_string, outer_border=self._border)],
             "base_divider": header_base_divider,
         })
 
-        start = time.perf_counter_ns()
-
-
         row_line_strings_list = []
         line_string = None
 
         if row_line_divider != "none":
             line_string = row_frame_divider(divider=row_line_divider,
                                             v_line_list_top=row_v_lines,
                                             v_line_list_bottom=row_v_lines)
@@ -255,22 +252,16 @@
 
         self._output_frame_list.append({
             "v_lines": row_v_lines,
             "line_strings": row_line_strings_list,
             "base_divider": frame_divider,
         })
 
-        end = time.perf_counter_ns()
-
-        print("add_table_frame()", end - start)
-
     def to_string(self):
 
-        start = time.perf_counter_ns()
-
         return_string = ""
         top_border_inner = row_frame_divider(divider=self._border,
                                              v_line_list_top=[],
                                              v_line_list_bottom=self._output_frame_list[0]["v_lines"])
         return_string += f"{' ' * self._left_padding}{top_left[self._border]}{top_border_inner}{top_right[self._border]}\n"
         for frame_index, frame_item in enumerate(self._output_frame_list):
             for row_index, row_item in enumerate(frame_item["line_strings"]):
@@ -285,18 +276,11 @@
                                                            row_divider=self._output_frame_list[frame_index]['base_divider'])
                     return_string += f"{' ' * self._left_padding}{frame_divider_outer}\n"
         bottom_border_inner = row_frame_divider(divider=self._border,
                                                 v_line_list_top=self._output_frame_list[-1]["v_lines"],
                                                 v_line_list_bottom=[])
         return_string += f"{' ' * self._left_padding}{bottom_left[self._border]}{bottom_border_inner}{bottom_right[self._border]}\n"
 
-        end = time.perf_counter_ns()
-        print("to_string()", end - start)
-
         return return_string
 
     def print(self):
-        print_string = self.to_string()
-        start = time.perf_counter_ns()
-        print(print_string)
-        end = time.perf_counter_ns()
-        print("print()", end - start)
+        print(self.to_string())
```

### Comparing `textframe-0.0.6/textframe/characters/matrix_cross.py` & `textframe-0.0.7/textframe/characters/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/characters/matrix_side.py` & `textframe-0.0.7/textframe/characters/matrix_side.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/helpers/cell_string.py` & `textframe-0.0.7/textframe/helpers/cell_string.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/helpers/grid_frame.py` & `textframe-0.0.7/textframe/helpers/grid_frame.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/helpers/row_frame_divider.py` & `textframe-0.0.7/textframe/helpers/row_frame_divider.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     """
     :param divider: BorderType
     :param v_line_list_top: [[col_width, BorderType]]
     :param v_line_list_bottom: [[col_width, BorderType]]
     :return: str
     """
 
-    start = time.perf_counter_ns()
-
     return_string = ""
 
     cumulative_top_count = 0
     cumulative_top = []
     for v_line_index in range(0, len(v_line_list_top),):
         cumulative_top_count += v_line_list_top[v_line_index][0]
         cumulative_top.append([v_line_list_top[v_line_index][0], cumulative_top_count, v_line_list_top[v_line_index][1]])
@@ -56,15 +54,9 @@
             if len(cumulative_bottom) > 0:
                 return_string += f"{h_line[divider] * cumulative_bottom[-1][0]}{cross_matrix['blank'][divider][cumulative_bottom[-1][2]]}"
                 if cumulative_bottom[-1][0] < 0:
                     return_string = return_string[0:cumulative_bottom[-1][0]]
                 cumulative_bottom.pop()
         current_v_line_index -= 1
 
-        end = time.perf_counter_ns()
-
-    print("row_frame_divider", end - start)
-
-    print(return_string)
-
     return return_string[0:-1]
```

### Comparing `textframe-0.0.6/textframe/helpers/row_outer_border.py` & `textframe-0.0.7/textframe/helpers/row_outer_border.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/tests/test.py` & `textframe-0.0.7/textframe/tests/test.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe/typing.py` & `textframe-0.0.7/textframe/typing.py`

 * *Files identical despite different names*

### Comparing `textframe-0.0.6/textframe.egg-info/PKG-INFO` & `textframe-0.0.7/textframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textframe
-Version: 0.0.6
+Version: 0.0.7
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `textframe-0.0.6/textframe.egg-info/SOURCES.txt` & `textframe-0.0.7/textframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

