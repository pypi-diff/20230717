# Comparing `tmp/gwdali-0.0.6.tar.gz` & `tmp/gwdali-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.0.6.tar", last modified: Wed Jun 21 17:19:34 2023, max compression
+gzip compressed data, was "gwdali-0.0.7.tar", last modified: Mon Jul 17 17:55:10 2023, max compression
```

## Comparing `gwdali-0.0.6.tar` & `gwdali-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.928870 gwdali-0.0.6/GWDALI/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.936870 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/
--rw-r--r--   0 josiel    (1000) josiel    (1000)    78018 2022-08-02 22:07:44.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_CE.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    78021 2022-12-22 19:03:32.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_ET.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    83058 2021-03-30 20:13:46.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_K.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    56323 2022-05-06 19:34:28.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_L.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)    84000 2020-01-20 12:10:56.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_V.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.6/GWDALI/Detectors_Sensitivity/plot_Sn.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     9246 2023-06-12 01:59:52.000000 gwdali-0.0.6/GWDALI/GWDALI.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.6/GWDALI/__init__.py
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/GWDALI/lib/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.6/GWDALI/lib/Angles_lib.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4176 2023-06-21 16:21:27.000000 gwdali-0.0.6/GWDALI/lib/Compute_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.6/GWDALI/lib/Corner_Plots.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5713 2023-06-12 02:03:46.000000 gwdali-0.0.6/GWDALI/lib/Derivatives_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.6/GWDALI/lib/Dictionaries.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8121 2023-06-09 16:38:20.000000 gwdali-0.0.6/GWDALI/lib/Likelihood.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1714 2023-06-21 16:06:21.000000 gwdali-0.0.6/GWDALI/lib/Symmetric_Indexies.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4650 2023-06-12 18:15:33.000000 gwdali-0.0.6/GWDALI/lib/Waveforms.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.6/GWDALI/lib/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.6/LICENSE
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-21 17:19:34.940870 gwdali-0.0.6/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.6/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-21 17:19:34.940870 gwdali-0.0.6/gwdali.egg-info/
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/PKG-INFO
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      703 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/SOURCES.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/dependency_links.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-21 17:19:34.000000 gwdali-0.0.6/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-21 17:19:34.940870 gwdali-0.0.6/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      760 2023-06-21 17:18:53.000000 gwdali-0.0.6/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-07-17 17:55:10.974619 gwdali-0.0.7/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-07-17 17:55:10.950618 gwdali-0.0.7/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-07-17 17:55:10.958619 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)    78018 2022-08-02 22:07:44.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_CE.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)    78021 2022-12-22 19:03:32.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_ET.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)    83058 2021-03-30 20:13:46.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_K.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)    56323 2022-05-06 19:34:28.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_L.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)    84000 2020-01-20 12:10:56.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_V.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/__init__.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.7/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     9257 2023-07-17 16:02:50.000000 gwdali-0.0.7/GWDALI/GWDALI.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.7/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-07-17 17:55:10.970619 gwdali-0.0.7/GWDALI/lib/
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.7/GWDALI/lib/Angles_lib.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     4131 2023-07-17 15:26:49.000000 gwdali-0.0.7/GWDALI/lib/Compute_Tensors.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.7/GWDALI/lib/Corner_Plots.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     6014 2023-07-17 15:27:27.000000 gwdali-0.0.7/GWDALI/lib/Derivatives_Tensors.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     2685 2023-07-17 15:26:04.000000 gwdali-0.0.7/GWDALI/lib/Dictionaries.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     8121 2023-06-09 16:38:20.000000 gwdali-0.0.7/GWDALI/lib/Likelihood.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     1714 2023-06-21 16:06:21.000000 gwdali-0.0.7/GWDALI/lib/Symmetric_Indexies.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     4784 2023-07-17 16:22:23.000000 gwdali-0.0.7/GWDALI/lib/Waveforms.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.7/GWDALI/lib/__init__.py
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.7/LICENSE
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5171 2023-07-17 17:55:10.970619 gwdali-0.0.7/PKG-INFO
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     4822 2023-07-17 17:42:50.000000 gwdali-0.0.7/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-07-17 17:55:10.970619 gwdali-0.0.7/gwdali.egg-info/
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)     5171 2023-07-17 17:55:10.000000 gwdali-0.0.7/gwdali.egg-info/PKG-INFO
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)      703 2023-07-17 17:55:10.000000 gwdali-0.0.7/gwdali.egg-info/SOURCES.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)        1 2023-07-17 17:55:10.000000 gwdali-0.0.7/gwdali.egg-info/dependency_links.txt
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)        7 2023-07-17 17:55:10.000000 gwdali-0.0.7/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-07-17 17:55:10.974619 gwdali-0.0.7/setup.cfg
+-rwxr-xr-x   0 josiel    (1000) josiel    (1000)      760 2023-07-17 17:54:45.000000 gwdali-0.0.7/setup.py
```

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_CE.txt` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_CE.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_ET.txt` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_ET.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_K.txt` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_K.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_L.txt` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_L.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/Sn_V.txt` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/Sn_V.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/Detectors_Sensitivity/plot_Sn.py` & `gwdali-0.0.7/GWDALI/Detectors_Sensitivity/plot_Sn.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/GWDALI.py` & `gwdali-0.0.7/GWDALI/GWDALI.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from time import time as now
 from tqdm import trange
 
 cosmo = FlatLambdaCDM(70,0.3)
 
 #-------------------------------------------------
 # From Dictionaries.py
-Waveforms, PSD, labels_tex = gwdict.Load_Dictionaries()
+PSD, labels_tex = gwdict.Load_Dictionaries()
 #-------------------------------------------------
 freq0 = 10**np.linspace(0,4,4000)
 
 #-------------------------------------------------------------------------------
 #	"Compute the (Moore-Penrose) pseudo-inverse of a matrix"
 #-------------------------------------------------------------------------------
 def invert_matrix(matrix, rcond): 
@@ -59,28 +59,28 @@
 		func_Sn = interp1d(freq0, Sn0, fill_value=np.inf, bounds_error=False)
 		detectors[idx]['freq'] = freq
 		detectors[idx]['Sn']   = func_Sn(freq)
 
 		h 	  = gwfunc.Signal(gw_prms, det, approximant)
 		SNR2  = gwfunc.ScalarProduct(det['freq'], det['Sn'],h,h)
 		rho2 += SNR2
-
+		print('#####'*10)
 		Strains.append(h)
 		SNR.append(np.sqrt(SNR2))
 
 	hp, hx = gwfunc.GW_Polarizations(gw_prms,freq, approximant)
 
 	return [hp,hx,freq], Strains, SNR, np.sqrt(rho2)
 #-------------------------------------------------------
 # Main Function
 #-------------------------------------------------------
 def GWDALI( Detection_Dict, 
 			FreeParams, 
 			detectors, 
-			approximant = 'TaylorF2',
+			approximant = 'TaylorF2_py',
 			fmin  = 1., 
 			fmax  = 1.e4, 
 			fsize = 3000, 
 			dali_method    = 'Doublet',
 			sampler_method = 'nestle', 
 			npoints      = 100,
 			rcond		 = 1.e-4,
```

### Comparing `gwdali-0.0.6/GWDALI/lib/Angles_lib.py` & `gwdali-0.0.7/GWDALI/lib/Angles_lib.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/lib/Compute_Tensors.py` & `gwdali-0.0.7/GWDALI/lib/Compute_Tensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os, sys
 import numpy as np
-import GWDALI.lib.Waveforms as wf
 import GWDALI.lib.Angles_lib as geo
 import GWDALI.lib.Dictionaries as gwdict
 import GWDALI.lib.Derivatives_Tensors as gwfunc
 import GWDALI.lib.Symmetric_Indexies as sym
 
 from itertools import permutations
 from tqdm import trange
 
 deg2rad = np.pi/180
 
-Waveforms, PSD, labels_tex = gwdict.Load_Dictionaries()
+PSD, labels_tex = gwdict.Load_Dictionaries()
 
 def get_idx(idxs,Np):
 	n = len(idxs)-1 ; IdxP = 0
 	for i in range(len(idxs)): 
 		IdxP += idxs[i]*Np**n ; n-=1
 	return IdxP
```

### Comparing `gwdali-0.0.6/GWDALI/lib/Corner_Plots.py` & `gwdali-0.0.7/GWDALI/lib/Corner_Plots.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/lib/Derivatives_Tensors.py` & `gwdali-0.0.7/GWDALI/lib/Derivatives_Tensors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import numpy as np
+import GWDALI.lib.Waveforms as wf
 import GWDALI.lib.Angles_lib as geo
 import GWDALI.lib.Dictionaries as gwdict
 
 rad = np.pi/180
 deg = 1./rad
 
 c = 3.e8
 R_earth = 6371.e3
 
-Waveforms, PSD, labels_tex = gwdict.Load_Dictionaries()
+PSD, labels_tex = gwdict.Load_Dictionaries()
 
 def Pattern_Func(alpha,beta,psi,shape): # signs fixed
 	Coeff = np.sin(shape) #np.sqrt(3.)/2
-	fp = Coeff*( 0.5*(1+np.cos(beta)**2)*np.cos(2*alpha) )
-	fx = -Coeff*( np.cos(beta)*np.sin(2*alpha) )
-	
-	Fp =  fp*np.cos(2*psi) + fx*np.sin(2*psi)
-	Fx = -fp*np.sin(2*psi) + fx*np.cos(2*psi)
+	fp = Coeff*( 0.5*(1.+np.cos(beta)**2)*np.cos(2.*alpha) )
+	fx = -Coeff*( np.cos(beta)*np.sin(2.*alpha) )
 	
+	Fp =  fp*np.cos(2.*psi) + fx*np.sin(2.*psi)
+	Fx = -fp*np.sin(2.*psi) + fx*np.cos(2.*psi)
+	#print('alpha,beta,psi:%.2f, %.2f, %.2f'% (alpha,beta,psi), end='\t')
+	#print('\nFp, Fx:', Fp, Fx,'\tFp^2+Fx^2',Fp**2+Fx**2,'\t psi_det:',psi,'\n')
+	#print('Fp^2+Fx^2:%.2f' % (Fp**2+Fx**2) , ' ; Fp, Fx: %.2f, %.2f' %(Fp, Fx))
 	return Fp, Fx
 
 #-------------------------------------------------
 def Integral(x,y):
 	return np.sum( np.array( [0.5*(y[i]+y[i-1])*(x[i]-x[i-1]) for i in range(1,len(x)) ] ) )
 
 def ScalarProduct(freq,Sn,A,B):
@@ -57,15 +60,15 @@
 	sx2 = params['sx2']
 	sy2 = params['sy2']
 	sz2 = params['sz2']
 
 	s1 = [sx1, sy1, sz1]
 	s2 = [sx2, sy2, sz2]
 
-	hp, hx, _ = Waveforms[approximant](m1,m2,iota,DL,s1,s2,freq)
+	hp, hx, _ = wf.Waveforms(m1,m2,iota,DL,s1,s2,freq, approx=approximant)
 
 	return hp, hx
 
 def Signal(params, detector, approximant):
 	alpha    = params['RA']*rad       # rad
 	beta     = (90-params['Dec'])*rad # rad
 	iota     = params['iota']         # rad
@@ -80,14 +83,15 @@
 	rot   = detector['rot']*rad # rad
 
 	phi   = lon*rad
 	theta = (90-lat)*rad
 
 	alpha_obs, beta_obs = geo.AngTransf(alpha,beta,theta,phi,rot)
 	psi_obs             = geo.poll_ang(alpha,beta,iota,psi,theta,phi,rot)
+	#psi_obs = psi # Adding by hand!!!
 
 	t_delay = -np.cos(beta_obs)*R_earth/c
 
 	Fp, Fx = Pattern_Func(alpha_obs,beta_obs,psi_obs,detector['shape']*rad)
 	hp, hx = GW_Polarizations(params, freq, approximant)
 
 	exp2 = np.exp(-1.j*phi_coal)
```

### Comparing `gwdali-0.0.6/GWDALI/lib/Dictionaries.py` & `gwdali-0.0.7/GWDALI/lib/Dictionaries.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 import numpy as np
 from scipy.interpolate import interp1d
 from pathlib import Path
 
-import GWDALI.lib.Waveforms as wf
-
-#------------------------------------------------------
-# PATTERN FUNCTIONS AND WAVEFORMS
-#------------------------------------------------------
-
 dets = ['ET','CE','aLIGO','aVirgo','KAGRA']
 
-Waveforms = {}
-Waveforms['Leading_Order'] = wf.Waveform_Simple
-Waveforms['TaylorF2']      = wf.Waveform_TaylorF2
-try:
-	Waveforms['TaylorF2_lal']  = wf.Waveform_TaylorF2_lal
-	Waveforms['IMRPhenomD']    = wf.Waveform_IMRPhenomD
-	Waveforms['IMRPhenomP']    = wf.Waveform_IMRPhenomP
-except:
-	pass
-
 #------------------------------------------------------
 # DETECTORS SENSITIVITY
 #------------------------------------------------------
 
 path = Path(__file__).parent / '../Detectors_Sensitivity/'
 
 data_LIGO  = np.loadtxt(path / 'Sn_L.txt')
@@ -90,10 +74,10 @@
 labels_tex['sy2']      = '$S_{y,2}$'
 labels_tex['sz2']      = '$S_{z,2}$'
 
 labels_tex['RA']  = '$RA$ [deg]'
 labels_tex['Dec'] = '$Dec$ [deg]'
 
 def Load_Dictionaries():
-	return Waveforms, PSD, labels_tex
+	return PSD, labels_tex
 
 #------------------------------------------------------
```

### Comparing `gwdali-0.0.6/GWDALI/lib/Likelihood.py` & `gwdali-0.0.7/GWDALI/lib/Likelihood.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/lib/Symmetric_Indexies.py` & `gwdali-0.0.7/GWDALI/lib/Symmetric_Indexies.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/GWDALI/lib/Waveforms.py` & `gwdali-0.0.7/GWDALI/lib/Waveforms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.interpolate import interp1d
+from scipy.interpolate import interp1d, CubicSpline
 
 wrn =\
 '''
 =======================================================
     WARNING: lalsuite or lalsimulation not instaled!
     Try to install them with: 
     \033[1m conda install -c conda-forge lalsuite \033[0m
@@ -47,15 +47,15 @@
 	hc = hc.data.data
 	
 	N = len(hp)
 	freqWF = np.linspace(0,dF*(N-1),N)
 	
 	func_hp = interp1d(freqWF, hp, fill_value=0, kind='linear', bounds_error=False)
 	func_hc = interp1d(freqWF, hc, fill_value=0, kind='linear', bounds_error=False)
-	
+
 	Hp = func_hp(freq)
 	Hx = func_hc(freq)
 
 	hp1 , hp2 = Hp.real, Hp.imag
 	hx1 , hx2 = Hx.real, Hp.imag
 
 	hp1 = np.nan_to_num(hp1)
@@ -64,23 +64,14 @@
 	hx2 = np.nan_to_num(hx2)
 
 	Hp = hp1 +1.j*hp2
 	Hx = hx1 +1.j*hx2
 	
 	return Hp, Hx, freq
 
-def Waveform_TaylorF2_lal(m1, m2, iota, DL, s1, s2, freq):
-	return Waveform_lal(m1, m2, iota, DL, s1, s2, freq, 'TaylorF2')
-
-def Waveform_IMRPhenomD(m1, m2, iota, DL, s1, s2, freq):	
-	return Waveform_lal(m1, m2, iota, DL, s1, s2, freq, 'IMRPhenomD')
-
-def Waveform_IMRPhenomP(m1, m2, iota, DL, s1, s2, freq):
-	return Waveform_lal(m1, m2, iota, DL, s1, s2, freq, 'IMRPhenomP')
-
 #==============================================================================================
 # PYTHON WAVEFORMS ( Leading Order and TaylorF2(3.5PN) )
 #==============================================================================================
 
 def GW_Amplitude(m1,m2,DL,freq):
 	DL *= 3.086e22     # DL [meters]
 	M = m1+m2			 # Total Mass
@@ -122,15 +113,17 @@
 		add += A[idx]*(np.pi*GM_c3*freq)**((idx-5)/3)
 	add *= 3./(128*eta)
 
 	t_coal, phi_coal = 0, 0
 	phase = 2*np.pi*freq*t_coal + phi_coal + add
 
 	return phase
-	
+
+#-----------------------------------------------------------------------------------------------
+
 def Waveform_TaylorF2(m1, m2, iota, DL, s1, s2, freq): # Sathyaprakash-Schutz(2009)
 	Amp   = GW_Amplitude(m1,m2,DL,freq)
 	phase = GW_Phase_TaylorF2(m1,m2,freq)
 	
 	exp = np.exp(1.j*(phase-np.pi/4))
 
 	cos_iota = np.cos(iota)
@@ -144,8 +137,18 @@
 	Amp = GW_Amplitude(m1,m2,DL,freq)
 	phase = GW_Phase_Simple(m1,m2,freq)
 	
 	cos_iota = np.cos(iota)
 	Gp, Gx = 0.5*(1.+cos_iota*cos_iota), cos_iota
 	Hplus  = Gp*Amp*np.exp(1.j*(phase-np.pi/4))
 	Hcross = Gx*Amp*np.exp(1.j*(phase+np.pi/4))
-	return Hplus, Hcross, freq
+	return Hplus, Hcross, freq
+
+#-----------------------------------------------------------------------------------------------
+
+def Waveforms(m1, m2, iota, DL, s1, s2, freq, approx):
+	if approx == 'Leading_Order':
+		return Waveform_Simple(m1, m2, iota, DL, s1, s2, freq)
+	elif approx == 'TaylorF2_py':
+		return Waveform_TaylorF2(m1, m2, iota, DL, s1, s2, freq)
+	else:
+		return Waveform_lal(m1, m2, iota, DL, s1, s2, freq, approx)
```

### Comparing `gwdali-0.0.6/LICENSE` & `gwdali-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/PKG-INFO` & `gwdali-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-Metadata-Version: 2.1
-Name: gwdali
-Version: 0.0.6
-Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
-Author: Josiel Mendonça Soares de Souza
-Author-email: jmsdsouza.phd@gmail.com
-License: MIT License
-Keywords: fisher matrix,gravitational waves,gw,dali
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **GWDALI Software**
 
 Software developed to perform parameter estimations of gravitational waves from compact objects coalescence (CBC) via Gaussian and Beyond-Gaussian approximation of GW likelihood. The Gaussian approximation is related to Fisher Matrix, from which it is direct to compute the covariance matrix by inverting the Fisher Matrix **[1]**. GWDALI also deals with the not-so-infrequent cases of Fisher Matrix with zero-determinant. The Beyond-Gaussian approach uses the Derivative Approximation for LIkelihoods (DALI) algorithm proposed in **[2]** and applied to gravitational waves in **[3]**, whose model parameter uncertainties are estimated via Monte Carlo sampling but less costly than using the GW likelihood with no approximation.
 
 
 ## Installation
 
 To install the software run the command below:
 
 ```
 $ pip install gwdali
 ```
+
+## Documentation
+
+Available in [https://gwdali.readthedocs.io/en/latest/](https://gwdali.readthedocs.io/en/latest/)
     
 ## Usage [example]
     import numpy as np
     #-------------------
     import GWDALI as gw
     #-------------------
     from tqdm import trange
@@ -66,23 +59,23 @@
     params['sz1'] = 0
     params['sx2'] = 0
     params['sy2'] = 0
     params['sz2'] = 0
 
     #----------------------------------------------------------------------
     # "approximant" options:
-    #               [Leading_Order, TaylorF2, TaylorF2_lal, IMRPhenomP, IMRPhenomD]
+    #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
     res = gw.GWDALI( Detection_Dict = params,
                      FreeParams     = FreeParams,
                      detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2',
+                     approximant    = 'TaylorF2_py',
                      dali_method    = 'Doublet',
                      sampler_method = 'nestle', # Same as Bilby sampling method
                      save_fisher    = False,
                      save_cov       = False,
                      plot_corner    = False,
                      save_samples   = False,
                      hide_info      = True,
@@ -109,8 +102,8 @@
 ## Authors
 
 - **Josiel Mendonça Soares de Souza** (developer)
 - **Riccardo Sturani** (collaborator)
 
 ## License
 
-MIT License
+MIT License
```

### Comparing `gwdali-0.0.6/README.md` & `gwdali-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+Metadata-Version: 2.1
+Name: gwdali
+Version: 0.0.7
+Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
+Author: Josiel Mendonça Soares de Souza
+Author-email: jmsdsouza.phd@gmail.com
+License: MIT License
+Keywords: fisher matrix,gravitational waves,gw,dali
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # **GWDALI Software**
 
 Software developed to perform parameter estimations of gravitational waves from compact objects coalescence (CBC) via Gaussian and Beyond-Gaussian approximation of GW likelihood. The Gaussian approximation is related to Fisher Matrix, from which it is direct to compute the covariance matrix by inverting the Fisher Matrix **[1]**. GWDALI also deals with the not-so-infrequent cases of Fisher Matrix with zero-determinant. The Beyond-Gaussian approach uses the Derivative Approximation for LIkelihoods (DALI) algorithm proposed in **[2]** and applied to gravitational waves in **[3]**, whose model parameter uncertainties are estimated via Monte Carlo sampling but less costly than using the GW likelihood with no approximation.
 
 
 ## Installation
 
 To install the software run the command below:
 
 ```
 $ pip install gwdali
 ```
+
+## Documentation
+
+Available in [https://gwdali.readthedocs.io/en/latest/](https://gwdali.readthedocs.io/en/latest/)
     
 ## Usage [example]
     import numpy as np
     #-------------------
     import GWDALI as gw
     #-------------------
     from tqdm import trange
@@ -55,23 +70,23 @@
     params['sz1'] = 0
     params['sx2'] = 0
     params['sy2'] = 0
     params['sz2'] = 0
 
     #----------------------------------------------------------------------
     # "approximant" options:
-    #               [Leading_Order, TaylorF2, TaylorF2_lal, IMRPhenomP, IMRPhenomD]
+    #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
     res = gw.GWDALI( Detection_Dict = params,
                      FreeParams     = FreeParams,
                      detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2',
+                     approximant    = 'TaylorF2_py',
                      dali_method    = 'Doublet',
                      sampler_method = 'nestle', # Same as Bilby sampling method
                      save_fisher    = False,
                      save_cov       = False,
                      plot_corner    = False,
                      save_samples   = False,
                      hide_info      = True,
@@ -98,8 +113,8 @@
 ## Authors
 
 - **Josiel Mendonça Soares de Souza** (developer)
 - **Riccardo Sturani** (collaborator)
 
 ## License
 
-MIT License
+MIT License
```

### Comparing `gwdali-0.0.6/gwdali.egg-info/PKG-INFO` & `gwdali-0.0.7/gwdali.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,14 +17,18 @@
 ## Installation
 
 To install the software run the command below:
 
 ```
 $ pip install gwdali
 ```
+
+## Documentation
+
+Available in [https://gwdali.readthedocs.io/en/latest/](https://gwdali.readthedocs.io/en/latest/)
     
 ## Usage [example]
     import numpy as np
     #-------------------
     import GWDALI as gw
     #-------------------
     from tqdm import trange
@@ -66,23 +70,23 @@
     params['sz1'] = 0
     params['sx2'] = 0
     params['sy2'] = 0
     params['sz2'] = 0
 
     #----------------------------------------------------------------------
     # "approximant" options:
-    #               [Leading_Order, TaylorF2, TaylorF2_lal, IMRPhenomP, IMRPhenomD]
+    #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
     res = gw.GWDALI( Detection_Dict = params,
                      FreeParams     = FreeParams,
                      detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2',
+                     approximant    = 'TaylorF2_py',
                      dali_method    = 'Doublet',
                      sampler_method = 'nestle', # Same as Bilby sampling method
                      save_fisher    = False,
                      save_cov       = False,
                      plot_corner    = False,
                      save_samples   = False,
                      hide_info      = True,
```

### Comparing `gwdali-0.0.6/gwdali.egg-info/SOURCES.txt` & `gwdali-0.0.7/gwdali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.6/setup.py` & `gwdali-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.0.6',
+	version = '0.0.7',
 	license = 'MIT License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'jmsdsouza.phd@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
```

