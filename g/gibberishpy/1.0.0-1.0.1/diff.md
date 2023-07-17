# Comparing `tmp/gibberishpy-1.0.0.tar.gz` & `tmp/gibberishpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gibberishpy-1.0.0.tar", last modified: Mon Jul 17 12:09:13 2023, max compression
+gzip compressed data, was "gibberishpy-1.0.1.tar", last modified: Mon Jul 17 12:13:30 2023, max compression
```

## Comparing `gibberishpy-1.0.0.tar` & `gibberishpy-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:09:13.078015 gibberishpy-1.0.0/
--rw-rw-rw-   0        0        0     1733 2023-07-17 12:09:13.077017 gibberishpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2023-07-17 11:48:18.000000 gibberishpy-1.0.0/README.md
--rw-rw-rw-   0        0        0      665 2023-07-17 12:08:57.000000 gibberishpy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 12:09:13.078015 gibberishpy-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 12:09:13.055015 gibberishpy-1.0.0/src/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:54:17.000000 gibberishpy-1.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:09:13.057014 gibberishpy-1.0.0/src/gibberishpy/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:54:10.000000 gibberishpy-1.0.0/src/gibberishpy/__init__.py
--rw-rw-rw-   0        0        0      295 2023-07-17 11:28:32.000000 gibberishpy-1.0.0/src/gibberishpy/_error.py
--rw-rw-rw-   0        0        0    10372 2023-07-17 11:43:34.000000 gibberishpy-1.0.0/src/gibberishpy/scanner.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:09:13.076015 gibberishpy-1.0.0/src/gibberishpy.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-07-17 12:09:13.000000 gibberishpy-1.0.0/src/gibberishpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-07-17 12:09:13.000000 gibberishpy-1.0.0/src/gibberishpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:09:13.000000 gibberishpy-1.0.0/src/gibberishpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-17 12:09:13.000000 gibberishpy-1.0.0/src/gibberishpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 12:13:30.721928 gibberishpy-1.0.1/
+-rw-rw-rw-   0        0        0     1733 2023-07-17 12:13:30.721928 gibberishpy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2023-07-17 11:48:18.000000 gibberishpy-1.0.1/README.md
+-rw-rw-rw-   0        0        0      665 2023-07-17 12:13:14.000000 gibberishpy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:13:30.722930 gibberishpy-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 12:13:30.702929 gibberishpy-1.0.1/src/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:54:17.000000 gibberishpy-1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:13:30.704928 gibberishpy-1.0.1/src/gibberishpy/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:54:10.000000 gibberishpy-1.0.1/src/gibberishpy/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-07-17 11:28:32.000000 gibberishpy-1.0.1/src/gibberishpy/_error.py
+-rw-rw-rw-   0        0        0    10372 2023-07-17 11:43:34.000000 gibberishpy-1.0.1/src/gibberishpy/scanner.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:13:30.720927 gibberishpy-1.0.1/src/gibberishpy.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-07-17 12:13:30.000000 gibberishpy-1.0.1/src/gibberishpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-07-17 12:13:30.000000 gibberishpy-1.0.1/src/gibberishpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:13:30.000000 gibberishpy-1.0.1/src/gibberishpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 12:13:30.000000 gibberishpy-1.0.1/src/gibberishpy.egg-info/top_level.txt
```

### Comparing `gibberishpy-1.0.0/PKG-INFO` & `gibberishpy-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gibberishpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Using Markov chain to detect gibberish in text.
 Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
-Project-URL: Homepage, https://github.com/yuenshingyan/pygibberish
-Project-URL: Bug Tracker, https://github.com/yuenshingyan/pygibberish/issues
+Project-URL: Homepage, https://github.com/yuenshingyan/gibberishpy
+Project-URL: Bug Tracker, https://github.com/yuenshingyan/gibberishpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # pygibberish
```

### Comparing `gibberishpy-1.0.0/README.md` & `gibberishpy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gibberishpy-1.0.0/pyproject.toml` & `gibberishpy-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "gibberishpy"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Yuen Shing Yan Hindy", email="yuenshingyan@gmail.com" },
 ]
 description = "Using Markov chain to detect gibberish in text."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/yuenshingyan/pygibberish"
-"Bug Tracker" = "https://github.com/yuenshingyan/pygibberish/issues"
+"Homepage" = "https://github.com/yuenshingyan/gibberishpy"
+"Bug Tracker" = "https://github.com/yuenshingyan/gibberishpy/issues"
 
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `gibberishpy-1.0.0/src/gibberishpy/scanner.py` & `gibberishpy-1.0.1/src/gibberishpy/scanner.py`

 * *Files identical despite different names*

### Comparing `gibberishpy-1.0.0/src/gibberishpy.egg-info/PKG-INFO` & `gibberishpy-1.0.1/src/gibberishpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gibberishpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Using Markov chain to detect gibberish in text.
 Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
-Project-URL: Homepage, https://github.com/yuenshingyan/pygibberish
-Project-URL: Bug Tracker, https://github.com/yuenshingyan/pygibberish/issues
+Project-URL: Homepage, https://github.com/yuenshingyan/gibberishpy
+Project-URL: Bug Tracker, https://github.com/yuenshingyan/gibberishpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # pygibberish
```

