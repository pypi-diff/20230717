# Comparing `tmp/django_encryption-0.3.8.tar.gz` & `tmp/django_encryption-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_encryption-0.3.8.tar", max compression
+gzip compressed data, was "django_encryption-0.3.9.tar", max compression
```

## Comparing `django_encryption-0.3.8.tar` & `django_encryption-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6295 2023-06-29 15:09:00.309046 django_encryption-0.3.8/README.md
--rw-r--r--   0        0        0       22 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/__init__.py
--rw-r--r--   0        0        0    15879 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/fields.py
--rw-r--r--   0        0        0        0 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/management/commands/__init__.py
--rw-r--r--   0        0        0     3278 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/management/commands/generate_vault_migration.py
--rw-r--r--   0        0        0        0 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/py.typed
--rw-r--r--   0        0        0    11063 2023-06-29 15:09:00.309046 django_encryption-0.3.8/django_encryption/vault_wrapper.py
--rw-r--r--   0        0        0     2160 2023-06-29 15:09:26.797049 django_encryption-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7837 1970-01-01 00:00:00.000000 django_encryption-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     6295 2023-07-05 17:29:20.991411 django_encryption-0.3.9/README.md
+-rw-r--r--   0        0        0       22 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/__init__.py
+-rw-r--r--   0        0        0    15879 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/fields.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/management/commands/__init__.py
+-rw-r--r--   0        0        0     3278 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/management/commands/generate_vault_migration.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/py.typed
+-rw-r--r--   0        0        0    11063 2023-07-05 17:29:20.991411 django_encryption-0.3.9/django_encryption/vault_wrapper.py
+-rw-r--r--   0        0        0     2160 2023-07-05 17:29:43.583754 django_encryption-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7837 1970-01-01 00:00:00.000000 django_encryption-0.3.9/PKG-INFO
```

### Comparing `django_encryption-0.3.8/README.md` & `django_encryption-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 This is a fork of
 <https://gitlab.com/lansharkconsulting/django/django-encrypted-model-fields> which in turn is a fork of <https://github.com/foundertherapy/django-cryptographic-fields>. It has
 been renamed, and updated to support encryption through Piiano Vault's API.
 
 **Note:**
 
-This package is compatible with Vault version 1.7.0.
+This package is compatible with Vault version 1.7.1.
 For a Vault client compatible with other versions of Vault, check [other versions of this package](https://pypi.org/project/django-encryption/).
 
 
 ## Usage
 
 First install the library:
```

### Comparing `django_encryption-0.3.8/django_encryption/fields.py` & `django_encryption-0.3.9/django_encryption/fields.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.8/django_encryption/management/commands/generate_vault_migration.py` & `django_encryption-0.3.9/django_encryption/management/commands/generate_vault_migration.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.8/django_encryption/vault_wrapper.py` & `django_encryption-0.3.9/django_encryption/vault_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.8/pyproject.toml` & `django_encryption-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-encryption"
-version = "0.3.8"
+version = "0.3.9"
 description = "A set of fields that wrap standard Django fields with encryption provided Piiano Vault."
 authors = ["Imri Goldberg <imri.goldberg@piiano.com>"]
 license = "MIT"
 packages = [ { include = "django_encryption" } ]
 readme = "README.md"
 repository = "https://github.com/piiano/vault-python"
 keywords = [ "encryption", "django", "fields" ]
```

### Comparing `django_encryption-0.3.8/PKG-INFO` & `django_encryption-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-encryption
-Version: 0.3.8
+Version: 0.3.9
 Summary: A set of fields that wrap standard Django fields with encryption provided Piiano Vault.
 Home-page: https://github.com/piiano/vault-python
 License: MIT
 Keywords: encryption,django,fields
 Author: Imri Goldberg
 Author-email: imri.goldberg@piiano.com
 Requires-Python: >=3.8,<4.0
@@ -59,15 +59,15 @@
 
 This is a fork of
 <https://gitlab.com/lansharkconsulting/django/django-encrypted-model-fields> which in turn is a fork of <https://github.com/foundertherapy/django-cryptographic-fields>. It has
 been renamed, and updated to support encryption through Piiano Vault's API.
 
 **Note:**
 
-This package is compatible with Vault version 1.7.0.
+This package is compatible with Vault version 1.7.1.
 For a Vault client compatible with other versions of Vault, check [other versions of this package](https://pypi.org/project/django-encryption/).
 
 
 ## Usage
 
 First install the library:
```

