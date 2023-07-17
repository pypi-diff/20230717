# Comparing `tmp/motti-0.0.4.tar.gz` & `tmp/motti-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motti-0.0.4.tar", last modified: Mon Jul 17 07:16:40 2023, max compression
+gzip compressed data, was "motti-0.0.5.tar", last modified: Mon Jul 17 12:02:04 2023, max compression
```

## Comparing `motti-0.0.4.tar` & `motti-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:16:40.275762 motti-0.0.4/
--rw-rw-rw-   0        0        0      135 2023-07-17 07:16:40.273751 motti-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-15 13:51:44.000000 motti-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 07:16:40.265748 motti-0.0.4/motti/
--rw-rw-rw-   0        0        0      136 2023-07-17 06:49:39.000000 motti-0.0.4/motti/__init__.py
--rw-rw-rw-   0        0        0      125 2023-07-15 14:09:04.000000 motti-0.0.4/motti/dev.py
--rw-rw-rw-   0        0        0      449 2023-07-17 06:52:47.000000 motti-0.0.4/motti/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:16:40.272755 motti-0.0.4/motti.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-17 07:16:40.000000 motti-0.0.4/motti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-17 07:16:40.000000 motti-0.0.4/motti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:16:40.000000 motti-0.0.4/motti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.4/motti.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-17 07:16:40.000000 motti-0.0.4/motti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 07:16:40.275762 motti-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-07-17 07:16:30.000000 motti-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.494141 motti-0.0.5/
+-rw-rw-rw-   0        0        0      135 2023-07-17 12:02:04.493143 motti-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-17 12:01:24.000000 motti-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.485142 motti-0.0.5/motti/
+-rw-rw-rw-   0        0        0      120 2023-07-17 12:00:05.000000 motti-0.0.5/motti/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.5/motti/dev.py
+-rw-rw-rw-   0        0        0      908 2023-07-17 11:49:49.000000 motti-0.0.5/motti/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:02:04.492142 motti-0.0.5/motti.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 15:12:08.000000 motti-0.0.5/motti.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-17 12:02:04.000000 motti-0.0.5/motti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:02:04.494141 motti-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-07-17 12:00:13.000000 motti-0.0.5/setup.py
```

