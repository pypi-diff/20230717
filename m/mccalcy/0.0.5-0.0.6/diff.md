# Comparing `tmp/mccalcy-0.0.5.tar.gz` & `tmp/mccalcy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.5.tar` & `mccalcy-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.5/.gitignore
--rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.5/115.ipynb
--rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.5/FirstProject_Calculator.ipynb
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.5/LICENSE
--rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.5/mccalcy/__init__.py
--rw-r--r--   0        0        0     3259 2023-07-17 18:45:23.154784 mccalcy-0.0.5/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-17 18:46:33.417576 mccalcy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1180 2023-07-17 17:53:57.742749 mccalcy-0.0.5/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.5/tox.ini
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.6/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.6/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.6/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.6/mccalcy/__init__.py
+-rw-r--r--   0        0        0     3279 2023-07-17 19:03:07.206526 mccalcy-0.0.6/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 19:05:53.919268 mccalcy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2228 2023-07-17 18:49:46.724742 mccalcy-0.0.6/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.6/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.6/PKG-INFO
```

### Comparing `mccalcy-0.0.5/.gitignore` & `mccalcy-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.5/115.ipynb` & `mccalcy-0.0.6/115.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.5/FirstProject_Calculator.ipynb` & `mccalcy-0.0.6/FirstProject_Calculator.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.5/LICENSE` & `mccalcy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.5/README.md` & `mccalcy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.5/mccalcy/mccalcy.py` & `mccalcy-0.0.6/mccalcy/mccalcy.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             The nth root of the number.
         """
 
         # Check if the root value is less than 1.
         if root_value < 1:
             # Print an error message if value provided is less than 1.
             print("n value can't be less than 1")
+            return
 
         # Try to calculate the nth root of the number.
         try:
             result = self.memory ** (1 / root_value)
         except TypeError:
             # Print an error message if value is not a number.
             print(f"{root_value} is not a number")
```

### Comparing `mccalcy-0.0.5/PKG-INFO` & `mccalcy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
```

