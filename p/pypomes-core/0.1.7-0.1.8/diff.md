# Comparing `tmp/pypomes_core-0.1.7.tar.gz` & `tmp/pypomes_core-0.1.8.tar.gz`

## Comparing `pypomes_core-0.1.7.tar` & `pypomes_core-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/README.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/PKG-INFO
```

### Comparing `pypomes_core-0.1.7/src/pypomes_core/__init__.py` & `pypomes_core-0.1.8/src/pypomes_core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,25 @@
 from .http_pomes import (
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_name, http_status_description, http_json_from_get, http_json_from_post
 )
 from .json_pomes import (
-    jsonify_dict, jsonify_iterable
+    json_normalize_dict, json_normalize_iterable, json_from_request
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform
 )
+from .logging_pomes import (
+    LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
+    LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
+    logging_log_msgs, logging_get_entries
+)
 from .str_pomes import (
     str_between, str_split_on_mark, str_find_whitespace
 )
 from .validation_pomes import (
     VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
     validate_date, validate_datetime, validate_ints, validate_strs,
@@ -70,24 +75,28 @@
     file_from_request,
     # http_pomes
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_name, http_status_description, http_json_from_get, http_json_from_post,
     # json_pomes
-    jsonify_dict, jsonify_iterable,
+    json_normalize_dict, json_normalize_iterable, json_from_request,
     # list_pomes
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
+    # logging_pomes
+    LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
+    LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
+    logging_log_msgs, logging_get_entries,
     # validation_pomes
     VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
     validate_date, validate_datetime, validate_ints, validate_strs,
     validate_format_error, validate_format_errors,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.7"
-__version_info__ = (0, 1, 7)
+__version__ = "0.1.8"
+__version_info__ = (0, 1, 8)
```

### Comparing `pypomes_core-0.1.7/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/dict_pomes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from flask import Request
 import inspect
 import types
+from flask import Request
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
     Indicate the existence of an element in *source* pointed to by the nested keys chain
     *[keys[0]: ... :keys[n]*. The path up to he last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
```

### Comparing `pypomes_core-0.1.7/src/pypomes_core/email_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/email_pomes.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import sys
 from email.message import EmailMessage
 from smtplib import SMTP
 from typing import Final
-import sys
 from .env_pomes import APP_PREFIX, env_get_str, env_get_int
 
 EMAIL_ACCOUNT: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_ACCOUNT")
 EMAIL_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_PWD")
 EMAIL_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_EMAIL_PORT")
 EMAIL_SERVER: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_SERVER")
```

### Comparing `pypomes_core-0.1.7/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/env_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/file_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/http_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/http_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
-from typing import Final
 import logging
 import requests
 import sys
+from typing import Final
 
 from .exception_pomes import exc_format
 
 # https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status
 
 MIMETYPE_BINARY: Final[str] = "application/octet-stream"
 MIMETYPE_CSS: Final[str] = "text/css"
```

### Comparing `pypomes_core-0.1.7/src/pypomes_core/list_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/str_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.1.8/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/LICENSE` & `pypomes_core-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.7/pyproject.toml` & `pypomes_core-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.1.7/PKG-INFO` & `pypomes_core-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

