# Comparing `tmp/mccalcy-0.0.3.tar.gz` & `tmp/mccalcy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.3.tar` & `mccalcy-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.3/.gitignore
--rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.3/115.ipynb
--rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.3/FirstProject_Calculator.ipynb
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.3/LICENSE
--rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.3/mccalcy/__init__.py
--rw-r--r--   0        0        0     2615 2023-07-17 18:02:18.998730 mccalcy-0.0.3/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-17 18:04:40.996352 mccalcy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1180 2023-07-17 17:53:57.742749 mccalcy-0.0.3/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.3/tox.ini
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.4/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.4/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.4/mccalcy/__init__.py
+-rw-r--r--   0        0        0     2673 2023-07-17 18:13:13.044789 mccalcy-0.0.4/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 18:16:02.396531 mccalcy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1180 2023-07-17 17:53:57.742749 mccalcy-0.0.4/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.4/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.4/PKG-INFO
```

### Comparing `mccalcy-0.0.3/.gitignore` & `mccalcy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/115.ipynb` & `mccalcy-0.0.4/115.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/FirstProject_Calculator.ipynb` & `mccalcy-0.0.4/FirstProject_Calculator.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/LICENSE` & `mccalcy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/README.md` & `mccalcy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/mccalcy/mccalcy.py` & `mccalcy-0.0.4/mccalcy/mccalcy.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,19 @@
                 The nth root of the number.
             """
 
         if root_value < 1:
             raise ValueError("The root value must be a positive number")
 
         try:
-            self.memory ** (1 / root_value)
+            result = self.memory ** (1 / root_value)
         except TypeError:
             print(f"{root_value} is not a number")
+        else:
+            self.memory = result
 
     def reset_memory(self) -> None:
         """
         Resets the memory to 0.
 
         Returns:
             None
```

### Comparing `mccalcy-0.0.3/tests/test_calc.py` & `mccalcy-0.0.4/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.3/PKG-INFO` & `mccalcy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
```

