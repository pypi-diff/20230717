# Comparing `tmp/CompactObject_TOV-1.3.1.tar.gz` & `tmp/CompactObject_TOV-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CompactObject_TOV-1.3.1.tar", last modified: Sun Jul 16 03:14:17 2023, max compression
+gzip compressed data, was "CompactObject_TOV-1.4.1.tar", last modified: Mon Jul 17 01:03:14 2023, max compression
```

## Comparing `CompactObject_TOV-1.3.1.tar` & `CompactObject_TOV-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-16 03:14:17.569864 CompactObject_TOV-1.3.1/
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-16 03:14:17.488636 CompactObject_TOV-1.3.1/CompactObject_TOV.egg-info/
--rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-16 03:14:16.000000 CompactObject_TOV-1.3.1/CompactObject_TOV.egg-info/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)      355 2023-07-16 03:14:17.000000 CompactObject_TOV-1.3.1/CompactObject_TOV.egg-info/SOURCES.txt
--rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-16 03:14:16.000000 CompactObject_TOV-1.3.1/CompactObject_TOV.egg-info/dependency_links.txt
--rw-r--r--   0 a9         (501) staff       (20)       10 2023-07-16 03:14:16.000000 CompactObject_TOV-1.3.1/CompactObject_TOV.egg-info/top_level.txt
--rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 01:27:29.000000 CompactObject_TOV-1.3.1/LICENSE
--rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-16 03:14:17.554309 CompactObject_TOV-1.3.1/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)     1754 2023-07-16 01:27:29.000000 CompactObject_TOV-1.3.1/README.md
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-16 03:14:17.553720 CompactObject_TOV-1.3.1/TOVsolver/
--rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 01:27:29.000000 CompactObject_TOV-1.3.1/TOVsolver/EoS_import.py
--rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-16 02:25:44.000000 CompactObject_TOV-1.3.1/TOVsolver/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)      129 2023-07-16 01:27:29.000000 CompactObject_TOV-1.3.1/TOVsolver/constant.py
--rw-r--r--   0 a9         (501) staff       (20)     5622 2023-07-16 02:37:27.000000 CompactObject_TOV-1.3.1/TOVsolver/main.py
--rw-r--r--   0 a9         (501) staff       (20)     8598 2023-07-16 02:32:49.000000 CompactObject_TOV-1.3.1/TOVsolver/solver_code.py
--rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 03:07:53.000000 CompactObject_TOV-1.3.1/TOVsolver/speed_of_sound.py
--rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 01:27:29.000000 CompactObject_TOV-1.3.1/TOVsolver/tests_script.py
--rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-16 03:14:17.575170 CompactObject_TOV-1.3.1/setup.cfg
--rw-r--r--   0 a9         (501) staff       (20)      136 2023-07-16 02:25:31.000000 CompactObject_TOV-1.3.1/setup.py
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.625498 CompactObject_TOV-1.4.1/
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.599250 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/
+-rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)      355 2023-07-17 01:03:14.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/SOURCES.txt
+-rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/dependency_links.txt
+-rw-r--r--   0 a9         (501) staff       (20)       10 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/top_level.txt
+-rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/LICENSE
+-rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-17 01:03:14.621157 CompactObject_TOV-1.4.1/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)     3418 2023-07-17 00:57:37.000000 CompactObject_TOV-1.4.1/README.md
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.618384 CompactObject_TOV-1.4.1/TOVsolver/
+-rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/EoS_import.py
+-rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-17 00:59:11.000000 CompactObject_TOV-1.4.1/TOVsolver/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)      129 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/constant.py
+-rw-r--r--   0 a9         (501) staff       (20)     5622 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/main.py
+-rw-r--r--   0 a9         (501) staff       (20)     8598 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/solver_code.py
+-rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/speed_of_sound.py
+-rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/tests_script.py
+-rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-17 01:03:14.625687 CompactObject_TOV-1.4.1/setup.cfg
+-rw-r--r--   0 a9         (501) staff       (20)      136 2023-07-17 00:59:39.000000 CompactObject_TOV-1.4.1/setup.py
```

### Comparing `CompactObject_TOV-1.3.1/LICENSE` & `CompactObject_TOV-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.3.1/TOVsolver/EoS_import.py` & `CompactObject_TOV-1.4.1/TOVsolver/EoS_import.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.3.1/TOVsolver/main.py` & `CompactObject_TOV-1.4.1/TOVsolver/main.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.3.1/TOVsolver/solver_code.py` & `CompactObject_TOV-1.4.1/TOVsolver/solver_code.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.3.1/TOVsolver/speed_of_sound.py` & `CompactObject_TOV-1.4.1/TOVsolver/speed_of_sound.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.3.1/TOVsolver/tests_script.py` & `CompactObject_TOV-1.4.1/TOVsolver/tests_script.py`

 * *Files identical despite different names*

