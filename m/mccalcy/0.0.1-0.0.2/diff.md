# Comparing `tmp/mccalcy-0.0.1.tar.gz` & `tmp/mccalcy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccalcy-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mccalcy-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mccalcy-0.0.1.tar` & `mccalcy-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.1/LICENSE
--rw-r--r--   0        0        0     1180 2023-07-15 19:52:14.010328 mccalcy-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.1/mccalcy/__init__.py
--rw-r--r--   0        0        0     1811 2023-07-15 20:19:29.407794 mccalcy-0.0.1/mccalcy/mccalcy.py
--rw-r--r--   0        0        0      481 2023-07-15 20:25:28.681458 mccalcy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1201 2023-07-15 20:19:54.345895 mccalcy-0.0.1/tests/test_calc.py
--rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.1/tox.ini
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 mccalcy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3238 2023-07-15 19:13:04.376500 mccalcy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     8182 2023-07-16 18:41:45.492165 mccalcy-0.0.2/115.ipynb
+-rw-r--r--   0        0        0     4123 2023-07-16 18:51:22.966875 mccalcy-0.0.2/FirstProject_Calculator.ipynb
+-rw-r--r--   0        0        0     1097 2023-07-15 19:51:19.024270 mccalcy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1157 2023-07-16 17:55:43.654001 mccalcy-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:32:48.274767 mccalcy-0.0.2/mccalcy/__init__.py
+-rw-r--r--   0        0        0     2593 2023-07-17 17:32:29.645089 mccalcy-0.0.2/mccalcy/mccalcy.py
+-rw-r--r--   0        0        0      481 2023-07-17 17:33:31.095158 mccalcy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1180 2023-07-15 21:15:27.774363 mccalcy-0.0.2/tests/test_calc.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:27:31.283657 mccalcy-0.0.2/tox.ini
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 mccalcy-0.0.2/PKG-INFO
```

### Comparing `mccalcy-0.0.1/.gitignore` & `mccalcy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.1/LICENSE` & `mccalcy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mccalcy-0.0.1/README.md` & `mccalcy-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 ```
 pip install mccalcy
 ```
 
 ## Usage
 
-First, import the `Calculator` class from the package:
+First, import the package:
 
 ```python
-from mccalcy import Calculator
+from mccalcy import mccalcy
 ```
 
 Create a Calculator instance:
 
 ```python
-calc = Calculator()
+calc = mccalcy.Calculator()
 ```
 
 Perform calculations using the available methods:
 
 ```python
 calc.add(5)
 calc.subtract(2)
```

### Comparing `mccalcy-0.0.1/tests/test_calc.py` & `mccalcy-0.0.2/tests/test_calc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import pytest
-from mccalcy import calculator
+from mccalcy import mccalcy
 
 
 def test_add() -> None:
     """
     Test the add() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(10)
     assert calc.memory == 10
 
 
 def test_subtract() -> None:
     """
     Test the subtract() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(10)
     calc.subtract(5)
     assert calc.memory == 5
 
 
 def test_multiply() -> None:
     """
     Test the multiply() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(10)
     calc.multiply(2)
     assert calc.memory == 20
 
 
 def test_divide() -> None:
     """
     Test the divide() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(10)
     calc.divide(2)
     assert calc.memory == 5
 
 
 def test_root() -> None:
     """
     Test the root() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(16)
     calc.root(2)
     assert calc.memory == 4
 
 
 def test_reset_memory() -> None:
     """
     Test the reset_memory() method.
     """
-    calc = calculator.Calculator()
+    calc = mccalcy.Calculator()
     calc.add(10)
     calc.reset_memory()
     assert calc.memory == 0
 
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `mccalcy-0.0.1/PKG-INFO` & `mccalcy-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccalcy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small test package with calculator module.
 Author-email: Vitalijus <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/VitalijusKiubis/mccalcy
 
@@ -18,24 +18,24 @@
 
 ```
 pip install mccalcy
 ```
 
 ## Usage
 
-First, import the `Calculator` class from the package:
+First, import the package:
 
 ```python
-from mccalcy import Calculator
+from mccalcy import mccalcy
 ```
 
 Create a Calculator instance:
 
 ```python
-calc = Calculator()
+calc = mccalcy.Calculator()
 ```
 
 Perform calculations using the available methods:
 
 ```python
 calc.add(5)
 calc.subtract(2)
```

