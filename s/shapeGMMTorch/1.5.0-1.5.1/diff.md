# Comparing `tmp/shapeGMMTorch-1.5.0.tar.gz` & `tmp/shapeGMMTorch-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapeGMMTorch-1.5.0.tar", last modified: Mon Jul 10 14:29:09 2023, max compression
+gzip compressed data, was "shapeGMMTorch-1.5.1.tar", last modified: Mon Jul 17 20:05:27 2023, max compression
```

## Comparing `shapeGMMTorch-1.5.0.tar` & `shapeGMMTorch-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.962952 shapeGMMTorch-1.5.0/
--rw-r--r--   0 mmccull    (502) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.5.0/LICENSE
--rw-r--r--   0 mmccull    (502) staff       (20)     7554 2023-07-10 14:29:09.962504 shapeGMMTorch-1.5.0/PKG-INFO
--rw-r--r--   0 mmccull    (502) staff       (20)     6967 2023-07-10 14:27:00.000000 shapeGMMTorch-1.5.0/README.md
--rw-r--r--   0 mmccull    (502) staff       (20)       38 2023-07-10 14:29:09.963068 shapeGMMTorch-1.5.0/setup.cfg
--rw-r--r--   0 mmccull    (502) staff       (20)     1006 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/setup.py
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.942210 shapeGMMTorch-1.5.0/src/
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.960735 shapeGMMTorch-1.5.0/src/shapeGMMTorch/
--rw-r--r--   0 mmccull    (502) staff       (20)        0 2023-06-28 14:43:45.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/__init__.py
--rw-r--r--   0 mmccull    (502) staff       (20)     2881 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/plots.py
--rw-r--r--   0 mmccull    (502) staff       (20)     7292 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/scripts.py
--rw-r--r--   0 mmccull    (502) staff       (20)    13593 2023-06-28 14:43:45.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_align.py
--rw-r--r--   0 mmccull    (502) staff       (20)     6529 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
--rw-r--r--   0 mmccull    (502) staff       (20)    19790 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_sgmm.py
--rw-r--r--   0 mmccull    (502) staff       (20)     5781 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.962172 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/
--rw-r--r--   0 mmccull    (502) staff       (20)     7554 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/PKG-INFO
--rw-r--r--   0 mmccull    (502) staff       (20)      471 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/SOURCES.txt
--rw-r--r--   0 mmccull    (502) staff       (20)        1 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/dependency_links.txt
--rw-r--r--   0 mmccull    (502) staff       (20)       18 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/requires.txt
--rw-r--r--   0 mmccull    (502) staff       (20)       14 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/top_level.txt
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-17 20:05:27.349305 shapeGMMTorch-1.5.1/
+-rw-r--r--   0 mmccull    (502) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.5.1/LICENSE
+-rw-r--r--   0 mmccull    (502) staff       (20)     7563 2023-07-17 20:05:27.348901 shapeGMMTorch-1.5.1/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)     6976 2023-07-17 19:13:34.000000 shapeGMMTorch-1.5.1/README.md
+-rw-r--r--   0 mmccull    (502) staff       (20)       38 2023-07-17 20:05:27.349387 shapeGMMTorch-1.5.1/setup.cfg
+-rw-r--r--   0 mmccull    (502) staff       (20)     1006 2023-07-13 16:40:56.000000 shapeGMMTorch-1.5.1/setup.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-17 20:05:27.314682 shapeGMMTorch-1.5.1/src/
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-17 20:05:27.346571 shapeGMMTorch-1.5.1/src/shapeGMMTorch/
+-rw-r--r--   0 mmccull    (502) staff       (20)        0 2023-06-28 14:43:45.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/__init__.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     2881 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/plots.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     7292 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/scripts.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    14075 2023-07-17 20:02:46.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_align.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     6633 2023-07-13 18:17:32.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    19965 2023-07-13 20:25:27.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_sgmm.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     5781 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-17 20:05:27.348534 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/
+-rw-r--r--   0 mmccull    (502) staff       (20)     7563 2023-07-17 20:05:26.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)      471 2023-07-17 20:05:27.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/SOURCES.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)        1 2023-07-17 20:05:26.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/dependency_links.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       18 2023-07-17 20:05:26.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/requires.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       14 2023-07-17 20:05:26.000000 shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/top_level.txt
```

### Comparing `shapeGMMTorch-1.5.0/LICENSE` & `shapeGMMTorch-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.5.0/PKG-INFO` & `shapeGMMTorch-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.5.0
+Version: 1.5.1
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 This package is dependent on the following packages:
 
 1. Python>=3.6 
 2. numpy
 3. torch>=1.11 (==1.11 if option 4 is used)
 4. Optional: torch_batch_svd available from https://github.com/KinglittleQ/torch-batch-svd
 
-The last package is for the SVD part of the alignment and is much faster than the native batch torch library.  It is, however, not compatible with the current version of torch (1.12) thus the requirement of torch 1.11.
+The last package is for the SVD part of the alignment and is faster than the native batch torch library for certain devices. I have found it to be slower than the torch native SVD for the latest hardware and software versions. 
 
 The examples are also dependent on:
 
 1. MDAnalysis
 2. matplotlib
 3. pyemma
 4. shapeGMM
```

### Comparing `shapeGMMTorch-1.5.0/README.md` & `shapeGMMTorch-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 This package is dependent on the following packages:
 
 1. Python>=3.6 
 2. numpy
 3. torch>=1.11 (==1.11 if option 4 is used)
 4. Optional: torch_batch_svd available from https://github.com/KinglittleQ/torch-batch-svd
 
-The last package is for the SVD part of the alignment and is much faster than the native batch torch library.  It is, however, not compatible with the current version of torch (1.12) thus the requirement of torch 1.11.
+The last package is for the SVD part of the alignment and is faster than the native batch torch library for certain devices. I have found it to be slower than the torch native SVD for the latest hardware and software versions. 
 
 The examples are also dependent on:
 
 1. MDAnalysis
 2. matplotlib
 3. pyemma
 4. shapeGMM
```

### Comparing `shapeGMMTorch-1.5.0/setup.py` & `shapeGMMTorch-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='shapeGMMTorch',
-    version='1.5.0',
+    version='1.5.1',
     author='Martin McCullagh',
     author_email='martin.mccullagh@okstate.edu',
     description='Gaussian Mixture Model clustering in size-and-shape space using PyTorch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mccullaghlab/shapeGMMTorch',
     project_urls = {
```

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/plots.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/plots.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/scripts.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/scripts.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_align.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_align.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # library of trajectory alignment protocols using PyTorch
 
 # import libraries
 import numpy as np
 import torch
 import importlib
-# check to see if fast SVD library is available
-svd_loader = importlib.util.find_spec('torch_bath_svd')
+# check to see if SVD library is available
+svd_loader = importlib.util.find_spec('torch_batch_svd')
 if svd_loader is not None:
     from torch_batch_svd import svd
     def torch_align_rot_mat(traj_tensor, ref_tensor):
         # compute correlation matrices using batched matmul
         c_mats = torch.matmul(ref_tensor.T,traj_tensor)
         # perfrom SVD of c_mats using batched SVD
         u, s, v = svd(c_mats)
@@ -193,14 +193,28 @@
 # determine the ln(det) of a singular matrix ignoring eigenvalues below threshold
 def _torch_pseudo_lndet(sigma, EigenValueThresh=1e-10):
     e = torch.linalg.eigvalsh(sigma) 
     e = torch.where(e > EigenValueThresh, e, 1.0)
     lpdet = torch.sum(torch.log(e))
     return lpdet
 
+# determine the pseudo inverse and ln(det) of a singular matrix ignoring first eigenvalue
+def _torch_pseudo_inv(sigma,device=torch.device("cuda:0")):
+    # diagonalize sigma
+    e, v = torch.linalg.eigh(sigma) 
+    # compute the log of the pseudo determinant of sigma
+    lpdet = torch.sum(torch.log(e[1:]))
+    # now compute multiplicative reciprocal of eigenvalues except first
+    e[1:] = torch.reciprocal(e[1:])
+    # set first eigenvalue/recirpical to zero
+    e[0] = 0.0
+    # construct the inverse
+    inv = torch.matmul(v,torch.matmul(torch.diag(e),v.T))
+    return inv, lpdet
+
 def _torch_kronecker_log_lik(disp, precision, lpdet):
     # meta data
     n_frames = disp.shape[0]
     n_atoms = disp.shape[1]
     # compute log Likelihood for all points
     log_lik = torch.matmul(disp[:,:,0].view(n_frames,1,n_atoms),torch.matmul(precision,disp[:,:,0].view(n_frames,n_atoms,1)))[:,0,0]
     log_lik += torch.matmul(disp[:,:,1].view(n_frames,1,n_atoms),torch.matmul(precision,disp[:,:,1].view(n_frames,n_atoms,1)))[:,0,0]
@@ -226,24 +240,23 @@
     while (delta_log_lik > thresh):
         # get rotation matrices
         rot_mat = torch_align_rot_mat(traj_tensor, weighted_avg)
         # do rotation
         traj_tensor = torch.matmul(traj_tensor,rot_mat)
         # compute new average
         avg = torch.mean(traj_tensor,0,False)
-        disp = (traj_tensor - avg).to(torch.float64)
         # compute covar using strided data
         covar = torch.zeros((n_atoms,n_atoms),dtype=torch.float64,device=device)
+        disp = (traj_tensor - avg).to(torch.float64)
         for frame in range(0,n_frames,stride):
             upper_limit = min(frame+stride,n_frames)
             covar += torch.sum(torch.matmul(disp[frame:upper_limit],torch.transpose(disp[frame:upper_limit],1,2)),0)
         covar *= covar_norm
         # log likelihood
-        precision = torch.linalg.pinv(covar, atol=1e-10, hermitian= True)
-        lpdet = _torch_pseudo_lndet(covar)
+        precision, lpdet =  _torch_pseudo_inv(covar,device=device)
         log_lik = _torch_kronecker_log_lik(disp, precision, lpdet)
         delta_log_lik = abs(log_lik - old_log_lik)
         if verbose == True:
             print(log_lik)
         old_log_lik = log_lik
         weighted_avg = torch.matmul(precision,avg.to(torch.float64)).to(dtype)
     # free up local variables 
@@ -292,24 +305,23 @@
     while (delta_log_lik > thresh):
         # get rotation matrices
         rot_mat = torch_align_rot_mat(traj_tensor, weighted_avg)
         # do rotation
         traj_tensor = torch.matmul(traj_tensor,rot_mat)
         # compute new average
         avg = torch.sum((traj_tensor*weight_tensor.view(-1,1,1)),0,False)
-        disp = (traj_tensor - avg).to(torch.float64)
         # compute covar using strided data
         covar = torch.zeros((n_atoms,n_atoms),dtype=torch.float64,device=device)
+        disp = (traj_tensor - avg).to(torch.float64)
         for frame in range(0,n_frames,stride):
             upper_limit = min(frame+stride,n_frames)
             covar += torch.sum(torch.matmul(disp[frame:upper_limit],torch.transpose(disp[frame:upper_limit],1,2))*weight_tensor[frame:upper_limit].view(-1,1,1),0)
         covar *= covar_norm
         # log likelihood
-        precision = torch.linalg.pinv(covar, atol=1e-10, hermitian= True)
-        lpdet = _torch_pseudo_lndet(covar)
+        precision, lpdet =  _torch_pseudo_inv(covar,device=device)
         log_lik = _torch_kronecker_weighted_log_lik(disp, weight_tensor, precision, lpdet)
         delta_log_lik = abs(log_lik - old_log_lik)
         if verbose == True:
             print(log_lik)
         old_log_lik = log_lik
         weighted_avg = torch.matmul(precision, avg.to(torch.float64)).to(dtype)     
     # free up local variables
```

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 warnings.filterwarnings('ignore')
 import random
 #import torch_align
 from . import torch_align
 import torch
 
-GAMMA_THRESH = 1e-15
+GAMMA_THRESH = 1e-20
 
 ##
 def kronecker_sgmm_log_likelihood(traj_tensor, clusters, thresh=1e-3, dtype=torch.float32, device=torch.device("cuda:0")):
     # meta data from inputs
     n_frames = traj_tensor.shape[0]
     n_clusters = np.unique(clusters).shape[0] 
     n_atoms = traj_tensor.shape[1]
@@ -66,28 +66,30 @@
     cluster_frame_ln_likelihoods_tensor = torch_sgmm_expectation_kronecker(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, dtype=dtype, device=device)
     
     # compute log likelihood and gamma normalization
     for k in range(n_clusters):
         cluster_frame_ln_likelihoods_tensor[:,k] += ln_weights_tensor[k]
     log_norm = torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)
     log_likelihood = torch.sum(frame_weights_tensor*log_norm,0)
+    #log_likelihood = torch.mean(log_norm)
     # determine gamma values
     # use the current values for the parameters to evaluate the posterior
     # probabilities of the data to have been generanted by each gaussian
     gamma_tensor = torch.exp(cluster_frame_ln_likelihoods_tensor - log_norm.view(-1,1))
     # multiply gamma by frame weights
     gamma_tensor *= frame_weights_tensor.view(-1,1)
-    # update the weights
+    # update the cluster weights
     ln_weights_tensor = torch.log(torch.sum(gamma_tensor,0))
+    #ln_weights_tensor = torch.log(torch.mean(gamma_tensor,0))
     # update averages and variances of each cluster
     for k in range(n_clusters):
         gamma_indeces = torch.argwhere(gamma_tensor[:,k] > gamma_thresh_tensor).flatten()
         if gamma_indeces.shape[0] > n_atoms:
             # update mean and variance
-            centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[gamma_indeces], gamma_tensor[gamma_indeces,k].to(dtype), ref_tensor=centers_tensor[k], ref_precision_tensor=precisions_tensor[k], dtype=dtype, thresh=thresh, device=device)[1:]
+            centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[gamma_indeces], gamma_tensor[gamma_indeces,k], ref_tensor=centers_tensor[k], ref_precision_tensor=precisions_tensor[k], dtype=dtype, thresh=thresh, device=device)[1:]
     return centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, log_likelihood    
     del cluster_frame_ln_likelihoods
     del log_lorm
     del gamma_tensor
     del gamma_indeces
     torch.cuda.empty_cache()
```

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_sgmm.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_sgmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         frame_weights (optional) - (n_frames) float numpy array of frame weights
 
         Returns an aligned trajectory, if requested.  Each cluster aligned to respective average.
         """
 
         # pass trajectory data to device
         traj_tensor = torch.tensor(traj_data,dtype=self.dtype,device=self.device)
+        # Remove the center-of-geometry from entire trajectory
+        torch_align.torch_remove_center_of_geometry(traj_tensor)
         # Initialize clusters if they have not been already
         if (self._init_clusters_flag == False):
             self._init_clusters(traj_tensor, cluster_ids)
         # frame weights
         if len(frame_weights) == 0:
             if (self.verbose==True):
                 print("Setting uniform frame weights")
@@ -141,15 +143,19 @@
             # assign clusters based on largest likelihood 
             self.cluster_ids = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
             traj_data, self.centers = self._align_clusters_kronecker(traj_tensor,centers_tensor, precisions_tensor)
             self.precisions = precisions_tensor.cpu().numpy()
             self.lpdets = lpdets_tensor.cpu().numpy()
             del precisions_tensor
             del lpdets_tensor
-        self.train_frame_log_likelihood = (frame_weights_tensor*torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)).cpu().numpy()
+        # determine log likelihood per frame and save it
+        for k in range(self.n_clusters):
+            cluster_frame_ln_likelihoods_tensor[:,k] += ln_weights_tensor[k]
+        self.train_frame_log_likelihood = (torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)).cpu().numpy()
+        # delete data
         del traj_tensor
         del ln_weights_tensor
         del cluster_frame_ln_likelihoods_tensor
         del centers_tensor
         torch.cuda.empty_cache()
         
         # sort object
@@ -250,17 +256,14 @@
             print("Number of frames being analyzed:", self.n_train_frames)
             print("Number of particles being analyzed:", self.n_atoms)
             print("Number of dimensions (must be 3):", self.n_dim)
             print("Initializing clustering using method:", self.init_cluster_method)
         # declare clusters
         self.cluster_ids = np.zeros(self.n_train_frames,dtype=np.int32)
 
-        # Remove the center-of-geometry from entire trajectory
-        torch_align.torch_remove_center_of_geometry(traj_tensor)
-
         # make initial clustering based on input user choice (default is random)
         if (self.init_cluster_method == "chunk"):
             for i in range(self.n_train_frames):
                 self.cluster_ids[i] = i*self.n_clusters // self.n_train_frames
         elif (self.init_cluster_method == "read"):
             # should affirm that there are n_train_frames clusters
             self.cluster_ids = cluster_ids
```

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch/torch_uniform_sgmm_lib.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/PKG-INFO` & `shapeGMMTorch-1.5.1/src/shapeGMMTorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.5.0
+Version: 1.5.1
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 This package is dependent on the following packages:
 
 1. Python>=3.6 
 2. numpy
 3. torch>=1.11 (==1.11 if option 4 is used)
 4. Optional: torch_batch_svd available from https://github.com/KinglittleQ/torch-batch-svd
 
-The last package is for the SVD part of the alignment and is much faster than the native batch torch library.  It is, however, not compatible with the current version of torch (1.12) thus the requirement of torch 1.11.
+The last package is for the SVD part of the alignment and is faster than the native batch torch library for certain devices. I have found it to be slower than the torch native SVD for the latest hardware and software versions. 
 
 The examples are also dependent on:
 
 1. MDAnalysis
 2. matplotlib
 3. pyemma
 4. shapeGMM
```

