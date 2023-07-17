# Comparing `tmp/tigersyn-0.0.2.tar.gz` & `tmp/tigersyn-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigersyn-0.0.2.tar", last modified: Mon Jul 17 08:27:29 2023, max compression
+gzip compressed data, was "tigersyn-0.0.2a0.tar", last modified: Mon Jul 17 09:04:31 2023, max compression
```

## Comparing `tigersyn-0.0.2.tar` & `tigersyn-0.0.2a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:27:29.025694 tigersyn-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      794 2023-07-17 08:27:29.024690 tigersyn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.2/README.md
--rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 08:27:29.026692 tigersyn-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-17 08:27:20.000000 tigersyn-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:27:29.010694 tigersyn-0.0.2/tigersyn/
--rw-rw-rw-   0        0        0       28 2023-07-17 08:16:50.000000 tigersyn-0.0.2/tigersyn/__init__.py
--rw-rw-rw-   0        0        0     2204 2023-07-17 08:16:29.000000 tigersyn-0.0.2/tigersyn/syn.py
--rw-rw-rw-   0        0        0     2268 2023-07-17 08:16:38.000000 tigersyn-0.0.2/tigersyn/syn_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-17 08:27:29.023691 tigersyn-0.0.2/tigersyn.egg-info/
--rw-rw-rw-   0        0        0      794 2023-07-17 08:27:28.000000 tigersyn-0.0.2/tigersyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-17 08:27:28.000000 tigersyn-0.0.2/tigersyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:27:28.000000 tigersyn-0.0.2/tigersyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 08:27:28.000000 tigersyn-0.0.2/tigersyn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 08:27:28.000000 tigersyn-0.0.2/tigersyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:04:31.348048 tigersyn-0.0.2a0/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.2a0/LICENSE
+-rw-rw-rw-   0        0        0      757 2023-07-17 09:04:31.346051 tigersyn-0.0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.2a0/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:04:31.348048 tigersyn-0.0.2a0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-07-17 09:01:27.000000 tigersyn-0.0.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:04:31.305046 tigersyn-0.0.2a0/tigersyn/
+-rw-rw-rw-   0        0        0       28 2023-07-17 08:16:50.000000 tigersyn-0.0.2a0/tigersyn/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-07-17 09:02:11.000000 tigersyn-0.0.2a0/tigersyn/syn.py
+-rw-rw-rw-   0        0        0     4006 2023-07-17 08:49:05.000000 tigersyn-0.0.2a0/tigersyn/syn_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:04:31.344177 tigersyn-0.0.2a0/tigersyn.egg-info/
+-rw-rw-rw-   0        0        0      757 2023-07-17 09:04:31.000000 tigersyn-0.0.2a0/tigersyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-17 09:04:31.000000 tigersyn-0.0.2a0/tigersyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:04:31.000000 tigersyn-0.0.2a0/tigersyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-17 09:04:31.000000 tigersyn-0.0.2a0/tigersyn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 09:04:31.000000 tigersyn-0.0.2a0/tigersyn.egg-info/top_level.txt
```

### Comparing `tigersyn-0.0.2/LICENSE` & `tigersyn-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.2/setup.py` & `tigersyn-0.0.2a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VESION = '0.0.2'
+VESION = '0.0.2a'
 DESCRIPTION = 'Processing MRI images based on deep-learning'
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: MIT License',
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `tigersyn-0.0.2/tigersyn/syn.py` & `tigersyn-0.0.2a0/tigersyn/syn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 import nibabel as nib
 from nilearn.image import resample_to_img
 import numpy as np
 
 from tigersyn import syn_tool
 
-model_ff = r"models\mprage_syntheseg_v001_unet.onnx"
+model_syn = r"mprage_syntheseg_v001_unet.onnx"
 
-def produce_mask(f, GPU):
+def produce_mask(model, f, GPU):
+    model_ff = syn_tool.get_model(model)
     input_nib = nib.load(f)
     input_nib_resp = syn_tool.read_file(model_ff, f)
 
     mask_nib_resp = syn_tool.run(
         model_ff, input_nib_resp,  GPU=GPU)
     
     mask_nib = resample_to_img(mask_nib_resp, input_nib, interpolation="nearest")
@@ -66,14 +67,14 @@
 
         ftemplate = basename(f).replace('.nii', f'_@@@@.nii')
         if get_z and '.gz' not in ftemplate:
             ftemplate += '.gz'
         ftemplate = join(f_output_dir, ftemplate)
         
         if syn:
-            aseg_nib = produce_mask(f, GPU=gpu)
+            aseg_nib = produce_mask(model_syn, f, GPU=gpu)
             fn = syn_tool.save_nib(aseg_nib, ftemplate, 'syn')
 
         print('Processing time: %d seconds' %  (time.time() - t))
 
 if __name__ == "__main__":
     run("sz", r"D:\synthseg_pc\dataset\cc359\Original", r"outputs")
```

