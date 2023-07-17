# Comparing `tmp/pypetal-0.1.0.tar.gz` & `tmp/pypetal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypetal-0.1.0.tar", max compression
+gzip compressed data, was "pypetal-0.1.1.tar", max compression
```

## Comparing `pypetal-0.1.0.tar` & `pypetal-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2023-03-31 05:43:01.607979 pypetal-0.1.0/LICENSE
--rw-r--r--   0        0        0     2298 2023-04-10 08:17:02.241055 pypetal-0.1.0/README.md
--rw-r--r--   0        0        0     1953 2023-05-02 06:14:35.987104 pypetal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       82 2023-03-31 05:43:00.382963 pypetal-0.1.0/src/pypetal/__init__.py
--rw-r--r--   0        0        0      106 2023-03-31 05:43:00.384963 pypetal-0.1.0/src/pypetal/drw_rej/__init__.py
--rw-r--r--   0        0        0     5118 2023-03-31 07:05:50.038710 pypetal-0.1.0/src/pypetal/drw_rej/module.py
--rw-r--r--   0        0        0    33665 2023-03-31 07:05:50.050710 pypetal-0.1.0/src/pypetal/drw_rej/utils.py
--rw-r--r--   0        0        0      122 2023-03-31 05:43:00.388963 pypetal-0.1.0/src/pypetal/fromfile/__init__.py
--rw-r--r--   0        0        0     6588 2023-04-13 06:41:54.650619 pypetal-0.1.0/src/pypetal/fromfile/run_toml.py
--rw-r--r--   0        0        0     2163 2023-03-31 07:05:50.058710 pypetal-0.1.0/src/pypetal/fromfile/write_bash.py
--rw-r--r--   0        0        0    13347 2023-03-31 07:05:50.067710 pypetal-0.1.0/src/pypetal/pipeline.py
--rw-r--r--   0        0        0      152 2023-03-31 05:43:00.392963 pypetal-0.1.0/src/pypetal/pyccf/__init__.py
--rw-r--r--   0        0        0     3332 2023-03-31 07:05:50.071710 pypetal-0.1.0/src/pypetal/pyccf/module.py
--rw-r--r--   0        0        0     6645 2023-04-13 01:05:03.009185 pypetal-0.1.0/src/pypetal/pyccf/plotting.py
--rw-r--r--   0        0        0    23444 2023-03-31 07:05:49.368701 pypetal-0.1.0/src/pypetal/pyccf/utils.py
--rw-r--r--   0        0        0      152 2023-03-31 05:43:00.448964 pypetal-0.1.0/src/pypetal/pyroa/__init__.py
--rw-r--r--   0        0        0     4774 2023-04-12 03:43:31.809483 pypetal-0.1.0/src/pypetal/pyroa/module.py
--rw-r--r--   0        0        0    17263 2023-04-12 05:25:13.009116 pypetal-0.1.0/src/pypetal/pyroa/plotting.py
--rw-r--r--   0        0        0    18318 2023-04-10 02:29:44.711516 pypetal-0.1.0/src/pypetal/pyroa/utils.py
--rw-r--r--   0        0        0      155 2023-03-31 05:43:00.456964 pypetal-0.1.0/src/pypetal/pyzdcf/__init__.py
--rw-r--r--   0        0        0     5040 2023-03-31 07:05:50.106711 pypetal-0.1.0/src/pypetal/pyzdcf/module.py
--rw-r--r--   0        0        0     5093 2023-04-13 00:50:57.786100 pypetal-0.1.0/src/pypetal/pyzdcf/plotting.py
--rw-r--r--   0        0        0     5094 2023-03-31 07:05:49.394701 pypetal-0.1.0/src/pypetal/pyzdcf/utils.py
--rw-r--r--   0        0        0      206 2023-03-31 05:43:00.460964 pypetal-0.1.0/src/pypetal/utils/__init__.py
--rw-r--r--   0        0        0     6914 2023-04-13 03:58:51.058676 pypetal-0.1.0/src/pypetal/utils/defaults.py
--rw-r--r--   0        0        0     6761 2023-03-31 05:43:00.464964 pypetal-0.1.0/src/pypetal/utils/detrending.py
--rw-r--r--   0        0        0    27212 2023-04-12 06:45:53.799385 pypetal-0.1.0/src/pypetal/utils/load.py
--rw-r--r--   0        0        0    10760 2023-04-08 07:40:52.654549 pypetal-0.1.0/src/pypetal/utils/petalio.py
--rw-r--r--   0        0        0      164 2023-03-31 05:43:00.466964 pypetal-0.1.0/src/pypetal/weighting/__init__.py
--rw-r--r--   0        0        0    11526 2023-04-13 04:00:00.944591 pypetal-0.1.0/src/pypetal/weighting/module.py
--rw-r--r--   0        0        0    14846 2023-03-31 07:05:50.145711 pypetal-0.1.0/src/pypetal/weighting/plotting.py
--rw-r--r--   0        0        0    26916 2023-04-12 18:43:04.737434 pypetal-0.1.0/src/pypetal/weighting/utils.py
--rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 pypetal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-17 03:18:40.628736 pypetal-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3706 2023-07-17 03:18:40.628736 pypetal-0.1.1/README.md
+-rw-r--r--   0        0        0     1953 2023-07-17 03:33:28.763991 pypetal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/__init__.py
+-rw-r--r--   0        0        0      106 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/drw_rej/__init__.py
+-rw-r--r--   0        0        0     5138 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/drw_rej/module.py
+-rw-r--r--   0        0        0    33665 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/drw_rej/utils.py
+-rw-r--r--   0        0        0      122 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/fromfile/__init__.py
+-rw-r--r--   0        0        0     6588 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/fromfile/run_toml.py
+-rw-r--r--   0        0        0     2163 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/fromfile/write_bash.py
+-rw-r--r--   0        0        0    13347 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/pipeline.py
+-rw-r--r--   0        0        0      152 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/pyccf/__init__.py
+-rw-r--r--   0        0        0     3352 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/pyccf/module.py
+-rw-r--r--   0        0        0     6645 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/pyccf/plotting.py
+-rw-r--r--   0        0        0    23464 2023-07-17 03:18:43.954726 pypetal-0.1.1/src/pypetal/pyccf/utils.py
+-rw-r--r--   0        0        0      152 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyroa/__init__.py
+-rw-r--r--   0        0        0     4774 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyroa/module.py
+-rw-r--r--   0        0        0    17263 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyroa/plotting.py
+-rw-r--r--   0        0        0    18398 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyroa/utils.py
+-rw-r--r--   0        0        0      155 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyzdcf/__init__.py
+-rw-r--r--   0        0        0     5060 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyzdcf/module.py
+-rw-r--r--   0        0        0     5093 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyzdcf/plotting.py
+-rw-r--r--   0        0        0     5094 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/pyzdcf/utils.py
+-rw-r--r--   0        0        0      206 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/utils/__init__.py
+-rw-r--r--   0        0        0     6914 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/utils/defaults.py
+-rw-r--r--   0        0        0     6761 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/utils/detrending.py
+-rw-r--r--   0        0        0    27212 2023-07-17 03:18:43.955726 pypetal-0.1.1/src/pypetal/utils/load.py
+-rw-r--r--   0        0        0    10760 2023-07-17 03:18:43.956726 pypetal-0.1.1/src/pypetal/utils/petalio.py
+-rw-r--r--   0        0        0      164 2023-07-17 03:18:43.956726 pypetal-0.1.1/src/pypetal/weighting/__init__.py
+-rw-r--r--   0        0        0    11526 2023-07-17 03:18:43.956726 pypetal-0.1.1/src/pypetal/weighting/module.py
+-rw-r--r--   0        0        0    14846 2023-07-17 03:18:43.956726 pypetal-0.1.1/src/pypetal/weighting/plotting.py
+-rw-r--r--   0        0        0    26916 2023-07-17 03:18:43.956726 pypetal-0.1.1/src/pypetal/weighting/utils.py
+-rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 pypetal-0.1.1/PKG-INFO
```

### Comparing `pypetal-0.1.0/LICENSE` & `pypetal-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/pyproject.toml` & `pypetal-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypetal"
-version = "0.1.0"
+version = "0.1.1"
 description = "A pipeline for estimating AGN time lags"
 authors = ["Zstone19 <stone28@illinois.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Zstone19/pypetal"
 repository = "https://github.com/Zstone19/pypetal"
 documentation = "https://pypetal.readthedocs.io"
```

### Comparing `pypetal-0.1.0/src/pypetal/drw_rej/module.py` & `pypetal-0.1.1/src/pypetal/drw_rej/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 #For multiprocessing
 def mp_map(func, args, threads):
     n_inputs = len(args)
 
     if (threads > 1) & (n_inputs > 1):
-        pool = mp.Pool(threads)
+        pool = mp.get_context('fork').Pool(threads)
         res = pool.starmap(func, args)
 
         pool.close()
         pool.join()
 
     else:
         res = list(itertools.starmap(func, args))
```

### Comparing `pypetal-0.1.0/src/pypetal/drw_rej/utils.py` & `pypetal-0.1.1/src/pypetal/drw_rej/utils.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/fromfile/run_toml.py` & `pypetal-0.1.1/src/pypetal/fromfile/run_toml.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/fromfile/write_bash.py` & `pypetal-0.1.1/src/pypetal/fromfile/write_bash.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pipeline.py` & `pypetal-0.1.1/src/pypetal/pipeline.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pyccf/module.py` & `pypetal-0.1.1/src/pypetal/pyccf/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 #For multiprocessing
 def mp_map(func, args, threads):
     n_inputs = len(args)
 
     if (threads > 1) & (n_inputs > 1):
-        pool = mp.Pool(threads)
+        pool = mp.get_context('fork').Pool(threads)
         res = pool.starmap(func, args)
 
         pool.close()
         pool.join()
 
     else:
         res = list(itertools.starmap(func, args))
```

### Comparing `pypetal-0.1.0/src/pypetal/pyccf/plotting.py` & `pypetal-0.1.1/src/pypetal/pyccf/plotting.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pyccf/utils.py` & `pypetal-0.1.1/src/pypetal/pyccf/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import scipy.stats as sst
 
 
 #For multiprocessing
 def mp_map(func, arg, threads):
 
     if threads > 1:
-        pool = mp.Pool(threads)
+        pool = mp.get_context('fork').Pool(threads)
         res = pool.map(func, arg)
 
         pool.close()
         pool.join()
 
     else:
         res = list(map(func, arg))
```

### Comparing `pypetal-0.1.0/src/pypetal/pyroa/module.py` & `pypetal-0.1.1/src/pypetal/pyroa/module.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pyroa/plotting.py` & `pypetal-0.1.1/src/pypetal/pyroa/plotting.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pyroa/utils.py` & `pypetal-0.1.1/src/pypetal/pyroa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,24 +552,24 @@
             filters = [line_names[0], line_names[i+1]]
 
             args = (lc_dir, objname, filters, prior_arr[i,:,:],)
             kwargs = {'add_var':add_var[i], 'init_tau':[init_tau[i]], 'init_delta':init_delta, 'sig_level':sig_level,
                       'delay_dist':delay_dist[i], 'psi_types':[psi_types[i]], 'Nsamples':nchain, 'Nburnin':nburn}
 
             if verbose:
-                proc = mp.Process(target=PyROA.Fit, args=args, kwargs=kwargs)
+                proc = mp.get_context('fork').Process(target=PyROA.Fit, args=args, kwargs=kwargs)
 
                 proc.start()
                 while proc.is_alive():
                     proc.is_alive()
                 proc.terminate()
 
             else:
                 with suppress_stdout_stderr():
-                    proc = mp.Process(target=PyROA.Fit, args=args, kwargs=kwargs)
+                    proc = mp.get_context('fork').Process(target=PyROA.Fit, args=args, kwargs=kwargs)
 
                     proc.start()
                     while proc.is_alive():
                         proc.is_alive()
                     proc.terminate()
 
 
@@ -586,24 +586,24 @@
 
 
         args = (lc_dir, objname, line_names, prior_arr,)
         kwargs = {'add_var':add_var, 'init_tau':init_tau, 'init_delta':init_delta, 'sig_level':sig_level,
                   'delay_dist':delay_dist, 'psi_types':psi_types, 'Nsamples':nchain, 'Nburnin':nburn}
 
         if verbose:
-            proc = mp.Process(target=PyROA.Fit, args=args, kwargs=kwargs)
+            proc = mp.get_context('fork').Process(target=PyROA.Fit, args=args, kwargs=kwargs)
 
             proc.start()
             while proc.is_alive():
                 proc.is_alive()
             proc.terminate()
 
         else:
             with suppress_stdout_stderr():
-                proc = mp.Process(target=PyROA.Fit, args=args, kwargs=kwargs)
+                proc = mp.get_context('fork').Process(target=PyROA.Fit, args=args, kwargs=kwargs)
 
                 proc.start()
                 while proc.is_alive():
                     proc.is_alive()
                 proc.terminate()
 
         move_output_files(cwd, line_dir)
```

### Comparing `pypetal-0.1.0/src/pypetal/pyzdcf/module.py` & `pypetal-0.1.1/src/pypetal/pyzdcf/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #For multiprocessing
 def mp_map(func, args, threads):
     n_inputs = len(args)
 
     if (threads > 1) & (n_inputs > 1):
-        pool = mp.Pool(threads)
+        pool = mp.get_context('fork').Pool(threads)
         res = pool.starmap(func, args)
 
         pool.close()
         pool.join()
 
     else:
         res = list(itertools.starmap(func, args))
```

### Comparing `pypetal-0.1.0/src/pypetal/pyzdcf/plotting.py` & `pypetal-0.1.1/src/pypetal/pyzdcf/plotting.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/pyzdcf/utils.py` & `pypetal-0.1.1/src/pypetal/pyzdcf/utils.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/utils/defaults.py` & `pypetal-0.1.1/src/pypetal/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/utils/detrending.py` & `pypetal-0.1.1/src/pypetal/utils/detrending.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/utils/load.py` & `pypetal-0.1.1/src/pypetal/utils/load.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/utils/petalio.py` & `pypetal-0.1.1/src/pypetal/utils/petalio.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/weighting/module.py` & `pypetal-0.1.1/src/pypetal/weighting/module.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/weighting/plotting.py` & `pypetal-0.1.1/src/pypetal/weighting/plotting.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/src/pypetal/weighting/utils.py` & `pypetal-0.1.1/src/pypetal/weighting/utils.py`

 * *Files identical despite different names*

### Comparing `pypetal-0.1.0/PKG-INFO` & `pypetal-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypetal
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pipeline for estimating AGN time lags
 Home-page: https://github.com/Zstone19/pypetal
 License: MIT
 Author: Zstone19
 Author-email: stone28@illinois.edu
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 3 - Alpha
@@ -46,21 +46,30 @@
 
 [![Documentation Status](https://readthedocs.org/projects/pypetal/badge/?version=latest)](https://pypetal.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Workflow Status](https://img.shields.io/github/actions/workflow/status/Zstone19/pypetal/python-package.yml)](https://img.shields.io/github/actions/workflow/status/Zstone19/pypetal/python-package.yml)
 [![License](https://img.shields.io/github/license/Zstone19/pypetal)](https://img.shields.io/github/license/Zstone19/pypetal)
 [![codecov](https://codecov.io/gh/Zstone19/pypetal/branch/main/graph/badge.svg?token=00O40N9H05)](https://codecov.io/gh/Zstone19/pypetal)
 
+[![pypi-ver](https://img.shields.io/pypi/v/pypetal)](https://img.shields.io/pypi/v/pypetal)
+[![python-ver](https://img.shields.io/pypi/pyversions/pypetal)](https://img.shields.io/pypi/pyversions/pypetal)
+[![pypi-downloads](https://static.pepy.tech/badge/pypetal)](https://pepy.tech/project/pypetal)
+
+
+pyPETaL is a time-series data analysis pipeline for AGN reverberation mapping (RM) data. It combines multiple different popular softwares using for AGN RM analysis, including PyCCF, PyZDCF, JAVELIN, and PyROA. This pipeline also implements outlier rejection using Damped Random Walk Gaussian proces fitting, and detrending through the LinMix algorithm. pyPetal implements a weighting scheme (for all modules) in order to mitigate aliasing in peaks of time lag distributions between light curves.
+
+pyPetal is very flexible, with almost every argument for each module allowing user input. pyPetal is designed to work with any combination of modules being run, allowing it to scale from the simplest to the most complex of projects.
+
 
 
 ## Installation
 
 ### pyPetal
 
-pyPetal is available on PyPI and can be installed with pip: **(NOT IMPLEMENTED YET)**
+pyPetal is available on PyPI and can be installed with pip:
 ```
     pip install pypetal
 ```
 
 Or, if you want to install the latest development version:
 ```
     git clone https://github.com/Zstone19/pypetal.git
@@ -71,28 +80,40 @@
 
 PLIKE is an optional algorithm that is used in pyPetal. There is a script available in the main directory to install and compile PLIKE (assuming that `gfortran` is installed). To install PLIKE, run the following command:
 ```
     sh build_plike.sh
 ```
 
 
+pyPetal offers the option to detrend the input light curves via the [LinMix](https://github.com/jmeyers314/linmix.git) algorithm. This package is not offered in the base version of pyPetal, but can be installed with pip:
+```
+    pip install "linmix @ git+https://github.com/jmeyers314/linmix.git"
+```
+
+Or with ``poetry``:
+```
+    poetry install --with extra
+
+```
+
 
 ### pyPetal and JAVELIN
 
 The JAVELIN software used in pyPetal runs on Python 2, though the bulk of pyPetal software relies on Python >=3.8. To circumvent this issue, pyPetal has a JAVELIN "module" (``pypetal-jav``) that can be installed as a separate package and used in conjunction with pyPetal, in a Python 2 environment.
 
 
 External requirements (not installed by ``pip`` or ``setup.py``):
 ```
     A Fortran compiler (>F90)
 ```
 
 
 pyPetal-jav is available on PyPI and can be installed with pip:
 ```
+    pip install --no-deps pypetal-jav
     pip install pypetal-jav
 ```
 
 
 Or, if you want to install the latest development version:
 ```
     git clone https://github.com/Zstone19/pypetal-jav.git
```

