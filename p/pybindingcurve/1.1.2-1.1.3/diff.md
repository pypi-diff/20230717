# Comparing `tmp/pybindingcurve-1.1.2.tar.gz` & `tmp/pybindingcurve-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\steve\Documents\Repos\pybindingcurve\dist\tmpqfsvhwzz\pybindingcurve-1.1.2.tar", last modified: Sun Aug 28 13:09:13 2022, max compression
+gzip compressed data, was "pybindingcurve-1.1.3.tar", last modified: Mon Jul 17 11:31:14 2023, max compression
```

## Comparing `pybindingcurve-1.1.2.tar` & `pybindingcurve-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-08-28 13:09:13.135869 pybindingcurve-1.1.2/
--rw-rw-rw-   0        0        0     1090 2021-02-26 17:30:06.000000 pybindingcurve-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2981 2022-08-28 13:09:13.134876 pybindingcurve-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2509 2022-07-03 21:36:19.000000 pybindingcurve-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-08-28 13:09:13.037163 pybindingcurve-1.1.2/pybindingcurve/
--rw-rw-rw-   0        0        0       31 2020-11-09 12:22:29.000000 pybindingcurve-1.1.2/pybindingcurve/__init__.py
--rw-rw-rw-   0        0        0    30922 2022-06-23 20:56:05.000000 pybindingcurve-1.1.2/pybindingcurve/pybindingcurve.py
--rw-rw-rw-   0        0        0      609 2022-07-03 21:36:47.000000 pybindingcurve-1.1.2/pybindingcurve/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-28 13:09:13.131872 pybindingcurve-1.1.2/pybindingcurve/systems/
--rw-rw-rw-   0        0        0      177 2021-04-06 13:46:50.000000 pybindingcurve-1.1.2/pybindingcurve/systems/__init__.py
--rw-rw-rw-   0        0        0    71965 2021-04-15 11:35:55.000000 pybindingcurve-1.1.2/pybindingcurve/systems/analytical_equations.py
--rw-rw-rw-   0        0        0     4384 2021-04-15 10:47:59.000000 pybindingcurve-1.1.2/pybindingcurve/systems/analytical_systems.py
--rw-rw-rw-   0        0        0     9159 2022-07-03 21:22:17.000000 pybindingcurve-1.1.2/pybindingcurve/systems/binding_system.py
--rw-rw-rw-   0        0        0     7679 2021-04-06 13:46:50.000000 pybindingcurve-1.1.2/pybindingcurve/systems/kinetic_systems.py
--rw-rw-rw-   0        0        0    16919 2021-04-06 13:46:51.000000 pybindingcurve-1.1.2/pybindingcurve/systems/kinetic_systems_1_to_1to5.py
--rw-rw-rw-   0        0        0    15566 2021-04-08 12:07:35.000000 pybindingcurve-1.1.2/pybindingcurve/systems/lagrange_binding_system_factory.py
--rw-rw-rw-   0        0        0    12905 2021-04-06 13:46:51.000000 pybindingcurve-1.1.2/pybindingcurve/systems/lagrange_systems.py
--rw-rw-rw-   0        0        0    17154 2022-08-28 13:03:33.000000 pybindingcurve-1.1.2/pybindingcurve/systems/minimizer_binding_system_factory.py
--rw-rw-rw-   0        0        0    13324 2021-04-15 21:44:41.000000 pybindingcurve-1.1.2/pybindingcurve/systems/minimizer_systems.py
--rw-rw-rw-   0        0        0      155 2021-04-06 13:46:51.000000 pybindingcurve-1.1.2/pybindingcurve/systems/systems.py
-drwxrwxrwx   0        0        0        0 2022-08-28 13:09:13.073029 pybindingcurve-1.1.2/pybindingcurve.egg-info/
--rw-rw-rw-   0        0        0     2981 2022-08-28 13:09:12.000000 pybindingcurve-1.1.2/pybindingcurve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2022-08-28 13:09:13.000000 pybindingcurve-1.1.2/pybindingcurve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-28 13:09:12.000000 pybindingcurve-1.1.2/pybindingcurve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2022-08-28 13:09:12.000000 pybindingcurve-1.1.2/pybindingcurve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-08-28 13:09:12.000000 pybindingcurve-1.1.2/pybindingcurve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-28 13:09:13.136860 pybindingcurve-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2022-08-28 13:04:46.000000 pybindingcurve-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:31:14.885814 pybindingcurve-1.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-07-17 11:31:14.884815 pybindingcurve-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:31:14.833322 pybindingcurve-1.1.3/pybindingcurve/
+-rw-rw-rw-   0        0        0       31 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/__init__.py
+-rw-rw-rw-   0        0        0    31088 2023-07-17 11:16:43.000000 pybindingcurve-1.1.3/pybindingcurve/pybindingcurve.py
+-rw-rw-rw-   0        0        0      609 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:31:14.883814 pybindingcurve-1.1.3/pybindingcurve/systems/
+-rw-rw-rw-   0        0        0      177 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/__init__.py
+-rw-rw-rw-   0        0        0    71965 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/analytical_equations.py
+-rw-rw-rw-   0        0        0     4384 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/analytical_systems.py
+-rw-rw-rw-   0        0        0     9159 2023-07-17 11:17:08.000000 pybindingcurve-1.1.3/pybindingcurve/systems/binding_system.py
+-rw-rw-rw-   0        0        0     7679 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/kinetic_systems.py
+-rw-rw-rw-   0        0        0    16919 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/kinetic_systems_1_to_1to5.py
+-rw-rw-rw-   0        0        0    15566 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/lagrange_binding_system_factory.py
+-rw-rw-rw-   0        0        0    12905 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/lagrange_systems.py
+-rw-rw-rw-   0        0        0    17154 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/minimizer_binding_system_factory.py
+-rw-rw-rw-   0        0        0    13324 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/minimizer_systems.py
+-rw-rw-rw-   0        0        0      155 2023-07-13 14:23:13.000000 pybindingcurve-1.1.3/pybindingcurve/systems/systems.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:31:14.845825 pybindingcurve-1.1.3/pybindingcurve.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-07-17 11:31:14.000000 pybindingcurve-1.1.3/pybindingcurve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-07-17 11:31:14.000000 pybindingcurve-1.1.3/pybindingcurve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:31:14.000000 pybindingcurve-1.1.3/pybindingcurve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-17 11:31:14.000000 pybindingcurve-1.1.3/pybindingcurve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 11:31:14.000000 pybindingcurve-1.1.3/pybindingcurve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:31:14.885814 pybindingcurve-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-17 11:30:52.000000 pybindingcurve-1.1.3/setup.py
```

### Comparing `pybindingcurve-1.1.2/LICENSE` & `pybindingcurve-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/PKG-INFO` & `pybindingcurve-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybindingcurve
-Version: 1.1.2
+Version: 1.1.3
 Summary: Protein ligand binding simulation in Python
 Home-page: https://github.com/stevenshave/pybindingcurve
 Author: Steven Shave
 Author-email: steve.nshave@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybindingcurve-1.1.2/README.md` & `pybindingcurve-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/pybindingcurve.py` & `pybindingcurve-1.1.3/pybindingcurve/pybindingcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,14 +410,17 @@
             pbc.Readout class.
         """
         if self.system is None:
             print("No system defined, could not proceed")
             return None
         self._initialize_plot()
         changing_parameters = self._find_changing_parameters(parameters)
+        if changing_parameters is None:
+            print("No changing parameters detected. Plotting curves requires something to be changing")
+            return
         if not len(changing_parameters) == 1:
             print("Must have 1 changing parameter, no curves added.")
             return
 
         y_values = self.system.query(parameters)
 
         if readout is not None:
```

### Comparing `pybindingcurve-1.1.2/pybindingcurve/setup.py` & `pybindingcurve-1.1.3/pybindingcurve/setup.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/analytical_equations.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/analytical_equations.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/analytical_systems.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/analytical_systems.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/binding_system.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/binding_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         
         # Are any parameters changing?
         changing_parameters = self._find_changing_parameters(parameters)
         if changing_parameters is None:  # Querying single point
             if self.analytical:
                 results = self._system(**parameters)  # Analytical
             else:
-                simulation_results=self._system(**tmp_params)
+                simulation_results=self._system(**parameters)
                 if self.default_readout not in simulation_results:
                     self.default_readout=f"{self.default_readout}_f"
                 results = simulation_results[self.default_readout]
                 
         else:
             # At least 1 changing parameter
             if len(changing_parameters) == 1:
```

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/kinetic_systems.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/kinetic_systems.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/kinetic_systems_1_to_1to5.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/kinetic_systems_1_to_1to5.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/lagrange_binding_system_factory.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/lagrange_binding_system_factory.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/lagrange_systems.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/lagrange_systems.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/minimizer_binding_system_factory.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/minimizer_binding_system_factory.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve/systems/minimizer_systems.py` & `pybindingcurve-1.1.3/pybindingcurve/systems/minimizer_systems.py`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/pybindingcurve.egg-info/PKG-INFO` & `pybindingcurve-1.1.3/pybindingcurve.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybindingcurve
-Version: 1.1.2
+Version: 1.1.3
 Summary: Protein ligand binding simulation in Python
 Home-page: https://github.com/stevenshave/pybindingcurve
 Author: Steven Shave
 Author-email: steve.nshave@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybindingcurve-1.1.2/pybindingcurve.egg-info/SOURCES.txt` & `pybindingcurve-1.1.3/pybindingcurve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybindingcurve-1.1.2/setup.py` & `pybindingcurve-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybindingcurve",
-    version="1.1.2",
+    version="1.1.3",
     author="Steven Shave",
     author_email="steve.nshave@gmail.com",
     description="Protein ligand binding simulation in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stevenshave/pybindingcurve",
     packages=setuptools.find_packages(),
```

