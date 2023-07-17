# Comparing `tmp/satori_playbook_validator-3.1.6.tar.gz` & `tmp/satori_playbook_validator-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-3.1.6.tar", last modified: Sun Jul 16 23:22:27 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.1.7.tar", last modified: Mon Jul 17 13:10:19 2023, max compression
```

## Comparing `satori_playbook_validator-3.1.6.tar` & `satori_playbook_validator-3.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/README.md
--rw-r--r--   0        0        0      518 2023-07-16 23:22:27.600602 satori_playbook_validator-3.1.6/pyproject.toml
--rw-r--r--   0        0        0      301 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     6201 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      298 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1906 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2361 2023-07-16 23:22:12.904464 satori_playbook_validator-3.1.6/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      100 2023-07-16 23:22:12.908464 satori_playbook_validator-3.1.6/src/satorici/validator/warnings.py
--rw-r--r--   0        0        0     2659 2023-07-16 23:22:12.908464 satori_playbook_validator-3.1.6/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-07-16 23:22:12.908464 satori_playbook_validator-3.1.6/tests/test_reference_finder.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/README.md
+-rw-r--r--   0        0        0      518 2023-07-17 13:10:19.259078 satori_playbook_validator-3.1.7/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     6212 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      298 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1906 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     2659 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.7/PKG-INFO
```

### Comparing `satori_playbook_validator-3.1.6/pyproject.toml` & `satori_playbook_validator-3.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-playbook-validator"
-version = "3.1.6"
+version = "3.1.7"
 description = ""
 authors = [
     { name = "Satori CI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "fastjsonschema>=2.17.1",
     "aws-cron-expression-validator>=1.1.6",
```

### Comparing `satori_playbook_validator-3.1.6/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.1.7/src/satorici/validator/_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
 
 def validate_settings(settings: dict):
     _validate(settings_schema, settings)
 
     if "cron" in settings:
         try:
             AWSCronExpressionValidator.validate(settings["cron"])
-        except Exception:
-            raise PlaybookValidationError("Invalid cron expression")
+        except Exception as e:
+            raise PlaybookValidationError(f"Invalid cron expression: {e}")
 
     if "cron" in settings or "rate" in settings:
         if not any(k.startswith("log") for k in settings):
             warnings.warn(NoLogMonitorWarning("Monitor without notifications."))
 
     if "timeout" in settings and "commandTimeout" in settings:
         if settings["timeout"] < settings["commandTimeout"]:
```

### Comparing `satori_playbook_validator-3.1.6/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.6/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.6/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.6/tests/test_playbook_validator.py` & `satori_playbook_validator-3.1.7/tests/test_playbook_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.6/tests/test_reference_finder.py` & `satori_playbook_validator-3.1.7/tests/test_reference_finder.py`

 * *Files identical despite different names*

