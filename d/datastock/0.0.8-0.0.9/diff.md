# Comparing `tmp/datastock-0.0.8.tar.gz` & `tmp/datastock-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastock-0.0.8.tar", last modified: Fri Apr  1 14:22:40 2022, max compression
+gzip compressed data, was "datastock-0.0.9.tar", last modified: Fri Apr  8 08:56:58 2022, max compression
```

## Comparing `datastock-0.0.8.tar` & `datastock-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:22:40.888500 datastock-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-01 14:22:14.000000 datastock-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-01 14:22:14.000000 datastock-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-04-01 14:22:40.888500 datastock-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-04-01 14:22:14.000000 datastock-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-04-01 14:22:14.000000 datastock-0.0.8/_updateversion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:22:40.888500 datastock-0.0.8/datastock/
--rw-r--r--   0 runner    (1001) docker     (121)    11099 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_DataCollection_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     4879 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class0.py
--rw-r--r--   0 runner    (1001) docker     (121)    21334 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class1.py
--rw-r--r--   0 runner    (1001) docker     (121)    44583 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class1_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    25801 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class1_compute.py
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class1_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)    44300 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class2_interactivity.py
--rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_class3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_direct_calls.py
--rw-r--r--   0 runner    (1001) docker     (121)    14083 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_generic_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    12097 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15155 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_BvsA_as_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    13053 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_BvsA_as_distribution_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    43566 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_as_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_correlations.py
--rw-r--r--   0 runner    (1001) docker     (121)    21729 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_plot_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-04-01 14:22:14.000000 datastock-0.0.8/datastock/_saveload.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-01 14:22:39.000000 datastock-0.0.8/datastock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:22:40.888500 datastock-0.0.8/datastock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-04-01 14:22:40.000000 datastock-0.0.8/datastock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-04-01 14:22:40.000000 datastock-0.0.8/datastock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 14:22:40.000000 datastock-0.0.8/datastock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-01 14:22:40.000000 datastock-0.0.8/datastock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-01 14:22:40.000000 datastock-0.0.8/datastock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-04-01 14:22:14.000000 datastock-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-01 14:22:40.888500 datastock-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-04-01 14:22:14.000000 datastock-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:58.909034 datastock-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-08 08:56:43.000000 datastock-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-08 08:56:43.000000 datastock-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8326 2022-04-08 08:56:58.909034 datastock-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7504 2022-04-08 08:56:43.000000 datastock-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-04-08 08:56:43.000000 datastock-0.0.9/_updateversion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:58.909034 datastock-0.0.9/datastock/
+-rw-r--r--   0 runner    (1001) docker     (121)     7143 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_DataCollection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4879 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class0.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21346 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49262 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class1_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24137 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class1_compute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class1_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44870 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14304 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class2_interactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_class3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_direct_calls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14089 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_generic_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12097 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15244 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_BvsA_as_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13002 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_BvsA_as_distribution_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43714 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_as_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21729 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_plot_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/_saveload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:58.909034 datastock-0.0.9/datastock/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:58.909034 datastock-0.0.9/datastock/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/tests/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-04-08 08:56:43.000000 datastock-0.0.9/datastock/tests/test_01_DataStock.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-08 08:56:57.000000 datastock-0.0.9/datastock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 08:56:58.909034 datastock-0.0.9/datastock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8326 2022-04-08 08:56:58.000000 datastock-0.0.9/datastock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-04-08 08:56:58.000000 datastock-0.0.9/datastock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 08:56:58.000000 datastock-0.0.9/datastock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-08 08:56:58.000000 datastock-0.0.9/datastock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-08 08:56:58.000000 datastock-0.0.9/datastock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-04-08 08:56:43.000000 datastock-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-08 08:56:58.909034 datastock-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-04-08 08:56:43.000000 datastock-0.0.9/setup.py
```

### Comparing `datastock-0.0.8/LICENSE` & `datastock-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/_updateversion.py` & `datastock-0.0.9/_updateversion.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_class0.py` & `datastock-0.0.9/datastock/_class0.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_class1.py` & `datastock-0.0.9/datastock/_class1.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,16 @@
         If log = 'raw', a dict of indices arrays is returned, showing the
         details for each criterion
 
         """
         which, dd = self.__check_which(which, return_dict=True)
         return _class1_check._select(
             dd=dd, dd_name=which,
-            log=log, returnas=returnas, **kwdargs,
+            log=log, returnas=returnas,
+            **kwdargs,
         )
 
     def _ind_tofrom_key(
         self,
         ind=None,
         key=None,
         returnas=int,
```

### Comparing `datastock-0.0.8/datastock/_class1_check.py` & `datastock-0.0.9/datastock/_class1_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,14 +672,28 @@
             )
             raise Exception(msg)
 
     # Check if valid ref candidate (monotonous = (True,))
     if c0_array:
         if data.dtype.type == np.str_:
             monotonous = tuple([False for ii in data.shape])
+        elif scpsp.issparse(data):
+            monot = np.all(np.isfinite(data.data))
+            data_temp = data.toarray()
+            monotonous = tuple([
+                bool(
+                    monot
+                    and (
+                        np.all(np.diff(data_temp, axis=aa) > 0.)
+                        or np.all(np.diff(data_temp, axis=aa) < 0.)
+                    )
+                )
+                for aa in range(data.ndim)
+            ])
+            del data_temp
         else:
             monot = np.all(np.isfinite(data))
             monotonous = tuple([
                 bool(
                     monot
                     and (
                         np.all(np.diff(data, axis=aa) > 0.)
@@ -1688,7 +1702,147 @@
         if returnas == bool:
             out[:] = True
         elif returnas == int:
             out = np.arange(0, len(lk))
         else:
             out = lk
     return out
+
+
+#############################################
+#############################################
+#       select
+#############################################
+
+
+def _select(dd=None, dd_name=None, log=None, returnas=None, **kwdargs):
+    """ Return the indices / keys of data matching criteria
+
+    The selection is done comparing the value of all provided parameters
+    The result is a boolean indices array, optionally with the keys list
+    It can include:
+        - log = 'all': only the data matching all criteria
+        - log = 'any': the data matching any criterion
+
+    If log = 'raw', a dict of indices arrays is returned, showing the
+    details for each criterion
+
+    """
+
+    # -----------
+    # check input
+
+    # log
+    log = _generic_check._check_var(
+        log,
+        'log',
+        types=str,
+        default='all',
+        allowed=['all', 'any', 'raw'],
+    )
+
+    # returnas
+    # 'raw' => return the full 2d array of boolean indices
+    returnas = _generic_check._check_var(
+        returnas,
+        'returnas',
+        default=bool if log == 'raw' else int,
+        allowed=[int, bool, str, 'key'],
+    )
+
+    kwdargs = {k0: v0 for k0, v0 in kwdargs.items() if v0 is not None}
+
+    # Get list of relevant criteria
+    lp = [kk for kk in list(dd.values())[0].keys() if kk != 'data']
+    lk = list(kwdargs.keys())
+    lk = _generic_check._check_var_iter(
+        lk,
+        'lk',
+        types_iter=str,
+        default=lp,
+        allowed=lp,
+    )
+
+    # --------------------
+    # Get raw bool indices
+
+    # Get list of accessible param
+    ltypes = (int, np.int_, float, np.float_)
+    lquant = [
+        kk for kk in kwdargs.keys()
+        if any([isinstance(dd[k0][kk], ltypes) for k0 in dd.keys()])
+    ]
+
+    # Prepare array of bool indices and populate
+    ind = np.zeros((len(kwdargs), len(dd)), dtype=bool)
+    for ii, kk in enumerate(kwdargs.keys()):
+        try:
+            par = _get_param(
+                dd=dd, dd_name=dd_name,
+                param=kk,
+                returnas=np.ndarray,
+            )[kk]
+            if kk in lquant:
+                # list => in interval
+                if isinstance(kwdargs[kk], list) and len(kwdargs[kk]) == 2:
+                    ind[ii, :] = (
+                        (kwdargs[kk][0] <= par) & (par <= kwdargs[kk][1])
+                    )
+
+                # tuple => out of interval
+                elif isinstance(kwdargs[kk], tuple) and len(kwdargs[kk]) == 2:
+                    ind[ii, :] = (
+                        (kwdargs[kk][0] > par) | (par > kwdargs[kk][1])
+                    )
+
+                # float / int => equal
+                else:
+                    ind[ii, :] = par == kwdargs[kk]
+            else:
+                ind[ii, :] = par == kwdargs[kk]
+        except Exception as err:
+            try:
+                ind[ii, :] = [
+                    dd[k0][kk] == kwdargs[kk] for k0 in dd.keys()
+                ]
+            except Exception as err:
+                msg = (
+                    "Could not determine whether:\n"
+                    + "\t- {}['{}'] == {}".format(
+                        dd_name, kk, kwdargs[kk],
+                    )
+                )
+                raise Exception(msg)
+
+    # -----------------
+    # Format output ind
+
+    # return raw 2d array of bool indices
+    if log == 'raw':
+        if returnas in [str, 'key']:
+            ind = {
+                kk: [k0 for jj, k0 in enumerate(dd.keys()) if ind[ii, jj]]
+                for ii, kk in enumerate(kwdargs.keys())
+            }
+        if returnas == int:
+            ind = {
+                kk: ind[ii, :].nonzero()[0]
+                for ii, kk in enumerate(kwdargs.keys())
+            }
+        else:
+            ind = {kk: ind[ii, :] for ii, kk in enumerate(kwdargs.keys())}
+
+    else:
+        # return all or any
+        if log == 'all':
+            ind = np.all(ind, axis=0)
+        else:
+            ind = np.any(ind, axis=0)
+
+        if returnas == int:
+            ind = ind.nonzero()[0]
+        elif returnas in [str, 'key']:
+            ind = np.array(
+                [k0 for jj, k0 in enumerate(dd.keys()) if ind[jj]],
+                dtype=str,
+            )
+    return ind
```

### Comparing `datastock-0.0.8/datastock/_class1_compute.py` & `datastock-0.0.9/datastock/_class1_compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -900,70 +900,7 @@
     else:
         out = _get_unique_ref_dind(
             dd=dd, group=group,
             lkey=[idq2dR],
             return_all=True,
         )
     return out
-
-
-#############################################
-#############################################
-#############################################
-#       1d fits
-#############################################
-#############################################
-
-
-# def fit_1d(data, x=None, axis=None, Type=None, func=None,
-           # dTypes=None, **kwdargs):
-
-    # lc = [Type is not None, func is not None]
-    # assert np.sum(lc) == 1
-
-    # if lc[0]:
-
-        # # Pre-defined models dict
-        # # ------------------------
-
-        # _DTYPES = {'staircase': _fit1d_staircase}
-
-        # # Use a pre-defined model
-        # # ------------------------
-
-        # if dTypes is None:
-            # dTypes = _DTYPES
-
-        # if Type not in dTypes.keys():
-            # msg = "Chosen Type not available:\n"
-            # msg += "    - provided: {}\n".format(Type)
-            # msg += "    - Available: {}".format(list(dTypes.keys()))
-            # raise Exception(msg)
-
-        # dout = dTypes[Type](data, x=x, axis=axis, **kwdargs)
-
-    # else:
-
-        # # Use a user-provided model
-        # # -------------------------
-
-        # dout = func(data, x=x, axis=axis, **kwdargs)
-
-    # return dout
-
-
-# # -------------------------------------------
-# #       1d fit models
-# # -------------------------------------------
-
-
-# def _fit1d_staircase(data, x=None, axis=None):
-    # """ Model data as a staircase (ramps + plateaux)
-
-    # Return a the fitted parameters as a dict:
-        # {'plateaux': {'plateaux': {'Dt': (2,N) np.ndarray
-                                   # '':
-                                    # }}
-        # - to be discussed.... ?
-
-    # """
-    # pass
```

### Comparing `datastock-0.0.8/datastock/_class1_interpolate.py` & `datastock-0.0.9/datastock/_class1_interpolate.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_class2.py` & `datastock-0.0.9/datastock/_class2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""
+Where the matplotlib interactivity is implemented
 
+"""
 
 import warnings
 
 
 import numpy as np
+import scipy.sparse as scpsparse
 import matplotlib.pyplot as plt
 
 
 from . import _generic_check
 from ._class1 import *
 from . import _class2_interactivity
 from . import _class1_compute
@@ -270,15 +274,25 @@
 
     @property
     def dax(self):
         return self.dobj.get('axes', {})
 
     @property
     def dinteractivity(self):
-        return self._dinteractivity
+        return self.dobj.get('interactivity', {})
+
+    # ------------------
+    # show basic commands
+    # ------------------
+
+    def show_commands(self, verb=None, returnas=None):
+        return _class2_interactivity.show_commands(
+            verb=verb,
+            returnas=returnas,
+        )
 
     # ------------------
     # Debug mode
     # ------------------
 
     def set_debug(self, debug=None):
         """ Set debug mode to True / False """
@@ -572,24 +586,23 @@
             # v0['handle'].manager.toolbar.release_zoom = self.mouserelease
             # v0['handle'].manager.toolbar.release_pan = self.mouserelease
 
             # make sure home button triggers background update
             # requires re-initializing because home is a Qt Action
             # only created by toolbar.addAction()
             v0['handle'].manager.toolbar.home = self.new_home
-            try:
-                # if _init_toolbar() implemented (matplotlib > )
+
+            # if _init_toolbar() implemented (matplotlib > )
+            if hasattr(v0['handle'].manager.toolbar, '_init_toolbar'):
                 v0['handle'].manager.toolbar._init_toolbar()
-            except NotImplementedError:
+            else:
                 v0['handle'].manager.toolbar.__init__(
                     v0['handle'],
                     v0['handle'].parent(),
                 )
-            except Exception as err:
-                raise err
 
             self._dobj['canvas'][k0]['cid'] = {
                 'keyp': keyp,
                 'keyr': keyr,
                 'butp': butp,
                 'res': res,
                 'butr': butr,
@@ -837,21 +850,23 @@
                 ddata=self._ddata,
                 k0=k0,
             )
 
         # --- Redraw all objects (due to background restore) --- 25 ms
         for k0, v0 in self._dobj['mobile'].items():
             v0['handle'].set_visible(v0['visible'])
-            try:
-                self._dobj['axes'][v0['axes']]['handle'].draw_artist(v0['handle'])
-            except Exception:
-                print(0, k0)        # DB
-                print(1, v0['axes'])    # DB
-                print(2, self._dobj['axes'][v0['axes']]['handle'])  # DB
-                print(3, v0['handle'])  # DB
+            # try:
+            self._dobj['axes'][v0['axes']]['handle'].draw_artist(v0['handle'])
+            # except Exception as err:
+                # print(0, k0)        # DB
+                # print(1, v0['axes'])    # DB
+                # print(2, self._dobj['axes'][v0['axes']]['handle'])  # DB
+                # print(3, v0['handle'])  # DB
+                # print(err)
+                # print()
 
         # ---- blit axes ------ 5 ms
         for aa in lax:
             self._dobj['canvas'][
                 self._dobj['axes'][aa]['canvas']
             ]['handle'].blit(self._dobj['axes'][aa]['handle'].bbox)
 
@@ -945,14 +960,19 @@
         # update ref indices
         if None not in [cur_refx, cur_refy] and cur_refx == cur_refy:
 
             cdx = self._ddata[cur_datax]['data']
             cdy = self._ddata[cur_datay]['data']
             dx = np.diff(ax.get_xlim())
             dy = np.diff(ax.get_ylim())
+
+            if scpsparse.issparse(cdx) or scpsparse.issparse(cdy):
+                msg = "No handling of pts selection for sparse data yet!"
+                raise Exception(msg)
+
             dist = ((cdx - event.xdata)/dx)**2 + ((cdy - event.ydata)/dy)**2
             if dist.ndim == 1:
                 ix = np.nanargmin(dist)
             elif dist.ndim == 2:
                 axis = self._ddata[cur_datax]['ref'].index(cur_refx)
                 ix = np.nanargmin(np.nanmin(dist, axis=1-axis))
             else:
```

### Comparing `datastock-0.0.8/datastock/_class2_interactivity.py` & `datastock-0.0.9/datastock/_class2_interactivity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 
 import numpy as np
+import scipy.sparse as scpsparse
+
+
+from . import _generic_check
+from . import _generic_utils
 
 
 _INCREMENTS = [1, 10]
 _DKEYS = {
     'control': {'val': False, 'action': 'generic'},
     'ctrl': {'val': False, 'action': 'generic'},
     'shift': {'val': False, 'action': 'generic'},
@@ -12,14 +17,84 @@
     'left': {'val': False, 'action': 'move'},
     'right': {'val': False, 'action': 'move'},
     'up': {'val': False, 'action': 'move'},
     'down': {'val': False, 'action': 'move'},
 }
 
 
+_DCOMMANDS = {
+    'shift + left clic': 'add a slice at selected location',
+    'left clic': 'move currently selected slice to selected location',
+    'ctrl + left clic': 'remove all visible slices',
+    '0, 1, 2...': 'select slice number 0, 1, 2...',
+    'f1, f2, f3...': 'select group of slice number 1, 2, 3...',
+    'left/right/up/down arrows': 'increment current slice index by 1',
+    'alt + left/right/up/down arrows': 'increment current slice index by 10',
+}
+
+
+# #############################################################################
+# #############################################################################
+#            show commands
+# #############################################################################
+
+
+def show_commands(
+    verb=None,
+    returnas=None,
+):
+
+    # ------------
+    # check inputs
+
+    verb = _generic_check._check_var(
+        verb, 'verb',
+        default=True,
+        types=bool,
+    )
+
+    returnas = _generic_check._check_var(
+        returnas, 'returnas',
+        default=False,
+        allowed=[False, str, dict],
+    )
+
+    # ------------
+    # get dcommands
+
+    dcom = dict(_DCOMMANDS)
+
+    # --------------
+    # col and ar
+
+    lcol = [['command', 'description']]
+    lar = [[
+        [
+            k0,
+            v0,
+        ]
+        for k0, v0 in dcom.items()
+    ]]
+
+    # -------
+    # return
+
+    out = _generic_utils.pretty_print(
+        headers=lcol,
+        content=lar,
+        verb=verb,
+        returnas=False if returnas is dict else returnas,
+    )
+    if returnas is dict:
+        return dcom
+    else:
+        return out
+
+
+
 # #############################################################################
 # #############################################################################
 #            setup interactivity
 # #############################################################################
 
 
 def _setup_dgroup(
@@ -379,14 +454,25 @@
         c0 = (
             dmobile[k0]['data'][0] == 'index'
             or ddata[dmobile[k0]['data'][0]]['data'].dtype.type == np.str_
         )
         if c0:
             dmobile[k0]['func_set_data'][0](*iref)
 
+        elif scpsparse.issparse(ddata[dmobile[k0]['data'][0]]['data']):
+            if ddata[dmobile[k0]['data'][0]]['data'].ndim <= 2:
+                dmobile[k0]['func_set_data'][0](
+                    ddata[dmobile[k0]['data'][0]]['data'][
+                        dmobile[k0]['func_slice'][0](*iref)
+                    ].data
+                )
+            else:
+                msg = "Sparse data of dim > 2: not handled yet"
+                raise Exception(msg)
+
         else:
             dmobile[k0]['func_set_data'][0](
                 ddata[dmobile[k0]['data'][0]]['data'][
                     dmobile[k0]['func_slice'][0](*iref)
                 ]
             )
 
@@ -394,13 +480,25 @@
         for ii in range(nocc):
             c0 = (
                 dmobile[k0]['data'][0] == 'index'
                 or ddata[dmobile[k0]['data'][0]]['data'].dtype.type == np.str_
             )
             if c0:
                 dmobile[k0]['func_set_data'][ii](iref[ii])
+
+            elif scpsparse.issparse(ddata[dmobile[k0]['data'][ii]]['data']):
+                if ddata[dmobile[k0]['data'][ii]]['data'].ndim <= 2:
+                    dmobile[k0]['func_set_data'][ii](
+                        ddata[dmobile[k0]['data'][ii]]['data'][
+                            dmobile[k0]['func_slice'][ii](iref[ii])
+                        ].data
+                    )
+                else:
+                    msg = "Sparse data of dim > 2: not handled yet"
+                    raise Exception(msg)
+
             else:
                 dmobile[k0]['func_set_data'][ii](
                     ddata[dmobile[k0]['data'][ii]]['data'][
                         dmobile[k0]['func_slice'][ii](iref[ii])
                     ]
                 )
```

### Comparing `datastock-0.0.8/datastock/_class3.py` & `datastock-0.0.9/datastock/_class3.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_direct_calls.py` & `datastock-0.0.9/datastock/_direct_calls.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_generic_check.py` & `datastock-0.0.9/datastock/_generic_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     if isinstance(keys, str):
         keys = [keys]
     keys = _check_var_iter(
         keys, 'keys',
         default=None,
         types=list,
         types_iter=str,
-        allowed=coll.ddata.keys(),
+        allowed=list(coll.ddata.keys()),
     )
 
     # inplace
     inplace = _check_var(
         inplace, 'inplace',
         types=bool,
         default=False,
```

### Comparing `datastock-0.0.8/datastock/_generic_utils.py` & `datastock-0.0.9/datastock/_generic_utils.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_plot_BvsA_as_distribution.py` & `datastock-0.0.9/datastock/_plot_BvsA_as_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Built-in
 # import itertools as itt
 # import warnings
 
 
 # Common
 import numpy as np
+import scipy.sparse as scpsparse
 import scipy.stats as scpstats
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 
 
 # library-specific
 from . import _generic_check
@@ -465,14 +466,16 @@
         coll2.add_axes(key=kax, harmonize=harmonize, **dax[kax])
 
     # connect
     if connect is True:
         coll2.setup_interactivity(kinter='inter0', dgroup=dgroup, dinc=dinc)
         coll2.disconnect_old()
         coll2.connect()
+
+        coll2.show_commands()
         return coll2
     else:
         return coll2, dgroup
 
 
 # #############################################################################
 # #############################################################################
@@ -500,15 +503,18 @@
     Agridplot = 0.5*(Agrid[1:] + Agrid[:-1])
     Agridplot = np.tile(Agridplot, (nAbin-1, 1))
     Bgrid = np.linspace(Bmin, Bmax, nBbin)
     Bgridplot = 0.5*(Bgrid[1:] + Bgrid[:-1])
     Bgridplot = np.tile(Bgridplot, (nBbin-1, 1))
     extent = (Amin, Amax, Bmin, Bmax)
 
+    # iok
     iok = np.isfinite(dataA) & np.isfinite(dataB)
+
+    # databin
     databin = scpstats.binned_statistic_2d(
         dataA[iok],
         dataB[iok],
         np.ones((iok.sum(),), dtype=int),
         statistic='sum',
         bins=(Agrid, Bgrid),
     )[0]
```

### Comparing `datastock-0.0.8/datastock/_plot_BvsA_as_distribution_check.py` & `datastock-0.0.9/datastock/_plot_BvsA_as_distribution_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 
 import numpy as np
+import scipy.sparse as scpsparse
 import matplotlib.colors as mcolors
 
 
 from . import _generic_check
 
 
 _CONNECT = True
@@ -323,21 +324,21 @@
             cmap=color_map,
             vmin=color_map_vmin,
             vmax=color_map_vmax,
         )
 
     # Amin, Amax, Bmin, Bmax
     if Amin is None:
-        Amin = np.nanmin(coll2._ddata[keyA]['data'])
+        Amin = np.nanmin(dataA)
     if Amax is None:
-        Amax = np.nanmax(coll2._ddata[keyA]['data'])
+        Amax = np.nanmax(dataA)
     if Bmin is None:
-        Bmin = np.nanmin(coll2._ddata[keyB]['data'])
+        Bmin = np.nanmin(dataB)
     if Bmax is None:
-        Bmax = np.nanmax(coll2._ddata[keyB]['data'])
+        Bmax = np.nanmax(dataB)
 
     # distribution binning
     if nAbin is None:
         nAbin = 100
     if nBbin is None:
         nBbin = nAbin
```

### Comparing `datastock-0.0.8/datastock/_plot_as_array.py` & `datastock-0.0.9/datastock/_plot_as_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     # ------------
     #  check inputs
 
     # check key, inplace flag and extract sub-collection
     key, inplace, coll2 = _generic_check._check_inplace(
         coll=coll,
-        keys=[key],
+        keys=None if key is None else [key],
         inplace=inplace,
     )
     key = key[0]
     ndim = coll2._ddata[key]['data'].ndim
 
     # --------------
     # check input
@@ -243,14 +243,16 @@
         coll2.add_axes(key=kax, harmonize=harmonize, **dax[kax])
 
     # connect
     if connect is True:
         coll2.setup_interactivity(kinter='inter0', dgroup=dgroup, dinc=dinc)
         coll2.disconnect_old()
         coll2.connect()
+
+        coll2.show_commands()
         return coll2
     else:
         return coll2, dgroup
 
 # #############################################################################
 # #############################################################################
 #                       check
@@ -424,15 +426,18 @@
             cmap = 'seismic'
         else:
             cmap = 'viridis'
 
     # vmin, vmax
     if vmin is None:
         if diverging:
-            vmin = -max(abs(nanmin), nanmax)
+            if isinstance(nanmin, np.bool_):
+                vmin = 0
+            else:
+                vmin = -max(abs(nanmin), nanmax)
         else:
             vmin = nanmin
         if vmax is None:
             if diverging:
                 vmax = max(abs(nanmin), nanmax)
             else:
                 vmax = nanmax
```

### Comparing `datastock-0.0.8/datastock/_plot_correlations.py` & `datastock-0.0.9/datastock/_plot_correlations.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_plot_misc.py` & `datastock-0.0.9/datastock/_plot_misc.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_plot_text.py` & `datastock-0.0.9/datastock/_plot_text.py`

 * *Files identical despite different names*

### Comparing `datastock-0.0.8/datastock/_saveload.py` & `datastock-0.0.9/datastock/_saveload.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,16 +176,16 @@
             raise Exception(msg)
 
     dout = _generic_utils.reshape_dict(dout, sep=sep)
 
     # -----------
     # Instanciate
 
-    from ._DataCollection_class import DataCollection
+    from ._class import DataStock
 
-    obj = DataCollection.from_dict(dout)
+    obj = DataStock.from_dict(dout)
 
     if verb:
         msg = f"Loaded from\n\t{pfe}"
         print(msg)
 
     return obj
```

### Comparing `datastock-0.0.8/datastock.egg-info/SOURCES.txt` & `datastock-0.0.9/datastock.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,8 +27,11 @@
 datastock/_plot_text.py
 datastock/_saveload.py
 datastock/version.py
 datastock.egg-info/PKG-INFO
 datastock.egg-info/SOURCES.txt
 datastock.egg-info/dependency_links.txt
 datastock.egg-info/requires.txt
-datastock.egg-info/top_level.txt
+datastock.egg-info/top_level.txt
+datastock/tests/__init__.py
+datastock/tests/test_01_DataStock.py
+datastock/tests/output/__init__.py
```

### Comparing `datastock-0.0.8/setup.py` & `datastock-0.0.9/setup.py`

 * *Files identical despite different names*

