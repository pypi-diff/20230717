# Comparing `tmp/DiadFit-0.0.66.tar.gz` & `tmp/DiadFit-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.66.tar", last modified: Fri Jul 14 19:55:15 2023, max compression
+gzip compressed data, was "DiadFit-0.0.68.tar", last modified: Mon Jul 17 16:28:19 2023, max compression
```

## Comparing `DiadFit-0.0.66.tar` & `DiadFit-0.0.68.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:55:15.177533 DiadFit-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-14 19:55:15.177533 DiadFit-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 19:54:56.000000 DiadFit-0.0.66/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:55:15.177533 DiadFit-0.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-14 19:55:01.000000 DiadFit-0.0.66/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:55:15.173533 DiadFit-0.0.66/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:55:15.177533 DiadFit-0.0.66/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/CO2_in_bubble_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/Highrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/Lowrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/Mediumrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/argon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/densimeter_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   165479 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35351 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    65096 2023-07-14 19:55:01.000000 DiadFit-0.0.66/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:55:15.177533 DiadFit-0.0.66/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-14 19:55:14.000000 DiadFit-0.0.66/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 19:55:15.000000 DiadFit-0.0.66/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:55:14.000000 DiadFit-0.0.66/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 19:55:14.000000 DiadFit-0.0.66/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 19:55:14.000000 DiadFit-0.0.66/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.338345 DiadFit-0.0.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 16:28:19.338345 DiadFit-0.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 16:28:00.000000 DiadFit-0.0.68/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:28:19.338345 DiadFit-0.0.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-17 16:28:05.000000 DiadFit-0.0.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.330345 DiadFit-0.0.68/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.334345 DiadFit-0.0.68/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/CO2_in_bubble_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Highrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Lowrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Mediumrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/densimeter_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165479 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35351 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65096 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.334345 DiadFit-0.0.68/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.66/PKG-INFO` & `DiadFit-0.0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.66
+Version: 0.0.68
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.66/README.md` & `DiadFit-0.0.68/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/setup.py` & `DiadFit-0.0.68/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.68/src/DiadFit/CO2_EOS.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/CO2_in_bubble_error.py` & `DiadFit-0.0.68/src/DiadFit/CO2_in_bubble_error.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.68/src/DiadFit/H2O_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/Highrho_polyfit_data.pkl` & `DiadFit-0.0.68/src/DiadFit/Highrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/Lowrho_polyfit_data.pkl` & `DiadFit-0.0.68/src/DiadFit/Lowrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/Mediumrho_polyfit_data.pkl` & `DiadFit-0.0.68/src/DiadFit/Mediumrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/Psensor.py` & `DiadFit-0.0.68/src/DiadFit/Psensor.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/__init__.py` & `DiadFit-0.0.68/src/DiadFit/__init__.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/argon_lines.py` & `DiadFit-0.0.68/src/DiadFit/argon_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.68/src/DiadFit/cosmicray_filter.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/densimeter_fitting.py` & `DiadFit-0.0.68/src/DiadFit/densimeter_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/densimeters.py` & `DiadFit-0.0.68/src/DiadFit/densimeters.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,15 +623,15 @@
 
     # Create the settings dictionary
     settings = {
         'meta_path': meta_path,
         'spectra_path': spectra_path,
         'filetype': filetype,
         'prefix': prefix,
-        'prefix_str': prefix_str,
+        'prefix_str': repr(prefix_str),
         'file_ext': file_ext,
         'TruPower': TruPower,
     }
 
     # Construct the settings file path
     settings_file_path = os.path.join(folder, 'settings.txt')
 
@@ -651,14 +651,17 @@
     settings = {}
     with open(settings_file_path, 'r') as file:
         for line in file:
             line = line.strip()
             if line:
                 key, value = line.split('=')
                 settings[key] = value
+                if key == 'prefix_str':
+                    value = eval(value)  # Evaluate the string to retrieve the original value
+                settings[key] = value
 
     if 'prefix' in settings:
         settings['prefix'] = settings['prefix'].lower() == 'true'
 
     if 'TruPower' in settings:
         settings['TruPower'] = settings['TruPower'].lower() == 'true'
```

### Comparing `DiadFit-0.0.66/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.68/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/diads.py` & `DiadFit-0.0.68/src/DiadFit/diads.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/error_propagation.py` & `DiadFit-0.0.68/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.68/src/DiadFit/importing_data_files.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit/ne_lines.py` & `DiadFit-0.0.68/src/DiadFit/ne_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.66/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.68/src/DiadFit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.66
+Version: 0.0.68
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.66/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.68/src/DiadFit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

