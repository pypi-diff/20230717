# Comparing `tmp/gibberishpy-1.0.2.tar.gz` & `tmp/gibberishpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gibberishpy-1.0.2.tar", last modified: Mon Jul 17 12:14:59 2023, max compression
+gzip compressed data, was "gibberishpy-1.0.3.tar", last modified: Mon Jul 17 12:16:11 2023, max compression
```

## Comparing `gibberishpy-1.0.2.tar` & `gibberishpy-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:59.975466 gibberishpy-1.0.2/
--rw-rw-rw-   0        0        0     1733 2023-07-17 12:14:59.975466 gibberishpy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2023-07-17 12:14:32.000000 gibberishpy-1.0.2/README.md
--rw-rw-rw-   0        0        0      665 2023-07-17 12:14:44.000000 gibberishpy-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 12:14:59.975466 gibberishpy-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:59.957466 gibberishpy-1.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:54:17.000000 gibberishpy-1.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:59.960470 gibberishpy-1.0.2/src/gibberishpy/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:54:10.000000 gibberishpy-1.0.2/src/gibberishpy/__init__.py
--rw-rw-rw-   0        0        0      295 2023-07-17 11:28:32.000000 gibberishpy-1.0.2/src/gibberishpy/_error.py
--rw-rw-rw-   0        0        0    10372 2023-07-17 11:43:34.000000 gibberishpy-1.0.2/src/gibberishpy/scanner.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:59.974465 gibberishpy-1.0.2/src/gibberishpy.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-07-17 12:14:59.000000 gibberishpy-1.0.2/src/gibberishpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-07-17 12:14:59.000000 gibberishpy-1.0.2/src/gibberishpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:14:59.000000 gibberishpy-1.0.2/src/gibberishpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-17 12:14:59.000000 gibberishpy-1.0.2/src/gibberishpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 12:16:11.456328 gibberishpy-1.0.3/
+-rw-rw-rw-   0        0        0     1732 2023-07-17 12:16:11.456328 gibberishpy-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1192 2023-07-17 12:15:59.000000 gibberishpy-1.0.3/README.md
+-rw-rw-rw-   0        0        0      665 2023-07-17 12:15:59.000000 gibberishpy-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:16:11.456328 gibberishpy-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 12:16:11.438331 gibberishpy-1.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:54:17.000000 gibberishpy-1.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:16:11.440330 gibberishpy-1.0.3/src/gibberishpy/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:54:10.000000 gibberishpy-1.0.3/src/gibberishpy/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-07-17 11:28:32.000000 gibberishpy-1.0.3/src/gibberishpy/_error.py
+-rw-rw-rw-   0        0        0    10372 2023-07-17 11:43:34.000000 gibberishpy-1.0.3/src/gibberishpy/scanner.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:16:11.455328 gibberishpy-1.0.3/src/gibberishpy.egg-info/
+-rw-rw-rw-   0        0        0     1732 2023-07-17 12:16:11.000000 gibberishpy-1.0.3/src/gibberishpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-07-17 12:16:11.000000 gibberishpy-1.0.3/src/gibberishpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:16:11.000000 gibberishpy-1.0.3/src/gibberishpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 12:16:11.000000 gibberishpy-1.0.3/src/gibberishpy.egg-info/top_level.txt
```

### Comparing `gibberishpy-1.0.2/PKG-INFO` & `gibberishpy-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gibberishpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Using Markov chain to detect gibberish in text.
 Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
 Project-URL: Homepage, https://github.com/yuenshingyan/gibberishpy
 Project-URL: Bug Tracker, https://github.com/yuenshingyan/gibberishpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 -----------
 
     from gibberishpy.scanner import GibberishScanner
     
     
     if __name__ == "__main__":
         scanner = GibberishScanner()
-        scanner.build_model(corpus_path="path/to//corpus.txt", n_gram_size=2)
+        scanner.build_model(corpus_path="path/to/corpus.txt", n_gram_size=2)
         scanner.save_model("transition_matrix_2d.tm", encoding="utf-8")
 
 Scan Gibberish
 --------------
 
     from gibberishpy.scanner import GibberishScanner
```

### Comparing `gibberishpy-1.0.2/README.md` & `gibberishpy-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 -----------
 
     from gibberishpy.scanner import GibberishScanner
     
     
     if __name__ == "__main__":
         scanner = GibberishScanner()
-        scanner.build_model(corpus_path="path/to//corpus.txt", n_gram_size=2)
+        scanner.build_model(corpus_path="path/to/corpus.txt", n_gram_size=2)
         scanner.save_model("transition_matrix_2d.tm", encoding="utf-8")
 
 Scan Gibberish
 --------------
 
     from gibberishpy.scanner import GibberishScanner
```

### Comparing `gibberishpy-1.0.2/pyproject.toml` & `gibberishpy-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gibberishpy"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Yuen Shing Yan Hindy", email="yuenshingyan@gmail.com" },
 ]
 description = "Using Markov chain to detect gibberish in text."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gibberishpy-1.0.2/src/gibberishpy/scanner.py` & `gibberishpy-1.0.3/src/gibberishpy/scanner.py`

 * *Files identical despite different names*

### Comparing `gibberishpy-1.0.2/src/gibberishpy.egg-info/PKG-INFO` & `gibberishpy-1.0.3/src/gibberishpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gibberishpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Using Markov chain to detect gibberish in text.
 Author-email: Yuen Shing Yan Hindy <yuenshingyan@gmail.com>
 Project-URL: Homepage, https://github.com/yuenshingyan/gibberishpy
 Project-URL: Bug Tracker, https://github.com/yuenshingyan/gibberishpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 -----------
 
     from gibberishpy.scanner import GibberishScanner
     
     
     if __name__ == "__main__":
         scanner = GibberishScanner()
-        scanner.build_model(corpus_path="path/to//corpus.txt", n_gram_size=2)
+        scanner.build_model(corpus_path="path/to/corpus.txt", n_gram_size=2)
         scanner.save_model("transition_matrix_2d.tm", encoding="utf-8")
 
 Scan Gibberish
 --------------
 
     from gibberishpy.scanner import GibberishScanner
```

