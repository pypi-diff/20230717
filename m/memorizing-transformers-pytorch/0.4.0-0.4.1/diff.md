# Comparing `tmp/memorizing-transformers-pytorch-0.4.0.tar.gz` & `tmp/memorizing-transformers-pytorch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorizing-transformers-pytorch-0.4.0.tar", last modified: Fri Mar 24 18:28:26 2023, max compression
+gzip compressed data, was "memorizing-transformers-pytorch-0.4.1.tar", last modified: Mon Jul 17 00:09:43 2023, max compression
```

## Comparing `memorizing-transformers-pytorch-0.4.0.tar` & `memorizing-transformers-pytorch-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:26.021009 memorizing-transformers-pytorch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-24 18:28:26.021009 memorizing-transformers-pytorch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:26.017009 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/knn_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/memorizing_transformers_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:26.021009 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-24 18:28:26.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-24 18:28:26.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:28:26.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-24 18:28:26.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 18:28:26.000000 memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 18:28:26.021009 memorizing-transformers-pytorch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-24 18:28:05.000000 memorizing-transformers-pytorch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:09:43.363104 memorizing-transformers-pytorch-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 00:09:43.363104 memorizing-transformers-pytorch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:09:43.363104 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/knn_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/memorizing_transformers_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:09:43.363104 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 00:09:43.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-17 00:09:43.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:09:43.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 00:09:43.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 00:09:43.000000 memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 00:09:43.363104 memorizing-transformers-pytorch-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-17 00:09:31.000000 memorizing-transformers-pytorch-0.4.1/setup.py
```

### Comparing `memorizing-transformers-pytorch-0.4.0/LICENSE` & `memorizing-transformers-pytorch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memorizing-transformers-pytorch-0.4.0/PKG-INFO` & `memorizing-transformers-pytorch-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memorizing-transformers-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Memorizing Transformer - Pytorch
 Home-page: https://github.com/lucidrains/memorizing-transformers-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,memory,retrieval
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memorizing-transformers-pytorch-0.4.0/README.md` & `memorizing-transformers-pytorch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/knn_memory.py` & `memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/knn_memory.py`

 * *Files identical despite different names*

### Comparing `memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch/memorizing_transformers_pytorch.py` & `memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch/memorizing_transformers_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,14 @@
 
 def cast_tuple(val, length = 1):
     return val if isinstance(val, tuple) else ((val,) * length)
 
 def l2norm(t):
     return F.normalize(t, dim = -1)
 
-def stable_softmax(t, dim = -1):
-    t = t - t.amax(dim = dim, keepdim = True).detach()
-    return F.softmax(t, dim = dim)
-
 # helper classes
 
 class PreNormResidual(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
         self.norm = nn.LayerNorm(dim)
@@ -153,15 +149,15 @@
 
         if exists(rel_pos_bias):
             sim = rel_pos_bias[..., -i:, -j:] + sim
 
         causal_mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
         sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
-        attn = stable_softmax(sim)
+        attn = sim.softmax(dim = -1)
         attn = self.dropout(attn)
 
         out = einsum('b h i j, b j d -> b h i d', attn, v)
         out = rearrange(out, 'b h n d -> b n (h d)')
 
         # new xl memories
 
@@ -269,15 +265,15 @@
 
         if add_knn_memory and new_kv_memories_discarded.numel() > 0:
             knn_memory.add(new_kv_memories_discarded)
 
         # attention (combining local and distant)
 
         sim = torch.cat((sim_mem, sim), dim = -1)
-        attn = stable_softmax(sim)
+        attn = sim.softmax(dim = -1)
         attn = self.dropout(attn)
 
         local_attn, mem_attn = attn[..., self.num_retrieved_memories:], attn[..., :self.num_retrieved_memories]
         local_out = einsum('b h i j, b j d -> b h i d', local_attn, v)
         mem_out = einsum('b h i j, b h i j d -> b h i d', mem_attn, mem_v)
 
         out = local_out + mem_out
```

### Comparing `memorizing-transformers-pytorch-0.4.0/memorizing_transformers_pytorch.egg-info/PKG-INFO` & `memorizing-transformers-pytorch-0.4.1/memorizing_transformers_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memorizing-transformers-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Memorizing Transformer - Pytorch
 Home-page: https://github.com/lucidrains/memorizing-transformers-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,memory,retrieval
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memorizing-transformers-pytorch-0.4.0/setup.py` & `memorizing-transformers-pytorch-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memorizing-transformers-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'Memorizing Transformer - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memorizing-transformers-pytorch',
   keywords = [
```

