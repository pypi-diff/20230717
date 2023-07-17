# Comparing `tmp/sanctify-1.0.5.tar.gz` & `tmp/sanctify-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.5.tar", last modified: Mon Jul 17 08:46:23 2023, max compression
+gzip compressed data, was "sanctify-1.0.6.tar", last modified: Mon Jul 17 13:54:33 2023, max compression
```

## Comparing `sanctify-1.0.5.tar` & `sanctify-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.066413 sanctify-1.0.5/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.5/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 08:46:23.066116 sanctify-1.0.5/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.5/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-17 08:42:31.000000 sanctify-1.0.5/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.065115 sanctify-1.0.5/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      852 2023-07-17 08:43:45.000000 sanctify-1.0.5/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.5/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12305 2023-07-17 08:43:45.000000 sanctify-1.0.5/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3455 2023-07-17 07:18:35.000000 sanctify-1.0.5/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9783 2023-07-17 08:43:46.000000 sanctify-1.0.5/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 08:46:23.065891 sanctify-1.0.5/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-17 08:46:23.000000 sanctify-1.0.5/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-17 08:46:23.066459 sanctify-1.0.5/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 13:54:33.714311 sanctify-1.0.6/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.6/LICENSE.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 13:54:33.714156 sanctify-1.0.6/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.6/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-17 13:52:52.000000 sanctify-1.0.6/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 13:54:33.713338 sanctify-1.0.6/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      852 2023-07-17 13:54:15.000000 sanctify-1.0.6/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 13:52:28.000000 sanctify-1.0.6/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 13:52:28.000000 sanctify-1.0.6/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.6/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12305 2023-07-17 13:54:15.000000 sanctify-1.0.6/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 13:52:28.000000 sanctify-1.0.6/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3455 2023-07-17 13:52:28.000000 sanctify-1.0.6/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9828 2023-07-17 13:54:15.000000 sanctify-1.0.6/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-17 13:54:33.713969 sanctify-1.0.6/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-17 13:54:33.000000 sanctify-1.0.6/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-17 13:54:33.000000 sanctify-1.0.6/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-17 13:54:33.000000 sanctify-1.0.6/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-17 13:54:33.000000 sanctify-1.0.6/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-17 13:54:33.714347 sanctify-1.0.6/setup.cfg
```

### Comparing `sanctify-1.0.5/LICENSE.txt` & `sanctify-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/PKG-INFO` & `sanctify-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.5
+Version: 1.0.6
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sanctify-1.0.5/README.md` & `sanctify-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/pyproject.toml` & `sanctify-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.5"
+version = "1.0.6"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Allowed config based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.0.5/sanctify/__init__.py` & `sanctify-1.0.6/sanctify/__init__.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/cleanser.py` & `sanctify-1.0.6/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/constants.py` & `sanctify-1.0.6/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/processor.py` & `sanctify-1.0.6/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/transformer.py` & `sanctify-1.0.6/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/utils.py` & `sanctify-1.0.6/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.5/sanctify/validator.py` & `sanctify-1.0.6/sanctify/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         Args:
             value: The value representing a date.
             date_order_tuple: A tuple specifying the order of year, month, and day in the date.
             comparison_operations: A dictionary of comparison operations and their operands.
 
         Returns:
-            The validated age value if all comparison operations pass.
+            The validated date value if all comparison operations pass.
 
         Raises:
             ValidationError: If any comparison operation fails.
         """
         parsed_datetime = Transformer.parse_date_from_string(
             value=value, date_order_tuple=date_order_tuple, return_datetime=True
         )
@@ -99,15 +99,15 @@
                     ComparisonOperations.GREATER_THAN_EQUALS.value: 18,
                     ComparisonOperations.LESS_THAN_EQUALS.value: 100,
                 },
             )
         except ValidationError:
             raise ValidationError("Age should be >=18 and <=100")
 
-        return value
+        return str(parsed_datetime.date())
 
     @staticmethod
     def validate_due_date(
         value: str | int,
         date_order_tuple: tuple,
         comparison_operations: dict[str: int | None] = None,
     ) -> str | int | Exception:
@@ -142,15 +142,15 @@
                         ComparisonOperations.LESS_THAN_EQUALS.value: 10,
                     },
                 )
 
             except ValidationError:
                 raise ValidationError("Should be less than 10 years")
 
-        return value
+        return str(parsed_datetime.date())
 
     @staticmethod
     def validate_email(
         value: str, check_deliverability: bool = False
     ) -> str | EmailNotValidError | EmailUndeliverableError | Exception:
         """
         Validate an email address.
```

### Comparing `sanctify-1.0.5/sanctify.egg-info/PKG-INFO` & `sanctify-1.0.6/sanctify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.5
+Version: 1.0.6
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

