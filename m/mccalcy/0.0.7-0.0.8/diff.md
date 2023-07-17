# Comparing `tmp/mccalcy-0.0.7.tar.gz` & `tmp/mccalcy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.7.tar` & `mccalcy-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.7/.gitignore
--rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.7/115.ipynb
--rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.7/FirstProject_Calculator.ipynb
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.7/LICENSE
--rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.7/mccalcy/__init__.py
--rw-r--r--   0        0        0     3063 2023-07-17 19:21:23.194988 mccalcy-0.0.7/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-17 19:21:34.434612 mccalcy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2228 2023-07-17 18:49:46.724742 mccalcy-0.0.7/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.7/tox.ini
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.8/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.8/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.8/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.8/mccalcy/__init__.py
+-rw-r--r--   0        0        0     3149 2023-07-17 19:26:10.902310 mccalcy-0.0.8/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 19:26:02.421129 mccalcy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2228 2023-07-17 18:49:46.724742 mccalcy-0.0.8/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.8/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.8/PKG-INFO
```

### Comparing `mccalcy-0.0.7/.gitignore` & `mccalcy-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/115.ipynb` & `mccalcy-0.0.8/115.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/FirstProject_Calculator.ipynb` & `mccalcy-0.0.8/FirstProject_Calculator.ipynb`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/LICENSE` & `mccalcy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/README.md` & `mccalcy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/mccalcy/mccalcy.py` & `mccalcy-0.0.8/mccalcy/mccalcy.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,41 +84,40 @@
             print("Can't divide by zero, please select different value")
         except TypeError:
             # Print an error message if value is not a number.
             print(f"{num} is not a number")
         else:
             self.memory = result
 
+    def nth_root(self, root_value: int) -> float:
+        """
+        Calculates the nth root of a number.
+
+        Args:
+            root_value: The root value.
+
+        Returns:
+            The nth root of the number.
+        """
+        try:
+            root_value = float(root_value)
+        except TypeError:
+            print(f"{root_value} is not a number")
+            return
+
+        if root_value < 1:
+            print("n value can't be less than 1")
+            return
 
-def nth_root(self, root_value: int) -> float:
-    """
-    Calculates the nth root of a number.
-
-    Args:
-        root_value: The root value.
-
-    Returns:
-        The nth root of the number.
-    """
-    try:
-        root_value = float(root_value)
-    except TypeError:
-        print(f"{root_value} is not a number")
-        return
-
-    if root_value < 1:
-        print("n value can't be less than 1")
-        return
-
-    try:
-        result = self.memory ** (1 / root_value)
-    except TypeError:
-        print(f"{self.memory} is not a number")
-    else:
-        self.memory = result
+        try:
+            result = self.memory ** (1 / root_value)
+        except TypeError:
+            print(f"{self.memory} is not a number")
+        else:
+            self.memory = result
 
     def reset_memory(self) -> None:
         """
         Resets the memory to 0.
 
         Returns:
             None
```

### Comparing `mccalcy-0.0.7/tests/test_calc.py` & `mccalcy-0.0.8/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.7/PKG-INFO` & `mccalcy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
```

