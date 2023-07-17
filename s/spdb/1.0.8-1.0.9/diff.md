# Comparing `tmp/spdb-1.0.8.tar.gz` & `tmp/spdb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.8.tar", last modified: Mon Jul 17 16:59:46 2023, max compression
+gzip compressed data, was "spdb-1.0.9.tar", last modified: Mon Jul 17 17:09:26 2023, max compression
```

## Comparing `spdb-1.0.8.tar` & `spdb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 16:59:46.939157 spdb-1.0.8/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.8/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2172 2023-07-17 16:59:46.935824 spdb-1.0.8/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1688 2023-07-17 16:59:19.000000 spdb-1.0.8/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 16:59:42.000000 spdb-1.0.8/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 16:59:46.939157 spdb-1.0.8/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 16:59:39.000000 spdb-1.0.8/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 16:59:46.935824 spdb-1.0.8/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.8/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.8/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.8/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.8/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.8/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.8/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.8/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 16:59:46.935824 spdb-1.0.8/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2172 2023-07-17 16:59:46.000000 spdb-1.0.8/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 16:59:46.000000 spdb-1.0.8/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 16:59:46.000000 spdb-1.0.8/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.8/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 16:59:46.000000 spdb-1.0.8/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 16:59:46.000000 spdb-1.0.8/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.9/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2910 2023-07-17 17:09:26.646797 spdb-1.0.9/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2427 2023-07-17 17:08:59.000000 spdb-1.0.9/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 17:09:15.000000 spdb-1.0.9/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 17:09:26.646797 spdb-1.0.9/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 17:09:12.000000 spdb-1.0.9/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.9/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.9/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.9/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.9/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.9/spdb/text_validator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.9/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.9/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2910 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.9/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.8/LICENSE` & `spdb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spdb-1.0.8/PKG-INFO` & `spdb-1.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,78 @@
-Metadata-Version: 2.1
-Name: spdb
-Version: 1.0.8
-Summary: Sassy Python Database (and auth) utils
-Author-email: Mrybs <mrybs2@gmail.com>
-Project-URL: Homepage, https://github.com/mrybs/spdb
-Project-URL: Bug Tracker, https://github.com/mrybs/spdb/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# =====================================
 
-=====================================
 # Sassy Python Database(and auth) utils
-=====================================
+
+# =====================================
+
+LICENSE: The MIT License
 
 
 ## Requirements
-============
+
+## ============
 
 - Python 3.7 or higher
 - pyotp
 - qrcode
 - setuptools
 
 
 ## Usage 
-=====
+
+## =====
 
 	import spdb
 
 ### Database
 
 --------
-	spdb.Database(path: str)
-	spdb.Database.create_tables(tables_names: list[str]) -> None
-	spdb.Database.execute(code) -> str
-	spdb.Database.read_dict(name: str, data_id: str) -> dict
-	spdb.Database.read_object(Class: class, name: str, data_id: str) -> Class
-	spdb.Database.write_dict(name: str, data_id: str, data: dict) -> None
-	spdb.Database.write_object(name: str, object_id: str, object: Class) -> None
+	spdb.Database(path: str)  # Create Database object
+	spdb.Database.create_tables(tables_names: list[str]) -> None  # Create tables if not exists
+	spdb.Database.execute(code) -> str  # Execute sqlite3 code
+	spdb.Database.read_dict(name: str, data_id: str) -> dict  # Read data by ID as dict
+	spdb.Database.read_object(Class: class, name: str, data_id: str) -> Class  # Read data by ID as object
+	spdb.Database.write_dict(name: str, data_id: str, data: dict) -> None  # Write dict by ID
+	spdb.Database.write_object(name: str, object_id: str, object: Class) -> None  # Write object by ID
 
 	Static:
-		spdb.Database.object_to_dict(object: Class) -> dict
-		spdb.Database.dict_to_object(Class: class, Dict: dict) -> Class
+		spdb.Database.object_to_dict(object: Class) -> dict  # Convert object into dict
+		spdb.Database.dict_to_object(Class: class, Dict: dict) -> Class  # Convert dict into object
 
 ### TOTP - HOTP
 
 -----------
-	spdb.OTP(token: str=None, app_name: str=None)
-	spdb.OTP.now() -> str
-	stdb.OTP.at(index: int) -> str
-	stdb.OTP.time_verify(code: str) -> bool
-	stdb.OTP.counter_verify(index: int, code: str) -> bool
-	stdb.OTP.TQR(name: str) ->
-	stdb.OTP.HQR(name: str) ->
+	spdb.OTP(token: str=None, app_name: str=None)  # Create OTP object
+	spdb.OTP.now() -> str  # Get TOTP code
+	stdb.OTP.at(index: int) -> str  # Get HOTP code
+	stdb.OTP.time_verify(code: str) -> bool  # Verify TOTP code
+	stdb.OTP.counter_verify(index: int, code: str) -> bool  # Verify HOTP code
+	stdb.OTP.TQR(name: str) ->  # Get TOTP QR-code for Google Authentificator
+	stdb.OTP.HQR(name: str) ->  # Get HOTP QR-code for Google Authentificator
 
 	Static:
-		stdb.OTP.generate_token() -> str
+		stdb.OTP.generate_token() -> str  # Generate random token
 
 ### Token Generator
 
 ---------------
-	stdb.TokenGenerator(code: str)
-	stdb.TokenGenerator.gen(type: str, ID: str, key: str) -> str
+	stdb.TokenGenerator(code: str)  # Create TokenGenerator object
+	stdb.TokenGenerator.gen(type: str, ID: str, key: str) -> str  # Generate token
 
 	Static:
-		stdb.TokenGenerator.parse_token(token: str) -> dict
+		stdb.TokenGenerator.parse_token(token: str) -> dict  # Parse token
 
 ### Text Validator
 
 --------------
-	stdb.TextValidator(min: int=4, max: int=64, regexp: str=r'([A-z]|[0-9]|_|-)+')
-	stdb.TextValidator.check(text: str) -> bool
+	stdb.TextValidator(min: int=4, max: int=64, regexp: str=r'([A-z]|[0-9]|_|-)+')  # Create TextValidator object
+	stdb.TextValidator.check(text: str) -> bool  # Check text for conditions
 
 ### Utils
 
 -----
-	stdb.utils.sha256(text: str) -> str
-	stdb.utils.b32encode(text: str) -> str
-	stdb.utils.random_text(length: int=None) -> str
-	stdb.utils.random_sha256() -> str
-	stdb.utils.random_b32 -> str
+	stdb.utils.sha256(text: str) -> str  # Get sha256 from text
+	stdb.utils.b32encode(text: str) -> str  # Encode str into base32 str
+	stdb.utils.random_text(length: int=None) -> str  # Get random text
+	stdb.utils.random_sha256() -> str  # Get random sha256 str
+	stdb.utils.random_b32 -> str  # Get random base32 str
+
```

### Comparing `spdb-1.0.8/spdb/db.py` & `spdb-1.0.9/spdb/db.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.8/spdb/generator_utils.py` & `spdb-1.0.9/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.8/spdb/otp.py` & `spdb-1.0.9/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.8/spdb/token_generator.py` & `spdb-1.0.9/spdb/token_generator.py`

 * *Files identical despite different names*

