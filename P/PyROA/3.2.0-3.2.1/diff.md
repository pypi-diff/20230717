# Comparing `tmp/PyROA-3.2.0.tar.gz` & `tmp/PyROA-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyROA-3.2.0.tar", last modified: Sun Jul 16 17:49:58 2023, max compression
+gzip compressed data, was "PyROA-3.2.1.tar", last modified: Mon Jul 17 13:19:39 2023, max compression
```

## Comparing `PyROA-3.2.0.tar` & `PyROA-3.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.733981 PyROA-3.2.0/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-16 17:49:58.732476 PyROA-3.2.0/PKG-INFO
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.709333 PyROA-3.2.0/PyROA/
--rw-r--r--   0 donnanf    (503) staff       (20)   111218 2023-05-26 11:57:59.000000 PyROA-3.2.0/PyROA/PyROA.py
--rw-r--r--   0 donnanf    (503) staff       (20)    42132 2023-03-21 15:13:42.000000 PyROA-3.2.0/PyROA/Utils.py
--rw-r--r--   0 donnanf    (503) staff       (20)      228 2023-05-26 12:03:09.000000 PyROA-3.2.0/PyROA/__init__.py
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.730747 PyROA-3.2.0/PyROA.egg-info/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/PKG-INFO
--rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/SOURCES.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/dependency_links.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/top_level.txt
--rw-rw-r--   0 donnanf    (503) staff       (20)    15163 2023-02-27 13:58:10.000000 PyROA-3.2.0/README.md
--rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-07-16 17:49:58.734230 PyROA-3.2.0/setup.cfg
--rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-05-26 12:04:29.000000 PyROA-3.2.0/setup.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.707255 PyROA-3.2.1/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-17 13:19:39.705322 PyROA-3.2.1/PKG-INFO
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.411310 PyROA-3.2.1/PyROA/
+-rw-r--r--   0 donnanf    (503) staff       (20)   111299 2023-07-17 12:31:49.000000 PyROA-3.2.1/PyROA/PyROA.py
+-rw-r--r--   0 donnanf    (503) staff       (20)    42132 2023-03-21 15:13:42.000000 PyROA-3.2.1/PyROA/Utils.py
+-rw-r--r--   0 donnanf    (503) staff       (20)      228 2023-07-17 13:19:06.000000 PyROA-3.2.1/PyROA/__init__.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.701896 PyROA-3.2.1/PyROA.egg-info/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/PKG-INFO
+-rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/SOURCES.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/dependency_links.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/top_level.txt
+-rw-rw-r--   0 donnanf    (503) staff       (20)    16574 2023-07-17 13:18:50.000000 PyROA-3.2.1/README.md
+-rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-07-17 13:19:39.707612 PyROA-3.2.1/setup.cfg
+-rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-07-17 13:18:23.000000 PyROA-3.2.1/setup.py
```

### Comparing `PyROA-3.2.0/PyROA/PyROA.py` & `PyROA-3.2.1/PyROA/PyROA.py`

 * *Files 0% similar despite different names*

```diff
@@ -1158,21 +1158,21 @@
         size = size + len(mjd)
         sizes[i+1] = len(mjd)   
      
         if (include_slow_comp==True):
             t_slow, m_slow, errs_slow = RunningOptimalAverage(mjd,flux,err, slow_comp_delta)
             m_slow = m_slow - np.mean(m_slow)
             m_s = interpolate.interp1d(t_slow, m_slow, kind="linear", fill_value="extrapolate")
-            pos_chunks[i][0] = np.std(flux - m_s(mjd)) #Set intial A to rms of data
-            pos_chunks[i][1] = np.mean(flux- m_s(mjd)) #Set initial B to mean of data
+            pos_chunks[i][0] = np.median(np.absolute(flux- m_s(mjd) - np.median(flux- m_s(mjd)))) #Set intial A to rms of data
+            pos_chunks[i][1] = np.median(flux- m_s(mjd)) #Set initial B to mean of data
 
 
         else:        
-            pos_chunks[i][0] = pos_chunks[i][0] + np.std(flux)# - m_s(mjd)) #Set intial A to rms of data
-            pos_chunks[i][1] = np.mean(flux)#- m_s(mjd)) #Set initial B to mean of data
+            pos_chunks[i][0] = pos_chunks[i][0] + np.median(np.absolute(flux - np.median(flux)))# - m_s(mjd)) #Set intial A to rms of data
+            pos_chunks[i][1] = np.median(flux)#- m_s(mjd)) #Set initial B to mean of data
```

### Comparing `PyROA-3.2.0/PyROA/Utils.py` & `PyROA-3.2.1/PyROA/Utils.py`

 * *Files identical despite different names*

### Comparing `PyROA-3.2.0/README.md` & `PyROA-3.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 ## Installation
 
 Install using pip: pip install PyROA
 
 
 ## Changes
 
+### v3.2.1
+ - Changed the priors in A and B expressed in units of RMS and mean to the MAD and mean. This should better handle lightcurves with lots of outliers when setting up the priors for A and B.
+
+### v3.2.0
+ - The effective number of parameters when delay_dist=True now only uses the driving lightcurve. This has a small effect but with this change, the number of parameters only depends on the smoothness of the driving lightcurve and not the width of the delay distributions
+ - Priors on the A and B (scale and shift) parameters are handled differently. The user now specifies unitless lower and upper limits as factors of the calculated RMS (A) and mean (B) of each lightcurve. This allows the prior range to vary for each lightcurve to provide more sensible limits especially in cases where the fluxes of each lightcurve vary drastically.
+ - The initial values of the walkers are now setup to better sample the parameter space, now set to 0.2*initial_value.
+ - Fixed an issue where delay_dist=True did not allow negative mean lags.
+ - Fixed error for the in-line output of the best-fit lags.
+
+
 #### v3.1.0
 - Added new utility functions (Utils.py) to analyse the outputs of PyROA. See the Utils_Tutorial for examples of usage. These include displaying lightcurve(+residuals), Convergence plots, corner and chain plots by parameter, Lag spectrum plot and Flux-Flux analysis plot.
 - Changes to the intercalibration files were added. It now outputs, for every datum the original telescope, ROA model+uncertainty at the point, and degree of freedom value.
 
 #### v3.0.0
 - Re-implemented the delay distribution function to now use a numerical convolution. This allows any type of transfer function to be modelled.
 - Added use of the emcee backend, which allows saving and resuming of progress.
@@ -52,26 +63,26 @@
 To measure the time delay between lightcurves of different wavelengths we first specify a directory, object name and filters. In the directory each lightcurve is a .dat file that contains three columns: time, flux, flux_err and is named: "objName_filter.dat". Using the mock data provided we would run the code using
 
 ```` import PyROA
 datadir = "/MockData/HighSN/"
 objName="TestObj"
 filters=["1","2","3"]
     
-priors = [[0.0, 20.0],[0.0, 100.0], [-50.0, 50.0], [0.01, 10.0], [0.0, 10.0]]
+priors = [[0.5, 2.0],[0.5, 2.0], [-50.0, 50.0], [0.01, 10.0], [0.0, 10.0]]
 
 fit = PyROA.Fit(datadir, objName, filters, priors, add_var=True) 
 ````
 
 
 
 Priors are uniform where the limits are specified in the following way:
 
 priors = [[A_lower, A_upper], [B_lower, B_upper], [tau_lower, tau_upper],[delta_lower, delta_upper], [sig_lower, sig_upper]]. In the above these limits are large but here is a quick rundown of what they mean:
-- The first parameter here is A, which the rms of each lightcurve (there is an A1, A2, A3 for three lightcurves) and must be positive hence some limits between 0 and some large value are appropriate. A1, A2, A3 share the same uniform prior. 
-- The next parameter, B, represents the mean of each lightcurve (there is an B1, B2, B3 for three lightcurves). 
+- The first parameter here is A, which the rms of each lightcurve (there is an A1, A2, A3 for three lightcurves). The user specified limits are fractions of the calculates rms for each raw lightcurve. This allows the true limits to be different for each lightcurve which is especially important if the scales drstically vary between lightcurves. Limits if [0.5, 2.0] should be sufficient for all use cases.
+- The next parameter, B, represents the mean of each lightcurve (there is an B1, B2, B3 for three lightcurves). This is similarly specified as a fraction of the calcualted mean of each lightcurve.  Limits if [0.5, 2.0] should be sufficient for all use cases.
 - Next, tau, is the time delay between lightcurves (here there is only tau2, tau3) and so this prior range gives the range of lags explored by the model. 
 - The next parameter delta gives the width of the window function which must be positive and non-zero. If your probability is returning nan, it may be because the lower limit on this prior is too small. 
 - The final parameter is the extra error parameter, which again is positive.
 
 Per lightcurve there are 4 parameters: A, B, tau, sig, with tau=0 for the first lightcurve.
 Delta controls the flexability of the running optimal average which is calculated using all of the lightcurves.
```

### Comparing `PyROA-3.2.0/setup.py` & `PyROA-3.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # upload to pip
 # pip install .
 # python3 setup.py sdist bdist_wheel
 # twine upload dist/pydoppler-0.1.8.tar.gz
 
 setuptools.setup(
      name='PyROA',
-     version='3.2.0',
+     version='3.2.1',
      packages=['PyROA'] ,
      author="Fergus Donnan,",
      author_email="fergus.donnan@physics.ox.ac.uk",
      description="PyROA is a tool for modelling quasar lightcurves",
    long_description_content_type="text/markdown",
      url="https://github.com/FergusDonnan/PyROA",
      classifiers=[
```

