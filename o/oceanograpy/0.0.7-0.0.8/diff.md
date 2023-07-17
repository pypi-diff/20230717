# Comparing `tmp/oceanograpy-0.0.7.tar.gz` & `tmp/oceanograpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanograpy-0.0.7.tar", last modified: Tue Jul 11 20:56:04 2023, max compression
+gzip compressed data, was "oceanograpy-0.0.8.tar", last modified: Mon Jul 17 17:29:16 2023, max compression
```

## Comparing `oceanograpy-0.0.7.tar` & `oceanograpy-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.241185 oceanograpy-0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      782 2023-07-11 20:56:04.240185 oceanograpy-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.218187 oceanograpy-0.0.7/oceanograpy/
--rw-rw-rw-   0        0        0      202 2023-07-11 20:55:23.000000 oceanograpy-0.0.7/oceanograpy/__init__.py
--rw-rw-rw-   0        0        0    24735 2023-07-11 18:15:27.000000 oceanograpy-0.0.7/oceanograpy/adcp_plot_tools.py
--rw-rw-rw-   0        0        0     2434 2023-07-11 20:22:37.000000 oceanograpy-0.0.7/oceanograpy/example.py
--rw-rw-rw-   0        0        0     2820 2023-07-11 20:50:48.000000 oceanograpy-0.0.7/oceanograpy/frma.py
--rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.7/oceanograpy/matplotlib_dhi.py
--rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.7/oceanograpy/processing_tools.py
--rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.7/oceanograpy/seabird_ctd.py
--rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.7/oceanograpy/workhorse_adcp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.239186 oceanograpy-0.0.7/oceanograpy.egg-info/
--rw-rw-rw-   0        0        0      782 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 20:56:04.241185 oceanograpy-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-11 20:55:57.000000 oceanograpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:29:16.723831 oceanograpy-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      782 2023-07-17 17:29:16.722814 oceanograpy-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 17:29:16.699849 oceanograpy-0.0.8/oceanograpy/
+-rw-rw-rw-   0        0        0      202 2023-07-11 20:55:23.000000 oceanograpy-0.0.8/oceanograpy/__init__.py
+-rw-rw-rw-   0        0        0    14353 2023-07-13 15:51:52.000000 oceanograpy-0.0.8/oceanograpy/adcp_data_visualizer.py
+-rw-rw-rw-   0        0        0    25061 2023-07-12 01:22:38.000000 oceanograpy-0.0.8/oceanograpy/adcp_plot_tools.py
+-rw-rw-rw-   0        0        0    18773 2023-07-14 18:51:13.000000 oceanograpy-0.0.8/oceanograpy/data_visualizer.py
+-rw-rw-rw-   0        0        0     8323 2023-07-14 18:37:53.000000 oceanograpy-0.0.8/oceanograpy/example.py
+-rw-rw-rw-   0        0        0     2820 2023-07-11 20:50:48.000000 oceanograpy-0.0.8/oceanograpy/frma.py
+-rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.8/oceanograpy/matplotlib_dhi.py
+-rw-rw-rw-   0        0        0     6007 2023-07-17 17:27:02.000000 oceanograpy-0.0.8/oceanograpy/processing_tools.py
+-rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.8/oceanograpy/seabird_ctd.py
+-rw-rw-rw-   0        0        0     1199 2023-07-17 17:07:23.000000 oceanograpy-0.0.8/oceanograpy/stones.py
+-rw-rw-rw-   0        0        0     9471 2023-07-12 22:46:23.000000 oceanograpy-0.0.8/oceanograpy/visualizer_template.py
+-rw-rw-rw-   0        0        0    79955 2023-07-13 23:46:15.000000 oceanograpy-0.0.8/oceanograpy/workhorse_adcp.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:29:16.720812 oceanograpy-0.0.8/oceanograpy.egg-info/
+-rw-rw-rw-   0        0        0      782 2023-07-17 17:29:16.000000 oceanograpy-0.0.8/oceanograpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-07-17 17:29:16.000000 oceanograpy-0.0.8/oceanograpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 17:29:16.000000 oceanograpy-0.0.8/oceanograpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 17:29:16.000000 oceanograpy-0.0.8/oceanograpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 17:29:16.724811 oceanograpy-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-17 17:28:00.000000 oceanograpy-0.0.8/setup.py
```

### Comparing `oceanograpy-0.0.7/LICENSE` & `oceanograpy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.7/PKG-INFO` & `oceanograpy-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.7/oceanograpy/adcp_plot_tools.py` & `oceanograpy-0.0.8/oceanograpy/adcp_plot_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib.collections import LineCollection
 import matplotlib.ticker as mticker
 
 from matplotlib_dhi import *
 from matplotlib_dhi import subplots
+
+import cmocean
 def import_multiple_pd0(paths,labels):
     '''
     reads multiple Workhorse ADCP files from a list of filepaths
 
 
     Parameters
     ----------
@@ -361,21 +363,28 @@
             X = np.flipud(X)
             extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
         return X,extent
         
     
     cmaps = {'PERCENT GOOD': plt.cm.bone,
              'ECHO INTENSITY': plt.cm.turbo,
-             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral}
+             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral,
+             'ABSOLUTE BACKSCATTER':cmocean.cm.thermal,
+             'SIGNAL TO NOISE RATIO':plt.cm.bone_r}
     cmap = cmaps[field]
     
     
+    for x in [x1,x2,x3,x4]:
+        x[x == 32768] = np.nan
+    
+    
     vmin = np.nanmin([x1,x2,x3,x4])
     vmax = np.nanmax([x1,x2,x3,x4])
     print(vmin)
+    print(vmax)
     
     x1,extent = get_plot_extent(x1)
     im = ax[0].imshow(x1, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
     
     x2,extent = get_plot_extent(x2)
     im = ax[1].imshow(x2, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
     
@@ -509,15 +518,17 @@
     else:
         x = np.flipud(x)
         extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
         
         
     cmaps = {'PERCENT GOOD': plt.cm.bone,
              'ECHO INTENSITY': plt.cm.turbo,
-             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral}
+             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral,
+             'ABSOLUTE BACKSCATTER':cmocean.cm.thermal,
+             'SIGNAL TO NOISE RATIO':plt.cm.Reds}
     cmap = cmaps[field]
     
     
     im = ax.imshow(x, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
     cbar = fig.colorbar(im, ax=ax,orientation="vertical",location = 'right',fraction=0.046)
     
     if beam == 0:
```

### Comparing `oceanograpy-0.0.7/oceanograpy/frma.py` & `oceanograpy-0.0.8/oceanograpy/frma.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.7/oceanograpy/matplotlib_dhi.py` & `oceanograpy-0.0.8/oceanograpy/matplotlib_dhi.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.7/oceanograpy/seabird_ctd.py` & `oceanograpy-0.0.8/oceanograpy/seabird_ctd.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.7/oceanograpy/workhorse_adcp.py` & `oceanograpy-0.0.8/oceanograpy/workhorse_adcp.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 @author: anba
 """
 
 import struct, os, datetime, numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
-
+from scipy import ndimage
+from processing_tools import processing_tools as ptools 
 # import os
 # import datetime
 # import numpy as np
 
 
 # import scipy as sp
 # import scipy.ndimage as ndimage
@@ -934,14 +935,47 @@
 
     '''
     
     theta = theta*np.pi/180
     R = np.array([[np.cos(theta),-np.sin(theta)],[np.sin(theta),np.cos(theta)]])
     return np.dot(R,X)
 
+
+def map_unsigned_2byte_integers_to_range(x,minval,maxval, lsd = None):
+    """
+    Function for converting 2-byte unsigned integers to the a specified range. 
+    It is assumed that input values in x are spanned by [0,65535]. The list 
+    will be mapped such that 0 is taken to minval, and 65535 is taken to maxval.
+
+    Parameters
+    ----------
+    x : list or list-like
+        values to scale
+    maxval : float
+        maximum value in scaled range.
+    minval : TYPE
+        maximum value for scale range.
+    lsd : int (optional)
+        If supplied, the scaled list will be rounded to the specified least significant digit place (e.g., 0 = 1, 1 = 0.1, 2 = 0.01). 
+
+    Returns
+    -------
+    x_scl : list or list-like (same as input)
+        scaled list of values with range [minval,maxval] 
+
+    """
+    
+    
+    x_scl = (x/65535)*(maxval - minval) + minval
+    #scaled = ((x- min(x))/(max(x) - min(x)))*(maxval - minval) + minval
+    
+    if lsd: 
+        x_scl = np.round(x_scl,lsd)
+    return x_scl
+
 #%%#####################  formatting information for pd0 fields ###############
  
 ## fields to parse (NAME, NUMBER OF BYTES TO READ, BYTE CONVENTION, DECODE)
 ensemble_header_fields = [('HEADER ID',1,'Little Endian',True),
                           ('DATA SOURCE ID',1,'Little Endian',True),
                           ('N BYTES IN ENSEMBLE',2,'Little Endian',True),
                           ('SPARE',1,'Little Endian',True),
@@ -1131,14 +1165,16 @@
         self.filepath = filepath
         self.PT3_filepath = PT3_filepath 
         self.timezone_correction = timezone_correction
         self.magnetic_deviation_correction = magnetic_deviation_correction
         self.instrument_depth = instrument_depth
         self.instrument_HAB = instrument_HAB
         
+        self.ensemble_fields = ['ECHO INTENSITY','CORRELATION MAGNITUDE','PERCENT GOOD']
+        
         if verbose == 1:
             _print = True
         else:
             _print = False
             
             
         if read_averages:
@@ -1158,23 +1194,20 @@
             elapsed_time = et - st
             print('\nExecution time:', elapsed_time, 'seconds')
         
         
 
         
         
-        
-        
-        # self.filter_echo_intensity_data()
+#        self.filter_echo_intensity_data()
     
-        # if PT3_filepath:
-        #     self.RSSI = read_PT3(self.PT3_filepath)
-        #     self.calculate_absolute_backscatter()
-        # else:
-        #     print('PT3 File not specified. Cannot calculate absolute backscatter')
+
+            
+            
+   
         
     def set_timezone_correction(self,timezone_correction):
         self.timezone_correction = timezone_correction
         self.ensemble_times = self.get_ensemble_datetimes()
         
     def set_magnetic_deviation_correction(self,magnetic_deviation_correction):
         self.magnetic_deviation_correction = magnetic_deviation_correction
@@ -1314,45 +1347,227 @@
         if self.beam_facing == 'DOWN':
             bin_midpoints_HAB = self.instrument_HAB - self.get_bin_midpoints()
         elif self.beam_facing =='UP':
             bin_midpoints_HAB = self.instrument_HAB + self.get_bin_midpoints()
             
         return bin_midpoints_HAB   
     
-    def get_transmit_pulse_lengths(self):
+    def get_sensor_transmit_pulse_lengths(self):
+        """
+        Get ADCP transmit pulse lengths. Data is from the ensemble variable headers.
+
+        Returns
+        -------
+        transmit_pulse_lengths : numpy array
+            ADCP transmit pule lengths. One value for each ensemble.
+
         """
-        Generate numpy array of transmit pulse distances. 
-        Args:
-            None
-        Returns:
-            numpy array with dimensions (n_ensembles)  
-        """          
         transmit_pulse_lengths = np.empty(self.n_ensembles)
-        
         for c,ensemble in enumerate(self.ensemble_data):
             transmit_pulse_lengths[c] = ensemble['FIXED LEADER']['XMIT PULSE LENGTH BASED ON {WT}']/100
         return transmit_pulse_lengths  
     
-    def get_temperature_data(self):
+    def get_sensor_temperature(self):
         """
-        Generate numpy array of temperature data recorded by ADCP in degrees C. 
-        Args:
-            None
-        Returns:
-            numpy array with dimensions (n_ensembles)  
+        Temperature of the water at the transducer head
+        (ET-command). This value may be a manual setting or a
+        reading from a temperature sensor.
+        Scaling: LSD = 0.01 degree; Range = -5.00 to +40.00 degrees
+        
+        Returns
+        -------
+        temperature : numpy array
+            ADCP temperature data in degrees C. One value for each ensemble.
 
-        """          
+        """
+        temperature = np.empty(self.n_ensembles)
         
-        temperature_data = np.empty(self.n_ensembles)
+        for c,ensemble in enumerate(self.ensemble_data):
+            temperature[c] = ensemble['VARIABLE LEADER']['TEMPERATURE {ET}']/100
+        #temperature = map_unsigned_2byte_integers_to_range(temperature,-5,40,lsd = 2)
+        return temperature
+    
+    def get_salinity(self):
+        """
+        Salinity value of the water at the transducer
+        head (ES-command). This value may be a manual setting or
+        a reading from a conductivity sensor.
+        Scaling: LSD = 1 part per thousand; Range = 0 to 40 ppt
         
+        Returns
+        -------
+        salinity : numpy array
+            One value for each ensemble.
+
+        """
+        salinity = np.empty(self.n_ensembles)
+        
+        for c,ensemble in enumerate(self.ensemble_data):
+            salinity[c] = ensemble['VARIABLE LEADER']['SALINITY {ES}']
+        #salinity = map_unsigned_2byte_integers_to_range(0,40,lsd = 2)
+        return salinity
+    
+    def get_sensor_pitch(self):
+        """
+        WorkHorse ADCP pitch angle (EP-command).
+        This value may be a manual setting or a reading from a tilt
+        sensor. Positive values mean that Beam #3 is spatially
+        higher than Beam #4.
+        Scaling: LSD = 0.01 degree; Range = -20.00 to +20.00 degrees
+        Returns
+        -------
+        pitch : numpy array
+            One value for each ensemble.
+
+        """
+        pitch = np.empty(self.n_ensembles)
         for c,ensemble in enumerate(self.ensemble_data):
-            temperature_data[c] = ensemble['VARIABLE LEADER']['TEMPERATURE {ET}']/100
-        return temperature_data
+            pitch[c] = ensemble['VARIABLE LEADER']['PITCH (TILT 1) {EP}']/100
+        ## per manual - scale from -20 to 20, LSD = 0.01 (2)
+        #pitch = map_unsigned_2byte_integers_to_range(pitch,-20,20,lsd = 2)
+        return pitch
+    
+    def get_sensor_roll(self):
+        """
+        WorkHorse ADCP roll angle (ER-command).
+        This value may be a manual setting or a reading from a tilt
+        sensor. For up-facing WorkHorse ADCPs, positive values
+        mean that Beam #2 is spatially higher than Beam #1. For
+        down-facing WorkHorse ADCPs, positive values mean that
+        Beam #1 is spatially higher than Beam #2.
+        Scaling: LSD = 0.01 degree; Range = -20.00 to +20.00 degrees
+
+        Returns
+        -------
+        roll : numpy array
+            One value for each ensemble.
 
+        """
+        roll = np.empty(self.n_ensembles)
+        for c,ensemble in enumerate(self.ensemble_data):
+            roll[c] = ensemble['VARIABLE LEADER']['ROLL (TILT 2) {ER}']/100
+        #roll = map_unsigned_2byte_integers_to_range(roll,-20,20,lsd = 2)
+        return roll
     
+    def get_sensor_heading(self):
+        """
+        WorkHorse ADCP heading angle (EHcommand).
+        This value may be a manual setting or a reading
+        from a heading sensor.
+        Scaling: LSD = 0.01 degree; Range = 000.00 to 359.99 degrees
+        
+        Returns
+        -------
+        heading : numpy array
+             One value for each ensemble.
+
+        """
+
+        heading = np.empty(self.n_ensembles)
+        for c,ensemble in enumerate(self.ensemble_data):
+            heading[c] = ensemble['VARIABLE LEADER']['HEADING {EH}']/100
+        #heading = map_unsigned_2byte_integers_to_range(heading,0,359.99,lsd = 2)
+        return heading
+    
+    def get_sensor_transducer_depth(self):
+        """
+        Depth of the transducer below the water surface
+        (ED-command). This value may be a manual setting or a
+        reading from a depth sensor.
+        Scaling: LSD = 1 decimeter; Range = 1 to 9999 decimeters
+        
+        Returns
+        -------
+        transducer_depth : numpy array
+             One value for each ensemble.
+
+        """
+
+        transducer_depth = np.empty(self.n_ensembles)
+        for c,ensemble in enumerate(self.ensemble_data):
+            transducer_depth[c] = ensemble['VARIABLE LEADER']['HEADING {EH}']
+        
+        transducer_depth = map_unsigned_2byte_integers_to_range(transducer_depth,0,9999,lsd = 2)
+        return heading
+    
+    def get_velocity(self):
+        """
+        Retrieve velocity vectors and calculate progressive vectors in m/s. Magnetic deviation correction is applied here. 
+    
+        Returns
+        -------
+        u : numpy array
+            u velocity
+        v : numpy array
+            v velocity
+        z : numpy array
+            z velocity.
+        du : numpy array
+            displacement in u direction.
+        dv : numpy array
+            displacement in v direction.
+        dz : numpy array
+            displacement in z direction.
+        err: numpy array
+            error velocity
+    
+        """
+        
+        global X,u,v
+        
+        
+        u = np.empty((self.n_ensembles,self.n_bins))
+        v = np.empty((self.n_ensembles,self.n_bins))
+        z = np.empty((self.n_ensembles,self.n_bins))
+        ev = np.empty((self.n_ensembles,self.n_bins))
+        for e,ensemble in enumerate(self.ensemble_data):
+            # cast velocity data as float
+            vel_data = np.array(ensemble['VELOCITY']).astype('float')
+            # mark nan values 
+            vel_data[vel_data==-32768] = np.nan
+            
+            # convert to m/s
+            vel_data = vel_data*.001
+
+
+            if len(vel_data) == self.n_bins:
+                u[e,:] = vel_data[:,0]
+                v[e,:] = vel_data[:,1]
+                z[e,:] = vel_data[:,2]
+                ev[e,:] = vel_data[:,3]
+            else:
+                u[e,:] = np.nan
+                v[e,:] = np.nan
+                z[e,:] = np.nan
+                ev[e,:] = np.nan
+            
+        # apply magnetic deviation correction
+        if self.magnetic_deviation_correction!=0:
+            #print(f'   Correcting for magnetic deviation ({self.magnetic_deviation_correction} degrees)')
+            for b in range(self.n_bins): # loop over all bins and calculate rotated velocites for each
+                X = np.array([u[:,b],v[:,b]])
+                X_rot = rotate(X,theta = self.magnetic_deviation_correction)
+                
+                # update u and v
+                u[:,b] = X_rot[0,:]
+                v[:,b] = X_rot[1,:]    
+                
+        ## gen prog vector components 
+        t = self.get_ensemble_datetimes()
+        to_sec = np.vectorize(lambda x: x.seconds) # vectorized function to convert datetime delta to total seconds
+        dt = np.empty(self.n_ensembles)
+        dt[:-1] = to_sec(np.diff(t))
+        dt[-1] = dt[-2] #assign last value
+        dt = np.outer(dt,np.ones(self.n_bins))
+        du = u*dt
+        dv = v*dt
+        dz = z*dt
+        
+        return u,v,z,ev     
+
     def get_bottom_track(self,beam_number):
         """
         
 
         Parameters
         ----------
         beam_number : int
@@ -1390,16 +1605,16 @@
             beam_number: beam number (integer). If no beam number is provided, the beam average (beam_number = 0) will be returned. 
             
         Returns:
             numpy array with dimensions (nbins,n_ensembles)  
 
         """    
         #check that field name is elegible
-        if not field_name in ["ECHO INTENSITY", "CORRELATION MAGNITUDE", "PERCENT GOOD", 'ABSOLUTE BACKSCATTER','FILTERED ECHO INTENSITY']:
-            raise ValueError('Invalid field name. Choose "ECHO INTENSITY", "CORRELATION MAGNITUDE", "PERCENT GOOD","ABSOLUTE BACKSCATTER","FILTERED ECHO INTENSITY"')
+        if not field_name in self.ensemble_fields:#["ECHO INTENSITY", "CORRELATION MAGNITUDE", "PERCENT GOOD", 'ABSOLUTE BACKSCATTER','FILTERED ECHO INTENSITY']:
+            raise ValueError(f'Invalid field name. Choose one of the following [self.ensemble_fields]')
 
         #check that beam_number is elegible
         if not beam_number in [0,1,2,3,4]:
             raise ValueError('Invalid beam number. Choose integer 0 (avg),1,2,3, or 4. ')
 
                
    
@@ -1423,35 +1638,51 @@
     
     def filter_echo_intensity_data(self):
         """
         Apply column-wise spike filter to echo intensity field of each ensemble, 
         then add to ensemble_data property of the WorkhorseADCP class 
         """
         X = np.empty((self.n_bins,self.n_ensembles,self.n_beams))
-        printProgressBar(0, self.n_beams,prefix = f'Filtering', taskname= f'Filtering 0%')
+        #printProgressBar(0, self.n_beams,prefix = f'Filtering', taskname= f'Filtering 0%')
         for beam in range(self.n_beams):
-            printProgressBar(beam+1, self.n_beams,prefix = f'Filtering {round(100*(beam+1)/self.n_beams,0)}%', taskname= f'Echo Intensity BM{beam+1}')
+            #printProgressBar(beam+1, self.n_beams,prefix = f'Filtering {round(100*(beam+1)/self.n_beams,0)}%', taskname= f'Echo Intensity BM{beam+1}')
             X[:,:,beam] = filter_echo_intensity_array(self.get_ensemble_array(field_name = 'ECHO INTENSITY', beam_number = beam+1))     
         self.append_to_ensembles(X,'FILTERED ECHO INTENSITY')
         
-    def calculate_absolute_backscatter(self):
+        
+    def calculate_absolute_backscatter(self,**kwargs):
         """
         Convert numpy array of ensemble data of echo intensity to absolute backscatter then added to ensemble_data property of the WorkhorseADCP class.
-        Args:
-            echo_intensity: numpy array of echo intensity data with dimensions (n_bins,n_ensembles,n_beams)
+
+
+        
+        Optional Args:
+            PT3_filepath - path to the instrument PT3 file
+            field_name : ensemble data type (string). "ECHO INTENSITY" (default), "CORRELATION MAGNITUDE", "PERCENT GOOD", or others added by the "append to ensembles" method.  
         
         """
         
-        global X
+        
+        
+        if self.PT3_filepath:
+            self.RSSI = read_PT3(self.PT3_filepath)
+        elif kwargs.get('PT3_filepath'):
+            self.RSSI = read_PT3(kwargs.get('PT3_filepath'))
+        else:
+            raise ValueError('PT3 File not specified. Cannot calculate absolute backscatter')
+            
+            
+        if kwargs.get('field_name'): field_name = kwargs.get('field_name')
+        else: field_name = 'ECHO INTENSITY'
         
         #self.filter_echo_intensity_data()
         #echo_intensity = self.get_ensemble_array(beam_number = 1)
-        temperature = np.outer(self.get_temperature_data(),np.ones(self.n_bins)).T
+        temperature = np.outer(self.get_sensor_temperature(),np.ones(self.n_bins)).T
         bin_distances = np.outer(self.get_bin_midpoints(),np.ones(self.n_ensembles))/np.cos(20*np.pi/180)#/100
-        transmit_pulse_lengths = np.outer(self.get_transmit_pulse_lengths(),np.ones(self.n_bins)).T#/100
+        transmit_pulse_lengths = np.outer(self.get_sensor_transmit_pulse_lengths(),np.ones(self.n_bins)).T#/100
         
         
         E_r =39 #nominal value provided by ViSea
         
         ## select these based on WB commmand (0 = 25%, 1 = 6.25%)
         
         WB = self.ensemble_data[0]['FIXED LEADER']['SYSTEM BANDWIDTH {WB}']
@@ -1489,132 +1720,210 @@
         #     alpha = 0.068
             
             
         global StN
         
         X = np.empty((self.n_bins,self.n_ensembles,self.n_beams))
         StN = np.empty((self.n_bins,self.n_ensembles,self.n_beams))
-        printProgressBar(0, self.n_beams,prefix = f'Calculating 0%', taskname= f'Absolute Backscatter 0%')
+        #printProgressBar(0, self.n_beams,prefix = f'Calculating 0%', taskname= f'Absolute Backscatter 0%')
         for beam in range(self.n_beams):
-            printProgressBar(beam+1, self.n_beams,prefix = f'Calculating {round(100*(beam+1)/self.n_beams,0)}%', taskname= f'Absolute Backscatter BM{beam+1}')
-            E = self.get_ensemble_array(field_name = 'FILTERED ECHO INTENSITY', beam_number = beam+1)
+            #printProgressBar(beam+1, self.n_beams,prefix = f'Calculating {round(100*(beam+1)/self.n_beams,0)}%', taskname= f'Absolute Backscatter BM{beam+1}')
+            E = self.get_ensemble_array(field_name = field_name, beam_number = beam+1)
             #E = self.get_ensemble_array(field_name = 'ECHO INTENSITY', beam_number = beam+1)
             
             
             StN[:,:,beam] = (10**(k_c[beam+1]*E/10) - 10**(k_c[beam+1]*E_r/10))/10**(k_c[beam+1]*E_r/10)
             
-            X[:,:,beam] = C + 10*np.log10((temperature + 273.16)*(bin_distances**2)) - 10*np.log10(transmit_pulse_lengths) - P_dbw + 2*alpha*bin_distances + 10*np.log10(10**(k_c[beam+1]*(E - E_r)/10)-1)
+            X[:,:,beam] = C + 10*np.log10((temperature + 273.16)*(bin_distances**2)) - 10*np.log10(transmit_pulse_lengths) - P_dbw + 2*alpha*bin_distances + 30*np.log10(10**(k_c[beam+1]*(E - E_r)/10)-1)
         
     
         self.append_to_ensembles(X,'ABSOLUTE BACKSCATTER')
-        #return abs_bs        
-    def get_velocity(self):
-        """
-        Retrieve velocity vectors and calculate progressive vectors in m/s. Magnetic deviation correction is applied here. 
-    
-        Returns
-        -------
-        u : numpy array
-            u velocity
-        v : numpy array
-            v velocity
-        z : numpy array
-            z velocity.
-        du : numpy array
-            displacement in u direction.
-        dv : numpy array
-            displacement in v direction.
-        dz : numpy array
-            displacement in z direction.
-        err: numpy array
-            error velocity
-    
-        """
         
-        global X,u,v
+        self.append_to_ensembles(np.log10(StN),'SIGNAL TO NOISE RATIO')
         
         
-        u = np.empty((self.n_ensembles,self.n_bins))
-        v = np.empty((self.n_ensembles,self.n_bins))
-        z = np.empty((self.n_ensembles,self.n_bins))
-        ev = np.empty((self.n_ensembles,self.n_bins))
-        for e,ensemble in enumerate(self.ensemble_data):
-            # cast velocity data as float
-            vel_data = np.array(ensemble['VELOCITY']).astype('float')
-            # mark nan values 
-            vel_data[vel_data==-32768] = np.nan
-            
-            # convert to m/s
-            vel_data = vel_data*.001
-
-
-            if len(vel_data) == self.n_bins:
-                u[e,:] = vel_data[:,0]
-                v[e,:] = vel_data[:,1]
-                z[e,:] = vel_data[:,2]
-                ev[e,:] = vel_data[:,3]
-            else:
-                u[e,:] = np.nan
-                v[e,:] = np.nan
-                z[e,:] = np.nan
-                ev[e,:] = np.nan
-            
-        # apply magnetic deviation correction
-        if self.magnetic_deviation_correction!=0:
-            #print(f'   Correcting for magnetic deviation ({self.magnetic_deviation_correction} degrees)')
-            for b in range(self.n_bins): # loop over all bins and calculate rotated velocites for each
-                X = np.array([u[:,b],v[:,b]])
-                X_rot = rotate(X,theta = self.magnetic_deviation_correction)
-                
-                # update u and v
-                u[:,b] = X_rot[0,:]
-                v[:,b] = X_rot[1,:]    
-                
-        ## gen prog vector components 
-        t = self.get_ensemble_datetimes()
-        to_sec = np.vectorize(lambda x: x.seconds) # vectorized function to convert datetime delta to total seconds
-        dt = np.empty(self.n_ensembles)
-        dt[:-1] = to_sec(np.diff(t))
-        dt[-1] = dt[-2] #assign last value
-        dt = np.outer(dt,np.ones(self.n_bins))
-        du = u*dt
-        dv = v*dt
-        dz = z*dt
+        #return abs_bs       
         
-
-
         
-        return u,v,z,du,dv,dz,ev 
+
        
-    def append_to_ensemble(self,X,title):
+    def append_to_ensembles(self,X,title):
         """
         Format numpy array of ensemble data into a list then add to ensemble_data property of the WorkhorseADCP class.
         Input array must have dimensions of (n_bins,n_ensemles,n_beams). In a typical use case, ensemble data is manipulated in 
         array format, then appended to the ensemble_data property and written to a PD0 file. 
         Args:
             X: numpy array with dimensions (n_bins,n_ensembles,n_beams)
             title: (string) title for the formatted data when appended to the ensemble_data property of the WorkhorseADCP class object. 
         """
-        
+        self.ensemble_fields.append(title) # update the list of ensemble field names
         for e in range(self.n_ensembles):
             ensemble_data = [] # data in the current ensemble
             for b in range(self.n_bins):
                 bin_data = [] # data in the current bin
                 for bm in range(self.n_beams):
                     
                     val = X[b,e,bm]
-                    
+                    #bin_data.append(int(val))
                     try:
                         bin_data.append(int(val))
                     except:
                         bin_data.append(32768)
                         
                         
                 ensemble_data.append(bin_data)
-            self.ensemble_data[e][title] = ensemble_data           
+            self.ensemble_data[e][title] = ensemble_data  
+            
+# set the sensor orientation. 
+
+    def set_sensor_orientation(self,orient_in):#orient_in = None):
+        """
+        Set the orientation data for the sensor. Accepts input orientation
+        timeseries, and assigns instrument position based on the closest position 
+        timestamp to each ensemble timestamp. All orientations are in degrees, 
+        with pitch and roll ranging[-180,179.99],and heading ranging from [0,359.99] 
+        
+        
+    
+        Parameters
+        ----------
+        orient_in : (optional)pandas dataframe containing a timeseries of roll,pitch,heading 
+                data corresponding to the orientation of the instrument. Must have 
+                columns named 'pitch', 'roll' and 'heading'. Index must be a pandas 
+                timestamp. If not specified, then the onboard gyroscope and compass data 
+                (from the variable headers) will be used. 
+    
+        Returns
+        -------
+        None.
+    
+        """
+        
+        self.orientation = np.full((3,self.n_ensembles),np.nan)
+        
+        
+        if type(orient_in) == type(None):
+            self.orientation[0,:] = self.get_sensor_pitch()
+            self.orientation[1,:] = self.get_sensor_roll()
+            self.orientation[2,:] = self.get_sensor_heading()
+        #if kwargs.get('orient_in'):
+        else:
+            et = self.ensemble_times # ensemble times
+            for i,etime in enumerate(et):
+                index = orient_in.index.get_indexer([etime], method='nearest')[0] # index of nearest input positon to the ensemble timestamp
+          
+                self.orientation[0,i] = orient_in.iloc[index].pitch
+                self.orientation[1,i] = orient_in.iloc[index].roll
+                self.orientation[2,i] = orient_in.iloc[index].heading 
+            
+
+        
+        
+        
+    def set_sensor_position(self,pos_in):
+        """
+        Set the position data for the sensor. Accepts input position timeseries,
+        and assigns instrument position based on the closest position timestamp to
+        each ensemble timestamp. 
+    
+        Parameters
+        ----------
+        pos_in : pandas dataframe
+            containing a timeseries of x,y,z data corresponding to the position of 
+            the instrument. Must have columns named 'x', 'y' and 'z'. Index must be
+            a pandas timestamp. 
+            
+    
+        Returns
+        -------
+        None.
+    
+        """
+        et = self.ensemble_times # ensemble times
+        self.position  = np.full((3,self.n_ensembles),np.nan)
+        for i,etime in enumerate(et):
+            index = pos_in.index.get_indexer([etime], method='nearest')[0] # index of nearest input positon to the ensembel timestamp
+      
+            self.position[0,i] = pos_in.iloc[index].x
+            self.position[1,i] = pos_in.iloc[index].y
+            self.position[2,i] = pos_in.iloc[index].z     
+        
+                
+
+    def set_beam_relative_geometry(self,rotation = 0,offset = (0,0,0), dr = 0.1):
+        """
+        Calculate the x,y,z position of each bin in each beam relative to the face 
+        of the ADCP. Accounts for 20 degree beam angle in x-z and y-z planes. 
+    
+        Parameters
+        ----------
+        rotation : float
+            Orientation of the ADCP. This is the number of degrees clockwise from the
+            forward direction of the mounting platform. (E.g., the bow of the vessel)
+            
+            
+            
+        offset : numpy array
+            numpy array containing x,y,z offsets for the instrument. This offset 
+            should be the relative distance between the position measuremet
+            (e.g., from the vessel GPS) and the center of the ADCP transducer face.
+            
+        dr : float
+            radial distance from the center of the face of the ADCP to the center 
+            of the transdecer faces. 
+            
+        Returns
+        -------
+        None.
+    
+        """
+    
+        # See WorkHorseCommands and Ouput Data Format page 53
+        # rotation = 45
+        # offset = adcp_offset
+        
+        # dr = 0.1 # distance from center of the unit to the center of each transducer face
+        R = ptools.gen_rot_z(theta = rotation)
+        
+        if self.beam_facing == 'DOWN':
+            self.relative_beam_origin = np.array([(dr,0,0),(-dr,0,0),(0,dr,0),(0,-dr,0)])# position of each beam relative to the center of the face of the instrument
+        if self.beam_facing == 'UP':
+            self.relative_beam_origin = np.array([(-dr,0,0),(dr,0,0),(0,dr,0),(0,-dr,0)])# position of each beam relative to the center of the face of the instrument
+            
+        self.relative_beam_origin = np.add(offset,self.relative_beam_origin)  # offset origin to be relative to the center of mass of the position measurement
+        self.relative_beam_origin = self.relative_beam_origin.dot(R).T # rotate the origin points - assums that positive y direction is forward (beam 3) 
+        
+        
+        self.relative_beam_midpoint_positions = []
+        for b in range(self.n_beams):
+            origin = self.relative_beam_origin[:,b]
+            beam_midpoints = np.outer(origin,np.ones(self.n_bins))
+            if self.beam_facing == 'DOWN':
+                beam_midpoints[2] += -self.bin_midpoints
+            else: 
+                beam_midpoints[2] += self.bin_midpoints
+            self.relative_beam_midpoint_positions.append(beam_midpoints)
+        
+        
+        # rotate the beams
+        
+
+        theta_beam = self.ensemble_data[0]['FIXED LEADER']['BEAM ANGLE']
+        
+        
+        Ry_cw = ptools.gen_rot_y(-theta_beam)
+        Rx_cw = ptools.gen_rot_x(-theta_beam)
+        Ry_ccw = ptools.gen_rot_y(theta_beam)
+        Rx_ccw = ptools.gen_rot_x(theta_beam)
+        self.relative_beam_midpoint_positions[0] = Rx_cw.dot(Ry_cw.dot(self.relative_beam_midpoint_positions[0]))
+        self.relative_beam_midpoint_positions[1] = Rx_ccw.dot(Ry_ccw.dot(self.relative_beam_midpoint_positions[1]))
+        self.relative_beam_midpoint_positions[2] = Rx_ccw.dot(Ry_cw.dot(self.relative_beam_midpoint_positions[2]))
+        self.relative_beam_midpoint_positions[3] = Rx_cw.dot(Ry_ccw.dot(self.relative_beam_midpoint_positions[3]))        
+        
+        
     
     def write_PD0(self,filename,path = os.getcwd(),data_type_5 = 'ECHO INTENSITY'):
         """
         Write ensemble_data to binary pd0 format. 
         Args:
             filename: name of the .000 file to b0e created
             path: path to directory where .000 file will be written
```

### Comparing `oceanograpy-0.0.7/oceanograpy.egg-info/PKG-INFO` & `oceanograpy-0.0.8/oceanograpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.7/setup.py` & `oceanograpy-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oceanograpy",
-    version="0.0.7",
+    version="0.0.8",
     author="Andy Banks",
     author_email="",
     description="Toolbox for importing and plotting ADCP and CTD data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=" ",
     packages=["oceanograpy"],
```

