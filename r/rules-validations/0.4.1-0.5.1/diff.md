# Comparing `tmp/rules_validations-0.4.1.tar.gz` & `tmp/rules_validations-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules_validations-0.4.1.tar", max compression
+gzip compressed data, was "rules_validations-0.5.1.tar", max compression
```

## Comparing `rules_validations-0.4.1.tar` & `rules_validations-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       19 2023-07-07 19:37:10.825817 rules_validations-0.4.1/README.md
--rw-r--r--   0        0        0      347 2023-07-07 19:37:27.273934 rules_validations-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2321 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/baseEnum.py
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-07-17 18:51:32.347143 rules_validations-0.5.1/README.md
+-rw-r--r--   0        0        0      337 2023-07-17 18:51:42.955287 rules_validations-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1926 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/baseEnum.py
+-rw-r--r--   0        0        0      633 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/normalize.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 rules_validations-0.5.1/PKG-INFO
```

