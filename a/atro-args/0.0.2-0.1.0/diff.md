# Comparing `tmp/atro_args-0.0.2.tar.gz` & `tmp/atro_args-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_args-0.0.2.tar", max compression
+gzip compressed data, was "atro_args-0.1.0.tar", max compression
```

## Comparing `atro_args-0.0.2.tar` & `atro_args-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_args-0.0.2/README.md
--rw-r--r--   0        0        0      275 2023-07-16 21:39:17.730280 atro_args-0.0.2/atro_args/__init__.py
--rw-r--r--   0        0        0      329 2023-07-16 21:43:43.709071 atro_args-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 atro_args-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 12:33:58.233092 atro_args-0.1.0/README.md
+-rw-r--r--   0        0        0      276 2023-07-16 21:47:16.150095 atro_args-0.1.0/atro_args/__init__.py
+-rw-r--r--   0        0        0      329 2023-07-17 21:43:35.030720 atro_args-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 atro_args-0.1.0/PKG-INFO
```

