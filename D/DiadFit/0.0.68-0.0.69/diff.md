# Comparing `tmp/DiadFit-0.0.68.tar.gz` & `tmp/DiadFit-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.68.tar", last modified: Mon Jul 17 16:28:19 2023, max compression
+gzip compressed data, was "DiadFit-0.0.69.tar", last modified: Mon Jul 17 20:54:33 2023, max compression
```

## Comparing `DiadFit-0.0.68.tar` & `DiadFit-0.0.69.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.338345 DiadFit-0.0.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 16:28:19.338345 DiadFit-0.0.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 16:28:00.000000 DiadFit-0.0.68/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:28:19.338345 DiadFit-0.0.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-17 16:28:05.000000 DiadFit-0.0.68/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.330345 DiadFit-0.0.68/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.334345 DiadFit-0.0.68/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/CO2_in_bubble_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Highrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Lowrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Mediumrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/argon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/densimeter_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   165479 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35351 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    65096 2023-07-17 16:28:05.000000 DiadFit-0.0.68/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:28:19.334345 DiadFit-0.0.68/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 16:28:19.000000 DiadFit-0.0.68/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:33.294978 DiadFit-0.0.69/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 20:54:33.294978 DiadFit-0.0.69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 20:54:11.000000 DiadFit-0.0.69/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:54:33.298978 DiadFit-0.0.69/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-17 20:54:17.000000 DiadFit-0.0.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:33.294978 DiadFit-0.0.69/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:33.294978 DiadFit-0.0.69/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/CO2_in_bubble_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/Highrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/Lowrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/Mediumrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/densimeter_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165479 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37148 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65097 2023-07-17 20:54:17.000000 DiadFit-0.0.69/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:33.294978 DiadFit-0.0.69/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 20:54:33.000000 DiadFit-0.0.69/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-17 20:54:33.000000 DiadFit-0.0.69/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:54:33.000000 DiadFit-0.0.69/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 20:54:33.000000 DiadFit-0.0.69/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:54:33.000000 DiadFit-0.0.69/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.68/PKG-INFO` & `DiadFit-0.0.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.68
+Version: 0.0.69
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.68/README.md` & `DiadFit-0.0.69/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/setup.py` & `DiadFit-0.0.69/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.69/src/DiadFit/CO2_EOS.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/CO2_in_bubble_error.py` & `DiadFit-0.0.69/src/DiadFit/CO2_in_bubble_error.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.69/src/DiadFit/H2O_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/Highrho_polyfit_data.pkl` & `DiadFit-0.0.69/src/DiadFit/Highrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/Lowrho_polyfit_data.pkl` & `DiadFit-0.0.69/src/DiadFit/Lowrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/Mediumrho_polyfit_data.pkl` & `DiadFit-0.0.69/src/DiadFit/Mediumrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/Psensor.py` & `DiadFit-0.0.69/src/DiadFit/Psensor.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/__init__.py` & `DiadFit-0.0.69/src/DiadFit/__init__.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/argon_lines.py` & `DiadFit-0.0.69/src/DiadFit/argon_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.69/src/DiadFit/cosmicray_filter.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/densimeter_fitting.py` & `DiadFit-0.0.69/src/DiadFit/densimeter_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/densimeters.py` & `DiadFit-0.0.69/src/DiadFit/densimeters.py`

 * *Files 3% similar despite different names*

```diff
@@ -581,92 +581,44 @@
                         +df_combo_sec_phase['Diad2_Voigt_Area']))
 
 
 
     return df_combo_sec_phase
 
 ## Merge peak fits together
-def merge_fit_files():
+def merge_fit_files(path):
     """
     This function merges the files Discarded_df.xlsx, Weak_Diads.xlsx, Medium_Diads.xlsx, Strong_Diads.xlsx
     if they exist into one combined dataframe
     """
-    import os.path
-    from os import path
-    if path.exists('Discarded_df.xlsx'):
-        discard=pd.read_excel('Discarded_df.xlsx')
+    import os
+    import pandas as pd
+
+    if os.path.exists(os.path.join(path, 'Discarded_df.xlsx')):
+        discard = pd.read_excel(os.path.join(path, 'Discarded_df.xlsx'))
     else:
-        discard=None
-    if path.exists('Weak_Diads.xlsx'):
-        grp1=pd.read_excel('Weak_Diads.xlsx')
+        discard = None
+
+    if os.path.exists(os.path.join(path, 'Weak_Diads.xlsx')):
+        grp1 = pd.read_excel(os.path.join(path, 'Weak_Diads.xlsx'))
     else:
-        grp1=None
-    if path.exists('Medium_Diads.xlsx'):
-        grp2=pd.read_excel('Medium_Diads.xlsx')
+        grp1 = None
+
+    if os.path.exists(os.path.join(path, 'Medium_Diads.xlsx')):
+        grp2 = pd.read_excel(os.path.join(path, 'Medium_Diads.xlsx'))
     else:
-        grp2=None
-    if path.exists('Strong_Diads.xlsx'):
-        grp3=pd.read_excel('Strong_Diads.xlsx')
+        grp2 = None
+
+    if os.path.exists(os.path.join(path, 'Strong_Diads.xlsx')):
+        grp3 = pd.read_excel(os.path.join(path, 'Strong_Diads.xlsx'))
     else:
-        grp3=None
-    df2=pd.concat([grp1, grp2, grp3], axis=0).reset_index(drop=True)
+        grp3 = None
+
+    df2 = pd.concat([grp1, grp2, grp3], axis=0).reset_index(drop=True)
+
     if discard is not None:
         discard_cols=discard[discard.columns.intersection(df2.columns)]
         df2=pd.concat([df2, discard_cols]).reset_index(drop=True)
     return df2
 
 
 
-## Save settings files
-def save_settings(meta_path, spectra_path, filetype, prefix, prefix_str, file_ext, TruPower):
-    # Get the current folder
-    folder = os.getcwd()
-
-    # Create the settings dictionary
-    settings = {
-        'meta_path': meta_path,
-        'spectra_path': spectra_path,
-        'filetype': filetype,
-        'prefix': prefix,
-        'prefix_str': repr(prefix_str),
-        'file_ext': file_ext,
-        'TruPower': TruPower,
-    }
-
-    # Construct the settings file path
-    settings_file_path = os.path.join(folder, 'settings.txt')
-
-    # Write the settings to the file
-    with open(settings_file_path, 'w') as file:
-        for key, value in settings.items():
-            file.write(f"{key}={value}\n")
-
-def get_settings():
-    # Get the current folder
-    folder = os.getcwd()
-
-    # Construct the settings file path
-    settings_file_path = os.path.join(folder, 'settings.txt')
-
-    # Read the settings from the file
-    settings = {}
-    with open(settings_file_path, 'r') as file:
-        for line in file:
-            line = line.strip()
-            if line:
-                key, value = line.split('=')
-                settings[key] = value
-                if key == 'prefix_str':
-                    value = eval(value)  # Evaluate the string to retrieve the original value
-                settings[key] = value
-
-    if 'prefix' in settings:
-        settings['prefix'] = settings['prefix'].lower() == 'true'
-
-    if 'TruPower' in settings:
-        settings['TruPower'] = settings['TruPower'].lower() == 'true'
-
-    # Return the settings
-    return settings.get('meta_path'), settings.get('spectra_path'), settings.get('filetype'), \
-           settings.get('prefix'), settings.get('prefix_str'), settings.get('file_ext'), settings.get('TruPower')
-
-
```

### Comparing `DiadFit-0.0.68/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.69/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/diads.py` & `DiadFit-0.0.69/src/DiadFit/diads.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/error_propagation.py` & `DiadFit-0.0.69/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.68/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.69/src/DiadFit/importing_data_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1171,7 +1171,64 @@
                 #df_Dense_loop.loc[df_Dense_loop['filename']==file, 'filename']= file + str(' ind_fit')
 
         df_Dense_Combo=df_Dense_loop.copy()
     else:
         df_Dense_Combo=df_Dense
 
     return df_Dense_Combo
+    
+    
+## Save settings files
+def save_settings(meta_path, spectra_path, filetype, prefix, prefix_str, file_ext, TruPower):
+    # Get the current folder
+    folder = os.getcwd()
+
+    # Create the settings dictionary
+    settings = {
+        'meta_path': meta_path,
+        'spectra_path': spectra_path,
+        'filetype': filetype,
+        'prefix': prefix,
+        'prefix_str': repr(prefix_str),
+        'file_ext': file_ext,
+        'TruPower': TruPower,
+    }
+
+    # Construct the settings file path
+    settings_file_path = os.path.join(folder, 'settings.txt')
+
+    # Write the settings to the file
+    with open(settings_file_path, 'w') as file:
+        for key, value in settings.items():
+            file.write(f"{key}={value}\n")
+
+def get_settings():
+    # Get the current folder
+    folder = os.getcwd()
+
+    # Construct the settings file path
+    settings_file_path = os.path.join(folder, 'settings.txt')
+
+    # Read the settings from the file
+    settings = {}
+    with open(settings_file_path, 'r') as file:
+        for line in file:
+            line = line.strip()
+            if line:
+                key, value = line.split('=')
+                settings[key] = value
+                if key == 'prefix_str':
+                    value = eval(value)  # Evaluate the string to retrieve the original value
+                settings[key] = value
+
+    if 'prefix' in settings:
+        settings['prefix'] = settings['prefix'].lower() == 'true'
+
+    if 'TruPower' in settings:
+        settings['TruPower'] = settings['TruPower'].lower() == 'true'
+
+    # Return the settings
+    return settings.get('meta_path'), settings.get('spectra_path'), settings.get('filetype'), \
+           settings.get('prefix'), settings.get('prefix_str'), settings.get('file_ext'), settings.get('TruPower')
+
+
+
```

### Comparing `DiadFit-0.0.68/src/DiadFit/ne_lines.py` & `DiadFit-0.0.69/src/DiadFit/ne_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
 
     # Flatten x and y if needed
     xdat=x.flatten()
     ydat=y_corr.flatten()
     
     df=pd.DataFrame(data={'Xdata': xdat,
     'Ydata': ydat})
-    df.to_clipboard(excel=True)
+    #df.to_clipboard(excel=True)
 
     # This defines the range you want to fit (e.g. how big the tails are)
     lower_pk1=Ne_center+x_span[0]
     upper_pk1=Ne_center+x_span[1]
 
     # This segments into the x and y variable, and variables to plot, which are a bit bigger.
     Ne_pk1_reg_x=x[(x>lower_pk1)&(x<upper_pk1)]
```

### Comparing `DiadFit-0.0.68/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.69/src/DiadFit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.68
+Version: 0.0.69
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.68/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.69/src/DiadFit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

