# Comparing `tmp/slicetca-0.1.8.tar.gz` & `tmp/slicetca-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicetca-0.1.8.tar", last modified: Tue Mar  7 11:26:38 2023, max compression
+gzip compressed data, was "slicetca-0.1.9.tar", last modified: Mon Jul 17 02:31:32 2023, max compression
```

## Comparing `slicetca-0.1.8.tar` & `slicetca-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.261112 slicetca-0.1.8/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-0.1.8/LICENSE.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2244 2023-03-07 11:26:38.261112 slicetca-0.1.8/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1724 2023-03-07 11:26:30.000000 slicetca-0.1.8/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2023-03-07 11:26:38.261112 slicetca-0.1.8/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      944 2023-03-07 11:24:31.000000 slicetca-0.1.8/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.257112 slicetca-0.1.8/slicetca/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      214 2023-03-07 11:24:31.000000 slicetca-0.1.8/slicetca/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.257112 slicetca-0.1.8/slicetca/core/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-0.1.8/slicetca/core/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    12323 2023-03-04 17:26:28.000000 slicetca-0.1.8/slicetca/core/decompositions.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.257112 slicetca-0.1.8/slicetca/invariance/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-0.1.8/slicetca/invariance/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-0.1.8/slicetca/invariance/analytic_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-0.1.8/slicetca/invariance/criteria.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-0.1.8/slicetca/invariance/helper.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1172 2023-03-06 12:14:41.000000 slicetca-0.1.8/slicetca/invariance/invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-0.1.8/slicetca/invariance/iterative_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-0.1.8/slicetca/invariance/transformations.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.257112 slicetca-0.1.8/slicetca/plotting/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       45 2023-03-04 21:19:31.000000 slicetca-0.1.8/slicetca/plotting/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-0.1.8/slicetca/plotting/additional.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-0.1.8/slicetca/plotting/factors.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.261112 slicetca-0.1.8/slicetca/run/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-0.1.8/slicetca/run/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3036 2023-03-07 10:54:02.000000 slicetca-0.1.8/slicetca/run/decompose.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4533 2023-03-06 12:14:41.000000 slicetca-0.1.8/slicetca/run/grid_search.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-0.1.8/slicetca/run/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.261112 slicetca-0.1.8/slicetca/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-0.1.8/slicetca/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-0.1.8/slicetca/tests/tests.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-03-07 11:26:38.257112 slicetca-0.1.8/slicetca.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2244 2023-03-07 11:26:38.000000 slicetca-0.1.8/slicetca.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      775 2023-03-07 11:26:38.000000 slicetca-0.1.8/slicetca.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-03-07 11:26:38.000000 slicetca-0.1.8/slicetca.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       28 2023-03-07 11:26:38.000000 slicetca-0.1.8/slicetca.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2023-03-07 11:26:38.000000 slicetca-0.1.8/slicetca.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-0.1.9/LICENSE.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2312 2023-07-17 02:31:32.277612 slicetca-0.1.9/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1792 2023-03-07 11:52:39.000000 slicetca-0.1.9/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2023-07-17 02:31:32.277612 slicetca-0.1.9/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      944 2023-07-17 02:31:27.000000 slicetca-0.1.9/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      214 2023-03-07 11:24:31.000000 slicetca-0.1.9/slicetca/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/core/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-0.1.9/slicetca/core/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    12757 2023-07-12 00:19:14.000000 slicetca-0.1.9/slicetca/core/decompositions.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/invariance/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-0.1.9/slicetca/invariance/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-0.1.9/slicetca/invariance/analytic_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-0.1.9/slicetca/invariance/criteria.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/invariance/helper.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1272 2023-07-13 15:26:21.000000 slicetca-0.1.9/slicetca/invariance/invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/invariance/iterative_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-0.1.9/slicetca/invariance/transformations.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/plotting/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       45 2023-03-04 21:19:31.000000 slicetca-0.1.9/slicetca/plotting/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-0.1.9/slicetca/plotting/additional.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-0.1.9/slicetca/plotting/factors.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/run/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-0.1.9/slicetca/run/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3125 2023-07-12 00:13:29.000000 slicetca-0.1.9/slicetca/run/decompose.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5056 2023-07-12 00:15:06.000000 slicetca-0.1.9/slicetca/run/grid_search.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-0.1.9/slicetca/run/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-0.1.9/slicetca/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/tests/tests.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2312 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      775 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       28 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/top_level.txt
```

### Comparing `slicetca-0.1.8/LICENSE.txt` & `slicetca-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/PKG-INFO` & `slicetca-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -47,14 +47,15 @@
 
 # your_data is a numpy array of shape (trials, neurons, time).
 data = torch.tensor(your_data, dtype=torch.float, device=device)
 
 # The tensor is decomposed into 2 trial-, 0 neuron- and 3 time-slicing components.
 components, model = slicetca.decompose(data, (2,0,3))
 
+# For a not positive decomposition, we apply uniqueness constraints
 model = slicetca.invariance(model)
 
 slicetca.plot(model)
 
 plt.show()
 ```
```

### Comparing `slicetca-0.1.8/README.md` & `slicetca-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 # your_data is a numpy array of shape (trials, neurons, time).
 data = torch.tensor(your_data, dtype=torch.float, device=device)
 
 # The tensor is decomposed into 2 trial-, 0 neuron- and 3 time-slicing components.
 components, model = slicetca.decompose(data, (2,0,3))
 
+# For a not positive decomposition, we apply uniqueness constraints
 model = slicetca.invariance(model)
 
 slicetca.plot(model)
 
 plt.show()
 ```
```

### Comparing `slicetca-0.1.8/setup.py` & `slicetca-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='slicetca',
     packages=find_packages(exclude=['tests*']),
-    version='0.1.8',
+    version='0.1.9',
 
     description='Package to perform Slice Tensor Component Analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/arthur-pe/slicetca',
     author='Arthur Pellegrino',
```

### Comparing `slicetca-0.1.8/slicetca/core/decompositions.py` & `slicetca-0.1.9/slicetca/core/decompositions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import torch
 from torch import nn
 import numpy as np
 import tqdm
+from collections.abc import Iterable
 
 from typing import Sequence, Union, Callable
 
+
 class PartitionTCA(nn.Module):
 
     def __init__(self,
                  dimensions: Sequence[int],
                  partitions: Sequence[Sequence[Sequence[int]]],
                  ranks: Sequence[int],
                  positive: Union[bool, Sequence[Sequence[Callable]]] = False,
                  initialization: str = 'uniform',
-                 init_weight: float = 1.0,
-                 init_bias: float = 0.0,
+                 init_weight: float = None,
+                 init_bias: float = None,
                  device: str = 'cpu'):
         """
         Parent class for the sliceTCA and TCA decompositions.
 
         :param dimensions: Dimensions of the data to decompose.
         :param partitions: List of partitions of the legs of the tensor.
                         [[[0],[1]]] would be a matrix rank decomposition.
@@ -32,32 +34,38 @@
         :param device: Torch device.
         """
 
         super(PartitionTCA, self).__init__()
 
         components = [[[dimensions[k] for k in j] for j in i] for i in partitions]
 
+        if init_weight is None:
+            if initialization == 'normal': init_weight = 1/np.sqrt(sum(ranks))
+            if initialization == 'uniform-positive': init_weight = ((0.5 / sum(ranks)) ** (1 / max([len(p) for p in partitions])))*2
+            if initialization == 'uniform': init_weight = 1/np.sqrt(sum(ranks))
+        if init_bias is None: init_bias = 0.0
+
         if isinstance(positive, bool):
             if positive: positive_function = [[torch.abs for j in i] for i in partitions]
             else: positive_function = [[self.identity for j in i] for i in partitions]
         elif isinstance(positive, tuple) or isinstance(positive, list): positive_function = positive
 
         vectors = nn.ModuleList([])
 
         for i in range(len(ranks)):
-            rank = ranks[i]
+            r = ranks[i]
             dim = components[i]
 
             # k-tensors of the outer product
             if initialization == 'normal':
-                v = [nn.Parameter(positive_function[i][j](torch.randn([rank]+d, device=device))) for j, d in enumerate(dim)]
+                v = [nn.Parameter(positive_function[i][j](torch.randn([r]+d, device=device)*init_weight + init_bias)) for j, d in enumerate(dim)]
             elif initialization == 'uniform':
-                v = [nn.Parameter(positive_function[i][j](torch.rand([rank] + d, device=device)*init_weight + init_bias)) for j, d in enumerate(dim)]
+                v = [nn.Parameter(positive_function[i][j](2*(torch.rand([r] + d, device=device)-0.5)*init_weight + init_bias)) for j, d in enumerate(dim)]
             elif initialization == 'uniform-positive':
-                v = [nn.Parameter(positive_function[i][j]((2*torch.rand([rank] + d, device=device)-1)*init_weight + init_bias)) for j, d in enumerate(dim)]
+                v = [nn.Parameter(positive_function[i][j](torch.rand([r] + d, device=device)*init_weight + init_bias)) for j, d in enumerate(dim)]
             else:
                 raise Exception('Undefined initialization, select one of : normal, uniform, uniform-positive')
 
             vectors.append(nn.ParameterList(v))
 
         self.vectors = vectors
 
@@ -250,16 +258,16 @@
 
 class SliceTCA(PartitionTCA):
     def __init__(self, 
                  dimensions: Sequence[int], 
                  ranks: Sequence[int], 
                  positive: bool = False, 
                  initialization: str = 'uniform',
-                 init_weight: float = 1.0, 
-                 init_bias: float = 0.0, 
+                 init_weight: float = None,
+                 init_bias: float = None,
                  device: str = 'cpu'):
         """
         Main sliceTCA decomposition class.
 
         :param dimensions: Dimensions of the data to decompose.
         :param ranks: Number of components of each slice type.
         :param positive: If False does nothing.
@@ -280,16 +288,16 @@
 
 class TCA(PartitionTCA):
     def __init__(self,
                  dimensions: Sequence[int],
                  rank: int,
                  positive: bool = False,
                  initialization: str = 'uniform',
-                 init_weight: float = 1.0,
-                 init_bias: float = 0.0,
+                 init_weight: float = None,
+                 init_bias: float = None,
                  device: str = 'cpu'):
         """
         Main TCA decomposition class.
 
         :param dimensions: Dimensions of the data to decompose.
         :param rank: Number of components.
         :param positive: If False does nothing.
@@ -297,15 +305,15 @@
                          If list of list, the list of functions to apply to a given partition and component.
         :param initialization: Components initialization 'uniform'~U(-1,1), 'uniform-positive'~U(0,1), 'normal'~N(0,1).
         :param init_weight: Coefficient to multiply the initial component by.
         :param init_bias: Coefficient to add to the initial component.
         :param device: Torch device.
         """
 
-        if type(rank) is not tuple:
+        if not isinstance(rank, Iterable):
             rank = (rank,)
 
         valence = len(dimensions)
         partitions = [[[j] for j in range(valence)]]
 
         super().__init__(dimensions=dimensions, ranks=rank, partitions=partitions, positive=positive,
                          initialization=initialization, init_weight=init_weight, init_bias=init_bias, device=device)
```

### Comparing `slicetca-0.1.8/slicetca/invariance/analytic_invariance.py` & `slicetca-0.1.9/slicetca/invariance/analytic_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/invariance/criteria.py` & `slicetca-0.1.9/slicetca/invariance/criteria.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/invariance/helper.py` & `slicetca-0.1.9/slicetca/invariance/helper.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/invariance/invariance.py` & `slicetca-0.1.9/slicetca/invariance/invariance.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,13 @@
     :param model: A sliceTCA model.
     :param L2: String, currently only supports 'regularization', you may add additional objectives.
     :param L3: String, currently only supports 'svd'.
     :param kwargs: Key-word arguments to be passed to L2 and L3 optimization functions. See iterative_function.py
     :return: model with modified components.
     """
 
-    model = sgd_invariance(model, objective_function=dict_L2_invariance_objectives[L2], **kwargs)
+    # Add check for model with single component type
+    if sum([r!=0 for r in model.ranks])>1:
+        model = sgd_invariance(model, objective_function=dict_L2_invariance_objectives[L2], **kwargs)
     model = dict_L3_invariance_functions[L3](model, **kwargs)
 
     return model
```

### Comparing `slicetca-0.1.8/slicetca/invariance/iterative_invariance.py` & `slicetca-0.1.9/slicetca/invariance/iterative_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/invariance/transformations.py` & `slicetca-0.1.9/slicetca/invariance/transformations.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/plotting/factors.py` & `slicetca-0.1.9/slicetca/plotting/factors.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/run/decompose.py` & `slicetca-0.1.9/slicetca/run/decompose.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from typing import Union, Sequence
 import numpy as np
 
 
 def decompose(data: Union[torch.Tensor, np.array],
               number_components: Union[Sequence[int], int],
               positive: bool = False,
-              initialization: str = 'uniform',
+              initialization: str = None,
               learning_rate: float = 5*10**-3,
               batch_prop: float = 0.2,
               max_iter: int = 10000,
               min_std: float = 10**-5,
-              iter_std: int = 100,
+              iter_std: int = 200,
               mask: torch.Tensor = None,
               verbose: bool = False,
               progress_bar: bool = True,
               seed: int = 7,
               weight_decay: float = None,
               batch_prop_decay: int = 1):
     """
@@ -42,22 +42,23 @@
     :return: model: A SliceTCA or TCA model. It can be used to access the losses over training and much more.
     """
 
     torch.manual_seed(seed)
 
     if isinstance(data, np.ndarray): data = torch.tensor(data, device='cuda' if torch.cuda.is_available() else 'cpu')
 
+    if initialization is None: initialization = 'uniform-positive' if positive else 'uniform'
+
     dimensions = list(data.shape)
 
     if isinstance(number_components, int): decomposition = TCA
     else: decomposition = SliceTCA
 
     model = decomposition(dimensions, number_components, positive, initialization, device=data.device)
 
     if weight_decay is None: optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
     else: optimizer = torch.optim.AdamW(model.parameters(), lr=learning_rate, weight_decay=weight_decay)
 
     for i in range(1,batch_prop_decay+1):
         model.fit(data, optimizer, 1-(1-batch_prop)**i, max_iter, min_std, iter_std, mask, verbose, progress_bar)
 
     return model.get_components(numpy=True), model
-
```

### Comparing `slicetca-0.1.8/slicetca/run/grid_search.py` & `slicetca-0.1.9/slicetca/run/grid_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from slicetca.run.decompose import decompose
 
-from multiprocessing import Pool
 import multiprocessing as mp
 from functools import partial
 from concurrent.futures import ProcessPoolExecutor as Pool
+from tqdm import tqdm
 import torch
 import numpy as np
 
 from typing import Sequence, Union
 
 
-def grid_search(data: Union[torch.Tensor, np.array],
+# To be fixed: high memory usage when using GPU.
+
+def grid_search(data: Union[torch.Tensor, np.array], #Only works with torch.Tensor atm
                 max_ranks: Sequence[int],
                 mask_train: torch.Tensor = None,
                 mask_test: torch.Tensor = None,
                 min_ranks: Sequence[int] = None,
                 sample_size: int = 1,
                 processes_sample: int = 1,
                 processes_grid: int = 1,
@@ -34,30 +36,42 @@
     :param seed: Numpy seed.
     :param kwargs: Same kwargs as decompose.
     :return: A (max_rank_1-min_rank_1, max_rank_2-min_rank_2, ..., sample_size) ndarray of losses masked entries.
     """
 
     np.random.seed(seed)
 
-    mp.set_start_method('spawn')
+    try:
+        mp.set_start_method('spawn', force=True)
+    except RuntimeError:
+        pass
 
     if min_ranks is None: min_ranks = [0 for i in max_ranks]
     max_ranks = [i+1 for i in max_ranks]
     rank_span = [max_ranks[i]-min_ranks[i] for i in range(len(max_ranks))]
 
     grid = get_grid_sample(min_ranks, max_ranks)
     grid = np.concatenate([grid, np.random.randint(10**2,10**6, grid.shape[0])[:,np.newaxis]], axis=-1)
 
-    print('Grid size:', str(rank_span), '- sample:', sample_size,
-          '- total_fit:', torch.tensor(grid).size()[0]*sample_size)
+    print('Grid shape:', str(rank_span),
+          '- Samples:', sample_size,
+          '- Grid entries:', torch.tensor(grid).size()[0],
+          '- Number of models to fit:', torch.tensor(grid).size()[0]*sample_size)
 
     dec = partial(decompose_mp_sample, data=data, mask_train=mask_train, mask_test=mask_test, sample_size=sample_size,
                   processes_sample=processes_sample, **kwargs)
 
-    with Pool(max_workers=processes_grid) as pool: out_grid = np.array(list(pool.map(dec, grid)), dtype=np.float32)
+    out_grid = []
+    with Pool(max_workers=processes_grid) as pool:
+        iterator = tqdm(pool.map(dec, grid), total=torch.tensor(grid).size()[0])
+        iterator.set_description('Number of components (completed): - ', refresh=True)
+        for i, p in enumerate(iterator):
+            out_grid.append(p)
+            iterator.set_description('Number of components (completed): '+str(np.unravel_index(i, tuple(max_ranks))) + ' ', refresh=True)
+    out_grid = np.array(out_grid, dtype=np.float32)
 
     loss_grid = out_grid[:,0]
     seed_grid = out_grid[:,1].astype(int)
 
     loss_grid = loss_grid.reshape(rank_span+[sample_size])
     seed_grid = seed_grid.reshape(rank_span+[sample_size])
 
@@ -67,20 +81,18 @@
 def decompose_mp_sample(number_components_seed, data, mask_train, mask_test, sample_size, processes_sample, **kwargs):
 
     number_components = number_components_seed[:-1]
     seed = number_components_seed[-1]
 
     np.random.seed(seed)
 
-    print('Starting fitting components:', number_components)
-
     dec = partial(decompose_mp,
                   data=data.clone(),
-                  mask_train=(mask_train.clone().float() if mask_train is not None else None),
-                  mask_test=(mask_test.clone().float() if mask_test is not None else None),
+                  mask_train=(mask_train.clone() if mask_train is not None else None),
+                  mask_test=(mask_test.clone() if mask_test is not None else None),
                   **kwargs)
 
     sample = number_components[np.newaxis].repeat(sample_size, 0)
     seeds = np.random.randint(10**2,10**6, sample_size)
 
     sample = np.concatenate([sample, seeds[:,np.newaxis]], axis=-1)
 
@@ -97,15 +109,15 @@
         data_hat = 0
     else:
         _, model = decompose(data, number_components, mask=mask_train, verbose=False, progress_bar=False, *args,
                              seed=seed, **kwargs)
         data_hat = model.construct()
 
     if mask_test is None: loss = torch.mean((data-data_hat)**2).item()
-    else: loss = torch.mean(((data-data_hat)*(1-mask_test))**2).item()
+    else: loss = torch.mean(((data-data_hat)[mask_test])**2).item()
 
     return loss
 
 
 def get_grid_sample(min_dims, max_dims):
 
     grid = np.meshgrid(*[np.array([i for i in range(min_dims[j],max_dims[j])]) for j in range(len(max_dims))])
```

### Comparing `slicetca-0.1.8/slicetca/run/utils.py` & `slicetca-0.1.9/slicetca/run/utils.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca/tests/tests.py` & `slicetca-0.1.9/slicetca/tests/tests.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.8/slicetca.egg-info/PKG-INFO` & `slicetca-0.1.9/slicetca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -47,14 +47,15 @@
 
 # your_data is a numpy array of shape (trials, neurons, time).
 data = torch.tensor(your_data, dtype=torch.float, device=device)
 
 # The tensor is decomposed into 2 trial-, 0 neuron- and 3 time-slicing components.
 components, model = slicetca.decompose(data, (2,0,3))
 
+# For a not positive decomposition, we apply uniqueness constraints
 model = slicetca.invariance(model)
 
 slicetca.plot(model)
 
 plt.show()
 ```
```

### Comparing `slicetca-0.1.8/slicetca.egg-info/SOURCES.txt` & `slicetca-0.1.9/slicetca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

