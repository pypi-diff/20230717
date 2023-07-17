# Comparing `tmp/resomapper-0.3.0.tar.gz` & `tmp/resomapper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resomapper-0.3.0.tar", max compression
+gzip compressed data, was "resomapper-0.4.0.tar", max compression
```

## Comparing `resomapper-0.3.0.tar` & `resomapper-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.3.0/LICENSE
--rw-r--r--   0        0        0      867 2023-07-07 08:48:52.387143 resomapper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.3.0/README.md
--rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.3.0/resomapper/__init__.py
--rw-r--r--   0        0        0     5560 2023-06-02 08:21:40.005388 resomapper-0.3.0/resomapper/cli.py
--rw-r--r--   0        0        0        0 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/dwi/__init__.py
--rw-r--r--   0        0        0    12887 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/dwi/adcm.py
--rw-r--r--   0        0        0    25353 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/file_system_functions.py
--rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.3.0/resomapper/myrelax/__init__.py
--rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.3.0/resomapper/myrelax/getT1TR.py
--rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.3.0/resomapper/myrelax/getT2T2star.py
--rw-r--r--   0        0        0     7534 2023-06-02 08:21:40.021012 resomapper-0.3.0/resomapper/preprocessing.py
--rw-r--r--   0        0        0    63576 2023-06-30 10:25:59.663437 resomapper-0.3.0/resomapper/processing.py
--rw-r--r--   0        0        0    19972 2023-06-02 08:21:40.052261 resomapper-0.3.0/resomapper/utils.py
--rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 resomapper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.4.0/LICENSE
+-rw-r--r--   0        0        0      867 2023-07-17 09:05:03.625714 resomapper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.4.0/README.md
+-rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.4.0/resomapper/__init__.py
+-rw-r--r--   0        0        0     5320 2023-07-17 08:58:48.114122 resomapper-0.4.0/resomapper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:25:59.647813 resomapper-0.4.0/resomapper/dwi/__init__.py
+-rw-r--r--   0        0        0    12887 2023-06-30 10:25:59.647813 resomapper-0.4.0/resomapper/dwi/adcm.py
+-rw-r--r--   0        0        0    25360 2023-07-17 08:58:48.119120 resomapper-0.4.0/resomapper/file_system_functions.py
+-rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.4.0/resomapper/myrelax/__init__.py
+-rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.4.0/resomapper/myrelax/getT1TR.py
+-rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.4.0/resomapper/myrelax/getT2T2star.py
+-rw-r--r--   0        0        0    21730 2023-07-17 08:58:48.123116 resomapper-0.4.0/resomapper/preprocessing.py
+-rw-r--r--   0        0        0    63590 2023-07-17 08:58:48.127114 resomapper-0.4.0/resomapper/processing.py
+-rw-r--r--   0        0        0    19972 2023-06-02 08:21:40.052261 resomapper-0.4.0/resomapper/utils.py
+-rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 resomapper-0.4.0/PKG-INFO
```

### Comparing `resomapper-0.3.0/LICENSE` & `resomapper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/pyproject.toml` & `resomapper-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resomapper"
-version = "0.3.0"
+version = "0.4.0"
 description = "Pipeline for processing MR images and generating parametric maps."
 authors = ["Biomedical-MR"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "resomapper" }
```

### Comparing `resomapper-0.3.0/README.md` & `resomapper-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/resomapper/cli.py` & `resomapper-0.4.0/resomapper/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import traceback
 import warnings
 
 from colorama import just_fix_windows_console
 
 import resomapper.file_system_functions as fs
-from resomapper.preprocessing import Preprocessing
+from resomapper.preprocessing import Denoising
 from resomapper.processing import (
     DTIProcessor,
     MTProcessor,
     TimeCollector,
     TMapProcessor,
 )
 from resomapper.utils import Headermsg as hmg
@@ -85,56 +85,55 @@
             print(
                 f'\n\n\n\n{hmg.new_patient1}{"_".join(patient_name)} {hmg.new_patient2}'
             )
         prev_patient_name = patient_name[:]
         current_modal = study_name.split("_")[0]
         print(f"\n\n{hmg.new_modal}Procesamiento del mapa de {current_modal}")
 
+        if ask_user(
+            "¿Deseas preprocesar este estudio con un filtro de reducción de ruido?"
+        ):
+            Denoising(study).denoise()
+
         # Mask specification and creation
         masker = Mask(study)
         mode = masker.select_mask_mode()
         mask_path = masker.create_mask(mode)
 
         if study_name.startswith("DT"):
             dti_map_pro = DTIProcessor(root_path, study)
             ok_mask = dti_map_pro.check_DTI_data()
             while not ok_mask:
                 mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = dti_map_pro.check_DTI_data()
 
-            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
-                Preprocessing([study]).preprocess()
             dti_map_pro.process_DTI()
 
         elif study_name.startswith("MT"):
             mt_map_pro = MTProcessor(study, mask_path)
             ok_mask = mt_map_pro.check_MT_data()
             while not ok_mask:
                 mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = mt_map_pro.check_MT_data()
 
-            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
-                Preprocessing([study]).preprocess()
             mt_map_pro.process_MT()
 
         else:
             n_cpu = multiprocessing.cpu_count() - 1
             t_map_pro = TMapProcessor(
                 study, mask_path, n_cpu=n_cpu, fitting_mode="nonlinear"
             )
             ok_mask = t_map_pro.check_T_data()
             while not ok_mask:
                 mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = t_map_pro.check_T_data()
 
-            if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
-                Preprocessing([study]).preprocess()
             t_map_pro.process_T_map(f_time_paths)
 
     print(f"\n{hmg.success}Procesamiento terminado.")
 
 
 def run_cli():
     """Runs the CLI of resomapper, catching keyboard interruption to exit the program
```

### Comparing `resomapper-0.3.0/resomapper/dwi/adcm.py` & `resomapper-0.4.0/resomapper/dwi/adcm.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/resomapper/file_system_functions.py` & `resomapper-0.4.0/resomapper/file_system_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         print(
             f"\n{hmg.ask}Marca qué modalidades deseas procesar en la ventana emergente."
         )
 
         # init tkinter
         root = tk.Tk()
-        root.title("MyX")
+        root.title("resomapper")
 
         row = 1
         selected_modals = []
         modalities = ["T1", "T2", "T2E", "DTI", "MT"]
 
         # add label
         tk.Label(root, text="Selecciona las modalidades que desees procesar.").grid(
```

### Comparing `resomapper-0.3.0/resomapper/myrelax/getT1TR.py` & `resomapper-0.4.0/resomapper/myrelax/getT1TR.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/resomapper/myrelax/getT2T2star.py` & `resomapper-0.4.0/resomapper/myrelax/getT2T2star.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/resomapper/processing.py` & `resomapper-0.4.0/resomapper/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1384,15 +1384,15 @@
                 print(
                     f"\n{hmg.ask}Indica cómo quieres guardar los mapas en la "
                     "ventana emergente."
                 )
 
                 # create a frame
                 root = tk.Tk()
-                root.title("MyX")
+                root.title("resomapper")
 
                 # declaring string variable for storing values
                 color_min = tk.IntVar()
                 color_max = tk.IntVar()
                 colormap = tk.StringVar()
 
                 tk.Label(root, text="Mínimo", font=("calibre", 10, "bold")).grid(
@@ -1539,15 +1539,15 @@
 
         print(
             f"\n{hmg.ask}Indica cómo quieres guardar los mapas en la ventana emergente."
         )
 
         # create a frame
         root = tk.Tk()
-        root.title("MyX")
+        root.title("resomapper")
 
         # declaring string variable for storing values
         color_min = tk.IntVar()
         color_max = tk.IntVar()
         colormap = tk.StringVar()
 
         tk.Label(root, text="Mínimo", font=("calibre", 10, "bold")).grid(
```

### Comparing `resomapper-0.3.0/resomapper/utils.py` & `resomapper-0.4.0/resomapper/utils.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.3.0/PKG-INFO` & `resomapper-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resomapper
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pipeline for processing MR images and generating parametric maps.
 License: MIT
 Author: Biomedical-MR
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

