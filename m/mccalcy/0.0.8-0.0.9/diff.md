# Comparing `tmp/mccalcy-0.0.8.tar.gz` & `tmp/mccalcy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.8.tar` & `mccalcy-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.8/.gitignore
--rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.8/115.ipynb
--rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.8/FirstProject_Calculator.ipynb
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.8/LICENSE
--rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.8/mccalcy/__init__.py
--rw-r--r--   0        0        0     3149 2023-07-17 19:26:10.902310 mccalcy-0.0.8/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-17 19:26:02.421129 mccalcy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2228 2023-07-17 18:49:46.724742 mccalcy-0.0.8/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.8/tox.ini
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.9/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.9/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.9/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.9/mccalcy/__init__.py
+-rw-r--r--   0        0        0     3204 2023-07-17 19:55:05.292221 mccalcy-0.0.9/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 19:55:15.047902 mccalcy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2570 2023-07-17 19:42:41.994737 mccalcy-0.0.9/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.9/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.9/PKG-INFO
```

### Comparing `mccalcy-0.0.8/.gitignore` & `mccalcy-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.8/115.ipynb` & `mccalcy-0.0.9/115.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.8/FirstProject_Calculator.ipynb` & `mccalcy-0.0.9/FirstProject_Calculator.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.8/LICENSE` & `mccalcy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.8/README.md` & `mccalcy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.8/mccalcy/mccalcy.py` & `mccalcy-0.0.9/mccalcy/mccalcy.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         Returns:
             None
         """
         try:
             self.memory += num
         except TypeError:
             # Print an error message if value is not a number.
-            print(f"{num} is not a number")
+            raise TypeError(f"{num} is not a number")
 
     def subtract(self, num: float) -> None:
         """
         Subtracts the given number from the memory.
 
         Args:
             num: The number to be subtracted.
@@ -43,15 +43,15 @@
         Returns:
             None
         """
         try:
             self.memory -= num
         except TypeError:
             # Print an error message if value is not a number.
-            print(f"{num} is not a number")
+            raise TypeError(f"{num} is not a number")
 
     def multiply(self, num: float) -> None:
         """
         Multiplies the memory by the given number.
 
         Args:
             num: The number to multiply by.
@@ -59,15 +59,15 @@
         Returns:
             None
         """
         try:
             self.memory *= num
         except TypeError:
             # Print an error message if value is not a number.
-            print(f"{num} is not a number")
+            raise TypeError(f"{num} is not a number")
 
     def divide(self, num: float) -> None:
         """
         Divides the memory by the given number.
 
         Args:
             num: The number to divide by.
@@ -80,44 +80,42 @@
         try:
             result = self.memory / num
         except ZeroDivisionError:
             # Print an error message if user tries to divide by zero.
             print("Can't divide by zero, please select different value")
         except TypeError:
             # Print an error message if value is not a number.
-            print(f"{num} is not a number")
+            raise TypeError(f"{num} is not a number")
         else:
             self.memory = result
 
-    def nth_root(self, root_value: int) -> float:
+    def nth_root(self, root_value: int) -> None:
         """
         Calculates the nth root of a number.
 
         Args:
             root_value: The root value.
 
         Returns:
-            The nth root of the number.
+            None
         """
         try:
             root_value = float(root_value)
-        except TypeError:
-            print(f"{root_value} is not a number")
-            return
+        except (TypeError, ValueError):
+            raise TypeError(f"Invalid value: '{root_value}' is not a number")
 
         if root_value < 1:
-            print("n value can't be less than 1")
-            return
+            raise ValueError("Root value must be greater than or equal to 1")
 
         try:
             result = self.memory ** (1 / root_value)
         except TypeError:
-            print(f"{self.memory} is not a number")
-        else:
-            self.memory = result
+            raise TypeError(f"Invalid value: '{self.memory}' is not a number")
+
+        self.memory = result
 
     def reset_memory(self) -> None:
         """
         Resets the memory to 0.
 
         Returns:
             None
```

### Comparing `mccalcy-0.0.8/PKG-INFO` & `mccalcy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
```

