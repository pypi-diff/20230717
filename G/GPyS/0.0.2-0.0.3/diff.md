# Comparing `tmp/GPyS-0.0.2.tar.gz` & `tmp/GPyS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyS-0.0.2.tar", last modified: Tue Feb 14 00:44:08 2023, max compression
+gzip compressed data, was "GPyS-0.0.3.tar", last modified: Mon Jul 17 18:50:18 2023, max compression
```

## Comparing `GPyS-0.0.2.tar` & `GPyS-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 00:44:08.545103 GPyS-0.0.2/
--rw-rw-rw-   0        0        0    34727 2023-02-13 22:23:53.000000 GPyS-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1609 2023-02-14 00:44:08.545103 GPyS-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1076 2023-02-14 00:13:39.000000 GPyS-0.0.2/README.md
--rw-rw-rw-   0        0        0      627 2023-02-14 00:43:50.000000 GPyS-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-14 00:44:08.545103 GPyS-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-14 00:44:08.533061 GPyS-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-14 00:44:08.538072 GPyS-0.0.2/src/GPyS.egg-info/
--rw-rw-rw-   0        0        0     1609 2023-02-14 00:44:08.000000 GPyS-0.0.2/src/GPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-02-14 00:44:08.000000 GPyS-0.0.2/src/GPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 00:44:08.000000 GPyS-0.0.2/src/GPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-02-14 00:44:08.000000 GPyS-0.0.2/src/GPyS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-14 00:44:08.540134 GPyS-0.0.2/src/GPyS_prediction/
--rw-rw-rw-   0        0        0    16814 2023-02-13 22:53:36.000000 GPyS-0.0.2/src/GPyS_prediction/GPyS_prediction.py
--rw-rw-rw-   0        0        0       41 2023-02-13 22:28:18.000000 GPyS-0.0.2/src/GPyS_prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 00:44:08.543128 GPyS-0.0.2/src/GPyS_preprocessor/
--rw-rw-rw-   0        0        0     2052 2023-02-13 23:01:26.000000 GPyS-0.0.2/src/GPyS_preprocessor/GPyS_preprocessor.py
--rw-rw-rw-   0        0        0       45 2023-02-13 22:28:46.000000 GPyS-0.0.2/src/GPyS_preprocessor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-13 22:27:48.000000 GPyS-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.671534 GPyS-0.0.3/
+-rw-rw-rw-   0        0        0    34727 2023-07-17 03:05:27.000000 GPyS-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1782 2023-07-17 18:50:18.670534 GPyS-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2023-07-17 17:17:44.000000 GPyS-0.0.3/README.md
+-rw-rw-rw-   0        0        0      588 2023-07-17 18:49:58.000000 GPyS-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:50:18.671534 GPyS-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.655534 GPyS-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.660534 GPyS-0.0.3/src/GPyS.egg-info/
+-rw-rw-rw-   0        0        0     1782 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.663534 GPyS-0.0.3/src/GPyS_LOOCV_error/
+-rw-rw-rw-   0        0        0     9311 2023-07-17 17:57:19.000000 GPyS-0.0.3/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
+-rw-rw-rw-   0        0        0       35 2023-07-17 17:39:29.000000 GPyS-0.0.3/src/GPyS_LOOCV_error/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.666534 GPyS-0.0.3/src/GPyS_prediction/
+-rw-rw-rw-   0        0        0    16517 2023-07-17 17:57:59.000000 GPyS-0.0.3/src/GPyS_prediction/GPyS_prediction.py
+-rw-rw-rw-   0        0        0       41 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_prediction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.668534 GPyS-0.0.3/src/GPyS_preprocessor/
+-rw-rw-rw-   0        0        0     2084 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_preprocessor/GPyS_preprocessor.py
+-rw-rw-rw-   0        0        0       45 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_preprocessor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/__init__.py
```

### Comparing `GPyS-0.0.2/LICENSE` & `GPyS-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.2/PKG-INFO` & `GPyS-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.2
-Summary: Gaussian Process Subspace Regression Prediction, Eigen-Decomposition Version
+Version: 0.0.3
+Summary: Gaussian Process Subspace Prediction
 Author-email: Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
-Project-URL: Homepage, https://github.com/TaiwoAdebiyi23/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,22 +17,27 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- python3 -m pip install GPyS
+- pip install GPyS==0.0.3
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
   - The remaining functions merely returns preprocessing quantities of interests
 
+#### For GPS Hyperparameter training:
+- from GPyS_LOOCV_error import LOOCV
+- Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
+- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
   - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.2/README.md` & `GPyS-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- python3 -m pip install GPyS
+- pip install GPyS==0.0.3
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
   - The remaining functions merely returns preprocessing quantities of interests
 
+#### For GPS Hyperparameter training:
+- from GPyS_LOOCV_error import LOOCV
+- Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
+- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
   - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.2/src/GPyS.egg-info/PKG-INFO` & `GPyS-0.0.3/src/GPyS.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.2
-Summary: Gaussian Process Subspace Regression Prediction, Eigen-Decomposition Version
+Version: 0.0.3
+Summary: Gaussian Process Subspace Prediction
 Author-email: Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
-Project-URL: Homepage, https://github.com/TaiwoAdebiyi23/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,22 +17,27 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- python3 -m pip install GPyS
+- pip install GPyS==0.0.3
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
   - The remaining functions merely returns preprocessing quantities of interests
 
+#### For GPS Hyperparameter training:
+- from GPyS_LOOCV_error import LOOCV
+- Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
+- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
   - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.2/src/GPyS_prediction/GPyS_prediction.py` & `GPyS-0.0.3/src/GPyS_prediction/GPyS_prediction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 import numpy as np
 import scipy
 import scipy.linalg as la
-#from GPyS_typings import Float_1D_Array, Float_2D_Array_type
 
 from GPyS_preprocessor import Preprocessor
 
 
 class Prediction(object):
     """"
   GP Subspace Regression Prediction, Eigen-Decomposition Version
     """
 
     @staticmethod
     def predict(X, sample, target, length_scale, t=None):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
-        :param t: truncation size (optional)
+        :param t (int): truncation size (optional)
         :returns: GPS Prediction
         """
         Preprocessor.setup(X)
         X = np.array(X)
         sample = np.array(sample)
         target = np.array(target)
-        length_scale = np.array(length_scale)  # get_length_scale()
+        length_scale = np.array(length_scale)  
 
         XtX = Preprocessor.get_XX_cross_product()
         K = Prediction.construct_corr_matrix0(sample, length_scale)
         cv = Prediction.construct_corr_vector0(sample, target, length_scale)
         l, k = Prediction.__get_dimensions(K, XtX)
-        t = t  # or k
+        t = t  
         v, diag_v = Prediction.__compute_v_and_diag_vinv(K, cv)
-        # tr = None  # Would be updated in the program #check and delete
         khat, k_tilda = Prediction.__compute_khat_and_k_tilda(K, diag_v)
         XPX = Prediction.__compute_XPX(l, k, k_tilda, XtX)
-        # U = Prediction.__XPX_decomposition(XPX)
         eps2 = Prediction.__compute_noise_variance(v, cv)
-        # eps2_1 = Prediction.__compute_noise_variance2(v, cv)
         CPC = Prediction.__compute_CPC(X, XPX)
         d1_squared, v_circ = Prediction.__compute_EVD(t, CPC)
-        # GPS_Prediction_0 = {"Vcirc": v_circ, "sigma^2": d1_squared, "eps^2": eps2}
         return Prediction.__GPS_Prediction(X, d1_squared, v_circ, eps2)
 
     @staticmethod
     def construct_corr_matrix0(sample, length_scale):
         """
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: a correlation matrix K
         """
         sample = np.array(sample)
         length_scale = np.array(length_scale)
         X1, X2 = sample, sample
         beta = length_scale
 
         if len(beta) == 1:
             scale1 = np.identity(X1.shape[0]) * (1 / beta)
             scale2 = np.identity(X2.shape[0]) * (1 / beta)
             theta_scaled = scale1 @ X1
             theta_prime_scaled = scale2 @ X2
         else:
-            scale = np.diag(1 / beta)  # cross check the direct application of the non-isotropic scale
+            scale = np.diag(1 / beta)  
             theta_scaled = scale @ X1
             theta_prime_scaled = scale @ X2
         dist = scipy.spatial.distance_matrix(theta_scaled, theta_prime_scaled)
         return np.exp(-(dist ** 2) / 2)
 
     @staticmethod
     def __get_dimensions(K, XtX):
@@ -80,31 +75,31 @@
         l = K.shape[-1]
         k = XtX.shape[-1] // l
         return l, k
 
     @staticmethod
     def get_dimensions(X, sample, length_scale):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: length of sample points (l) and subspace dimension (k)
         """
         Preprocessor.setup(X)
         XtX = Preprocessor.get_XX_cross_product()
         K = Prediction.construct_corr_matrix0(sample, length_scale)
         l = K.shape[-1]
         k = XtX.shape[-1] // l
         return l, k
 
     @staticmethod
     def construct_corr_vector0(sample, target, length_scale):
         """
-        :param sample: vector of scalar parameters, or matrix of vector parameters
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
         :param target: New parameter
         :param length_scale: length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: a covariance vector cv
         """
         X1, X2 = np.array(sample), np.array(target)
         beta = np.array(length_scale)
@@ -134,17 +129,17 @@
         v = la.solve(K, cv)
         diag_v = np.diag(1 / v)
         return v, diag_v
 
     @staticmethod
     def compute_v_and_diag_vinv(sample, target, length_scale):
         """
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: New parameter
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): New parameter
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: v and inverse of diag_v
         """
         K = Prediction.construct_corr_matrix0(sample, length_scale)
         cv = Prediction.construct_corr_vector0(sample, target, length_scale)
         v = la.solve(K, cv)
         diag_v = np.diag(1 / v)
@@ -162,17 +157,17 @@
         tr = np.sum(abs(np.diag(k_tilda)))
         k_tilda += np.finfo('float').eps * np.eye(len(K)) * tr  # add nugget for numerical stability
         return khat, k_tilda
 
     @staticmethod
     def compute_khat_and_k_tilda(sample, target, length_scale):
         """
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: New parameter
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): New parameter
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: khat and k_tilda
         """
         K = Prediction.construct_corr_matrix0(sample, length_scale)
         _, diag_v = Prediction.compute_v_and_diag_vinv(sample, target, length_scale)
 
         khat = la.solve(K, diag_v)
@@ -196,18 +191,18 @@
         tr = np.sum(abs(np.diag(XPX)))
         XPX += np.finfo('float').eps * np.eye(l * k) * tr
         return XPX
 
     @staticmethod
     def compute_XPX(X, sample, target, length_scale):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: Block matrix structure
         """
         Preprocessor.setup(X)
         XtX = Preprocessor.get_XX_cross_product()
         l, k = Prediction.get_dimensions(X, sample, length_scale)
         _, k_tilda = Prediction.compute_khat_and_k_tilda(sample, target, length_scale)
@@ -228,18 +223,18 @@
         U = la.cholesky(XPX)
         # returns upper triangular
         return U
 
     @staticmethod
     def XPX_decomposition(X, sample, target, length_scale):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         returns: upper triangular Cholesky factor
         """
         XPX = Prediction.compute_XPX(X, sample, target, length_scale)
         U = la.cholesky(XPX)
         # returns upper triangular
         return U
@@ -253,17 +248,17 @@
         """
         eps2 = 1 - (cv.T @ v)
         return eps2
 
     @staticmethod
     def compute_noise_variance(sample, target, length_scale):
         """
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: noise variance
         """
         cv = Prediction.construct_corr_vector0(sample, target, length_scale)
         v, _ = Prediction.compute_v_and_diag_vinv(sample, target, length_scale)
         eps2 = 1 - (cv.T @ v)
         return eps2
@@ -278,18 +273,18 @@
         PC = la.solve(XPX, Preprocessor.get_Xt_V())
         CPC = Preprocessor.get_Vt_X() @ PC
         return CPC
 
     @staticmethod
     def compute_CPC(X, sample, target, length_scale):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
         :returns: matrix cross product of tideL
         """
         Preprocessor.setup(X)
         XPX = Prediction.compute_XPX(X, sample, target, length_scale)
         PC = la.solve(XPX, Preprocessor.get_Xt_V())
         CPC = Preprocessor.get_Vt_X() @ PC
@@ -307,20 +302,20 @@
         else:
             d1_squared, v_circ = scipy.linalg.eigh(CPC)
         return d1_squared, v_circ
 
     @staticmethod
     def compute_EVD(X, sample, target, length_scale, t=None):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
-        :param t: truncation size (optional)
+        :param t (int): truncation size (optional)
         :returns: truncated if t is provided, else returns full EVD
         """
         CPC = Prediction.compute_CPC(X, sample, target, length_scale)
         if t != None:
             d1_squared, v_circ = scipy.sparse.linalg.eigsh(CPC, t)
         else:
             d1_squared, v_circ = scipy.linalg.eigh(CPC)
@@ -338,20 +333,20 @@
         v = Preprocessor.get_V_D_Wt()[0]
         GPS_Prediction = [v @ v_circ, d1_squared, eps2]
         return GPS_Prediction
 
     @staticmethod
     def GPS_Prediction(X, sample, target, length_scale, t=None):
         """
-        :param X: Concatenated orthonormal bases
-        :param sample: vector of scalar parameters, or matrix of vector parameters
-        :param target: parameter point for prediction
-        :param length_scale: length-scale of correlation, isotropic (scaler)
+        :param X ([[float]]): Concatenated orthonormal bases
+        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
+        :param target ([[float]]): parameter point for prediction
+        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
                              or separable (vector), defaults to 1
-        :param t: truncation size (optional)
+        :param t (int): truncation size (optional)
         :returns: principal directions, principal variances, and noise variance
         """
         return Prediction.predict(
             X=X,
             sample=sample,
             target=target,
             length_scale=length_scale,
@@ -413,12 +408,7 @@
     # # Test compute_CPC()
     # CPC = Prediction.compute_CPC(X, sample, target, length_scale)
     # print("compute_CPC: \n", CPC)
 
     # # Test compute_EVD()
     d1_squared, v_circ = Prediction.compute_EVD(X, sample, target, length_scale, t=None)
     print("compute_EVD: \n", d1_squared, v_circ)
-
-# ---------------------------------------------------------------------------------
-# Clarifications for Sir John
-# why was he checking through other code before converting any function to static method?
-# I guess those private functions will be called in the init function whose input arguments have been previously defined?....
```

### Comparing `GPyS-0.0.2/src/GPyS_preprocessor/GPyS_preprocessor.py` & `GPyS-0.0.3/src/GPyS_preprocessor/GPyS_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     V, D, Wt = None, None, None
     Vt_X = None
     Xt_V = None
 
     @classmethod
     def setup(cls, X):
         """
-        :param X: Concatenated orthonormal bases
-        :returns: X and X-transposed cross product; SVD of X;
+        :param X ([[float]]): Concatenated orthonormal bases
+        :returns: X and X-transposed cross product; 
+                  SVD of X;
                   Cross product of svdX$D and svdX$Wt, and
                   Transposed Vt_X
         """
         Preprocessor.X = np.array(X)
         Preprocessor.XX_cross_product = Preprocessor.X.T @ Preprocessor.X
 
         U, s, Vh = la.svd(Preprocessor.X, full_matrices=False)
```

