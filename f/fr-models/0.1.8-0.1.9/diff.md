# Comparing `tmp/fr_models-0.1.8.tar.gz` & `tmp/fr_models-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fr_models-0.1.8.tar", last modified: Tue Mar  7 20:10:12 2023, max compression
+gzip compressed data, was "fr_models-0.1.9.tar", last modified: Tue Mar  7 20:27:00 2023, max compression
```

## Comparing `fr_models-0.1.8.tar` & `fr_models-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.023760 fr_models-0.1.8/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2022-11-07 07:22:50.000000 fr_models-0.1.8/LICENSE
--rw-r--r--   0 hoyinchau   (501) staff       (20)       96 2023-03-07 20:10:12.023626 fr_models-0.1.8/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2397 2022-11-07 07:22:50.000000 fr_models-0.1.8/README.md
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.020028 fr_models-0.1.8/fr_models/
--rw-r--r--   0 hoyinchau   (501) staff       (20)      164 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/__init__.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.021932 fr_models-0.1.8/fr_models/_torch/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       82 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     4332 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/core.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1554 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/integrate.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     9488 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/linalg.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1085 2023-02-13 23:11:30.000000 fr_models-0.1.8/fr_models/_torch/nn.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      949 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/parametrize.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    11943 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/stats.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2304 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/_torch/utils.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7752 2023-01-01 17:03:19.000000 fr_models-0.1.8/fr_models/analytic_models.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3393 2023-03-07 18:14:27.000000 fr_models-0.1.8/fr_models/constraints.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      204 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/criteria.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      366 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/exceptions.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.022569 fr_models-0.1.8/fr_models/geom/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       19 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/geom/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2065 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/geom/curve.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3642 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/geom/manifold.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)       20 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/geom/plane.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     9681 2023-03-07 19:48:55.000000 fr_models-0.1.8/fr_models/gridtools.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     5334 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/interp.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     9411 2023-02-13 19:17:41.000000 fr_models-0.1.8/fr_models/kernels.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    18012 2023-03-07 19:58:07.000000 fr_models-0.1.8/fr_models/numerical_models.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    15763 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/optimize.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     4740 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/periodic.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      230 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/regularizers.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    14499 2023-03-07 19:53:25.000000 fr_models-0.1.8/fr_models/response_models.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1294 2022-11-07 07:22:50.000000 fr_models-0.1.8/fr_models/timeout.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     6162 2022-12-12 18:39:20.000000 fr_models-0.1.8/fr_models/viz.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.020808 fr_models-0.1.8/fr_models.egg-info/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       96 2023-03-07 20:10:11.000000 fr_models-0.1.8/fr_models.egg-info/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1048 2023-03-07 20:10:11.000000 fr_models-0.1.8/fr_models.egg-info/SOURCES.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-03-07 20:10:11.000000 fr_models-0.1.8/fr_models.egg-info/dependency_links.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       90 2023-03-07 20:10:11.000000 fr_models-0.1.8/fr_models.egg-info/requires.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       10 2023-03-07 20:10:11.000000 fr_models-0.1.8/fr_models.egg-info/top_level.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-03-07 20:10:12.023807 fr_models-0.1.8/setup.cfg
--rw-r--r--   0 hoyinchau   (501) staff       (20)      449 2023-03-07 20:09:50.000000 fr_models-0.1.8/setup.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:10:12.023458 fr_models-0.1.8/test/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2918 2022-11-07 07:22:50.000000 fr_models-0.1.8/test/test_interp.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     6687 2022-11-07 07:22:50.000000 fr_models-0.1.8/test/test_kernels.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2104 2023-03-07 18:51:50.000000 fr_models-0.1.8/test/test_num_model.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3346 2023-03-07 20:05:11.000000 fr_models-0.1.8/test/test_resp_model.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3424 2023-03-07 20:08:36.000000 fr_models-0.1.8/test/test_response.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     4123 2022-11-07 07:22:50.000000 fr_models-0.1.8/test/test_torch_core.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2772 2022-11-07 07:22:50.000000 fr_models-0.1.8/test/test_torch_linalg.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     8729 2022-11-07 07:22:50.000000 fr_models-0.1.8/test/test_torch_stats.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.696748 fr_models-0.1.9/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2022-11-07 07:22:50.000000 fr_models-0.1.9/LICENSE
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       96 2023-03-07 20:27:00.696597 fr_models-0.1.9/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2397 2022-11-07 07:22:50.000000 fr_models-0.1.9/README.md
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.693875 fr_models-0.1.9/fr_models/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      164 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/__init__.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.695173 fr_models-0.1.9/fr_models/_torch/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       82 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     4332 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/core.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1554 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/integrate.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     9488 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/linalg.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1085 2023-02-13 23:11:30.000000 fr_models-0.1.9/fr_models/_torch/nn.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      949 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/parametrize.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    11943 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/stats.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2304 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/_torch/utils.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7752 2023-01-01 17:03:19.000000 fr_models-0.1.9/fr_models/analytic_models.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3404 2023-03-07 20:26:29.000000 fr_models-0.1.9/fr_models/constraints.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      204 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/criteria.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      366 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/exceptions.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.695572 fr_models-0.1.9/fr_models/geom/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       19 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/geom/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2065 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/geom/curve.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3642 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/geom/manifold.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       20 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/geom/plane.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     9681 2023-03-07 19:48:55.000000 fr_models-0.1.9/fr_models/gridtools.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     5334 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/interp.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     9411 2023-02-13 19:17:41.000000 fr_models-0.1.9/fr_models/kernels.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    18012 2023-03-07 19:58:07.000000 fr_models-0.1.9/fr_models/numerical_models.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    15763 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/optimize.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     4740 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/periodic.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      230 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/regularizers.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    14499 2023-03-07 19:53:25.000000 fr_models-0.1.9/fr_models/response_models.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1294 2022-11-07 07:22:50.000000 fr_models-0.1.9/fr_models/timeout.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6162 2022-12-12 18:39:20.000000 fr_models-0.1.9/fr_models/viz.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.694382 fr_models-0.1.9/fr_models.egg-info/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       96 2023-03-07 20:27:00.000000 fr_models-0.1.9/fr_models.egg-info/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1048 2023-03-07 20:27:00.000000 fr_models-0.1.9/fr_models.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-03-07 20:27:00.000000 fr_models-0.1.9/fr_models.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       90 2023-03-07 20:27:00.000000 fr_models-0.1.9/fr_models.egg-info/requires.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       10 2023-03-07 20:27:00.000000 fr_models-0.1.9/fr_models.egg-info/top_level.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-03-07 20:27:00.696801 fr_models-0.1.9/setup.cfg
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      449 2023-03-07 20:26:52.000000 fr_models-0.1.9/setup.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-07 20:27:00.696364 fr_models-0.1.9/test/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2918 2022-11-07 07:22:50.000000 fr_models-0.1.9/test/test_interp.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6687 2022-11-07 07:22:50.000000 fr_models-0.1.9/test/test_kernels.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2104 2023-03-07 18:51:50.000000 fr_models-0.1.9/test/test_num_model.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3346 2023-03-07 20:05:11.000000 fr_models-0.1.9/test/test_resp_model.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3424 2023-03-07 20:08:36.000000 fr_models-0.1.9/test/test_response.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     4123 2022-11-07 07:22:50.000000 fr_models-0.1.9/test/test_torch_core.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2772 2022-11-07 07:22:50.000000 fr_models-0.1.9/test/test_torch_linalg.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     8729 2022-11-07 07:22:50.000000 fr_models-0.1.9/test/test_torch_stats.py
```

### Comparing `fr_models-0.1.8/LICENSE` & `fr_models-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/README.md` & `fr_models-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/core.py` & `fr_models-0.1.9/fr_models/_torch/core.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/integrate.py` & `fr_models-0.1.9/fr_models/_torch/integrate.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/linalg.py` & `fr_models-0.1.9/fr_models/_torch/linalg.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/nn.py` & `fr_models-0.1.9/fr_models/_torch/nn.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/parametrize.py` & `fr_models-0.1.9/fr_models/_torch/parametrize.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/stats.py` & `fr_models-0.1.9/fr_models/_torch/stats.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/_torch/utils.py` & `fr_models-0.1.9/fr_models/_torch/utils.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/analytic_models.py` & `fr_models-0.1.9/fr_models/analytic_models.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/constraints.py` & `fr_models-0.1.9/fr_models/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         
 #     def forward(self, r_model):
 #         return self.max_spectral_radius - r_model.a_model.spectral_radius(r_model.r_star, **self.kwargs)
 
 class StabilityCon(Constraint):
     def __init__(self, max_instability=0.99, **kwargs):
         super().__init__()
-        self.max_instability = 0.99
+        self.max_instability = max_instability
         self.kwargs = kwargs
         
     @property
     def type(self):
         return Types.INEQ
     
     def forward(self, r_model):
```

### Comparing `fr_models-0.1.8/fr_models/geom/curve.py` & `fr_models-0.1.9/fr_models/geom/curve.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/geom/manifold.py` & `fr_models-0.1.9/fr_models/geom/manifold.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/gridtools.py` & `fr_models-0.1.9/fr_models/gridtools.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/interp.py` & `fr_models-0.1.9/fr_models/interp.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/kernels.py` & `fr_models-0.1.9/fr_models/kernels.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/numerical_models.py` & `fr_models-0.1.9/fr_models/numerical_models.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/optimize.py` & `fr_models-0.1.9/fr_models/optimize.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/periodic.py` & `fr_models-0.1.9/fr_models/periodic.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/response_models.py` & `fr_models-0.1.9/fr_models/response_models.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/timeout.py` & `fr_models-0.1.9/fr_models/timeout.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models/viz.py` & `fr_models-0.1.9/fr_models/viz.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/fr_models.egg-info/SOURCES.txt` & `fr_models-0.1.9/fr_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_interp.py` & `fr_models-0.1.9/test/test_interp.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_kernels.py` & `fr_models-0.1.9/test/test_kernels.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_num_model.py` & `fr_models-0.1.9/test/test_num_model.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_resp_model.py` & `fr_models-0.1.9/test/test_resp_model.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_response.py` & `fr_models-0.1.9/test/test_response.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_torch_core.py` & `fr_models-0.1.9/test/test_torch_core.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_torch_linalg.py` & `fr_models-0.1.9/test/test_torch_linalg.py`

 * *Files identical despite different names*

### Comparing `fr_models-0.1.8/test/test_torch_stats.py` & `fr_models-0.1.9/test/test_torch_stats.py`

 * *Files identical despite different names*

