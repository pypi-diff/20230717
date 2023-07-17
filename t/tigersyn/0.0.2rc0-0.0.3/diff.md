# Comparing `tmp/tigersyn-0.0.2rc0.tar.gz` & `tmp/tigersyn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigersyn-0.0.2rc0.tar", last modified: Mon Jul 17 09:53:53 2023, max compression
+gzip compressed data, was "tigersyn-0.0.3.tar", last modified: Mon Jul 17 10:08:45 2023, max compression
```

## Comparing `tigersyn-0.0.2rc0.tar` & `tigersyn-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.261006 tigersyn-0.0.2rc0/
--rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.2rc0/LICENSE
--rw-rw-rw-   0        0        0      758 2023-07-17 09:53:53.260011 tigersyn-0.0.2rc0/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.2rc0/README.md
--rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.2rc0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 09:53:53.261006 tigersyn-0.0.2rc0/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-07-17 09:53:44.000000 tigersyn-0.0.2rc0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.235012 tigersyn-0.0.2rc0/tigersyn/
--rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.2rc0/tigersyn/__init__.py
--rw-rw-rw-   0        0        0     2252 2023-07-17 09:43:55.000000 tigersyn-0.0.2rc0/tigersyn/syn.py
--rw-rw-rw-   0        0        0     3948 2023-07-17 09:52:58.000000 tigersyn-0.0.2rc0/tigersyn/syn_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:53:53.258015 tigersyn-0.0.2rc0/tigersyn.egg-info/
--rw-rw-rw-   0        0        0      758 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 09:53:53.000000 tigersyn-0.0.2rc0/tigersyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.290538 tigersyn-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-07-17 10:08:45.288513 tigersyn-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.3/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:08:45.290538 tigersyn-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-17 10:08:04.000000 tigersyn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.229515 tigersyn-0.0.3/tigersyn/
+-rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.3/tigersyn/__init__.py
+-rw-rw-rw-   0        0        0     2199 2023-07-17 10:07:35.000000 tigersyn-0.0.3/tigersyn/syn.py
+-rw-rw-rw-   0        0        0     3948 2023-07-17 09:52:58.000000 tigersyn-0.0.3/tigersyn/syn_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.287556 tigersyn-0.0.3/tigersyn.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/top_level.txt
```

### Comparing `tigersyn-0.0.2rc0/LICENSE` & `tigersyn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.2rc0/PKG-INFO` & `tigersyn-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.2rc0
+Version: 0.0.3
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tigersyn-0.0.2rc0/setup.py` & `tigersyn-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VESION = '0.0.2c'
+VESION = '0.0.3'
 DESCRIPTION = 'Processing MRI images based on deep-learning'
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: MIT License',
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `tigersyn-0.0.2rc0/tigersyn/syn.py` & `tigersyn-0.0.3/tigersyn/syn.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from tigersyn import syn_tool
 
 model_syn = r"mprage_syntheseg_v001_unet.onnx"
 
 def produce_mask(model, f, GPU):
     model_ff = syn_tool.get_model(model)
-    print(model_ff)
     input_nib = nib.load(f)
     input_nib_resp = syn_tool.read_file(model_ff, f)
 
     mask_nib_resp = syn_tool.run(
         model_ff, input_nib_resp,  GPU=GPU)
     
     mask_nib = resample_to_img(mask_nib_resp, input_nib, interpolation="nearest")
@@ -74,8 +73,8 @@
         if syn:
             aseg_nib = produce_mask(model_syn, f, GPU=gpu)
             fn = syn_tool.save_nib(aseg_nib, ftemplate, 'syn')
 
         print('Processing time: %d seconds' %  (time.time() - t))
 
 if __name__ == "__main__":
-    run("sz", r"T1w.nii.gz", r"outputs")
+    pass
```

### Comparing `tigersyn-0.0.2rc0/tigersyn/syn_tool.py` & `tigersyn-0.0.3/tigersyn/syn_tool.py`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.2rc0/tigersyn.egg-info/PKG-INFO` & `tigersyn-0.0.3/tigersyn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.2rc0
+Version: 0.0.3
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

