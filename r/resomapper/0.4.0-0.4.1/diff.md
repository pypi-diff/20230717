# Comparing `tmp/resomapper-0.4.0.tar.gz` & `tmp/resomapper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resomapper-0.4.0.tar", max compression
+gzip compressed data, was "resomapper-0.4.1.tar", max compression
```

## Comparing `resomapper-0.4.0.tar` & `resomapper-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.4.0/LICENSE
--rw-r--r--   0        0        0      867 2023-07-17 09:05:03.625714 resomapper-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.4.0/README.md
--rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.4.0/resomapper/__init__.py
--rw-r--r--   0        0        0     5320 2023-07-17 08:58:48.114122 resomapper-0.4.0/resomapper/cli.py
--rw-r--r--   0        0        0        0 2023-06-30 10:25:59.647813 resomapper-0.4.0/resomapper/dwi/__init__.py
--rw-r--r--   0        0        0    12887 2023-06-30 10:25:59.647813 resomapper-0.4.0/resomapper/dwi/adcm.py
--rw-r--r--   0        0        0    25360 2023-07-17 08:58:48.119120 resomapper-0.4.0/resomapper/file_system_functions.py
--rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.4.0/resomapper/myrelax/__init__.py
--rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.4.0/resomapper/myrelax/getT1TR.py
--rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.4.0/resomapper/myrelax/getT2T2star.py
--rw-r--r--   0        0        0    21730 2023-07-17 08:58:48.123116 resomapper-0.4.0/resomapper/preprocessing.py
--rw-r--r--   0        0        0    63590 2023-07-17 08:58:48.127114 resomapper-0.4.0/resomapper/processing.py
--rw-r--r--   0        0        0    19972 2023-06-02 08:21:40.052261 resomapper-0.4.0/resomapper/utils.py
--rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 resomapper-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.4.1/LICENSE
+-rw-r--r--   0        0        0      887 2023-07-17 11:35:21.759514 resomapper-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.4.1/README.md
+-rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.4.1/resomapper/__init__.py
+-rw-r--r--   0        0        0     5320 2023-07-17 08:58:48.114122 resomapper-0.4.1/resomapper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:25:59.647813 resomapper-0.4.1/resomapper/dwi/__init__.py
+-rw-r--r--   0        0        0    12887 2023-06-30 10:25:59.647813 resomapper-0.4.1/resomapper/dwi/adcm.py
+-rw-r--r--   0        0        0    25360 2023-07-17 08:58:48.119120 resomapper-0.4.1/resomapper/file_system_functions.py
+-rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.4.1/resomapper/myrelax/__init__.py
+-rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.4.1/resomapper/myrelax/getT1TR.py
+-rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.4.1/resomapper/myrelax/getT2T2star.py
+-rw-r--r--   0        0        0    23759 2023-07-17 11:33:40.550196 resomapper-0.4.1/resomapper/preprocessing.py
+-rw-r--r--   0        0        0    63590 2023-07-17 08:58:48.127114 resomapper-0.4.1/resomapper/processing.py
+-rw-r--r--   0        0        0    19972 2023-06-02 08:21:40.052261 resomapper-0.4.1/resomapper/utils.py
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 resomapper-0.4.1/PKG-INFO
```

### Comparing `resomapper-0.4.0/LICENSE` & `resomapper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/pyproject.toml` & `resomapper-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resomapper"
-version = "0.4.0"
+version = "0.4.1"
 description = "Pipeline for processing MR images and generating parametric maps."
 authors = ["Biomedical-MR"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "resomapper" }
@@ -15,17 +15,18 @@
 click = "^8.1.3"
 bruker2nifti = "1.0.4"
 colorama = "^0.4.6"
 dipy = "1.5.0"
 matplotlib = "^3.5.3"
 nibabel = "^4.0.2"
 pandas = "^1.4.4"
+numexpr = "^2.7.3"
 Pillow = "^9.2.0"
 seaborn = "^0.12.0"
-numpy = ">=1.23.3, <1.25.0"
+numpy = ">=1.23.3, <1.24.0"
 opencv-python = "^4.6.0.66"
 scikit-image = "^0.19.3"
 scikit-learn = "^1.1.2"
 scipy = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `resomapper-0.4.0/README.md` & `resomapper-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/cli.py` & `resomapper-0.4.1/resomapper/cli.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/dwi/adcm.py` & `resomapper-0.4.1/resomapper/dwi/adcm.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/file_system_functions.py` & `resomapper-0.4.1/resomapper/file_system_functions.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/myrelax/getT1TR.py` & `resomapper-0.4.1/resomapper/myrelax/getT1TR.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/myrelax/getT2T2star.py` & `resomapper-0.4.1/resomapper/myrelax/getT2T2star.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/preprocessing.py` & `resomapper-0.4.1/resomapper/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tkinter as tk
 import warnings
 from math import trunc
+import matplotlib
 
 import matplotlib.pyplot as plt
 import nibabel as nib
 import numpy as np
 
 # from scipy.ndimage import rotate
 from dipy.core.gradients import gradient_table
@@ -19,14 +20,15 @@
 from skimage.restoration import denoise_nl_means
 from skimage.transform import rotate
 
 from resomapper.utils import Headermsg as hmg
 from resomapper.utils import ask_user, ask_user_options
 
 warnings.filterwarnings("ignore")
+matplotlib.use("TkAgg")
 
 
 ######################################### OLD ##########################################
 def get_preprocessing_params():
     """Show a window to select the parameters to perform non local means denoising.
 
     Returns:
@@ -98,31 +100,34 @@
 ################################### ^^ OLD ^^ ##########################################
 
 
 def ask_user_parameters(parameter_dict):
     root = tk.Tk()
     root.title("resomapper")
 
+    values = {}
+
     def submit():
-        global values
-        values = {}
+        nonlocal values
+        # global values
+        # values = {}
         for parameter, info in parameter_dict.items():
             value = entry_boxes[parameter].get()
             predetermined_value = info[0]
             value_type = type(predetermined_value)
             try:
                 value = value_type(value)
                 if value_type == str and not value:
                     raise ValueError
                 values[parameter] = value
             except (ValueError, TypeError):
                 error_label.config(text=f"Invalid input for {parameter}!")
                 return
         root.destroy()
-
+        root.quit()
         # return values  # Return parameter selection
 
     entry_boxes = {}
     for parameter, info in parameter_dict.items():
         label_text = f"[{parameter}] {info[1]}"
         label = tk.Label(root, text=label_text)
         label.pack(padx=50, pady=(10, 0))
@@ -198,19 +203,21 @@
                     )
                 elif selected_filter == "m":
                     denoised_image, params = self.mp_pca_denoising(
                         original_image, params
                     )
 
                 if i == 0:
-                    self.show_denoised_output(original_image, denoised_image)
-                    process_again = ask_user(
-                        "¿Deseas cambiar los parámetros de filtrado?"
+                    process_again = self.show_denoised_output(
+                        original_image, denoised_image
                     )
-                    plt.close()
+                    # process_again = ask_user(
+                    #     "¿Deseas cambiar los parámetros de filtrado?"
+                    # )
+                    # plt.close()
 
                 if not process_again:
                     self.save_nii(study_nii, denoised_image)
 
     def select_denoising_filter(self):
         question = "Elige el filtro que deseas aplicar."
         options = {
@@ -266,27 +273,34 @@
         ax.flat[0].set_title("Original")
         ax.flat[1].imshow(den.T, cmap="gray", interpolation="none")
         ax.flat[1].set_title("Denoised Output")
         ax.flat[2].imshow(rms_diff.T, cmap="gray", interpolation="none")
         ax.flat[2].set_title("Residuals")
         fig1.show()
 
+        process_again = ask_user("¿Deseas cambiar los parámetros de filtrado?")
+        plt.close(fig1)
+        return process_again
+
     ############################### Denoising methods ##################################
 
     def non_local_means_denoising(self, image, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
-
         parameters_nlm = {
             "patch_size": [3, "Size of patches used for denoising."],
             "patch_distance": [7, "Maximal search distance (pixels)."],
             "h": [4.5, "Cut-off distance (in gray levels)."],
         }
 
-        selection = ask_user_parameters(parameters_nlm) if params is None else params
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_nlm)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_nlm) if params is None else params
 
         p_imas = []  # processed images
         p_serie = []
 
         if len(image.shape) == 4:
             for serie in np.moveaxis(image, -1, 0):
                 for ima in np.moveaxis(serie, -1, 0):
@@ -315,50 +329,63 @@
                 )
                 p_imas.append(d_ima)
             r_imas = np.moveaxis(np.array(p_imas), 0, -1)
 
         return r_imas, selection
 
     def non_local_means_2_denoising(self, image, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro non-local means (version 2).\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+        # print(f"\n{hmg.info}Has seleccionado el filtro non-local means (version 2).\n")
+        # print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
 
         parameters_nlm_2 = {
             "N_sigma": [0, ""],
             "patch_radius": [1, ""],
             "block_radius": [2, ""],
             "rician": [True, ""],
         }
-        selection = ask_user_parameters(parameters_nlm_2) if params is None else params
+
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_nlm_2)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_nlm_2) if params is None else params
 
         sigma = estimate_sigma(image, N=selection["N_sigma"])
         return (
             nlmeans(
                 image,
                 sigma=sigma,
                 # mask=mask,
                 patch_radius=selection["patch_radius"],
                 block_radius=selection["block_radius"],
                 rician=selection["rician"],
             ),
-            params,
+            selection,
         )
 
     def ascm_denoising(self, image, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro ASCM.\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+        # print(f"\n{hmg.info}Has seleccionado el filtro ASCM.\n")
+        # print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
 
         parameters_ascm = {
             "N_sigma": [0, ""],
             "patch_radius_small": [1, ""],
             "patch_radius_large": [2, ""],
             "block_radius": [2, ""],
             "rician": [True, ""],
         }
-        selection = ask_user_parameters(parameters_ascm) if params is None else params
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_ascm)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_ascm) if params is None else params
 
         sigma = estimate_sigma(image, N=selection["N_sigma"])
 
         den_small = nlmeans(
             image,
             sigma=sigma,
             # mask=mask,
@@ -373,89 +400,107 @@
             # mask=mask,
             patch_radius=selection["patch_radius_large"],
             block_radius=selection["block_radius"],
             rician=selection["rician"],
         )
 
         if len(image.shape) == 3:
-            return adaptive_soft_matching(image, den_small, den_large, sigma), params
+            return adaptive_soft_matching(image, den_small, den_large, sigma), selection
 
         denoised_image = []
         for i in range(image.shape[-1]):
             denoised_vol = adaptive_soft_matching(
                 image[:, :, :, i],
                 den_small[:, :, :, i],
                 den_large[:, :, :, i],
                 sigma[i],
             )
             denoised_image.append(denoised_vol)
 
         denoised_image = np.moveaxis(np.array(denoised_image), 0, -1)
-        return denoised_image, params
+        return denoised_image, selection
 
     def local_pca_denoising(self, image, gtab, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro local PCA.\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+        # print(f"\n{hmg.info}Has seleccionado el filtro local PCA.\n")
+        # print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
 
         parameters_lpca = {
             "correct_bias": [True, ""],
             "smooth": [3, ""],
             "tau_factor": [2.3, ""],
             "patch_radius": [2, ""],
         }
-        selection = ask_user_parameters(parameters_lpca) if params is None else params
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_lpca)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_lpca) if params is None else params
 
         sigma = pca_noise_estimate(
             image,
             gtab,
             correct_bias=selection["correct_bias"],
             smooth=selection["smooth"],
         )
         return (
             localpca(
                 image,
                 sigma,
                 tau_factor=selection["tau_factor"],
                 patch_radius=selection["patch_radius"],
             ),
-            params,
+            selection,
         )
 
     def mp_pca_denoising(self, image, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro Marcenko-Pasteur PCA.\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+        # print(f"\n{hmg.info}Has seleccionado el filtro Marcenko-Pasteur PCA.\n")
+        # print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
 
         parameters_mp_pca = {
             "patch_radius": [2, ""],
         }
-        selection = ask_user_parameters(parameters_mp_pca) if params is None else params
-        return mppca(image, patch_radius=selection["patch_radius"]), params
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_mp_pca)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_mp_pca) if params is None else params
+        return mppca(image, patch_radius=selection["patch_radius"]), selection
 
     def patch2self_denoising(self, image, bvals, params):
-        print(f"\n{hmg.info}Has seleccionado el filtro patch2self.\n")
-        print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+        # print(f"\n{hmg.info}Has seleccionado el filtro patch2self.\n")
+        # print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
 
         parameters_p2s = {
             "model": ["ols", ""],
             "shift_intensity": [True, ""],
             "clip_negative_vals": [False, ""],
             "b0_threshold": [50, ""],
         }
-        selection = ask_user_parameters(parameters_p2s) if params is None else params
+        if params is None:
+            print(f"\n{hmg.info}Has seleccionado el filtro non-local means.\n")
+            print(f"{hmg.ask}Selecciona los parámetros en la ventana emergente.")
+            selection = ask_user_parameters(parameters_p2s)
+        else:
+            selection = params
+        # selection = ask_user_parameters(parameters_p2s) if params is None else params
 
         return (
             patch2self(
                 image,
                 bvals,
                 model=selection["model"],
                 shift_intensity=selection["shift_intensity"],
                 clip_negative_vals=selection["clip_negative_vals"],
                 b0_threshold=selection["b0_threshold"],
             ),
-            params,
+            selection,
         )
 
 
 ######################################### OLD ##########################################
 class Preprocessing:
     def __init__(self, studies_paths):
         self.studies_paths = studies_paths
```

### Comparing `resomapper-0.4.0/resomapper/processing.py` & `resomapper-0.4.1/resomapper/processing.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/resomapper/utils.py` & `resomapper-0.4.1/resomapper/utils.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.4.0/PKG-INFO` & `resomapper-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resomapper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pipeline for processing MR images and generating parametric maps.
 License: MIT
 Author: Biomedical-MR
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,16 @@
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: bruker2nifti (==1.0.4)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dipy (==1.5.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: nibabel (>=4.0.2,<5.0.0)
-Requires-Dist: numpy (>=1.23.3,<1.25.0)
+Requires-Dist: numexpr (>=2.7.3,<3.0.0)
+Requires-Dist: numpy (>=1.23.3,<1.24.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
```

