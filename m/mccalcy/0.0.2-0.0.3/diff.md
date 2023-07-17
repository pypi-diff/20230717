# Comparing `tmp/mccalcy-0.0.2.tar.gz` & `tmp/mccalcy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.2.tar` & `mccalcy-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.2/.gitignore
--rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.2/115.ipynb
--rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.2/FirstProject_Calculator.ipynb
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.2/LICENSE
--rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.2/mccalcy/__init__.py
--rw-r--r--   0        0        0     2593 2023-07-17 17:32:29.645089 mccalcy-0.0.2/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-17 17:33:31.095158 mccalcy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1180 2023-07-15 21:15:27.774363 mccalcy-0.0.2/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.2/tox.ini
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.3/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.3/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.3/mccalcy/__init__.py
+-rw-r--r--   0        0        0     2615 2023-07-17 18:02:18.998730 mccalcy-0.0.3/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 18:04:40.996352 mccalcy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1180 2023-07-17 17:53:57.742749 mccalcy-0.0.3/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.3/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.3/PKG-INFO
```

### Comparing `mccalcy-0.0.2/.gitignore` & `mccalcy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/115.ipynb` & `mccalcy-0.0.3/115.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/FirstProject_Calculator.ipynb` & `mccalcy-0.0.3/FirstProject_Calculator.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/LICENSE` & `mccalcy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/README.md` & `mccalcy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/mccalcy/mccalcy.py` & `mccalcy-0.0.3/mccalcy/mccalcy.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             Returns:
                 None
             """
 
         try:
             result = self.memory / num
         except ZeroDivisionError:
-            print("Division by zero error")
+            print("Can't divide by zero, please select different value")
         except TypeError:
             print(f"{num} is not a number")
         else:
             self.memory = result
 
     def nth_root(self, root_value: int) -> float:
         """
@@ -93,15 +93,15 @@
                 The nth root of the number.
             """
 
         if root_value < 1:
             raise ValueError("The root value must be a positive number")
 
         try:
-            return self.memory ** (1 / root_value)
+            self.memory ** (1 / root_value)
         except TypeError:
             print(f"{root_value} is not a number")
 
     def reset_memory(self) -> None:
         """
         Resets the memory to 0.
```

### Comparing `mccalcy-0.0.2/tests/test_calc.py` & `mccalcy-0.0.3/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.2/PKG-INFO` & `mccalcy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
```

