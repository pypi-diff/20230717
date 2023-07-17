# Comparing `tmp/yotpy-0.0.88.tar.gz` & `tmp/yotpy-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.88.tar", last modified: Thu Jul 13 05:57:28 2023, max compression
+gzip compressed data, was "yotpy-0.0.89.tar", last modified: Mon Jul 17 18:54:39 2023, max compression
```

## Comparing `yotpy-0.0.88.tar` & `yotpy-0.0.89.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.88/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.88/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.88/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.88/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.88/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.88/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.88/docs/yotpy.html
--rw-r--r--   0        0        0      847 2023-06-05 17:53:47.739564 yotpy-0.0.88/pyproject.toml
--rw-r--r--   0        0        0      318 2023-07-13 05:56:36.958537 yotpy-0.0.88/yotpy/__init__.py
--rw-r--r--   0        0        0    34571 2023-07-13 05:55:39.817008 yotpy-0.0.88/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.88/yotpy/exceptions.py
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yotpy-0.0.88/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.89/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.89/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.89/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.89/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.89/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.89/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.89/docs/yotpy.html
+-rw-r--r--   0        0        0      847 2023-06-05 17:53:47.739564 yotpy-0.0.89/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-07-17 18:53:32.379867 yotpy-0.0.89/yotpy/__init__.py
+-rw-r--r--   0        0        0    34090 2023-07-17 18:53:20.545865 yotpy-0.0.89/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.89/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yotpy-0.0.89/PKG-INFO
```

### Comparing `yotpy-0.0.88/.github/workflows/static.yml` & `yotpy-0.0.89/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/LICENSE` & `yotpy-0.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/docs/search.js` & `yotpy-0.0.89/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/docs/yotpy.html` & `yotpy-0.0.89/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/pyproject.toml` & `yotpy-0.0.89/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/yotpy/core.py` & `yotpy-0.0.89/yotpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,65 +352,56 @@
 
         # Reset the BytesIO object's position to the beginning
         csv_bytesio.seek(0)
 
         return csv_bytesio
 
     @staticmethod
-    def to_xlsx_bytesio(headers: set, rows: list[dict], helper: bool = False) -> BytesIO:
+    def to_xlsx_bytesio(headers: set, rows: list[dict]) -> BytesIO:
         """
         Convert a list of rows into a Excel formatted BytesIO object.
-
         This method takes a list of rows (dictionaries) and a set of headers, and writes them into
         an Excel formatted BytesIO object. It can be used to create an Excel file-like object without
         creating an actual file on the filesystem.
-
         Args:
             headers (set): A set of headers to use for the Excel data.
             rows (list[dict]): A list of rows to convert into an Excel formatted BytesIO object.
-            helper (bool, optional): If True, enables automatic parsing and filling of unformatted data. Defaults to False.
-
         Returns:
             BytesIO: An Excel formatted BytesIO object.
         """
-
-        # Helper function used to parse a usable value when a value error is throw.
-        def value_parser(value, header):
-            if isinstance(value, list | set):
-                return value.pop() if len(value) else ""
-            elif isinstance(value, tuple):
-                return value[0] if len(value) else ""
-            elif isinstance(value, dict):
-                return value.get(header, "")
-
         # Create a Workbook object
         wb = Workbook()
         ws = wb.active
 
         # Write headers
         ws.append(list(headers))
 
+        def retrv(obj):
+            if hasattr(obj, 'pop') and len(obj) == 1:
+                return obj.pop()
+            elif isinstance(obj, set):
+                return ';'.join(obj)
+            else:
+                return obj
+
         # Write rows
         for row in rows:
-            for header in headers:
-                try:
-                    ws.append(row[header])
-                except ValueError:
-                    ws.append(value_parser(row[header], header))
+            ws.append([retrv(row[h]) for h in headers])
 
         # Save workbook to a BytesIO object
         xlsx_bytesio = BytesIO()
         wb.save(xlsx_bytesio)
 
         # Reset the BytesIO object's position to the beginning
         xlsx_bytesio.seek(0)
 
         return xlsx_bytesio
 
 
+
 class YotpoAPIWrapper:
     # NOTE: Update docstring if more methods are added to account for any added functionality outside of the defined scope.
     """
     A class for interacting with the Yotpo API to fetch app and account information, review data, and send manual review requests.
 
     The YotpoAPIWrapper uses the provided app_key and secret for authentication and constructs the necessary API endpoints for making requests.
```

### Comparing `yotpy-0.0.88/yotpy/exceptions.py` & `yotpy-0.0.89/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.88/PKG-INFO` & `yotpy-0.0.89/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.88
+Version: 0.0.89
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

