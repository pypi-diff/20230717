# Comparing `tmp/pysid-0.1.0.tar.gz` & `tmp/pysid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysid-0.1.0.tar", last modified: Mon Mar 21 21:57:17 2022, max compression
+gzip compressed data, was "dist/pysid-0.1.1.tar", last modified: Mon Jul 17 20:18:48 2023, max compression
```

## Comparing `pysid-0.1.0.tar` & `pysid-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     1074 2021-12-31 18:13:43.000000 pysid-0.1.0/LICENSE
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      965 2022-03-21 21:57:17.878758 pysid-0.1.0/PKG-INFO
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      487 2021-12-31 18:13:43.000000 pysid-0.1.0/README.md
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/pysid/
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      379 2021-12-31 18:13:43.000000 pysid-0.1.0/pysid/__init__.py
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/pysid/correlation/
--rw-r--r--   0 edumapu   (1000) edumapu   (1000)       87 2021-10-13 13:46:58.000000 pysid-0.1.0/pysid/correlation/__init__.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6008 2021-10-14 12:42:23.000000 pysid-0.1.0/pysid/correlation/autocorr.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6442 2021-10-14 12:42:23.000000 pysid-0.1.0/pysid/correlation/croscorr.py
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/pysid/identification/
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      174 2021-12-31 18:13:43.000000 pysid-0.1.0/pysid/identification/__init__.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     5247 2021-10-14 12:42:23.000000 pysid-0.1.0/pysid/identification/accr.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2979 2022-03-21 21:50:53.000000 pysid-0.1.0/pysid/identification/comcrit.py
--rw-r--r--   0 edumapu   (1000) edumapu   (1000)     2665 2021-10-13 13:46:58.000000 pysid-0.1.0/pysid/identification/ivmethod.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6016 2022-03-21 21:50:53.000000 pysid-0.1.0/pysid/identification/models.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)    49501 2022-03-21 21:50:53.000000 pysid-0.1.0/pysid/identification/pemethod.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     3459 2022-02-01 22:02:15.000000 pysid-0.1.0/pysid/identification/solvers.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     5503 2022-02-01 22:00:09.000000 pysid-0.1.0/pysid/identification/tseries.py
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/pysid/io/
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       86 2022-03-20 21:50:54.000000 pysid-0.1.0/pysid/io/__init__.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2900 2022-02-01 20:27:21.000000 pysid-0.1.0/pysid/io/check.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2979 2022-03-20 13:15:53.000000 pysid-0.1.0/pysid/io/csv_data.py
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     5287 2022-03-20 13:15:53.000000 pysid-0.1.0/pysid/io/print.py
-drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2022-03-21 21:57:17.878758 pysid-0.1.0/pysid.egg-info/
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      965 2022-03-21 21:57:17.000000 pysid-0.1.0/pysid.egg-info/PKG-INFO
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      611 2022-03-21 21:57:17.000000 pysid-0.1.0/pysid.egg-info/SOURCES.txt
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)        1 2022-03-21 21:57:17.000000 pysid-0.1.0/pysid.egg-info/dependency_links.txt
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       23 2022-03-21 21:57:17.000000 pysid-0.1.0/pysid.egg-info/requires.txt
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)        6 2022-03-21 21:57:17.000000 pysid-0.1.0/pysid.egg-info/top_level.txt
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       38 2022-03-21 21:57:17.878758 pysid-0.1.0/setup.cfg
--rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      797 2022-03-21 21:57:09.000000 pysid-0.1.0/setup.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:48.092147 pysid-0.1.1/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     1074 2021-12-31 18:13:43.000000 pysid-0.1.1/LICENSE
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      965 2023-07-17 20:18:48.092147 pysid-0.1.1/PKG-INFO
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      487 2021-12-31 18:13:43.000000 pysid-0.1.1/README.md
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:47.900147 pysid-0.1.1/pysid/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      378 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/__init__.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:47.944147 pysid-0.1.1/pysid/correlation/
+-rw-r--r--   0 edumapu   (1000) edumapu   (1000)       87 2021-10-13 13:46:58.000000 pysid-0.1.1/pysid/correlation/__init__.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6008 2021-10-14 12:42:23.000000 pysid-0.1.1/pysid/correlation/autocorr.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6442 2021-10-14 12:42:23.000000 pysid-0.1.1/pysid/correlation/croscorr.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:48.020147 pysid-0.1.1/pysid/identification/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      199 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/__init__.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     5247 2021-10-14 12:42:23.000000 pysid-0.1.1/pysid/identification/accr.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2979 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/comcrit.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2655 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/ivmethod.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     6266 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/models.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)    58425 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/pemethod.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     8035 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/recursive.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     3767 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/solvers.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     5493 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/identification/tseries.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:48.060147 pysid-0.1.1/pysid/io/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       86 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/io/__init__.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     4222 2023-07-10 22:34:24.000000 pysid-0.1.1/pysid/io/check.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     2983 2023-07-10 22:35:36.000000 pysid-0.1.1/pysid/io/csv_data.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)     7059 2023-07-10 22:38:49.000000 pysid-0.1.1/pysid/io/print.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:48.072147 pysid-0.1.1/pysid/tests/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)        0 2023-04-04 23:49:32.000000 pysid-0.1.1/pysid/tests/__init__.py
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      506 2023-04-05 00:15:34.000000 pysid-0.1.1/pysid/tests/pem tests.py
+drwxrwxr-x   0 edumapu   (1000) edumapu   (1000)        0 2023-07-17 20:18:47.912147 pysid-0.1.1/pysid.egg-info/
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      965 2023-07-17 20:18:43.000000 pysid-0.1.1/pysid.egg-info/PKG-INFO
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      694 2023-07-17 20:18:44.000000 pysid-0.1.1/pysid.egg-info/SOURCES.txt
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)        1 2023-07-17 20:18:43.000000 pysid-0.1.1/pysid.egg-info/dependency_links.txt
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       23 2023-07-17 20:18:44.000000 pysid-0.1.1/pysid.egg-info/requires.txt
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)        6 2023-07-17 20:18:44.000000 pysid-0.1.1/pysid.egg-info/top_level.txt
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)       38 2023-07-17 20:18:48.092147 pysid-0.1.1/setup.cfg
+-rw-rw-r--   0 edumapu   (1000) edumapu   (1000)      797 2023-07-17 20:16:44.000000 pysid-0.1.1/setup.py
```

### Comparing `pysid-0.1.0/LICENSE` & `pysid-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysid-0.1.0/PKG-INFO` & `pysid-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysid
-Version: 0.1.0
+Version: 0.1.1
 Summary: System Identification tools for python
 Home-page: https://github.com/edumapurunga/pysid
 Author: Eduardo Mapurunga
 Author-email: edumapurunga@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysid-0.1.0/pysid/correlation/autocorr.py` & `pysid-0.1.1/pysid/correlation/autocorr.py`

 * *Files identical despite different names*

### Comparing `pysid-0.1.0/pysid/correlation/croscorr.py` & `pysid-0.1.1/pysid/correlation/croscorr.py`

 * *Files identical despite different names*

### Comparing `pysid-0.1.0/pysid/identification/accr.py` & `pysid-0.1.1/pysid/identification/accr.py`

 * *Files identical despite different names*

### Comparing `pysid-0.1.0/pysid/identification/comcrit.py` & `pysid-0.1.1/pysid/identification/comcrit.py`

 * *Files identical despite different names*

### Comparing `pysid-0.1.0/pysid/identification/ivmethod.py` & `pysid-0.1.1/pysid/identification/ivmethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Module for Instrumental Variables methods
 
 @author: edumapurunga
 """
 
 #%% imports
-from numpy import arange, array, append, asscalar, copy, count_nonzero, ones,\
+from numpy import arange, array, append, copy, count_nonzero, ones,\
 delete, dot, empty, sum, size, amax, matrix, concatenate, shape, zeros, kron,\
 eye, reshape, convolve, sqrt, where, nonzero, correlate, equal, ndarray, pi, \
 absolute, exp, log, real
 from scipy.linalg import qr, solve, toeplitz
 from numpy.linalg import matrix_rank
 from scipy.signal import lfilter, periodogram
 from scipy.optimize import leastsq, least_squares
```

### Comparing `pysid-0.1.0/pysid/identification/models.py` & `pysid-0.1.1/pysid/identification/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     This module implements the models used in the pysid package
 """
 #%%
 # Imports
 from numpy import log
+from pysid.io.print import print_model
 # Classes
 class polymodel():
     """
     This model represents a general linear polynomial model as follows
         A(q) y(t) = B(q) / F(q) u(t) + C(q)/ D(q) e(t) 
     """
 
@@ -23,42 +24,49 @@
         self.nparam = nparam
         self.data = data
         self.nu = nu
         self.ny = ny
         self.ts = ts
 
         # TODO: Ensure that setcov() is always called in pemethod.py
-        self.ecov = -1
+        self.parameters = None
+        self.ecov = None
+        self.residuals = None
+        self.M = None
 
     # Iterable
     def __iter__(self):
         return (i for i in (self.A, self.B, self.C, self.D, self.F))
 
     def __repr__(self):
         polymodelname = type(self).__name__
         s = '{}({!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r})'\
             .format(polymodelname, self.name, self.A, self.B, self.C, self.D, self.F, self.delay, 'data', self.nu, self.ny, self.ts)
         return s
 
     def __str__(self):
-        s = 'A ' + self.name + ' model'
+        print('A ' + self.name + ' model')
+        print_model(self,only_polynomials=True)
         polymodelname = type(self).__name__
-        return s
+        return ''
 
     def __eq__(self, other):
         return tuple(self) == tuple(other)
 
     def getdata(self):
         return self.data
 
     def setcov(self, V, accuracy, ncov):
         self.P = accuracy
         self.ecov = ncov
         self.costfunction = V
 
+    def setparameters(self,p):
+        self.parameters = p
+
     def setaic(self, J=None, N=None, p=None):
         """Sets the AIC criterion"""
         if J is None:
             J = self.costfunction
         if N is None:
             N = len(self.data[0])
         if p is None:
@@ -168,27 +176,27 @@
             mask[1] = mask[4] = True
         elif self.name == "BJ":
             mask[1] = mask[2] = mask[3] = mask[4] = True
         elif self.name == "PEM":
             mask[0] = mask[1] = mask[2] = mask[3] = mask[4] = True
         else:
             raise ValueError('Invalid model name.')
-
+        
         index = 0
         for poly in self:
             if mask[index]:
                 model_str = model_str + self.gen_poly_string(poly,dims[index],names[index]) + "\n"
             index = index + 1
 
         model_str = model_str + "\nMODEL PROPERTIES:"
         model_str = model_str + "\nSample time: " + str(self.ts)
         model_str = model_str + "\nTime delay:\n" + str(self.delay)
 
         # TODO: Define setcov() parameters for all pemethod.py functions
-        if self.ecov != -1:
+        if self.ecov is not None:
             model_str = model_str + "\n\necov: " + str(self.ecov)
             model_str = model_str + "\nCost function per sample: " + str(self.costfunction)
             model_str = model_str + "\n\nAccuracy:\n" + str(self.P)
 
         model_str = model_str + "\n________________________________________________________\n"
 
         return model_str
```

### Comparing `pysid-0.1.0/pysid/identification/pemethod.py` & `pysid-0.1.1/pysid/identification/pemethod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """
     Module for Prediction error methods
 """
 
 # Imports
-from numpy import arange, atleast_2d, asarray, array, append, asscalar, copy, count_nonzero, ones,\
-delete, dot, empty, sum, size, amax, matrix, concatenate, shape, zeros, kron,\
-eye, reshape, convolve, sqrt, where, nonzero, correlate, equal, ndarray, pi, \
-absolute, exp, log, real, issubdtype, integer, expand_dims
-from scipy.linalg import qr, solve, toeplitz, inv
-from numpy.linalg import matrix_rank
-from scipy.signal import lfilter, periodogram
-from scipy.optimize import leastsq, least_squares
-from .tseries import arma
+from numpy import arange, array, append, copy, count_nonzero,\
+delete, dot, empty, sum, size, amax, concatenate, shape, zeros, kron,\
+eye, reshape, convolve, where, equal, ndarray, floor
+from scipy.linalg import toeplitz, inv
+from scipy.signal import lfilter
+from scipy.optimize import least_squares
 from .solvers import ls, qrsol
 from ..io.check import chckin
 from .models import polymodel
-import numpy.fft as fft
 
 # functions
 __all__ = ['fir', 'arx', 'armax', 'oe', 'bj', 'pem']
 
 # Implementation
-def filtmat(matrix, signal, diag=-1, isvec=True):
+def filtmat(matrix, signal, diag=-1, isvec=True, isrational=False):
     """
     Filters a set of input signals (x) through a matrix (M) of polynomials, such that:
         y(t) = M*x(t)
     If a diagonal matrix (D) is also passed as a parameter, the output is then filtered
     by the inverse of (D), resulting in:
         y(t) = D^(-1)*M*x(t)
     The diagonal matrix can be (and is, by default) represented as a column vector
@@ -37,39 +33,52 @@
         Matrix of polynomials for linear filtering.
     signal : ndarray
         Input signal to be filtered.
     diag : ndarray of ndarray, optional
         Diagonal matrix to be used in inverse filtering. Default is -1, which bypasses filtering.
     isvec: boolean, optional
         Flag that indicates whether the diagonal matrix (diag) is represented as a vector.
+    isrational: boolean, optional
+        Flag that indicates whether the matrix (matrix) is a tuple matrix of rational polynomials
+        such that matrix = (num, den)
     Returns
     -------
     out : ndarray
         Filtered output signal.
     """
+    # Checking type
+    if not isinstance(matrix, ndarray) or not isinstance(signal,ndarray):
+        raise Exception("Input arguments type must be numpy.ndarray.")
+
     m, n = matrix.shape
     ms, ns = signal.shape
 
-    # Checking type
-    if not isinstance(matrix, ndarray) or not isinstance(signal,ndarray):
-        raise Exception("Input arguments' type must be numpy.ndarray.")
 
     # Checking dimension
     if ns != n:
         raise Exception("The input signal must have the same number of columns than the input matrix")
 
     output = zeros([ms, m])
     for i in range(m):
         for j in range(n):
-            output[:, i] += lfilter(matrix[i, j], [1], signal[:, j], axis = 0)
-        if diag != -1:
-            if isvec == True:
-                output[:, i] = lfilter([1], diag[i, 0], output[:, i], axis = 0)
+            if isrational:
+                output[:, i] += lfilter(matrix[i, j][0], matrix[i, j][1], signal[:, j], axis = 0)
             else:
-                output[:, i] = lfilter([1], diag[i, i], output[:, i], axis = 0)
+                output[:, i] += lfilter(matrix[i, j], [1], signal[:, j], axis = 0)
+        if type(diag) != int:
+            if isrational:
+                if isvec == True:
+                    output[:, i] = lfilter(diag[i, 0][0], diag[i, 0][1], output[:, i], axis = 0)
+                else:
+                    output[:, i] = lfilter(diag[i, i][0], diag[i, i][1], output[:, i], axis = 0)
+            else:
+                if isvec == True:
+                    output[:, i] = lfilter([1], diag[i, 0], output[:, i], axis = 0)
+                else:
+                    output[:, i] = lfilter([1], diag[i, i], output[:, i], axis = 0)
     return output
 
 def sortmat(A):
     """
     Sorts a square matrix whose diagonal elements have been shifted to its first column,
     such as:
     A = [A11, A12, A13, A14]
@@ -100,25 +109,33 @@
             Ao[i,i] = Ao[i,0]
             for j in range(0,i):
                 Ao[i,j] = A[i,j+1]
     return Ao
 
 def fir(nb, nk, u, y):
     """
-    This function estimates a FIR model based on the input-ouput data provided
-    in the form of vectors (u, y). This particular function returns the
-    polynomial B(q) from the following FIR model:
-        y(t) = B(q)u(t) + e(t)
-    Inputs:
-        nb - a scalar (or a matrix ny x nu)
-        nk - a scalar (or a matrix ny x nu)
-        u  - data input - vector (or matrix N x nu)
-        y  - data output - vector (or matrix N x ny)
-    Outputs:
-        B - vector containing the polynomial B(q)
+    Estimates a FIR model based on input (u(t)) and output (y(t)) vectors.
+    Returns the polynomial B(q) relative to the MIMO FIR model with nu inputs
+    and ny outputs, also affected by white gaussian noise e(t), as follows:
+        y(t) = B(q)*u(t) + e(t)   
+
+    Parameters
+    ----------
+    nb : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for B(q).
+    nk : array_like
+        Array of integers (ny x nu) that represents the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    B : ndarray
+        Array containing the polynomial coefficients of B(q).
     """
     # Transform everything in array for use with numpy
     _, nb, _, _, _, nk, u, y = chckin([], nb, [], [], [], nk, u, y)
     # Input handling
     Ny, ny = shape(y)
     Nu, nu = shape(u)
     nbk = nb + nk
@@ -162,27 +179,38 @@
     M = M/Ny
     # Set model parameters
     m.setcov(V**2/Ny, inv(M)/Ny, sig)
     return m
 
 def arx(na, nb, nk, u, y, opt=0):
     """
-    This function estimates a ARX model based on the input-ouput data provided
-    in the form of vectors (u, y). This particular function returns the
-    polynomials A(q) and B(q) from the following ARX model:
-        A(q)y(t) = B(q)u(t) + e(t)
-    Inputs:
-        na - a scalar (or a matrix ny x ny)
-        nb - a scalar (or a matrix ny x nu)
-        nk - a scalar (or a matrix ny x nu)
-        u  - data input - vector (or matrix N x nu)
-        y  - data output - vector (or matrix N x ny)
-    Outputs:
-        A - vector containing the polynomial A(q)
-        B - vector containing the polynomial B(q)
+    Estimates an ARX model based on input (u(t)) and output (y(t)) vectors.
+    Returns the polynomials A(q) and B(q) relative to the MIMO ARX model with
+    nu inputs and ny outputs, also affected by white gaussian noise e(t), 
+    as follows:
+        A(q)*y(t) = B(q)*u(t) + e(t)   
+        
+    Parameters
+    ----------
+    na : array_like
+        Array of integers (ny x ny) that represents the polynomial orders for A(q).        
+    nb : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for B(q).
+    nk : array_like
+        Array of integers (ny x nu) that represents the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    A : ndarray
+        Array containing the polynomial coefficients of A(q).
+    B : ndarray
+        Array containing the polynomial coefficients of B(q).
     """
     # Transform everything in array for use with numpy
     na, nb, _, _, _, nk, u, y = chckin(na, nb, [], [], [], nk, u, y)
     # Input handling
     Ny, ny = shape(y)
     Nu, nu = shape(u)
     nbk = nb + nk
@@ -228,41 +256,55 @@
             if (i == j):
                 A[i, j] = append([1], a[ka:ka+na[i,j]])
             else:
                 A[i, j] = append([0], a[ka:ka+na[i,j]])
             ka += na[i, j]
     # Model
     m = polymodel('arx', A, B, None, None, None, nk, da+db, (u, y), nu, ny, 1)
-    e = filtmat(A, yo[L:Ny, 0:ny]) - filtmat(B, u[L:Nu, 0:nu])
+    e = (filtmat(A, yo) - filtmat(B, u))[L:Ny, 0:ny]
     sig = (e.T @ e)/Ny
     isig = inv(sig)
     M = zeros((da + db, da + db))
     for k in range(0, phi.shape[0], ny):
         M += phi[k:k+ny, :].T @ isig @ phi[k:k+ny, :]
     M /= Ny # phi.T @ inv(sig) @ phi
     m.setcov(V**2/Ny, inv(M)/Ny, sig)
+    m.setparameters(array(a.tolist() + b.tolist()))
     return m
 
 def armax(na, nb, nc, nk, u, y):
     """
-    This function estimates an ARMAX model based on the input-ouput data provided
-    in the form of vectors (u, y). This particular function returns the
-    polynomials A(q), B(q) and C(q) from the following ARMAX model:
-        A(q)y(t) = B(q)u(t) + C(q)e(t)
-    Inputs:
-        na - a scalar (or a matrix ny x ny)
-        nb - a scalar (or a matrix ny x nu)
-        nc - a scalar (or a matrix ny x 1)
-        nk - a scalar (or a matrix ny x nu)
-        u  - data input - vector (or matrix N x nu)
-        y  - data output - vector (or matrix N x ny)
-    Outputs:
-        A - vector containing the polynomial A(q)
-        B - vector containing the polynomial B(q)
-        C - vector containing the polynomial C(q)
+    Estimates an ARMAX model based on input (u(t)) and output (y(t)) vectors.
+    Returns the polynomials A(q), B(q) and C(q) relative to the MIMO ARMAX
+    model with nu inputs and ny outputs, also affected by white gaussian
+    noise e(t), as follows:
+        A(q)*y(t) = B(q)*u(t) + C(q)*e(t)   
+        
+    Parameters
+    ----------
+    na : array_like
+        Array of integers (ny x ny) that represents the polynomial orders for A(q).        
+    nb : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for B(q).
+    nc : array_like
+        Array of integers (ny x 1) that represents the polynomial orders for C(q).
+    nk : array_like
+        Array of integers (ny x nu) that represents the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    A : ndarray
+        Array containing the polynomial coefficients of A(q).
+    B : ndarray
+        Array containing the polynomial coefficients of B(q).
+    C : ndarray
+        Array containing the polynomial coefficients of C(q).
     """
     # Transform everything into array
     na, nb, nc, _, _, nk, u, y = chckin(na, nb, nc, [], [], nk, u, y)
     #Input Handling
     Nu, nu = shape(u)
     Ny, ny = shape(y)
     da = sum(sum(na))
@@ -287,21 +329,24 @@
             a = append([0], A[k:k+na[i]])
             e -= lfilter(a, c, -y[:,i], axis=0)
             k = k + na[i]
         return e
     # Initial Guess
     A = empty((ny, ny), dtype=object)
     B = empty((ny, nu), dtype=object)
-    C = empty((ny,), dtype = object)
+    C = empty((ny, 1), dtype = object)
     for i in range(0, ny):
         A_ = []
         B_ = []
         E = copy(y[:,i:i+1])
         # High order model
-        mho = arx(50, [50,]*nu, [1,]*nu, u, y[:, i:i+1])
+        ho = int(floor((Nu - amax(nk)*(nu+1))/(nu+2)))
+        if(ho > 50):
+            ho = 50
+        mho = arx(ho, [ho,]*nu, [1,]*nu, u, y[:, i:i+1])
         aho, bho = mho.A, mho.B
         # Estimate of the prediction errors
         ehat = lfilter(aho[0][0], [1], y[:, i:i+1], axis=0)
         for j in range(0, nu):
             ehat -= lfilter(bho[0][j], [1], u[:, j:j+1], axis=0)
         # Index
         index = arange(ny)
@@ -317,45 +362,122 @@
         # Solve the minimization problem
         tar = y[0:Ny,i:i+1]
         tarna = na[i, i].reshape((1,))
         Y = concatenate((tar, y[0:Ny,index]), axis=1)
         NA = concatenate((tarna, na[i][index]))
         sol = least_squares(pe, thetai, args=(NA, nb[i], nc[i], nk[i], u.reshape(Nu, nu), Y.reshape((Ny, ny))))
         theta = sol.x
-        C[i] = append([1], theta[sum(na[i])+sum(nb[i]+1):sum(na[i])+sum(nb[i]+1)+sum(nc[i])+1])
+        C[i,0] = append([1], theta[sum(na[i])+sum(nb[i]+1):sum(na[i])+sum(nb[i]+1)+sum(nc[i])+1])
         k = sum(na[i])
         for j in range(0, nu):
             B[i, j] = append(zeros((1, nk[i,j])), theta[k:k+nb[i, j]+1])
             k += nb[i, j] + 1
         k = 0
         for j in range(0, ny):
-            if (i == j):
+            if (j == 0):
                 A[i, j] = append([1], theta[k:k+na[i, j]])
             else:
                 A[i, j] = append([0], theta[k:k+na[i, j]])
             k += na[i, j]
-        # Model
-        m = polymodel('armax', A, B, C, None, None, nk, da+db+dc, (u, y), nu, ny, 1)
+    # Sort A
+    As = sortmat(A)
+    # Estimate the prediction error: e(t) = C**-1 (y - G u)
+    # Get covariance:
+    L = amax([amax(na), amax(nb + nk), amax(nc)])
+    I = empty((ny, ny), dtype='object')
+    for i in range(ny):
+        for j in range(ny):
+            if i == j:
+                I[i, j] = array([1])
+            else:
+                I[i, j] = array([0])
+    ehat = (filtmat(As, y, C) - filtmat(B, u, C)) #[L:Ny, 0:ny]
+    # Get covariance of ehat
+    sig = (ehat.T @ ehat)/Ny
+    # Inverse of sig
+    isig = inv(sig)
+    # Model
+    m = polymodel('armax', As, B, C, None, None, nk, da+db+dc, (u, y), nu, ny, 1)
+    # Get filtered signals
+    Iny = eye(ny)
+    psiy = zeros(((Ny-L)*ny, da))
+    psiu = zeros(((Nu-L)*ny, db))
+    psie = zeros(((Ny-L)*ny, dc))
+    ka = 0
+    kb = 0
+    kc = 0
+    # Output regressors and Input Regressors
+    for i in range(0, ny):
+        # Get filtered signals
+        uf = lfilter([1], C[i][0], u, axis=0)
+        yf = lfilter([1], C[i][0], y, axis=0)
+        ef = lfilter([1], C[i][0], ehat, axis=0)
+        # Input
+        for j in range(0, nu):
+            if (nb[i, j] > -1):
+                psiu[:, kb:kb+nb[i, j]+1] = kron(toeplitz(uf[L-nk[i, j]:Nu-nk[i, j], j], uf[L-nk[i, j]-nb[i, j]:L-nk[i, j]+1, j][::-1]), Iny[:, i:i+1])
+                kb += nb[i, j] + 1
+        # Output
+        for j in range(0, ny):
+            if (na[i, j] > 0):
+                psiy[:, ka:ka+na[i,j]] = kron(-toeplitz(yf[L-1:-1, j], yf[L-na[i, j]:L, j][::-1]),Iny[:, i:i+1])
+                ka += na[i,j]
+        # Error
+        if (nc[i][0] > 0):
+            psie[:, kc:kc+nc[i][0]] = kron(toeplitz(ef[L-1:-1, i], ef[L-nc[i][0]:L, i][::-1]),Iny[:, i:i+1])
+            kc += nc[i][0]
+    psi = concatenate((psiy, psiu, psie), axis=1)
+    # Get gradient of the prediction error
+    # Initialize information matrix
+    M = zeros((da + db + dc, da + db + dc))
+    for k in range(0, psi.shape[0], ny):
+        M += psi[k:k+ny, :].T @ isig @ psi[k:k+ny, :]
+    M /= Ny
+    m.M = M
+    m.setcov(sig**2, inv(M)/Ny, sig)
+    # Collect parameters
+    thetaa = []
+    thetab = []
+    thetac = []
+    for i in range(ny):
+        for j in range(ny):
+            thetaa += As[i, j][1:].tolist()
+        for j in range(nu):
+            thetab += B[i, j][nk[i, j]:].tolist()
+        thetac += C[i][0][1:].tolist()
+
+    m.setparameters(array(thetaa+thetab+thetac))
     return m
 
 def oe(nb, nf, nk, u, y):
     """
-    This function estimates an OE model based on the input-ouput data provided
-    in the form of vectors (u, y). This particular function returns the
-    polynomials F(q) and B(q)  from the following OE model:
-        y(t) = (B(q)/F(q))u(t) + e(t)
-    Inputs:
-        nb - a scalar (or a matrix ny x nu)
-        nf - a scalar (or a matrix ny x nu)
-        nk - a scalar (or a matrix ny x nu)
-        u  - data input - vector (or matrix N x nu)
-        y  - data output - vector (or matrix N x ny)
-    Outputs:
-        B - vector containing the polynomial B(q)
-        F - vector containing the polynomial F(q)
+    Estimates an OE model based on input (u(t)) and output (y(t)) vectors.
+    Returns the polynomials B(q) and F(q) relative to the MIMO OE model
+    with nu inputs and ny outputs, also affected by white gaussian noise e(t), 
+    as follows:
+        y(t) = [B(q)/F(q)]*u(t) + e(t)   
+        
+    Parameters
+    ----------
+    nb : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for B(q).
+    nf : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for F(q).
+    nk : array_like
+        Array of integers (ny x nu) that represents the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    B : ndarray
+        Array containing the polynomial coefficients of B(q).
+    F : ndarray
+        Array containing the polynomial coefficients of F(q).
     """
     # Transform everything into array
     _, nb, _, _, nf, nk, u, y = chckin([], nb, [], [], nf, nk, u, y)
     # Input Handling
     Nu, nu = shape(u)
     Ny, ny = shape(y)
     db = sum(sum(nb+1))
@@ -377,16 +499,19 @@
             kb += nb[i] + 1
             yu = lfilter(b, f, u[:,i], axis=0)
             e -= yu
                 #e -= lfilter(b, f, u[:,i], axis=0)
                 #TODO verify the strange lfilter behavior here too
         return e
     # Initialization
+    parb = []
+    parf = []
     B = empty((ny, nu), dtype=object)
     F = empty((ny, nu), dtype=object)
+    BdF = empty((ny, nu), dtype=object)
     for j in range(0, ny):
         A = []
         B_ = []
         yn = copy(y[:,j:j+1])
         for i in range(0, nu):
             a, b = ls(nf[j, i], nb[j, i], nk[j, i], u[:,i:i+1], yn)
             A = append(A, a)
@@ -401,41 +526,99 @@
         sol = least_squares(pe, thetai, args=(nf[j], nb[j], nk[j], u.reshape((Nu, nu)), y[:,j]))
         # Output
         theta = sol.x
         kf = 0
         kb = 0
         f = theta[0:sum(nf[j])]
         b = theta[sum(nf[j]):sum(nf[j])+sum(nb[j]+1)+2]
+        parb += b.flatten().tolist()
+        parf += f.flatten().tolist()
         for i in range(0, nu):
             B[j, i] = append(zeros((1, nk[j, i])), b[kb:kb+nb[j, i]+1])
             F[j, i] = append([1], f[kf:kf+nf[j, i]])
+            BdF[j, i] = (B[j, i], F[j, i])
             kf += nf[j, i]
             kb += nb[j, i] + 1
-        m = polymodel('oe', None, B, None, None, F, nk, db+df, (u, y), nu, ny, 1)
+    ehat = y - filtmat(BdF, u, isrational=True) #[L:Ny, 0:ny]
+    # Get covariance of ehat
+    sig = (ehat.T @ ehat)/Ny
+    # Inverse of sig
+    isig = inv(sig)
+    # Model
+    kb = 0
+    kf = 0
+    # Get covariance:
+    L = amax([amax(nf), amax(nb + nk)])
+    Iny = eye(ny)
+    psiy = zeros(((Ny-L)*ny, df))
+    psiu = zeros(((Nu-L)*ny, db))
+    # Output regressors and Input Regressors
+    for i in range(0, ny):
+        kw = 0
+        # Get filtered signals
+        uf = zeros((Ny, nu))
+        wf = zeros((Ny, nu))
+        # Input
+        for j in range(0, nu):
+            if (nb[i, j] > -1):
+                wf[:, kw] = lfilter(B[i, j], convolve(F[i, j], F[i, j]), u[:, j], axis=0)
+                uf[:, kw] = lfilter([1], F[i, j], u[:, j], axis=0)
+                psiu[:, kb:kb+nb[i, j]+1] = kron(toeplitz(uf[L-nk[i, j]:Nu-nk[i, j], j], uf[L-nk[i, j]-nb[i, j]:L-nk[i, j]+1, j][::-1]), Iny[:, i:i+1])
+                psiy[:, kf:kf+nf[i,j]] = kron(-toeplitz(wf[L-1:-1, kw], wf[L-nf[i, j]:L, kw][::-1]),Iny[:, i:i+1])
+                kb += nb[i, j] + 1
+                kf += nf[i,j]
+                kw += 1
+    # Get Model
+    m = polymodel('oe', None, B, None, None, F, nk, db+df, (u, y), nu, ny, 1)
+    psi = concatenate((psiu, psiy), axis=1)
+    # Get gradient of the prediction error
+    # Initialize information matrix
+    M = zeros((df + db, df + db))
+    for k in range(0, psi.shape[0], ny):
+        M += psi[k:k+ny, :].T @ isig @ psi[k:k+ny, :]
+    M /= Ny
+    m.M = M
+    m.setcov(sol.cost, inv(M)/Ny, sig)
+    m.setparameters(array(parb+parf))
     return m
 
 def bj(nb, nc, nd, nf, nk, u, y):
     """
-    This function estimates a BJ model based on the input-ouput data provided
-    in the form of vectors (u, y). This particular function returns the
-    polynomials B(q), F(q), C(q) and D(q)  from the following BJ model:
-        y(t) = (B(q)/F(q))u(t) + (C(q)/D(q))e(t)
-    Inputs:
-        nb - a scalar (or a matrix ny x nu)
-        nc - a scalar (or a matrix ny x 1)
-        nd - a scalar (or a matrix ny x 1)
-        nf - a scalar (or a matrix ny x nu)
-        nk - a scalar (or a matrix ny x nu)
-        u  - data input - vector (or matrix N x nu)
-        y  - data output - vector (or matrix N x ny)
-    Outputs:
-        B - vector containing the polynomial B(q)
-        C - vector containing the polynomial C(q)
-        D - vector containing the polynomial D(q)
-        F - vector containing the polynomial F(q)
+    Estimates an BJ model based on input (u(t)) and output (y(t)) vectors.
+    Returns the polynomials B(q), F(q), C(q) and D(q) relative to the MIMO
+    BJ model with nu inputs and ny outputs, also affected by white gaussian
+    noise e(t), as follows:
+        y(t) = [B(q)/F(q)]*u(t) + [C(q)/D(q)]*e(t)   
+        
+    Parameters
+    ----------
+    nb : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for B(q).
+    nc : array_like
+        Array of integers (ny x 1) that represents the polynomial orders for C(q).
+    nd : array_like
+        Array of integers (ny x 1) that represents the polynomial orders for D(q).
+    nf : array_like
+        Array of integers (ny x nu) that represents the polynomial orders for F(q).
+    nk : array_like
+        Array of integers (ny x nu) that represents the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    B : ndarray
+        Array containing the polynomial coefficients of B(q).
+    C : ndarray
+        Array containing the polynomial coefficients of C(q).
+    D : ndarray
+        Array containing the polynomial coefficients of D(q).
+    F : ndarray
+        Array containing the polynomial coefficients of F(q).
     """
     _, nb, nc, nd, nf, nk, u, y = chckin([], nb, nc, nd, nf, nk, u, y)
     # Input Handling
     Nu, nu = shape(u)
     Ny, ny = shape(y)
     db = sum(sum(nb+1))
     dc = sum(sum(nc))
@@ -462,17 +645,22 @@
             kb += nb[i] + 1
             db = convolve(b, d)
             fc = convolve(f, c)
             e -= lfilter(db, fc, u[0:,i], axis=0)
         return e
     # Initial Guess
     B = empty((ny, nu), dtype=object)
-    C = empty((ny, ), dtype=object)
-    D = empty((ny, ), dtype=object)
+    C = empty((ny,1), dtype=object)
+    D = empty((ny,1), dtype=object)
     F = empty((ny, nu), dtype=object)
+    # Parameter
+    parb = []
+    parc = []
+    pard = []
+    parf = []
     # TODO: Verify a way to compute an ARMA process
     for j in range(0, ny):
         thetaf = []
         thetab = []
         yn = copy(y[:, j:j+1])
         for i in range(0, nu):
             a, b = ls(nf[j, i], nb[j, i], nk[j, i], u[:, i:i+1], y[:,j:j+1])
@@ -497,28 +685,94 @@
             thetai = append(thetai, c)
         else:
             thetai = append(thetai, (c, d))
         # Solve the minimization problem
         sol = least_squares(pe, thetai, args=(nf[j], nb[j], nc[j][0], nd[j][0], nk[j], u.reshape(Nu, nu), y[:,j]))
         theta = sol.x
         #B[j] = append(zeros((1, nk[j])), theta[nf[j]:nf[j]+nb[j]+1])
-        C[j] = append([1], theta[sum(nf[j])+sum(nb[j]+1):nc[j][0]+sum(nf[j])+sum(nb[j]+1)])
-        D[j] = append([1], theta[nc[j][0]+sum(nf[j])+sum(nb[j]+1):nd[j][0]+nc[j][0]+sum(nf[j])+sum(nb[j]+1)])
+        C[j,0] = append([1], theta[sum(nf[j])+sum(nb[j]+1):nc[j][0]+sum(nf[j])+sum(nb[j]+1)])
+        D[j,0] = append([1], theta[nc[j][0]+sum(nf[j])+sum(nb[j]+1):nd[j][0]+nc[j][0]+sum(nf[j])+sum(nb[j]+1)])
+        parc += C[j, 0][1:].tolist()
+        pard += D[j, 0][1:].tolist()
         #F[j] = append([1], theta[0:nf[j]])
         F_ = theta[0:sum(nf[j])]
         B_ = theta[sum(nf[j]):sum(nf[j])+sum(nb[j]+1)]
         kf = 0
         kb = 0
         for i in range(0, nu):
             F[j, i] = append([1], F_[kf:kf+nf[j, i]])
             B[j, i] = append(zeros((1, nk[j, i])), B_[kb:kb+nb[j, i]+1])
+            parf += F[j, i][1:].tolist()
+            parb += B_[kb:kb+nb[j, i]+1].tolist()
             kf += nf[j, i]
             kb += nb[j, i] + 1
         # Model
-        m = polymodel('boxjenkins', None, B, C, D, F, nk, db+dc+dd+df, (u, y), nu, ny, 1)
+    m = polymodel('boxjenkins', None, B, C, D, F, nk, db+dc+dd+df, (u, y), nu, ny, 1)
+    # Set the parameters
+    m.setparameters(array(parb + parc + pard + parf))
+    # Get the prediction error
+    ehat = zeros((Ny, ny))
+    for k in range(ny):
+        ehat[:, k] = lfilter(D[k, 0], C[k, 0], y[:, k], axis=0)
+        for i in range(nu):
+            ehat[:, k] -= lfilter(convolve(B[k, i], D[k, 0]),
+                                  convolve(C[k, 0], F[k, i]), u[:, i], axis=0)
+    # Get covariance of ehat
+    sig = (ehat.T @ ehat)/Ny
+    # Inverse of sig
+    isig = inv(sig)
+    # Get covariance:
+    L = amax([amax(nf), amax(nb + nk), amax(nc), amax(nd)])
+    Iny = eye(ny)
+    psiy = zeros(((Ny-L)*ny, df))
+    psiu = zeros(((Nu-L)*ny, db))
+    psiec = zeros(((Nu-L)*ny, dc))
+    psied = zeros(((Nu-L)*ny, dd))
+    kb = 0
+    kc = 0
+    kd = 0
+    kf = 0
+    # Output regressors and Input Regressors
+    for i in range(0, ny):
+        kw = 0
+        # Get filtered signals
+        uf = zeros((Ny, nu))
+        w = zeros((Ny, 1))
+        wf = zeros((Ny, nu))
+        ef = lfilter([1], C[i, 0], ehat, axis=0)
+        psiec[:, kc:kc+nc[i][0]] = kron(toeplitz(ef[L-1:-1, i], ef[L-nc[i][0]:L, i][::-1]), Iny[:, i:i+1])
+        kc += nc[i][0]
+        # Input
+        for j in range(0, nu):
+            if (nb[i, j] > -1):
+                w[:, 0] += lfilter(B[i, j], F[i, j], u[:, j], axis=0)
+                wf[:, kw] = lfilter(convolve(B[i, j], D[i, 0]),
+                                    convolve(convolve(F[i, j], F[i, j]), C[i, 0]),
+                                             u[:, j], axis=0)
+                uf[:, kw] = lfilter(D[i, 0], convolve(F[i, j], C[i, 0]), u[:, j], axis=0)
+
+                psiu[:, kb:kb+nb[i, j]+1] = kron(toeplitz(uf[L-nk[i, j]:Nu-nk[i, j], j], uf[L-nk[i, j]-nb[i, j]:L-nk[i, j]+1, j][::-1]), Iny[:, i:i+1])
+                psiy[:, kf:kf+nf[i,j]] = kron(-toeplitz(wf[L-1:-1, kw], wf[L-nf[i, j]:L, kw][::-1]), Iny[:, i:i+1])
+                kb += nb[i, j] + 1
+                kf += nf[i, j]
+                kw += 1
+        # Get the last one
+        vf = lfilter([1], C[i, 0], w-y[:, i:i+1], axis=0)
+        psied[:, kd:kd+nd[i][0]] = kron(toeplitz(vf[L-1:-1, 0], vf[L-nd[i][0]:L, 0][::-1]), Iny[:, i:i+1])
+        kd += nd[i][0]
+    # Make the information matrix
+    psi = concatenate((psiu, psiec, psied, psiy), axis=1)
+    # Get gradient of the prediction error
+    # Initialize information matrix
+    M = zeros((df + db + dc + dd, df + db + dc + dd))
+    for k in range(0, psi.shape[0], ny):
+        M += psi[k:k+ny, :].T @ isig @ psi[k:k+ny, :]
+    M /= Ny
+    m.M = M
+    m.setcov(sol, inv(M)/Ny, sig)
     return m
 
 # %% Testing functions
 def pem(A, B, C, D, F, u, y, mu=[] ,solver='lm'):
     """
     This functions implements the prediction error method for the gerenal
     tranfer function black-box model:
@@ -1057,15 +1311,16 @@
                 if nf[i] != 0:
                     F[i] = append([1], theta[k:k+nf[i]])
                     k += nf[i]
                 else:
                     F[i] = 1
     #SIMO case
     elif (nu==1):
-        do = nothing
+        #do = nothing
+        pass
     #MIMO case
     else:
         #Define the orders of the polynomials
         na = zeros((ny, ny), dtype = 'int32')
         nb = zeros((ny, nu), dtype = 'int32')
         nc = zeros((ny,), dtype = 'int32')
         nd = zeros((ny,), dtype = 'int32')
@@ -1126,15 +1381,15 @@
                 #Number of known elements
                 kA = zeros((ny,), dtype = 'int32')
                 ukA = zeros((ny,), dtype = 'int32')
                 for i in range(0, ny):
                     #Known Elements
                     kA[i] = count_nonzero(muA[i])
                     #Unknown elements
-                    uKA[i] = na[i] - kA[i]
+                    ukA[i] = na[i] - kA[i]
                 kB = zeros((nu,), dtype = 'int32')
                 kF = zeros((nu,), dtype = 'int32')
                 #Unknown
                 ukB = zeros((nu,), dtype = 'int32')
                 ukF = zeros((nu,), dtype = 'int32')
                 for i in range(0, nu):
                     #Known elements
```

### Comparing `pysid-0.1.0/pysid/identification/solvers.py` & `pysid-0.1.1/pysid/identification/solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,25 @@
     M = concatenate((A, B), axis=1)
     Q, R = qr(M)
     R1 = R[0:d, 0:d]
     R2 = R[0:d, d]
     V = R[d, d]
     theta = solve(R1, R2)
     return [theta, V, R1]
+
+def qrsolm(psi,y):
+    """
+    Solve the least saqures problem using QR-factorization but for mimo systems
+    """
+    ny = y.shape[1];
+    theta = zeros((psi.shape[1],ny))
+    for i in range(ny):
+        theta_i = qrsol(psi, y[:,i].reshape((y.shape[0],1)))[0]
+        theta[:,i] = theta_i
+    return theta
  
 def levinson(R, n):
     """
     This function implements the Levinson algorithm for fast parameters computations
     """
     A = empty((n,), dtype='object')
     alfa = append(R[1], zeros((1, n)))
```

### Comparing `pysid-0.1.0/pysid/identification/tseries.py` & `pysid-0.1.1/pysid/identification/tseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Module for estimate time series models (AR, MA, ARMA)
 
 author: @edumapurunga
 """
 
 # Imports
-from numpy import arange, array, append, asscalar, copy, count_nonzero, ones,\
+from numpy import arange, array, append, copy, count_nonzero, ones,\
 delete, dot, empty, sum, size, amax, matrix, concatenate, shape, zeros, kron,\
 eye, reshape, convolve, sqrt, where, nonzero, correlate, equal, ndarray, pi, \
 absolute, exp, log, real
 from scipy.linalg import qr, solve, toeplitz
 from numpy.linalg import matrix_rank
 from scipy.signal import lfilter, periodogram
 from scipy.optimize import leastsq, least_squares
```

### Comparing `pysid-0.1.0/pysid/io/check.py` & `pysid-0.1.1/pysid/io/check.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,62 @@
 """
     Module for checking the arguments of several functions
 """
 
 # Imports
-from numpy import array, amax, ndarray, expand_dims, size, shape
+from numpy import array, amax, ndarray, expand_dims, size, shape, floor
 # Variables
 __all__ = ['chckin']
 
 
 # functions
 def chckin(na, nb, nc, nd, nf, nk, u, y):
     """
-    Function used to handle input argument and throw errors
+    Function used to handle input arguments for prediction error method (PEM)
+    identification, following the general polynomial model:
+        A(q)y(t) = [B(q)/F(q)]*u(t) + [C(q)/D(q)]*e(t)
+  
+    Parameters
+    ----------
+    na : array_like
+        Array of integers relative to the A(q) polynomial.   
+    nb : array_like
+        Array of integers relative to the B(q) polynomial.
+    nc : array_like
+        Array of integers relative to the C(q) polynomial.
+    nd : array_like
+        Array of integers relative to the D(q) polynomial.
+    nf : array_like
+        Array of integers relative to the F(q) polynomial.     
+    nk : array_like
+        Array of integers relative to the model's time delay.
+    u : array_like
+        Input data array.
+    y : array_like
+        Output data array.
+    Returns
+    -------
+    na : array_like
+        Validated na parameter.
+    nb : array_like
+        Validated nb parameter.
+    nc : array_like
+        Validated nc parameter.
+    nd : array_like
+        Validated nd parameter.
+    nf : array_like
+        Validated nf parameter.   
+    nk : array_like
+        Validated nk parameter. 
+    u : array_like
+        Validated input array.
+    y : array_like
+        Validated output array.
     """
+
     # Check if is at least a list or array
     if not isinstance(na, (int, list, ndarray)) or not isinstance(nb, (int, list, ndarray)) or\
        not isinstance(nc, (int, list, ndarray)) or not isinstance(nd, (int, list, ndarray)) or\
        not isinstance(nf, (int, list, ndarray)) or not isinstance(nk, (int, list, ndarray)) or\
        not isinstance(u, (int, list, ndarray)) or not isinstance(y, (int, list, ndarray)):
         raise Exception('Input arguments must be either list or numpy.ndarray type')
     # Verify if the arguments are lists and transform them in 2D arrays
@@ -50,15 +90,16 @@
     rd = shape(nd)[0]
     rf, cf = shape(nf)
     rk, ck = shape(nk)
     L = int(amax([amax(na, initial=0), amax(nb + nk, initial=0), amax(nc, initial=0), amax(nd, initial=0), amax(nf, initial=0)]))
     # Different number of Data
     if Ny != Nu:
         raise Exception('Input and Output must be the same number of data samples')
-    if Ny < L:
+    #second case for when its not possible to make the high order model in armax
+    if Ny < L or int(floor((Nu - amax(nk)*(nu+1))/(nu+2))) <= 1:
         raise Exception('Not enough data for model identification')
     # Classify Into the structures: Initial Variables
     #isAR = True
     #isARX = True
     #isARMA = True
     #isARMAX = True
     #isBB = True
```

### Comparing `pysid-0.1.0/pysid/io/csv_data.py` & `pysid-0.1.1/pysid/io/csv_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
     author: @lima84
     Loads a dataset into a variable. Default format is .csv
     
     Parameters
     ----------
     filename : string
-    Name of the file (with extension) from which the dataset is loaded.
+        Name of the file (with extension) from which the dataset is loaded.
     delim : string, optional
         Column delimiter. Default is "," for .csv files.
     skip_rows : int, optional
         Number of skipped rows. Default is 1, for the file header.
     Returns
     -------
     data : ndarray
```

### Comparing `pysid-0.1.0/pysid/io/print.py` & `pysid-0.1.1/pysid/io/print.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from IPython.display import display, Math
+from shutil import which
 
 def coef_to_str(c,prec=3):
     """Converts a float coefficient (c) into a string, with precision given by prec."""
-    return "{:.{precision}f}".format(c, precision = prec)
+    return "{:.{precision}g}".format(c, precision = prec)
+
 
 def poly_to_str(P,prec=3):
     """
     Converts a MIMO set of polynomials (P) into an equivalent display string,
     following LaTeX syntax. P must be an array of arrays. For example, let A 
     be a 2 x 2 matrix of polynomials, then
         P = [A11, A12, A21, A22]
 
     Parameters
     ----------
     P : ndarray of ndarray
-        Set of polynomials to be displayed.
-        
+        Set of polynomials to be displayed.        
     prec : integer, optional
         Decimal precision for the coefficients. Default is prec = 3.
     Returns
     -------
-    
+    label : string
+        Formatted string in LaTeX ready to be displayed.
+
     """
     if P is None:
         raise Exception("Polynomial is equal to None.")
     label = []
     aux = ""
     power = 0
     first_elem = True
-    #if P.shape == (1,1):
+   #if P.shape == (1,1):
     #    P = P.reshape(1,)
     for row in P:
         for poly in row:
             for coef in poly:
                 if coef != 0:
                     if first_elem == True:
-                        # Appending the first element (without the sum sign in front)
-                        if power == 0:
+                       # Appending the first element (without the sum sign in front)
+                        if power == 0 and coef==1:
                             # For monic polynomials
                             aux = aux + str(1)
+                        elif power == 0 and coef!=1:
+                            aux = aux + coef_to_str(coef,prec)
                         else:
                             # For non-monic polynomials
                             aux = aux + coef_to_str(coef,prec) + "q^{" + "{0}".format(-power) + "}"
                         # Sets first element flag to False
                         first_elem = False
                     elif coef > 0:
                         # Appeding a positive element
@@ -73,27 +78,38 @@
     prec : integer, optional
         Decimal precision for the coefficients. Default is prec = 3.
     Returns
     -------
 
     """
     m,n = matrix.shape
-
+    #if which('latex') is not None:
     label = r"\begin{bmatrix}"
     for row in range(m):
         for col in range(n):
             label = label + coef_to_str(matrix[row][col],prec)
             if col != n-1:
                 label = label + r"&"
         if row != m-1:
             label = label + r"\\ "
 
     label = label + "\end{bmatrix}"
     return label
 
+def print_matrix(matrix,prec):
+    m,n = matrix.shape
+    for row in range(m):
+        print("|",end="")
+        for col in range(n):
+            if matrix[row][col] > 0:
+                print(" "+coef_to_str(matrix[row][col],prec=prec),end="\t")
+            else:
+                print(coef_to_str(matrix[row][col],prec=prec),end="\t" )
+        print("|")
+                
 def print_poly(P,dim,name,prec=3):
     """
     Prints a MIMO polynomial model.
 
     Parameters
     ----------
     P : ndarray
@@ -109,53 +125,84 @@
     
     """
     if P is None:
         raise Exception("Polynomial is equal to None.")
     s = poly_to_str(P,prec)
     rows, cols = dim[0], dim[1]
     index = 0
-    for row in range(rows):
-        for col in range(cols):
-            if rows == 1 and cols == 1:
-                # Prints SISO subcase
-                display(Math(r'' + name + '(q^{-1}) = ' + s[index]))
-            else:
-                if name == "C" or name == "D":
-                    poly_index = "{" + str(row+1) + "}"
-                    display(Math(r'' + name + "_" + poly_index + '(q^{-1}) = ' + s[index]))
+    #print(which('latex'))
+    if which('latex') is not None:
+        for row in range(rows):
+            for col in range(cols):
+                if rows == 1 and cols == 1:
+                    # Prints SISO subcase
+                    display(Math(r'' + name + '(q^{-1}) = ' + s[index]))
                 else:
-                    # Prints general MIMO case
-                    poly_index = "{" + str(row+1) + str(col+1) + "}"
-                    display(Math(r'' + name + "_" + poly_index + '(q^{-1}) = ' + s[index]))
-            index = index + 1
+                    if name == "C" or name == "D":
+                        poly_index = "{" + str(row+1) + "}"
+                        display(Math(r'' + name + "_" + poly_index + '(q^{-1}) = ' + s[index]))
+                    else:
+                        # Prints general MIMO case
+                        poly_index = "{" + str(row+1) + str(col+1) + "}"
+                        display(Math(r'' + name + "_" + poly_index + '(q^{-1}) = ' + s[index]))
+                index = index + 1
+    else:
+        for row in range(rows):
+            for col in range(cols):
+                if rows == 1 and cols == 1:
+                    # Prints SISO subcase
+                    print(r'' + name + '(q^{-1}) = ' + s[index])
+                else:
+                    if name == "C" or name == "D":
+                        poly_index = str(row+1)
+                        print(r'' + name + poly_index + ' (q^{-1}) = ' + s[index])
+                    else:
+                        # Prints general MIMO case
+                        poly_index = str(row+1) + str(col+1)
+                        print(r'' + name + poly_index + ' (q^{-1}) = ' + s[index])
+                index = index + 1
+    print("\n")
+
 
-def print_model(model,prec=3,names=['A','B','C','D','F']):
+def print_model(model,prec=3,only_polynomials=False):
     """
     Prints the set of polynomials that define a given model.
 
     Parameters
     ----------
     model : polymodel object
         Identification model object containing a set of polynomials.
     prec : integer, optional
         Decimal precision for the coefficients. Default is prec = 3.
-    names : list of strings
-        Name displayed for each polynomial in the model. Default is 'A','B','C','D','F']
     Returns
-    -------
     
     """
+    names = []
+    if any(model.A) != None:
+        names.append('A')
+    if any(model.B) != None:
+        names.append('B')
+    if any(model.C) != None:
+        names.append('C')
+    if any(model.D) != None:
+        names.append('D')
+    if any(model.F) != None:
+        names.append('F')
     # Model should be a pysid.identification.models.polymodel() object
     index = 0
     ny, nu = model.ny, model.nu
     dims = [[ny,ny],[ny,nu],[ny,1],[ny,1],[ny,nu]]
     for poly in model:
         if poly is not None:
             print_poly(poly,dims[index],names[index],prec)
             index = index + 1
 
-    if hasattr(model, 'costfunction'):
-        print(f'Cost function per sample: ' + coef_to_str(model.costfunction,prec))
-
-    if hasattr(model, 'P'):
-        print(f'Accuracy:')
-        display(Math(matrix_to_str(model.P,prec)))
+    if not only_polynomials:
+        if hasattr(model, 'costfunction'):
+            print(f'Cost function per sample: ' + coef_to_str(model.costfunction,prec))
+    
+        if hasattr(model, 'P'):
+            print(f'Accuracy:')
+            if which('latex') is not None:
+                display(Math(matrix_to_str(model.P,prec)))
+            else:
+                print_matrix(model.P,prec)
```

### Comparing `pysid-0.1.0/pysid.egg-info/PKG-INFO` & `pysid-0.1.1/pysid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysid
-Version: 0.1.0
+Version: 0.1.1
 Summary: System Identification tools for python
 Home-page: https://github.com/edumapurunga/pysid
 Author: Eduardo Mapurunga
 Author-email: edumapurunga@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysid-0.1.0/pysid.egg-info/SOURCES.txt` & `pysid-0.1.1/pysid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,13 +12,16 @@
 pysid/correlation/croscorr.py
 pysid/identification/__init__.py
 pysid/identification/accr.py
 pysid/identification/comcrit.py
 pysid/identification/ivmethod.py
 pysid/identification/models.py
 pysid/identification/pemethod.py
+pysid/identification/recursive.py
 pysid/identification/solvers.py
 pysid/identification/tseries.py
 pysid/io/__init__.py
 pysid/io/check.py
 pysid/io/csv_data.py
-pysid/io/print.py
+pysid/io/print.py
+pysid/tests/__init__.py
+pysid/tests/pem tests.py
```

### Comparing `pysid-0.1.0/setup.py` & `pysid-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 # Read README contents
 with open("README.md") as fh:
     long_description = fh.read()
 # Set the setup file
 setuptools.setup(
     name="pysid",
-    version="0.1.0",
+    version="0.1.1",
     author="Eduardo Mapurunga",
     author_email="edumapurunga@gmail.com",
     description="System Identification tools for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edumapurunga/pysid",
     packages=setuptools.find_packages(),
```

