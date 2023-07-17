# Comparing `tmp/spdb-1.0.6.tar.gz` & `tmp/spdb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.6.tar", last modified: Mon Jul 17 13:03:39 2023, max compression
+gzip compressed data, was "spdb-1.0.7.tar", last modified: Mon Jul 17 13:04:46 2023, max compression
```

## Comparing `spdb-1.0.6.tar` & `spdb-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:03:39.748371 spdb-1.0.6/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.6/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2148 2023-07-17 13:03:39.748371 spdb-1.0.6/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1664 2023-07-17 13:03:27.000000 spdb-1.0.6/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 13:03:33.000000 spdb-1.0.6/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 13:03:39.748371 spdb-1.0.6/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 13:03:36.000000 spdb-1.0.6/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:03:39.748371 spdb-1.0.6/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.6/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.6/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.6/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.6/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.6/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.6/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.6/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:03:39.748371 spdb-1.0.6/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2148 2023-07-17 13:03:39.000000 spdb-1.0.6/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 13:03:39.000000 spdb-1.0.6/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 13:03:39.000000 spdb-1.0.6/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.6/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 13:03:39.000000 spdb-1.0.6/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 13:03:39.000000 spdb-1.0.6/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:04:46.311198 spdb-1.0.7/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.7/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2176 2023-07-17 13:04:46.311198 spdb-1.0.7/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1692 2023-07-17 13:04:36.000000 spdb-1.0.7/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 13:04:39.000000 spdb-1.0.7/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 13:04:46.311198 spdb-1.0.7/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 13:04:42.000000 spdb-1.0.7/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:04:46.311198 spdb-1.0.7/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.7/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.7/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.7/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.7/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.7/spdb/text_validator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.7/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.7/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 13:04:46.311198 spdb-1.0.7/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2176 2023-07-17 13:04:46.000000 spdb-1.0.7/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 13:04:46.000000 spdb-1.0.7/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 13:04:46.000000 spdb-1.0.7/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.7/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 13:04:46.000000 spdb-1.0.7/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 13:04:46.000000 spdb-1.0.7/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.6/LICENSE` & `spdb-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spdb-1.0.6/PKG-INFO` & `spdb-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 Metadata-Version: 2.1
 Name: spdb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Sassy Python Database (and auth) utils
 Author-email: Mrybs <mrybs2@gmail.com>
 Project-URL: Homepage, https://github.com/mrybs/spdb
 Project-URL: Bug Tracker, https://github.com/mrybs/spdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 =====================================
 
-Sassy Python Database(and auth) utils
+# Sassy Python Database(and auth) utils
 
 =====================================
 
 
-Requirements
+## Requirements
 
 ============
 
 - Python 3.7 or higher
 - pyotp
 - qrcode
 - setuptools
 
 
-Usage 
+## Usage 
 
 =====
 
 	import spdb
 
-Database
+### Database
 
 --------
 	spdb.Database(path: str)
 	spdb.Database.create_tables(tables_names: list[str]) -> None
 	spdb.Database.execute(code) -> str
 	spdb.Database.read_dict(name: str, data_id: str) -> dict
 	spdb.Database.read_object(Class: class, name: str, data_id: str) -> Class
 	spdb.Database.write_dict(name: str, data_id: str, data: dict) -> None
 	spdb.Database.write_object(name: str, object_id: str, object: Class) -> None
 
 	Static:
 		spdb.Database.object_to_dict(object: Class) -> dict
 		spdb.Database.dict_to_object(Class: class, Dict: dict) -> Class
 
-TOTP - HOTP
+### TOTP - HOTP
 
 -----------
 	spdb.OTP(token: str=None, app_name: str=None)
 	spdb.OTP.now() -> str
 	stdb.OTP.at(index: int) -> str
 	stdb.OTP.time_verify(code: str) -> bool
 	stdb.OTP.counter_verify(index: int, code: str) -> bool
 	stdb.OTP.TQR(name: str) ->
 	stdb.OTP.HQR(name: str) ->
 
 	Static:
 		stdb.OTP.generate_token() -> str
 
-Token Generator
+### Token Generator
 
 ---------------
 	stdb.TokenGenerator(code: str)
 	stdb.TokenGenerator.gen(type: str, ID: str, key: str) -> str
 
 	Static:
 		stdb.TokenGenerator.parse_token(token: str) -> dict
 
-Text Validator
+### Text Validator
 
 --------------
 	stdb.TextValidator(min: int=4, max: int=64, regexp: str=r'([A-z]|[0-9]|_|-)+')
 	stdb.TextValidator.check(text: str) -> bool
 
-Utils
+### Utils
 
 -----
 	stdb.utils.sha256(text: str) -> str
 	stdb.utils.b32encode(text: str) -> str
 	stdb.utils.random_text(length: int=None) -> str
 	stdb.utils.random_sha256() -> str
 	stdb.utils.random_b32 -> str
```

### Comparing `spdb-1.0.6/README.md` & `spdb-1.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 =====================================
 
-Sassy Python Database(and auth) utils
+# Sassy Python Database(and auth) utils
 
 =====================================
 
 
-Requirements
+## Requirements
 
 ============
 
 - Python 3.7 or higher
 - pyotp
 - qrcode
 - setuptools
 
 
-Usage 
+## Usage 
 
 =====
 
 	import spdb
 
-Database
+### Database
 
 --------
 	spdb.Database(path: str)
 	spdb.Database.create_tables(tables_names: list[str]) -> None
 	spdb.Database.execute(code) -> str
 	spdb.Database.read_dict(name: str, data_id: str) -> dict
 	spdb.Database.read_object(Class: class, name: str, data_id: str) -> Class
 	spdb.Database.write_dict(name: str, data_id: str, data: dict) -> None
 	spdb.Database.write_object(name: str, object_id: str, object: Class) -> None
 
 	Static:
 		spdb.Database.object_to_dict(object: Class) -> dict
 		spdb.Database.dict_to_object(Class: class, Dict: dict) -> Class
 
-TOTP - HOTP
+### TOTP - HOTP
 
 -----------
 	spdb.OTP(token: str=None, app_name: str=None)
 	spdb.OTP.now() -> str
 	stdb.OTP.at(index: int) -> str
 	stdb.OTP.time_verify(code: str) -> bool
 	stdb.OTP.counter_verify(index: int, code: str) -> bool
 	stdb.OTP.TQR(name: str) ->
 	stdb.OTP.HQR(name: str) ->
 
 	Static:
 		stdb.OTP.generate_token() -> str
 
-Token Generator
+### Token Generator
 
 ---------------
 	stdb.TokenGenerator(code: str)
 	stdb.TokenGenerator.gen(type: str, ID: str, key: str) -> str
 
 	Static:
 		stdb.TokenGenerator.parse_token(token: str) -> dict
 
-Text Validator
+### Text Validator
 
 --------------
 	stdb.TextValidator(min: int=4, max: int=64, regexp: str=r'([A-z]|[0-9]|_|-)+')
 	stdb.TextValidator.check(text: str) -> bool
 
-Utils
+### Utils
 
 -----
 	stdb.utils.sha256(text: str) -> str
 	stdb.utils.b32encode(text: str) -> str
 	stdb.utils.random_text(length: int=None) -> str
 	stdb.utils.random_sha256() -> str
 	stdb.utils.random_b32 -> str
```

### Comparing `spdb-1.0.6/spdb/db.py` & `spdb-1.0.7/spdb/db.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.6/spdb/generator_utils.py` & `spdb-1.0.7/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.6/spdb/otp.py` & `spdb-1.0.7/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.6/spdb/token_generator.py` & `spdb-1.0.7/spdb/token_generator.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.6/spdb.egg-info/PKG-INFO` & `spdb-1.0.7/spdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 Metadata-Version: 2.1
 Name: spdb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Sassy Python Database (and auth) utils
 Author-email: Mrybs <mrybs2@gmail.com>
 Project-URL: Homepage, https://github.com/mrybs/spdb
 Project-URL: Bug Tracker, https://github.com/mrybs/spdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 =====================================
 
-Sassy Python Database(and auth) utils
+# Sassy Python Database(and auth) utils
 
 =====================================
 
 
-Requirements
+## Requirements
 
 ============
 
 - Python 3.7 or higher
 - pyotp
 - qrcode
 - setuptools
 
 
-Usage 
+## Usage 
 
 =====
 
 	import spdb
 
-Database
+### Database
 
 --------
 	spdb.Database(path: str)
 	spdb.Database.create_tables(tables_names: list[str]) -> None
 	spdb.Database.execute(code) -> str
 	spdb.Database.read_dict(name: str, data_id: str) -> dict
 	spdb.Database.read_object(Class: class, name: str, data_id: str) -> Class
 	spdb.Database.write_dict(name: str, data_id: str, data: dict) -> None
 	spdb.Database.write_object(name: str, object_id: str, object: Class) -> None
 
 	Static:
 		spdb.Database.object_to_dict(object: Class) -> dict
 		spdb.Database.dict_to_object(Class: class, Dict: dict) -> Class
 
-TOTP - HOTP
+### TOTP - HOTP
 
 -----------
 	spdb.OTP(token: str=None, app_name: str=None)
 	spdb.OTP.now() -> str
 	stdb.OTP.at(index: int) -> str
 	stdb.OTP.time_verify(code: str) -> bool
 	stdb.OTP.counter_verify(index: int, code: str) -> bool
 	stdb.OTP.TQR(name: str) ->
 	stdb.OTP.HQR(name: str) ->
 
 	Static:
 		stdb.OTP.generate_token() -> str
 
-Token Generator
+### Token Generator
 
 ---------------
 	stdb.TokenGenerator(code: str)
 	stdb.TokenGenerator.gen(type: str, ID: str, key: str) -> str
 
 	Static:
 		stdb.TokenGenerator.parse_token(token: str) -> dict
 
-Text Validator
+### Text Validator
 
 --------------
 	stdb.TextValidator(min: int=4, max: int=64, regexp: str=r'([A-z]|[0-9]|_|-)+')
 	stdb.TextValidator.check(text: str) -> bool
 
-Utils
+### Utils
 
 -----
 	stdb.utils.sha256(text: str) -> str
 	stdb.utils.b32encode(text: str) -> str
 	stdb.utils.random_text(length: int=None) -> str
 	stdb.utils.random_sha256() -> str
 	stdb.utils.random_b32 -> str
```

