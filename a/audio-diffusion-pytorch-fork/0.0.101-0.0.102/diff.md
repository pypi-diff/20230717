# Comparing `tmp/audio-diffusion-pytorch-fork-0.0.101.tar.gz` & `tmp/audio-diffusion-pytorch-fork-0.0.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-diffusion-pytorch-fork-0.0.101.tar", last modified: Thu Jul 13 19:41:43 2023, max compression
+gzip compressed data, was "audio-diffusion-pytorch-fork-0.0.102.tar", last modified: Mon Jul 17 20:11:48 2023, max compression
```

## Comparing `audio-diffusion-pytorch-fork-0.0.101.tar` & `audio-diffusion-pytorch-fork-0.0.102.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1068 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12252 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      832 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    22680 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15989 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/model.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    46830 2023-07-09 21:47:45.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/modules.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3609 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      499 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      115 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       29 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:38:47.000000 audio-diffusion-pytorch-fork-0.0.101/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-13 19:41:43.000000 audio-diffusion-pytorch-fork-0.0.101/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      976 2023-07-13 19:32:20.000000 audio-diffusion-pytorch-fork-0.0.101/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1068 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12252 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      832 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    22680 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15989 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/model.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    47071 2023-07-15 04:53:26.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/modules.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3609 2023-06-18 22:14:54.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      626 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      499 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      115 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       29 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:38:47.000000 audio-diffusion-pytorch-fork-0.0.102/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-17 20:11:48.000000 audio-diffusion-pytorch-fork-0.0.102/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      976 2023-07-17 20:04:30.000000 audio-diffusion-pytorch-fork-0.0.102/setup.py
```

### Comparing `audio-diffusion-pytorch-fork-0.0.101/LICENSE` & `audio-diffusion-pytorch-fork-0.0.102/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/PKG-INFO` & `audio-diffusion-pytorch-fork-0.0.102/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-diffusion-pytorch-fork
-Version: 0.0.101
+Version: 0.0.102
 Summary: A fork of Flavio Schneider's Audio Diffusion - PyTorch
 Home-page: https://github.com/harmonai-org/audio-diffusion-pytorch-fork
 Author: Harmonai
 License: MIT
 Keywords: artificial intelligence,deep learning,audio generation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `audio-diffusion-pytorch-fork-0.0.101/README.md` & `audio-diffusion-pytorch-fork-0.0.102/README.md`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/__init__.py` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/__init__.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/diffusion.py` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/diffusion.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/model.py` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/model.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/modules.py` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1172,16 +1172,22 @@
             if batch_cfg:
                 batch_x = torch.cat([x, x], dim=0)
                 batch_time = torch.cat([time, time], dim=0)
                 batch_embed = torch.cat([embedding, fixed_embedding], dim=0)
                 batch_mask = None
                 if embedding_mask is not None:
                     batch_mask = torch.cat([embedding_mask, embedding_mask], dim=0)
+
+                batch_features = None
+                if self.use_context_features:
+                    features = kwargs.pop("features")
+                    batch_features = torch.cat([features, features], dim=0)
+
                 # Compute both normal and fixed embedding outputs
-                batch_out = super().forward(batch_x, batch_time, embedding=batch_embed, embedding_mask=batch_mask, **kwargs)
+                batch_out = super().forward(batch_x, batch_time, embedding=batch_embed, embedding_mask=batch_mask, features=batch_features, **kwargs)
                 out, out_masked = batch_out.chunk(2, dim=0)
            
             else:
                 # Compute both normal and fixed embedding outputs
                 out = super().forward(x, time, embedding=embedding, embedding_mask=embedding_mask, **kwargs)
                 out_masked = super().forward(x, time, embedding=fixed_embedding, embedding_mask=embedding_mask, **kwargs)
```

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork/utils.py` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork/utils.py`

 * *Files identical despite different names*

### Comparing `audio-diffusion-pytorch-fork-0.0.101/audio_diffusion_pytorch_fork.egg-info/PKG-INFO` & `audio-diffusion-pytorch-fork-0.0.102/audio_diffusion_pytorch_fork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-diffusion-pytorch-fork
-Version: 0.0.101
+Version: 0.0.102
 Summary: A fork of Flavio Schneider's Audio Diffusion - PyTorch
 Home-page: https://github.com/harmonai-org/audio-diffusion-pytorch-fork
 Author: Harmonai
 License: MIT
 Keywords: artificial intelligence,deep learning,audio generation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `audio-diffusion-pytorch-fork-0.0.101/setup.py` & `audio-diffusion-pytorch-fork-0.0.102/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="audio-diffusion-pytorch-fork",
     packages=find_packages(exclude=[]),
-    version="0.0.101",
+    version="0.0.102",
     license="MIT",
     description="A fork of Flavio Schneider's Audio Diffusion - PyTorch",
     long_description_content_type="text/markdown",
     author="Harmonai",
     url="https://github.com/harmonai-org/audio-diffusion-pytorch-fork",
     keywords=["artificial intelligence", "deep learning", "audio generation"],
     install_requires=[
```

