# Comparing `tmp/frechet_audio_distance-0.1.0.tar.gz` & `tmp/frechet_audio_distance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frechet_audio_distance-0.1.0.tar", last modified: Sat Apr 22 03:53:38 2023, max compression
+gzip compressed data, was "frechet_audio_distance-0.1.1.tar", last modified: Mon Jul 17 03:45:17 2023, max compression
```

## Comparing `frechet_audio_distance-0.1.0.tar` & `frechet_audio_distance-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.157359 frechet_audio_distance-0.1.0/
--rw-r--r--   0 haohao_tan   (501) staff       (20)     1087 2022-12-11 06:36:10.000000 frechet_audio_distance-0.1.0/LICENSE
--rw-r--r--   0 haohao_tan   (501) staff       (20)     3756 2023-04-22 03:53:38.157114 frechet_audio_distance-0.1.0/PKG-INFO
--rw-r--r--   0 haohao_tan   (501) staff       (20)     2085 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/README.md
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.153614 frechet_audio_distance-0.1.0/frechet_audio_distance/
--rw-r--r--   0 haohao_tan   (501) staff       (20)       18 2023-04-16 14:03:24.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/__init__.py
--rw-r--r--   0 haohao_tan   (501) staff       (20)     8809 2023-04-22 03:47:22.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/fad.py
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.156474 frechet_audio_distance-0.1.0/frechet_audio_distance/models/
--rw-r--r--   0 haohao_tan   (501) staff       (20)        0 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/__init__.py
--rw-r--r--   0 haohao_tan   (501) staff       (20)   121695 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/pann.py
--rw-r--r--   0 haohao_tan   (501) staff       (20)     8452 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/pytorch_utils.py
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.155511 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/
--rw-r--r--   0 haohao_tan   (501) staff       (20)     3756 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/PKG-INFO
--rw-r--r--   0 haohao_tan   (501) staff       (20)      475 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/SOURCES.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)        1 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/dependency_links.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)       41 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/requires.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)       23 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/top_level.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)      722 2023-04-22 03:52:13.000000 frechet_audio_distance-0.1.0/pyproject.toml
--rw-r--r--   0 haohao_tan   (501) staff       (20)       38 2023-04-22 03:53:38.157438 frechet_audio_distance-0.1.0/setup.cfg
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.156772 frechet_audio_distance-0.1.0/test/
--rw-r--r--   0 haohao_tan   (501) staff       (20)     2352 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/test/test_examples.py
+drwxr-xr-x   0 haohao     (502) staff       (20)        0 2023-07-17 03:45:17.857668 frechet_audio_distance-0.1.1/
+-rw-r--r--   0 haohao     (502) staff       (20)     1087 2023-07-17 03:27:21.000000 frechet_audio_distance-0.1.1/LICENSE
+-rw-r--r--   0 haohao     (502) staff       (20)     4005 2023-07-17 03:45:17.857538 frechet_audio_distance-0.1.1/PKG-INFO
+-rw-r--r--   0 haohao     (502) staff       (20)     2341 2023-07-17 03:33:25.000000 frechet_audio_distance-0.1.1/README.md
+drwxr-xr-x   0 haohao     (502) staff       (20)        0 2023-07-17 03:45:17.855714 frechet_audio_distance-0.1.1/frechet_audio_distance/
+-rw-r--r--   0 haohao     (502) staff       (20)       18 2023-07-17 02:54:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance/__init__.py
+-rw-r--r--   0 haohao     (502) staff       (20)     9263 2023-07-17 03:44:47.000000 frechet_audio_distance-0.1.1/frechet_audio_distance/fad.py
+drwxr-xr-x   0 haohao     (502) staff       (20)        0 2023-07-17 03:45:17.857232 frechet_audio_distance-0.1.1/frechet_audio_distance/models/
+-rw-r--r--   0 haohao     (502) staff       (20)        0 2023-07-17 02:54:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance/models/__init__.py
+-rw-r--r--   0 haohao     (502) staff       (20)   121695 2023-07-17 02:54:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance/models/pann.py
+-rw-r--r--   0 haohao     (502) staff       (20)     8452 2023-07-17 02:54:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance/models/pytorch_utils.py
+drwxr-xr-x   0 haohao     (502) staff       (20)        0 2023-07-17 03:45:17.856294 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/
+-rw-r--r--   0 haohao     (502) staff       (20)     4005 2023-07-17 03:45:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/PKG-INFO
+-rw-r--r--   0 haohao     (502) staff       (20)      475 2023-07-17 03:45:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/SOURCES.txt
+-rw-r--r--   0 haohao     (502) staff       (20)        1 2023-07-17 03:45:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/dependency_links.txt
+-rw-r--r--   0 haohao     (502) staff       (20)       54 2023-07-17 03:45:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/requires.txt
+-rw-r--r--   0 haohao     (502) staff       (20)       23 2023-07-17 03:45:17.000000 frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/top_level.txt
+-rw-r--r--   0 haohao     (502) staff       (20)      740 2023-07-17 03:25:44.000000 frechet_audio_distance-0.1.1/pyproject.toml
+-rw-r--r--   0 haohao     (502) staff       (20)       38 2023-07-17 03:45:17.857704 frechet_audio_distance-0.1.1/setup.cfg
+drwxr-xr-x   0 haohao     (502) staff       (20)        0 2023-07-17 03:45:17.857387 frechet_audio_distance-0.1.1/test/
+-rw-r--r--   0 haohao     (502) staff       (20)     2352 2023-07-17 03:44:38.000000 frechet_audio_distance-0.1.1/test/test_examples.py
```

### Comparing `frechet_audio_distance-0.1.0/LICENSE` & `frechet_audio_distance-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Hao Hao Tan
+Copyright (c) 2023 Hao Hao Tan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `frechet_audio_distance-0.1.0/PKG-INFO` & `frechet_audio_distance-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: frechet_audio_distance
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight library of Frechet Audio Distance calculation.
 Author-email: Hao Hao Tan <helloharry66@gmail.com>
 License: MIT License
         
-        Copyright (c) 2022 Hao Hao Tan
+        Copyright (c) 2023 Hao Hao Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -47,25 +47,27 @@
 ### Demo
 
 ```python
 from frechet_audio_distance import FrechetAudioDistance
 
 # to use `vggish`
 frechet = FrechetAudioDistance(
-    model_name="vggish"
+    model_name="vggish",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 # to use `PANN`
 frechet = FrechetAudioDistance(
-    model_name="pann"
+    model_name="pann",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 fad_score = frechet.score("/path/to/background/set", "/path/to/eval/set")
 
 ```
 
 ### Result validation
 
@@ -80,14 +82,19 @@
 
 **Test 2: Distorted sine waves on PANN**
 
 |                              |   baseline vs test1   |     baseline vs test2    |
 |:----------------------------:|:---------------------:|:------------------------:|
 |    `frechet_audio_distance`  |        0.000465       |          0.00008594      |
 
+### To contribute
+
+- Run `python3 -m build` to build your version locally. The built wheel should be in `dist/`.
+- `pip install` your local wheel version, and run `pytest test/` to validate your changes.
+
 ### References
 
 VGGish in PyTorch: https://github.com/harritaylor/torchvggish
 
 Frechet distance implementation: https://github.com/mseitzer/pytorch-fid
 
 Frechet Audio Distance paper: https://arxiv.org/abs/1812.08466
```

### Comparing `frechet_audio_distance-0.1.0/README.md` & `frechet_audio_distance-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 ### Demo
 
 ```python
 from frechet_audio_distance import FrechetAudioDistance
 
 # to use `vggish`
 frechet = FrechetAudioDistance(
-    model_name="vggish"
+    model_name="vggish",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 # to use `PANN`
 frechet = FrechetAudioDistance(
-    model_name="pann"
+    model_name="pann",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 fad_score = frechet.score("/path/to/background/set", "/path/to/eval/set")
 
 ```
 
 ### Result validation
 
@@ -46,14 +48,19 @@
 
 **Test 2: Distorted sine waves on PANN**
 
 |                              |   baseline vs test1   |     baseline vs test2    |
 |:----------------------------:|:---------------------:|:------------------------:|
 |    `frechet_audio_distance`  |        0.000465       |          0.00008594      |
 
+### To contribute
+
+- Run `python3 -m build` to build your version locally. The built wheel should be in `dist/`.
+- `pip install` your local wheel version, and run `pytest test/` to validate your changes.
+
 ### References
 
 VGGish in PyTorch: https://github.com/harritaylor/torchvggish
 
 Frechet distance implementation: https://github.com/mseitzer/pytorch-fid
 
 Frechet Audio Distance paper: https://arxiv.org/abs/1812.08466
```

### Comparing `frechet_audio_distance-0.1.0/frechet_audio_distance/fad.py` & `frechet_audio_distance-0.1.1/frechet_audio_distance/fad.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,44 @@
 from multiprocessing.dummy import Pool as ThreadPool
 from .models.pann import Cnn14_16k
 
 
 SAMPLE_RATE = 16000
 
 
-def load_audio_task(fname):
-    wav_data, sr = sf.read(fname, dtype='int16')
-    assert wav_data.dtype == np.int16, 'Bad sample type: %r' % wav_data.dtype
-    wav_data = wav_data / 32768.0  # Convert to [-1.0, +1.0]
-
+def load_audio_task(fname, dtype="float32"):
+    if dtype not in ['float64', 'float32', 'int32', 'int16']:
+        raise ValueError(f"dtype not supported: {dtype}")
+
+    wav_data, sr = sf.read(fname, dtype=dtype)
+    # For integer type PCM input, convert to [-1.0, +1.0]
+    if dtype == 'int16':
+        wav_data = wav_data / 32768.0
+    elif dtype == 'int32':
+        wav_data = wav_data / float(2**31)
+    
     # Convert to mono
     if len(wav_data.shape) > 1:
         wav_data = np.mean(wav_data, axis=1)
 
     if sr != SAMPLE_RATE:
         wav_data = resampy.resample(wav_data, sr, SAMPLE_RATE)
 
     return wav_data
 
 
 class FrechetAudioDistance:
-    def __init__(self, model_name="vggish", use_pca=False, use_activation=False, verbose=False, audio_load_worker=8):
+    def __init__(
+        self, 
+        model_name="vggish", 
+        use_pca=False, 
+        use_activation=False, 
+        verbose=False, 
+        audio_load_worker=8
+    ):
         self.model_name = model_name
         self.device = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
         self.__get_model(model_name=model_name, use_pca=use_pca, use_activation=use_activation)
         self.verbose = verbose
         self.audio_load_worker = audio_load_worker
     
     def __get_model(self, model_name="vggish", use_pca=False, use_activation=False):
@@ -153,37 +166,47 @@
             covmean = covmean.real
 
         tr_covmean = np.trace(covmean)
 
         return (diff.dot(diff) + np.trace(sigma1)
                 + np.trace(sigma2) - 2 * tr_covmean)
     
-    def __load_audio_files(self, dir):
+    def __load_audio_files(self, dir, dtype="float32"):
         task_results = []
 
         pool = ThreadPool(self.audio_load_worker)
         pbar = tqdm(total=len(os.listdir(dir)), disable=(not self.verbose))
 
         def update(*a):
             pbar.update()
 
         if self.verbose:
             print("[Frechet Audio Distance] Loading audio from {}...".format(dir))
         for fname in os.listdir(dir):
-            res = pool.apply_async(load_audio_task, args=(os.path.join(dir, fname),), callback=update)
+            res = pool.apply_async(
+                load_audio_task, 
+                args=(os.path.join(dir, fname), dtype,), 
+                callback=update
+            )
             task_results.append(res)
         pool.close()
         pool.join()     
 
         return [k.get() for k in task_results] 
 
-    def score(self, background_dir, eval_dir, store_embds=False):
+    def score(
+        self, 
+        background_dir, 
+        eval_dir, 
+        store_embds=False,
+        dtype="float32"
+    ):
         try:
-            audio_background = self.__load_audio_files(background_dir)
-            audio_eval = self.__load_audio_files(eval_dir)
+            audio_background = self.__load_audio_files(background_dir, dtype=dtype)
+            audio_eval = self.__load_audio_files(eval_dir, dtype=dtype)
 
             embds_background = self.get_embeddings(audio_background)
             embds_eval = self.get_embeddings(audio_eval)
 
             if store_embds:
                 np.save("embds_background.npy", embds_background)
                 np.save("embds_eval.npy", embds_eval)
```

### Comparing `frechet_audio_distance-0.1.0/frechet_audio_distance/models/pann.py` & `frechet_audio_distance-0.1.1/frechet_audio_distance/models/pann.py`

 * *Files identical despite different names*

### Comparing `frechet_audio_distance-0.1.0/frechet_audio_distance/models/pytorch_utils.py` & `frechet_audio_distance-0.1.1/frechet_audio_distance/models/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/PKG-INFO` & `frechet_audio_distance-0.1.1/frechet_audio_distance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: frechet-audio-distance
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight library of Frechet Audio Distance calculation.
 Author-email: Hao Hao Tan <helloharry66@gmail.com>
 License: MIT License
         
-        Copyright (c) 2022 Hao Hao Tan
+        Copyright (c) 2023 Hao Hao Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -47,25 +47,27 @@
 ### Demo
 
 ```python
 from frechet_audio_distance import FrechetAudioDistance
 
 # to use `vggish`
 frechet = FrechetAudioDistance(
-    model_name="vggish"
+    model_name="vggish",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 # to use `PANN`
 frechet = FrechetAudioDistance(
-    model_name="pann"
+    model_name="pann",
     use_pca=False, 
     use_activation=False,
-    verbose=False
+    verbose=False,
+    dtype="float32"
 )
 fad_score = frechet.score("/path/to/background/set", "/path/to/eval/set")
 
 ```
 
 ### Result validation
 
@@ -80,14 +82,19 @@
 
 **Test 2: Distorted sine waves on PANN**
 
 |                              |   baseline vs test1   |     baseline vs test2    |
 |:----------------------------:|:---------------------:|:------------------------:|
 |    `frechet_audio_distance`  |        0.000465       |          0.00008594      |
 
+### To contribute
+
+- Run `python3 -m build` to build your version locally. The built wheel should be in `dist/`.
+- `pip install` your local wheel version, and run `pytest test/` to validate your changes.
+
 ### References
 
 VGGish in PyTorch: https://github.com/harritaylor/torchvggish
 
 Frechet distance implementation: https://github.com/mseitzer/pytorch-fid
 
 Frechet Audio Distance paper: https://arxiv.org/abs/1812.08466
```

### Comparing `frechet_audio_distance-0.1.0/pyproject.toml` & `frechet_audio_distance-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frechet_audio_distance"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Hao Hao Tan", email="helloharry66@gmail.com" },
 ]
 description = "A lightweight library of Frechet Audio Distance calculation."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -20,11 +20,12 @@
 dependencies = [
   'numpy',
   'torch',
   'scipy',
   'tqdm',
   'soundfile',
   'resampy',
+  'torchlibrosa'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gudgud96/frechet-audio-distance"
```

### Comparing `frechet_audio_distance-0.1.0/test/test_examples.py` & `frechet_audio_distance-0.1.1/test/test_examples.py`

 * *Files identical despite different names*

