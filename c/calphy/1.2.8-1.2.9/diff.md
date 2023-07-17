# Comparing `tmp/calphy-1.2.8.tar.gz` & `tmp/calphy-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calphy-1.2.8.tar", last modified: Mon Mar 13 09:50:23 2023, max compression
+gzip compressed data, was "calphy-1.2.9.tar", last modified: Fri Jun  2 06:44:56 2023, max compression
```

## Comparing `calphy-1.2.8.tar` & `calphy-1.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:50:23.676066 calphy-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-03-13 09:50:20.000000 calphy-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-13 09:50:20.000000 calphy-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-13 09:50:23.676066 calphy-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-13 09:50:20.000000 calphy-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:50:23.672066 calphy-1.2.8/calphy/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/composition_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27125 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/liquid.py
--rw-r--r--   0 runner    (1001) docker     (123)    41096 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/queuekernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/solid.py
--rw-r--r--   0 runner    (1001) docker     (123)    61627 2023-03-13 09:50:20.000000 calphy-1.2.8/calphy/splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:50:23.672066 calphy-1.2.8/calphy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-13 09:50:23.000000 calphy-1.2.8/calphy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 09:50:23.676066 calphy-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-13 09:50:23.000000 calphy-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:50:23.676066 calphy-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_liquid_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_solid_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-13 09:50:20.000000 calphy-1.2.8/tests/test_solid_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:44:56.658512 calphy-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-06-02 06:44:51.000000 calphy-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 06:44:51.000000 calphy-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-02 06:44:56.658512 calphy-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-02 06:44:51.000000 calphy-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:44:56.654512 calphy-1.2.9/calphy/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/composition_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27125 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/liquid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41096 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/queuekernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61627 2023-06-02 06:44:51.000000 calphy-1.2.9/calphy/splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:44:56.654512 calphy-1.2.9/calphy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 06:44:56.000000 calphy-1.2.9/calphy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:44:56.658512 calphy-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-02 06:44:56.000000 calphy-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:44:56.658512 calphy-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_liquid_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_solid_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-02 06:44:51.000000 calphy-1.2.9/tests/test_solid_methods.py
```

### Comparing `calphy-1.2.8/LICENSE` & `calphy-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/PKG-INFO` & `calphy-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calphy
-Version: 1.2.8
+Version: 1.2.9
 Summary: free energy calculation for python
 Home-page: https://github.com/ICAMS/calphy
 Author: Sarath Menon, Yury Lysogorskiy, Ralf Drautz
 Author-email: sarathmenon@mailbox.org
 License: GNU General Public License v3
 Keywords: calphy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calphy-1.2.8/README.md` & `calphy-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/alchemy.py` & `calphy-1.2.9/calphy/alchemy.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/composition_transformation.py` & `calphy-1.2.9/calphy/composition_transformation.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/errors.py` & `calphy-1.2.9/calphy/errors.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/helpers.py` & `calphy-1.2.9/calphy/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,29 +113,29 @@
             lmp.command(
                 "read_dump        %s 0 x y z scaled no box yes add keep" % calc.lattice
             )
             lmp.command("change_box       all triclinic")
         else:
             lmp.command("read_data      %s" % calc.lattice)
     else:
-        lmp.lattice(l, alat)
-        lmp.region("box block", 0, calc.repeat[0], 0, calc.repeat[1], 0, calc.repeat[2])
-        lmp.create_box("1 box")
-        lmp.create_atoms("1 box")
+        lmp.command(f'lattice {l} {alat}')
+        lmp.command(f'region box block 0 {calc.repeat[0]} 0 {calc.repeat[1]} 0 {calc.repeat[2]}')
+        lmp.command(f'create_box 1 box')
+        lmp.command(f'create_atoms 1 box')
     return lmp
 
 
 def set_mass(lmp, options, ghost_elements=0):
     count = 1
     for i in range(options.n_elements):
-        lmp.mass(i + 1, options.mass[i])
+        lmp.command(f'mass {i+1} {options.mass[i]}')
         count += 1
 
     for i in range(ghost_elements):
-        lmp.mass(count + i, 1.00)
+        lmp.command(f'mass {count+i} 1.00')
 
     return lmp
 
 
 def set_potential(lmp, options, ghost_elements=0):
     """
     Set the interatomic potential
@@ -347,21 +347,21 @@
 
 
 def write_data(lmp, file):
     lmp.command(f"write_data {file}")
     return lmp
 
 
-def reset_timestep(conf, file="current.data"):
+def reset_timestep(conf, file="current.data", init_commands=None):
     lmp = create_object(
         cores=1,
         directory=os.path.dirname(file),
         timestep=0,
         cmdargs=None,
-        init_commands=None,
+        init_commands=init_commands,
     )
     lmp = read_data(lmp, file)
     lmp = write_data(lmp, conf)
     return lmp
 
     # with open(file, "r") as f:
     #    with open(conf, "w") as c:
```

### Comparing `calphy-1.2.8/calphy/input.py` & `calphy-1.2.9/calphy/input.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/integrators.py` & `calphy-1.2.9/calphy/integrators.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/kernel.py` & `calphy-1.2.9/calphy/kernel.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/lattice.py` & `calphy-1.2.9/calphy/lattice.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/liquid.py` & `calphy-1.2.9/calphy/liquid.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/phase.py` & `calphy-1.2.9/calphy/phase.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/queuekernel.py` & `calphy-1.2.9/calphy/queuekernel.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/routines.py` & `calphy-1.2.9/calphy/routines.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/scheduler.py` & `calphy-1.2.9/calphy/scheduler.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/solid.py` & `calphy-1.2.9/calphy/solid.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy/splines.py` & `calphy-1.2.9/calphy/splines.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/calphy.egg-info/PKG-INFO` & `calphy-1.2.9/calphy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calphy
-Version: 1.2.8
+Version: 1.2.9
 Summary: free energy calculation for python
 Home-page: https://github.com/ICAMS/calphy
 Author: Sarath Menon, Yury Lysogorskiy, Ralf Drautz
 Author-email: sarathmenon@mailbox.org
 License: GNU General Public License v3
 Keywords: calphy
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `calphy-1.2.8/calphy.egg-info/SOURCES.txt` & `calphy-1.2.9/calphy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/setup.py` & `calphy-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='calphy',
     name='calphy',
     packages=find_packages(include=['calphy', 'calphy.*']),
     test_suite='tests',
     url='https://github.com/ICAMS/calphy',
-    version='1.2.8',
+    version='1.2.9',
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'calphy = calphy.kernel:main',
             'calphy_kernel = calphy.queuekernel:main',
         ],
     }
```

### Comparing `calphy-1.2.8/tests/test_composition.py` & `calphy-1.2.9/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/tests/test_helpers.py` & `calphy-1.2.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/tests/test_liquid_avg.py` & `calphy-1.2.9/tests/test_liquid_avg.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/tests/test_solid_avg.py` & `calphy-1.2.9/tests/test_solid_avg.py`

 * *Files identical despite different names*

### Comparing `calphy-1.2.8/tests/test_solid_methods.py` & `calphy-1.2.9/tests/test_solid_methods.py`

 * *Files identical despite different names*

