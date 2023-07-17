# Comparing `tmp/nvidia-dali-nightly-cuda120-1.29.0.dev20230714.tar.gz` & `tmp/nvidia-dali-nightly-cuda120-1.29.0.dev20230717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda120-1.29.0.dev20230714.tar", last modified: Fri Jul 14 13:44:30 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda120-1.29.0.dev20230717.tar", last modified: Mon Jul 17 11:04:50 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda120-1.29.0.dev20230714.tar` & `nvidia-dali-nightly-cuda120-1.29.0.dev20230717.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-14 13:44:30.610370 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-14 13:44:30.610370 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-14 13:44:30.610370 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-14 13:44:30.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-14 13:44:30.610370 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230714/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-17 11:04:50.211624 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-17 11:04:50.211624 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-17 11:04:50.211624 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-17 11:04:50.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-17 11:04:50.211624 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda120-1.29.0.dev20230717/setup.py
```

### Comparing `nvidia-dali-nightly-cuda120-1.29.0.dev20230714/LICENSE.md` & `nvidia-dali-nightly-cuda120-1.29.0.dev20230717/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda120-1.29.0.dev20230714/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.29.0.dev20230717/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.29.0.dev20230714
+Version: 1.29.0.dev20230717
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.29.0.dev20230714/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.29.0.dev20230717/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.29.0.dev20230714
+Version: 1.29.0.dev20230717
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.29.0.dev20230714/setup.py` & `nvidia-dali-nightly-cuda120-1.29.0.dev20230717/setup.py`

 * *Files identical despite different names*

