# Comparing `tmp/pyees-1.4.0.tar.gz` & `tmp/pyees-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.0.tar", last modified: Sun Jul 16 07:04:10 2023, max compression
+gzip compressed data, was "pyees-1.4.1.tar", last modified: Mon Jul 17 07:26:26 2023, max compression
```

## Comparing `pyees-1.4.0.tar` & `pyees-1.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:04:09.433721 pyees-1.4.0/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-16 07:04:10.172283 pyees-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 07:04:09.983787 pyees-1.4.0/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.0/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.0/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.0/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.0/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.0/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.0/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.0/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.0/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-16 06:54:08.000000 pyees-1.4.0/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.0/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.4.0/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.0/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.0/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-16 07:04:09.908988 pyees-1.4.0/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.4.0/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.0/pyees/unit.py
--rw-rw-rw-   0        0        0    34114 2023-07-16 07:04:10.000740 pyees-1.4.0/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:04:10.142365 pyees-1.4.0/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-16 07:04:09.000000 pyees-1.4.0/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 07:04:10.156326 pyees-1.4.0/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-16 07:04:10.202201 pyees-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-16 07:04:00.000000 pyees-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.625005 pyees-1.4.1/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-17 07:26:26.640630 pyees-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.328119 pyees-1.4.1/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.1/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.1/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.1/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.1/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.1/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.1/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.1/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.1/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.1/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.1/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.1/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.1/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.1/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.4.1/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84033 2023-07-17 07:24:33.000000 pyees-1.4.1/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.1/pyees/unit.py
+-rw-rw-rw-   0        0        0    33943 2023-07-17 07:25:31.000000 pyees-1.4.1/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.562502 pyees-1.4.1/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-17 07:26:26.656255 pyees-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-17 07:26:19.000000 pyees-1.4.1/setup.py
```

### Comparing `pyees-1.4.0/LICENSE.txt` & `pyees-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/PKG-INFO` & `pyees-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.0
+Version: 1.4.1
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.0/README.md` & `pyees-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/fit.py` & `pyees-1.4.1/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/profileFit.py` & `pyees-1.4.1/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/profilePyees.py` & `pyees-1.4.1/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/prop.py` & `pyees-1.4.1/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/sheet.py` & `pyees-1.4.1/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/solve.py` & `pyees-1.4.1/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/stackOverflowODR.py` & `pyees-1.4.1/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testFit.py` & `pyees-1.4.1/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testProp.py` & `pyees-1.4.1/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testPyees.py` & `pyees-1.4.1/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testSheet.py` & `pyees-1.4.1/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testSolve.py` & `pyees-1.4.1/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testUnit.py` & `pyees-1.4.1/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/testVariable.py` & `pyees-1.4.1/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1307,14 +1307,29 @@
         diameter = variable(40, 'cm', 0.2)
         area = np.pi / 4 * diameter ** 2
         area.convert('m2')
         self.assertEqual(area.value, 0.12566370614359172953850573)
         self.assertEqual(area.unit, 'm2')
         self.assertEqual(area.uncert, np.sqrt((2 * np.pi / 4 * 0.4 * 0.002)**2))  
 
+        time = variable([1,2,3], 's', [0.1, 0.2, 0.3])
+        time.convert('min')
+        np.testing.assert_array_equal(time.value, np.array([1,2,3]) / 60)
+        self.assertEqual(time.unit, 'min')
+        np.testing.assert_array_equal(time.uncert, np.array([0.1,0.2,0.3]) / 60)
+        self.assertEqual(time[0].value, 1/60)
+        self.assertEqual(time[1].value, 2/60)
+        self.assertEqual(time[2].value, 3/60)
+        self.assertEqual(time[0].unit, 'min')
+        self.assertEqual(time[1].unit, 'min')
+        self.assertEqual(time[2].unit, 'min')
+        self.assertEqual(time[0].uncert, 0.1/60)
+        self.assertEqual(time[1].uncert, 0.2/60)
+        self.assertEqual(time[2].uncert, 0.3/60)
+
     def testCompare(self):
         a = variable(1, 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
         np.testing.assert_equal(a > b, [False, False, False])
         np.testing.assert_equal(a >= b, [False, False, False])
```

### Comparing `pyees-1.4.0/pyees/unit.py` & `pyees-1.4.1/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.0/pyees/variable.py` & `pyees-1.4.1/pyees/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,18 +888,20 @@
         return variable(self.value[index], self.unit, self.uncert[index])
     
     def mean(self):
         return sum(self) / len(self)
     
     def convert(self, newUnit):
         converter = self._unitObject.getConverter(newUnit)
+        newUnit = unit(newUnit)
         for elem in self.scalarVariables:
             elem._value = converter.convert(elem._value, useOffset=not self._unitObject.isCombinationUnit())
             elem._uncert = converter.convert(elem._uncert, useOffset=False)
-        self._unitObject = unit(newUnit)
+            elem._unitObject = newUnit
+        self._unitObject = newUnit
 
     def __iter__(self):
         self.n = 0
         return self
 
     def __next__(self):
         if self.n < len(self):
@@ -945,19 +947,13 @@
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 if __name__ == "__main__":
-    a = variable(23, 'deg', 2)
-    # a = variable(np.pi / 180 * 23, 'rad', np.pi /  180 *2)
-    b = np.sin(a)
-    print(b.dependsOn[a])
-    a.convert('rad')
-    print(b.dependsOn[a])
-    c = a * b
+    time = variable([601.15],'s')
+    time.convert('min')
     
-    
-    val = np.pi / 180 * 23
-    unc = np.pi / 180 * 2
-    print(c.uncert, np.sqrt((unc * (np.sin(val) + val * np.cos(val)))**2))
+    print(time)
+    print(time[0])
+
```

### Comparing `pyees-1.4.0/pyees.egg-info/PKG-INFO` & `pyees-1.4.1/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.0
+Version: 1.4.1
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.0/setup.py` & `pyees-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.0',
+    version='1.4.1',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

