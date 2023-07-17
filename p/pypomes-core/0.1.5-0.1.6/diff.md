# Comparing `tmp/pypomes_core-0.1.5.tar.gz` & `tmp/pypomes_core-0.1.6.tar.gz`

## Comparing `pypomes_core-0.1.5.tar` & `pypomes_core-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/README.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.6/PKG-INFO
```

### Comparing `pypomes_core-0.1.5/src/pypomes_core/__init__.py` & `pypomes_core-0.1.6/src/pypomes_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .file_pomes import (
     file_from_request
 )
 from .http_pomes import (
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
-    http_status_name, http_status_description, htpp_json_from_get, htpp_json_from_post
+    http_status_name, http_status_description, http_json_from_get, http_json_from_post
 )
 from .json_pomes import (
     jsonify_dict, jsonify_iterable
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform
@@ -68,15 +68,15 @@
     exc_format,
     # file_pomes
     file_from_request,
     # http_pomes
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
-    http_status_name, http_status_description, htpp_json_from_get, htpp_json_from_post,
+    http_status_name, http_status_description, http_json_from_get, http_json_from_post,
     # json_pomes
     jsonify_dict, jsonify_iterable,
     # list_pomes
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
     # validation_pomes
     VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
@@ -85,9 +85,9 @@
     validate_format_error, validate_format_errors,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.5"
-__version_info__ = (0, 1, 5)
+__version__ = "0.1.6"
+__version_info__ = (0, 1, 6)
```

### Comparing `pypomes_core-0.1.5/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/email_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/env_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/file_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/http_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/http_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     item: dict = __HTTP_STATUS.get(status_code, {"description": "Unknown status code"})
     result = f"HTTP status code {status_code}: {item.get('description')}"
 
     return result
 
 
-def htpp_json_from_get(errors: list[str], url: str, headers: dict = None,
+def http_json_from_get(errors: list[str], url: str, headers: dict = None,
                        req_params: dict = None, logger: logging.Logger = None) -> dict:
 
     if logger is not None:
         logger.info(f"Invoking GET: '{url}'")
 
     # initialize return variable
     result: dict | None = None
@@ -226,15 +226,15 @@
         if logger is not None:
             logger.info(msg)
         errors.append(msg)
 
     return result
 
 
-def htpp_json_from_post(errors: list[str], url: str, headers: dict = None, req_params: dict = None,
+def http_json_from_post(errors: list[str], url: str, headers: dict = None, req_params: dict = None,
                         req_data: dict = None, req_json: dict = None, logger: logging.Logger = None) -> dict:
 
     if logger is not None:
         logger.info(f"Invoking POST: '{url}'")
 
     # initialize return variable
     result: dict | None = None
```

### Comparing `pypomes_core-0.1.5/src/pypomes_core/json_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/list_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/str_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.1.6/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/LICENSE` & `pypomes_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.5/pyproject.toml` & `pypomes_core-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.1.5/PKG-INFO` & `pypomes_core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

