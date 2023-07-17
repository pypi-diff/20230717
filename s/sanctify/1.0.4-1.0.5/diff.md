# Comparing `tmp/sanctify-1.0.4.tar.gz` & `tmp/sanctify-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.4.tar", last modified: Sun Jul 16 14:34:30 2023, max compression
+gzip compressed data, was "sanctify-1.0.5.tar", last modified: Mon Jul 17 08:46:23 2023, max compression
```

## Comparing `sanctify-1.0.4.tar` & `sanctify-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.942379 sanctify-1.0.4/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.4/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-16 14:34:30.942130 sanctify-1.0.4/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.4/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1552 2023-07-16 14:34:24.000000 sanctify-1.0.4/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.941338 sanctify-1.0.4/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      833 2023-07-16 14:31:35.000000 sanctify-1.0.4/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7629 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2613 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.4/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12233 2023-07-16 14:31:36.000000 sanctify-1.0.4/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8744 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3417 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9745 2023-07-16 14:31:36.000000 sanctify-1.0.4/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.941949 sanctify-1.0.4/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-16 14:34:30.942443 sanctify-1.0.4/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.066413 sanctify-1.0.5/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.5/LICENSE.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 08:46:23.066116 sanctify-1.0.5/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.5/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-17 08:42:31.000000 sanctify-1.0.5/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.065115 sanctify-1.0.5/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      852 2023-07-17 08:43:45.000000 sanctify-1.0.5/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.5/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12305 2023-07-17 08:43:45.000000 sanctify-1.0.5/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3455 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9783 2023-07-17 08:43:46.000000 sanctify-1.0.5/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.065891 sanctify-1.0.5/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-17 08:46:23.066459 sanctify-1.0.5/setup.cfg
```

### Comparing `sanctify-1.0.4/LICENSE.txt` & `sanctify-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.4/PKG-INFO` & `sanctify-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.4
+Version: 1.0.5
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sanctify-1.0.4/README.md` & `sanctify-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.4/pyproject.toml` & `sanctify-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 [tool.isort]
 atomic=true
-python-version=310
+py_version=311
 default_section='THIRDPARTY'
 known_first_party='sanctify'
-project='sanctify'
 combine_as_imports=true
-combine-star=true
-combine-straight-imports=true
 overwrite_in_place=true
-ensure-newline-before-comments=true
-balanced=true
-import_heading_stdlib='Standard Library'
-import_heading_firstparty='Studio Imports'
-float-to-top=true
+import_heading_stdlib='External Imports'
+import_heading_firstparty='Internal Imports'
 
 [tool.black]
 fast=true
-target-version=['py310']
+target-version=['py311']
 color=true
 line-length=120
 exclude='''
 /(
     \.git
     | \.mypy_cache
     | \.tox
@@ -59,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Allowed config based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.0.4/sanctify/__init__.py` & `sanctify-1.0.5/sanctify/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Internal Imports
 from sanctify.cleanser import Cleanser
 from sanctify.constants import (
     PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP,
     AbstractDataTypes,
     CalendarDateComponents,
     ComparisonOperations,
     Constants,
```

### Comparing `sanctify-1.0.4/sanctify/cleanser.py` & `sanctify-1.0.5/sanctify/cleanser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 from frozendict import frozendict
 
+# Internal Imports
 from sanctify.constants import Constants, DefaultColumns
 from sanctify.utils import replace_dict_keys
 
 
 class Cleanser:
     """
     The Cleanser class is responsible for validating and checking if a column is present and should be used.
```

### Comparing `sanctify-1.0.4/sanctify/constants.py` & `sanctify-1.0.5/sanctify/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# External Imports
 import string
 from enum import Enum, StrEnum, auto
 
 import pandas as pd
 from frozendict import frozendict
```

### Comparing `sanctify-1.0.4/sanctify/processor.py` & `sanctify-1.0.5/sanctify/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# External Imports
 from typing import Callable
 
 import pandas as pd
 from frozendict import frozendict
 from loguru import logger
 
+# Internal Imports
 from sanctify.constants import (
     PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP,
     AbstractDataTypes,
     Constants,
     DefaultColumns,
     PrimitiveDataTypes,
 )
@@ -183,15 +185,15 @@
 
     Returns:
         pd.Series: Series containing the modified value and error message (if any).
     """
     func_value = value
     error_message = None
 
-    if not func_value:  # All possible absent value cases
+    if not func_value or func_value == "nan":  # All possible absent value cases
         error_message = f"{col_name} is required"
         func_value = None
 
     else:
         for function in functions:
             func = function
             kwargs = {}
@@ -257,15 +259,16 @@
 
         if col_config == {}:
             logger.error(f"Column({col_name})'s column config not provided in the input dataframe | {col_config = }")
             # Continue to next column in the column mapping schema
             continue  # Skip empty config items
         else:
             logger.debug(f"Parsing Column({col_name}) as str dtype | {col_config = }")
-            df[col_name] = df[col_name].astype(str)  # Convert column rows to string data type
+            # Convert column rows to string data type
+            df[col_name] = df[col_name].astype(str)
 
         transformations, validations = [], []
 
         d_type_transformations, d_type_validations = handle_data_type(data_type_schema, col_config)
         d_order_transformations, d_order_validations = handle_date_order_tuple(col_config)
         (
             comparison_op_transformations,
```

### Comparing `sanctify-1.0.4/sanctify/transformer.py` & `sanctify-1.0.5/sanctify/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# External Imports
 import re
 from datetime import datetime
 
 import phonenumbers
 from dateutil import parser
 from loguru import logger
 
+# Internal Imports
 from sanctify.constants import STRING_TRANSLATION_TABLE, CalendarDateComponents
 from sanctify.exception import ValidationError
 
 
 class Transformer:
     @staticmethod
     def parse_boolean(value: str):
```

### Comparing `sanctify-1.0.4/sanctify/utils.py` & `sanctify-1.0.5/sanctify/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# External Imports
 from datetime import date
 
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
+# Internal Imports
 from sanctify.constants import ComparisonOperations
 
 
 def replace_dict_keys(original_dict: dict, key_mapping: dict) -> dict:
     """
     Replace keys in a dictionary with the corresponding values from a key mapping dictionary.
```

### Comparing `sanctify-1.0.4/sanctify/validator.py` & `sanctify-1.0.5/sanctify/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# External Imports
 from typing import Any
 
 from email_validator import EmailNotValidError, EmailUndeliverableError, ValidatedEmail, validate_email
 from loguru import logger
 
+# Internal Imports
 from sanctify.constants import ComparisonOperations
 from sanctify.exception import ValidationError
 from sanctify.transformer import Transformer
 from sanctify.utils import calculate_age, match_comparision_operation
 
 
 class Validator:
```

### Comparing `sanctify-1.0.4/sanctify.egg-info/PKG-INFO` & `sanctify-1.0.5/sanctify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.4
+Version: 1.0.5
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

