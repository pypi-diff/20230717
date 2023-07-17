# Comparing `tmp/escnn-1.0.7.tar.gz` & `tmp/escnn-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/escnn-1.0.7.tar", last modified: Tue Mar  7 23:35:12 2023, max compression
+gzip compressed data, was "dist/escnn-1.0.8.tar", last modified: Thu May 18 16:30:43 2023, max compression
```

## Comparing `escnn-1.0.7.tar` & `escnn-1.0.8.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1664 2022-10-08 11:28:46.000000 escnn-1.0.7/LICENSE
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19243 2023-03-07 23:35:12.000000 escnn-1.0.7/PKG-INFO
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18767 2023-03-07 23:31:39.000000 escnn-1.0.7/README.md
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      388 2023-03-07 23:33:40.000000 escnn-1.0.7/escnn/__about__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      523 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/__init__.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/group/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2375 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11336 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/_clebsh_gordan.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    29901 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/group/_numerical.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    31209 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/directproduct.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5681 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/doublegroup.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    41360 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/group.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/group/groups/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      524 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/groups/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    12848 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/groups/_numerical_thomson.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20855 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/cyclicgroup.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    30920 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/dihedralgroup.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11960 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/groups/factory.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    25793 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/ico.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    33160 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/group/groups/o2group.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    80577 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/o3group.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    25812 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/groups/octa.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19631 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/so2group.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    15904 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/groups/so3_utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    49034 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/group/groups/so3group.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1245 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/groups/utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20917 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/homspace.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10533 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/group/irrep.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    53633 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/group/representation.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1610 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/group/utils.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/gspaces/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      607 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/gspaces/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18716 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/gspaces/gspace.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3055 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/gspaces/r0.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9444 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/gspaces/r2.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13557 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/gspaces/r3.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3542 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/gspaces/utils.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/kernels/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2736 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8022 2022-11-17 22:28:27.000000 escnn-1.0.7/escnn/kernels/basis.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3614 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/harmonic_polynomial_r3.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    33704 2023-02-02 21:36:19.000000 escnn-1.0.7/escnn/kernels/polar_basis.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19343 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/r2.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    25568 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/r3.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11426 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/sparse_basis.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    24387 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/kernels/steerable_basis.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    12813 2022-11-17 22:28:07.000000 escnn-1.0.7/escnn/kernels/steerable_filters_basis.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19145 2022-11-17 22:28:27.000000 escnn-1.0.7/escnn/kernels/wignereckart_solver.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      305 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    24948 2022-11-17 10:02:02.000000 escnn-1.0.7/escnn/nn/field_type.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    36991 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/nn/geometric_tensor.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5451 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/init.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4710 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/__init__.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/basismanager/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1339 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/basismanager/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18806 2023-03-07 23:33:40.000000 escnn-1.0.7/escnn/nn/modules/basismanager/basisexpansion_blocks.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     7853 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/nn/modules/basismanager/basisexpansion_singleblock.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1371 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/basismanager/basismanager.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    21955 2023-03-07 23:33:40.000000 escnn-1.0.7/escnn/nn/modules/basismanager/basissampler_blocks.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4753 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/nn/modules/basismanager/basissampler_singleblock.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      422 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14194 2023-02-02 21:36:19.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/gnorm.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    26897 2022-12-17 15:40:11.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/iid.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11543 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/induced_norm.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     9989 2023-02-02 21:36:19.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/inner.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10632 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/nn/modules/batchnormalization/norm.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9916 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/branching_module.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/conv/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      461 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/conv/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10521 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/conv/r2_transposed_convolution.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    21602 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/conv/r2convolution.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6381 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/conv/r3_ico_convolution.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6459 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/conv/r3_ico_transposed_convolution.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10984 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/conv/r3_transposed_convolution.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20875 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/conv/r3convolution.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18400 2023-02-10 18:31:29.000000 escnn-1.0.7/escnn/nn/modules/conv/rd_convolution.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    16291 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/conv/rd_transposed_convolution.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5569 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/disentangle_module.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/dropout/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      132 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/dropout/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5854 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/dropout/field.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2805 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/dropout/pointwise.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5831 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/equivariant_module.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3247 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/nn/modules/harmonic_polynomial_r3.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1726 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/identity_module.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/invariantmaps/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      216 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/invariantmaps/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8901 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/invariantmaps/gpool.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6828 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/invariantmaps/induced_norm.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5333 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/invariantmaps/norm.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    14891 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/linear.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2744 2022-10-08 11:28:46.000000 escnn-1.0.7/escnn/nn/modules/masking_module.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     4724 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/merge_module.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6917 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/multiple_module.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      983 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9694 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/concatenated.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3768 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/elu.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    12181 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/fourier.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14898 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/fourier_quotient.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11239 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/gated1.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9292 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/gated2.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5659 2022-11-17 20:46:21.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/gated3.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11424 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/induced_gated1.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9557 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/induced_norm.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8712 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/norm.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3904 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/pointwise.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3628 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/relu.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8697 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/tensor.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     4916 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/nonlinearities/vectorfield.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/pointconv/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      212 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/pointconv/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    12325 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/pointconv/r2_point_convolution.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9509 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/pointconv/r3_point_convolution.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19872 2023-03-07 23:33:40.000000 escnn-1.0.7/escnn/nn/modules/pointconv/rd_point_convolution.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn/nn/modules/pooling/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1468 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/__init__.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9183 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/pooling/norm_max.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6162 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/pointwise_adaptive_avg.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6330 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/pointwise_adaptive_max.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8736 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/pointwise_avg.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8926 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/pointwise_avg_3d.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    17597 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/pooling/pointwise_max.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    15995 2023-03-07 23:31:39.000000 escnn-1.0.7/escnn/nn/modules/rdupsampling.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3580 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/reshuffle_module.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3319 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/restriction_module.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5630 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/sequential_module.py
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1432 2022-10-08 11:28:47.000000 escnn-1.0.7/escnn/nn/modules/utils.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-03-07 23:35:12.000000 escnn-1.0.7/escnn.egg-info/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19243 2023-03-07 23:35:11.000000 escnn-1.0.7/escnn.egg-info/PKG-INFO
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4360 2023-03-07 23:35:11.000000 escnn-1.0.7/escnn.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        1 2023-03-07 23:35:11.000000 escnn-1.0.7/escnn.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       64 2023-03-07 23:35:11.000000 escnn-1.0.7/escnn.egg-info/requires.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        6 2023-03-07 23:35:11.000000 escnn-1.0.7/escnn.egg-info/top_level.txt
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)      103 2023-03-07 23:35:12.000000 escnn-1.0.7/setup.cfg
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1209 2023-02-10 18:31:29.000000 escnn-1.0.7/setup.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1664 2022-10-08 11:28:46.000000 escnn-1.0.8/LICENSE
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19243 2023-05-18 16:30:43.000000 escnn-1.0.8/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18767 2023-03-07 23:31:39.000000 escnn-1.0.8/README.md
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      388 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/__about__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      523 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/group/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2375 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11336 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/_clebsh_gordan.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    29901 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/group/_numerical.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    31209 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/directproduct.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5681 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/doublegroup.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    41360 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/group.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/group/groups/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      524 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/groups/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    12848 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/groups/_numerical_thomson.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20855 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/groups/cyclicgroup.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    31447 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/group/groups/dihedralgroup.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11960 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/groups/factory.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    25793 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/groups/ico.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    33160 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/group/groups/o2group.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    80577 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/groups/o3group.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    25812 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/groups/octa.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19631 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/groups/so2group.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    15904 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/groups/so3_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    49034 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/group/groups/so3group.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1245 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/groups/utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20917 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/homspace.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10533 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/group/irrep.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    53633 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/group/representation.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1610 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/group/utils.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/gspaces/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      607 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/gspaces/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18716 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/gspaces/gspace.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3055 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/gspaces/r0.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10126 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/gspaces/r2.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14228 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/gspaces/r3.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3542 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/gspaces/utils.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/kernels/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2736 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8022 2022-11-17 22:28:27.000000 escnn-1.0.8/escnn/kernels/basis.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3614 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/harmonic_polynomial_r3.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    33704 2023-02-02 21:36:19.000000 escnn-1.0.8/escnn/kernels/polar_basis.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19343 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/r2.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    25568 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/r3.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11426 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/sparse_basis.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    24387 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/kernels/steerable_basis.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    12813 2022-11-17 22:28:07.000000 escnn-1.0.8/escnn/kernels/steerable_filters_basis.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19145 2022-11-17 22:28:27.000000 escnn-1.0.8/escnn/kernels/wignereckart_solver.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn/nn/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      305 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    24948 2022-11-17 10:02:02.000000 escnn-1.0.8/escnn/nn/field_type.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    36991 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/nn/geometric_tensor.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5451 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/init.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4710 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/basismanager/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1339 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/basismanager/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18806 2023-03-07 23:33:40.000000 escnn-1.0.8/escnn/nn/modules/basismanager/basisexpansion_blocks.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     7853 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/nn/modules/basismanager/basisexpansion_singleblock.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1371 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/basismanager/basismanager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    21955 2023-03-07 23:33:40.000000 escnn-1.0.8/escnn/nn/modules/basismanager/basissampler_blocks.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4753 2023-02-10 18:31:29.000000 escnn-1.0.8/escnn/nn/modules/basismanager/basissampler_singleblock.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      422 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14194 2023-02-02 21:36:19.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/gnorm.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    26897 2022-12-17 15:40:11.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/iid.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11543 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/induced_norm.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     9989 2023-02-02 21:36:19.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/inner.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10632 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/nn/modules/batchnormalization/norm.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9916 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/branching_module.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/conv/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      461 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/conv/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10644 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/r2_transposed_convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    21725 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/r2convolution.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6381 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/conv/r3_ico_convolution.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6459 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/conv/r3_ico_transposed_convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11107 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/r3_transposed_convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    20997 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/r3convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    18523 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/rd_convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    16414 2023-05-18 16:08:50.000000 escnn-1.0.8/escnn/nn/modules/conv/rd_transposed_convolution.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5569 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/disentangle_module.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/dropout/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      132 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/dropout/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5854 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/dropout/field.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2805 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/dropout/pointwise.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5831 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/equivariant_module.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3247 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/nn/modules/harmonic_polynomial_r3.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1726 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/identity_module.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/invariantmaps/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      216 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/invariantmaps/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8901 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/invariantmaps/gpool.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6828 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/invariantmaps/induced_norm.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5333 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/invariantmaps/norm.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    14891 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/linear.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     2744 2022-10-08 11:28:46.000000 escnn-1.0.8/escnn/nn/modules/masking_module.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     4724 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/merge_module.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     6917 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/multiple_module.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      983 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9694 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/concatenated.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3768 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/elu.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    12181 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/fourier.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14898 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/fourier_quotient.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11239 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/gated1.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9292 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/gated2.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5659 2022-11-17 20:46:21.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/gated3.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    11424 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/induced_gated1.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9557 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/induced_norm.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8712 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/norm.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3904 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/pointwise.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3628 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/relu.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     8697 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/tensor.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     4916 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/nonlinearities/vectorfield.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/pointconv/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      212 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/pointconv/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    12325 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/pointconv/r2_point_convolution.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9509 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/pointconv/r3_point_convolution.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19872 2023-03-07 23:33:40.000000 escnn-1.0.8/escnn/nn/modules/pointconv/rd_point_convolution.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:43.000000 escnn-1.0.8/escnn/nn/modules/pooling/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1468 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/__init__.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     9183 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/pooling/norm_max.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6162 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/pointwise_adaptive_avg.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6330 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/pointwise_adaptive_max.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8736 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/pointwise_avg.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8926 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/pointwise_avg_3d.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    17597 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/pooling/pointwise_max.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    15995 2023-03-07 23:31:39.000000 escnn-1.0.8/escnn/nn/modules/rdupsampling.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3580 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/reshuffle_module.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     3319 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/restriction_module.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     5630 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/sequential_module.py
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)     1432 2022-10-08 11:28:47.000000 escnn-1.0.8/escnn/nn/modules/utils.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn.egg-info/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    19243 2023-05-18 16:30:41.000000 escnn-1.0.8/escnn.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4360 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        1 2023-05-18 16:30:41.000000 escnn-1.0.8/escnn.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       64 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        6 2023-05-18 16:30:42.000000 escnn-1.0.8/escnn.egg-info/top_level.txt
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)      103 2023-05-18 16:30:43.000000 escnn-1.0.8/setup.cfg
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1209 2023-02-10 18:31:29.000000 escnn-1.0.8/setup.py
```

### Comparing `escnn-1.0.7/LICENSE` & `escnn-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/PKG-INFO` & `escnn-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: escnn
-Version: 1.0.7
+Version: 1.0.8
 Summary: E(n)-Equivariant CNNs Library for PyTorch
 Home-page: https://github.com/QUVA-Lab/escnn
-Download-URL: https://github.com/QUVA-Lab/escnn/archive/v1.0.7.tar.gz
+Download-URL: https://github.com/QUVA-Lab/escnn/archive/v1.0.8.tar.gz
 Author: Gabriele Cesa
 Author-email: cesa.gabriele@gmail.com
 License: BSD 3-Clause Clear
 Keywords: pytorch,cnn,convolutional-networksequivariant,isometries
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `escnn-1.0.7/README.md` & `escnn-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/__init__.py` & `escnn-1.0.8/escnn/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/__init__.py` & `escnn-1.0.8/escnn/group/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/_clebsh_gordan.py` & `escnn-1.0.8/escnn/group/_clebsh_gordan.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/_numerical.py` & `escnn-1.0.8/escnn/group/_numerical.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/directproduct.py` & `escnn-1.0.8/escnn/group/directproduct.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/doublegroup.py` & `escnn-1.0.8/escnn/group/doublegroup.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/group.py` & `escnn-1.0.8/escnn/group/group.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/__init__.py` & `escnn-1.0.8/escnn/group/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/_numerical_thomson.py` & `escnn-1.0.8/escnn/group/groups/_numerical_thomson.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/cyclicgroup.py` & `escnn-1.0.8/escnn/group/groups/cyclicgroup.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/dihedralgroup.py` & `escnn-1.0.8/escnn/group/groups/dihedralgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,14 +345,30 @@
             # parent_mapping = lambda e, ratio=ratio, axis=axis: self.element((e._element[0], e._element[1] * ratio + e._element[0] * axis))
             # child_mapping = lambda e, ratio=ratio, axis=axis, sg=sg: None if (e._element[1] - e._element[0] * axis) % ratio > 0 else sg.element((e._element[0], int((e._element[1] - e._element[0] * axis) / ratio)))
             parent_mapping = dm_to_dn(axis, self)
             child_mapping = dn_to_dm(axis, sg)
 
         return sg, parent_mapping, child_mapping
 
+    def grid(self, type: str, N: int) -> List[GroupElement]:
+        r"""
+            .. todo ::
+                Add docs
+
+        """
+
+        if type == 'rand':
+            return [self.sample() for _ in range(N)]
+        elif type == 'regular':
+            assert self.rotation_order % N == 0
+            r = self.rotation_order // N
+            return [self.element((0, i*r)) for i in range(N)] + [self.element((1, i*r)) for i in range(N)]
+        else:
+            raise ValueError(f'Grid type "{type}" not recognized!')
+
     def _combine_subgroups(self, sg_id1, sg_id2):
     
         sg_id1 = self._process_subgroup_id(sg_id1)
         sg1, inclusion, restriction = self.subgroup(sg_id1)
         sg_id2 = sg1._process_subgroup_id(sg_id2)
         
         if sg_id1[0] is None:
```

### Comparing `escnn-1.0.7/escnn/group/groups/factory.py` & `escnn-1.0.8/escnn/group/groups/factory.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/ico.py` & `escnn-1.0.8/escnn/group/groups/ico.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/o2group.py` & `escnn-1.0.8/escnn/group/groups/o2group.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/o3group.py` & `escnn-1.0.8/escnn/group/groups/o3group.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/octa.py` & `escnn-1.0.8/escnn/group/groups/octa.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/so2group.py` & `escnn-1.0.8/escnn/group/groups/so2group.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/so3_utils.py` & `escnn-1.0.8/escnn/group/groups/so3_utils.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/so3group.py` & `escnn-1.0.8/escnn/group/groups/so3group.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/groups/utils.py` & `escnn-1.0.8/escnn/group/groups/utils.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/homspace.py` & `escnn-1.0.8/escnn/group/homspace.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/irrep.py` & `escnn-1.0.8/escnn/group/irrep.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/representation.py` & `escnn-1.0.8/escnn/group/representation.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/group/utils.py` & `escnn-1.0.8/escnn/group/utils.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/gspaces/__init__.py` & `escnn-1.0.8/escnn/gspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/gspaces/gspace.py` & `escnn-1.0.8/escnn/gspaces/gspace.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/gspaces/r0.py` & `escnn-1.0.8/escnn/gspaces/r0.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/gspaces/r2.py` & `escnn-1.0.8/escnn/gspaces/r2.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,23 @@
 
 
 class GSpace2D(gspaces.GSpace):
     
     def __init__(self, sg_id: Tuple, maximum_frequency: int = 6):
         r"""
 
-        Describes reflectional and rotational symmetries of the plane :math:`\R^3`.
+        A ``GSpace`` tha describes the set (or subset) of reflectional and rotational symmetries of the 2D
+        Euclidean Space :math:`\R^2`.
+        The subset of symmetries is determined by the subgroup of :math:`\O2` that is specified by `sg_id`
+        (check the documentation of :class:`escnn.group.O2`).
+
+        Args:
+            sg_id (tuple): The ID of the subgroup within the fiber group :math:`\O2` that determines the reflectional and rotational symmetries to consider. For detailed documentation on the ID of each subgroup, refer to the documentation of :class:`escnn.group.O2`
+
+            maximum_frequency (int): Maximum frequency of the irreps to pre-instantiate, if the symmetry group (identified by `sg_id`) contains all continuous rotations.
 
         .. note ::
             A point :math:`\bold{v} \in \R^2` is parametrized using an :math:`(X, Y)` convention,
             i.e. :math:`\bold{v} = (x, y)^T`.
             The representation :attr:`escnn.gspaces.GSpace2D.basespace_action` also assumes this convention.
             
             However, when working with data on a pixel grid, the usual :math:`(-Y, X)` convention is used.
```

### Comparing `escnn-1.0.7/escnn/gspaces/r3.py` & `escnn-1.0.8/escnn/gspaces/r3.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,25 @@
 
 
 class GSpace3D(gspaces.GSpace):
     
     def __init__(self, sg_id: Tuple, maximum_frequency: int = 2):
         r"""
 
-        Describes reflectional and rotational symmetries of the plane :math:`\R^3`.
-        
+        A ``GSpace`` tha describes the set (or subset) of reflectional and rotational symmetries of the
+        3D Euclidean Space :math:`\R^3`.
+        The subset of symmetries is determined by the subgroup of :math:`\O3` that is specified by `sg_id`
+        (check the documentation of :class:`escnn.group.O3`).
+
+        Args:
+            sg_id (tuple): The ID of the subgroup within the fiber group :math:`\O3` that determines the reflectional and rotational symmetries to consider. For detailed documentation on the ID of each subgroup, refer to the documentation of :class:`escnn.group.O3`
+
+            maximum_frequency (int): Maximum frequency of the irreps to pre-instantiate, if the symmetry group (identified by `sg_id`) contains continuous rotations.
+
+
         .. note ::
             A point :math:`\bold{v} \in \R^3` is parametrized using an :math:`(X, Y, Z)` convention,
             i.e. :math:`\bold{v} = (x, y, z)^T`.
             The representation :attr:`escnn.gspaces.GSpace3D.basespace_action` also assumes this convention.
             
             However, when working with voxel data, the :math:`(-Z, -Y, X)` convention is used.
             That means that, in a 5-dimensional feature tensor of shape ``(B, C, D1, D2, D3)``, the last dimension
@@ -99,15 +108,15 @@
                          in_repr: Representation,
                          out_repr: Representation,
                          rings: List[float],
                          sigma: List[float],
                          **kwargs,
                          ) -> kernels.KernelBasis:
         r"""
-        Method that builds the analitical basis that spans the space of equivariant filters which
+        Method that builds the analytical basis that spans the space of equivariant filters which
         are intertwiners between the representations induced from the representation ``in_repr`` and ``out_repr``.
 
         `kwargs` can be used to specify `maximum_frequency`
         
         Args:
             in_repr (Representation): the input representation
             out_repr (Representation): the output representation
```

### Comparing `escnn-1.0.7/escnn/gspaces/utils.py` & `escnn-1.0.8/escnn/gspaces/utils.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/__init__.py` & `escnn-1.0.8/escnn/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/basis.py` & `escnn-1.0.8/escnn/kernels/basis.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/harmonic_polynomial_r3.py` & `escnn-1.0.8/escnn/kernels/harmonic_polynomial_r3.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/polar_basis.py` & `escnn-1.0.8/escnn/kernels/polar_basis.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/r2.py` & `escnn-1.0.8/escnn/kernels/r2.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/r3.py` & `escnn-1.0.8/escnn/kernels/r3.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/sparse_basis.py` & `escnn-1.0.8/escnn/kernels/sparse_basis.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/steerable_basis.py` & `escnn-1.0.8/escnn/kernels/steerable_basis.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/steerable_filters_basis.py` & `escnn-1.0.8/escnn/kernels/steerable_filters_basis.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/kernels/wignereckart_solver.py` & `escnn-1.0.8/escnn/kernels/wignereckart_solver.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/field_type.py` & `escnn-1.0.8/escnn/nn/field_type.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/geometric_tensor.py` & `escnn-1.0.8/escnn/nn/geometric_tensor.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/init.py` & `escnn-1.0.8/escnn/nn/init.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/__init__.py` & `escnn-1.0.8/escnn/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/__init__.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/basisexpansion_blocks.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/basisexpansion_blocks.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/basisexpansion_singleblock.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/basisexpansion_singleblock.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/basismanager.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/basismanager.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/basissampler_blocks.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/basissampler_blocks.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/basismanager/basissampler_singleblock.py` & `escnn-1.0.8/escnn/nn/modules/basismanager/basissampler_singleblock.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/batchnormalization/gnorm.py` & `escnn-1.0.8/escnn/nn/modules/batchnormalization/gnorm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/batchnormalization/iid.py` & `escnn-1.0.8/escnn/nn/modules/batchnormalization/iid.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/batchnormalization/induced_norm.py` & `escnn-1.0.8/escnn/nn/modules/batchnormalization/induced_norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/batchnormalization/inner.py` & `escnn-1.0.8/escnn/nn/modules/batchnormalization/inner.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/batchnormalization/norm.py` & `escnn-1.0.8/escnn/nn/modules/batchnormalization/norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/branching_module.py` & `escnn-1.0.8/escnn/nn/modules/branching_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r2_transposed_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r2_transposed_convolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
+
 
         .. warning ::
             
             Transposed convolution can produce artifacts which can harm the overall equivariance of the model.
             We suggest using :class:`~escnn.nn.R2Upsampling` combined with :class:`~escnn.nn.R2Conv` to perform
             upsampling.
```

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r2convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r2convolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,17 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
+
         During training, in each forward pass the module expands the basis of G-steerable kernels with learned weights
         before calling :func:`torch.nn.functional.conv2d`.
         When :meth:`~torch.nn.Module.eval()` is called, the filter is built with the current trained weights and stored
         for future reuse such that no overhead of expanding the kernel remains.
         
         .. warning ::
```

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r3_ico_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r3_ico_convolution.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r3_ico_transposed_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r3_ico_transposed_convolution.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r3_transposed_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r3_transposed_convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
+
         .. warning ::
             
             Transposed convolution can produce artifacts which can harm the overall equivariance of the model.
             We suggest using :class:`~escnn.nn.R2Upsampling` combined with :class:`~escnn.nn.R3Conv` to perform
             upsampling.
         
         .. seealso ::
```

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/r3convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/r3convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
 
         During training, in each forward pass the module expands the basis of G-steerable kernels with learned weights
         before calling :func:`torch.nn.functional.conv2d`.
         When :meth:`~torch.nn.Module.eval()` is called, the filter is built with the current trained weights and stored
         for future reuse such that no overhead of expanding the kernel remains.
 
         .. warning ::
```

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/rd_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/rd_convolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
+
         During training, in each forward pass the module expands the basis of G-steerable kernels with learned weights
         before performing the convolution.
         When :meth:`~torch.nn.Module.eval()` is called, the filter is built with the current trained weights and stored
         for future reuse such that no overhead of expanding the kernel remains.
         
         .. warning ::
```

### Comparing `escnn-1.0.7/escnn/nn/modules/conv/rd_transposed_convolution.py` & `escnn-1.0.8/escnn/nn/modules/conv/rd_transposed_convolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
             This class implements a *discretized* convolution operator over a discrete grid.
             This means that equivariance to continuous symmetries is *not* perfect.
             In practice, by using sufficiently band-limited filters, the equivariance error introduced by the
             discretization of the filters and the features is contained, but some design choices may have a negative
             effect on the overall equivariance of the architecture.
 
+            We provide some :doc:`practical notes <conv_notes>` on using this discretized
+            convolution module.
+
 
         .. warning ::
 
             Transposed convolution can produce artifacts which can harm the overall equivariance of the model.
             We suggest using :class:`~escnn.nn.R2Upsampling` combined with :class:`~escnn.nn.R2Conv` to perform
             upsampling.
```

### Comparing `escnn-1.0.7/escnn/nn/modules/disentangle_module.py` & `escnn-1.0.8/escnn/nn/modules/disentangle_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/dropout/field.py` & `escnn-1.0.8/escnn/nn/modules/dropout/field.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/dropout/pointwise.py` & `escnn-1.0.8/escnn/nn/modules/dropout/pointwise.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/equivariant_module.py` & `escnn-1.0.8/escnn/nn/modules/equivariant_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/harmonic_polynomial_r3.py` & `escnn-1.0.8/escnn/nn/modules/harmonic_polynomial_r3.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/identity_module.py` & `escnn-1.0.8/escnn/nn/modules/identity_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/invariantmaps/gpool.py` & `escnn-1.0.8/escnn/nn/modules/invariantmaps/gpool.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/invariantmaps/induced_norm.py` & `escnn-1.0.8/escnn/nn/modules/invariantmaps/induced_norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/invariantmaps/norm.py` & `escnn-1.0.8/escnn/nn/modules/invariantmaps/norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/linear.py` & `escnn-1.0.8/escnn/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/masking_module.py` & `escnn-1.0.8/escnn/nn/modules/masking_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/merge_module.py` & `escnn-1.0.8/escnn/nn/modules/merge_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/multiple_module.py` & `escnn-1.0.8/escnn/nn/modules/multiple_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/__init__.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/concatenated.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/concatenated.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/elu.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/elu.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/fourier.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/fourier.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/fourier_quotient.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/fourier_quotient.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/gated1.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/gated1.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/gated2.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/gated2.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/gated3.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/gated3.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/induced_gated1.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/induced_gated1.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/induced_norm.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/induced_norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/norm.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/norm.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/pointwise.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/pointwise.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/relu.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/relu.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/tensor.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/tensor.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/nonlinearities/vectorfield.py` & `escnn-1.0.8/escnn/nn/modules/nonlinearities/vectorfield.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pointconv/r2_point_convolution.py` & `escnn-1.0.8/escnn/nn/modules/pointconv/r2_point_convolution.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pointconv/r3_point_convolution.py` & `escnn-1.0.8/escnn/nn/modules/pointconv/r3_point_convolution.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pointconv/rd_point_convolution.py` & `escnn-1.0.8/escnn/nn/modules/pointconv/rd_point_convolution.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/__init__.py` & `escnn-1.0.8/escnn/nn/modules/pooling/__init__.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/norm_max.py` & `escnn-1.0.8/escnn/nn/modules/pooling/norm_max.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/pointwise_adaptive_avg.py` & `escnn-1.0.8/escnn/nn/modules/pooling/pointwise_adaptive_avg.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/pointwise_adaptive_max.py` & `escnn-1.0.8/escnn/nn/modules/pooling/pointwise_adaptive_max.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/pointwise_avg.py` & `escnn-1.0.8/escnn/nn/modules/pooling/pointwise_avg.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/pointwise_avg_3d.py` & `escnn-1.0.8/escnn/nn/modules/pooling/pointwise_avg_3d.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/pooling/pointwise_max.py` & `escnn-1.0.8/escnn/nn/modules/pooling/pointwise_max.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/rdupsampling.py` & `escnn-1.0.8/escnn/nn/modules/rdupsampling.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/reshuffle_module.py` & `escnn-1.0.8/escnn/nn/modules/reshuffle_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/restriction_module.py` & `escnn-1.0.8/escnn/nn/modules/restriction_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/sequential_module.py` & `escnn-1.0.8/escnn/nn/modules/sequential_module.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn/nn/modules/utils.py` & `escnn-1.0.8/escnn/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/escnn.egg-info/PKG-INFO` & `escnn-1.0.8/escnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: escnn
-Version: 1.0.7
+Version: 1.0.8
 Summary: E(n)-Equivariant CNNs Library for PyTorch
 Home-page: https://github.com/QUVA-Lab/escnn
-Download-URL: https://github.com/QUVA-Lab/escnn/archive/v1.0.7.tar.gz
+Download-URL: https://github.com/QUVA-Lab/escnn/archive/v1.0.8.tar.gz
 Author: Gabriele Cesa
 Author-email: cesa.gabriele@gmail.com
 License: BSD 3-Clause Clear
 Keywords: pytorch,cnn,convolutional-networksequivariant,isometries
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `escnn-1.0.7/escnn.egg-info/SOURCES.txt` & `escnn-1.0.8/escnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `escnn-1.0.7/setup.py` & `escnn-1.0.8/setup.py`

 * *Files identical despite different names*

