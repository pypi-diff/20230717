# Comparing `tmp/pylib_essentials-0.0.3.tar.gz` & `tmp/pylib_essentials-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib_essentials-0.0.3.tar", last modified: Wed Jul 12 21:16:49 2023, max compression
+gzip compressed data, was "pylib_essentials-0.0.4.tar", last modified: Mon Jul 17 21:06:54 2023, max compression
```

## Comparing `pylib_essentials-0.0.3.tar` & `pylib_essentials-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.789196 pylib_essentials-0.0.3/
--rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 21:16:49.788196 pylib_essentials-0.0.3/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.3/README.md
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.449194 pylib_essentials-0.0.3/pylib_essentials/
--rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.3/pylib_essentials/__init__.py
--rw-r--r--   0 feiye    (49086) vims     (50001)   184978 2023-07-12 21:14:37.000000 pylib_essentials-0.0.3/pylib_essentials/schism_file.py
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-12 21:16:49.760196 pylib_essentials-0.0.3/pylib_essentials.egg-info/
--rw-r--r--   0 feiye    (49086) vims     (50001)      218 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      278 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       42 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/requires.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-12 21:16:49.000000 pylib_essentials-0.0.3/pylib_essentials.egg-info/top_level.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-12 21:16:49.790196 pylib_essentials-0.0.3/setup.cfg
--rw-r--r--   0 feiye    (49086) vims     (50001)      391 2023-07-12 21:15:35.000000 pylib_essentials-0.0.3/setup.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:54.126747 pylib_essentials-0.0.4/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      312 2023-07-17 21:06:54.125748 pylib_essentials-0.0.4/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.4/README.md
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:53.852746 pylib_essentials-0.0.4/pylib_essentials/
+-rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.4/pylib_essentials/__init__.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)   182932 2023-07-17 20:33:36.000000 pylib_essentials-0.0.4/pylib_essentials/schism_file.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)    53637 2023-07-17 18:11:09.000000 pylib_essentials-0.0.4/pylib_essentials/utility_functions.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:54.095747 pylib_essentials-0.0.4/pylib_essentials.egg-info/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      312 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      316 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)      163 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/requires.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/top_level.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-17 21:06:54.127747 pylib_essentials-0.0.4/setup.cfg
+-rw-r--r--   0 feiye    (49086) vims     (50001)      600 2023-07-17 18:04:10.000000 pylib_essentials-0.0.4/setup.py
```

### Comparing `pylib_essentials-0.0.3/pylib_essentials/schism_file.py` & `pylib_essentials-0.0.4/pylib_essentials/schism_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,20 @@
   nan, isnan, loadtxt, savetxt, load, linspace, meshgrid, concatenate,\
   squeeze, mod, angle, pi, sign
 from matplotlib.pyplot import figure, show, savefig, tricontour,\
     tricontourf, tripcolor, colorbar, gca, gcf, plot, axis, xlim, ylim,\
     triplot, title, xlabel, ylabel, gca, gcf, setp, getp, close
 import matplotlib.cm as cm
 import matplotlib as mpl
-try:
-    from pylib_utils.utility_functions import proj
-except:
-    try:
-        from pylib.utility_functions import proj
-    except:
-        print("projection module not found; install pylib_utils or pylib")
+
+from pylib_essentials.utility_functions import loadz, savez, zdata, signa, \
+    get_VINFO, proj
 
 # for experimental features
+from pathlib import Path
 import numpy as np
 import pickle
 import pandas as pd
 import copy
 import scipy
 import unittest
 
@@ -3217,15 +3214,82 @@
         #resize window
         wd.geometry('600x180'); wd.update(); xm=max([i.winfo_width() for i in fms])
         for i in arange(0,100,3):
             L1['text']=' '*i; L2['text']=' '*i; wd.update(); xs=fms[-1].winfo_width()
             if xs>xm: wd.geometry('{}x210'.format(xs)); wd.update(); break
         return wd,w
 
-# -------------------------------------experimental-------------------------------------
+# ---------------------experimental functions and classes-------------------------------------
+def read_schism_hgrid_cached(fname, overwrite_cache=False):
+    gd_fname = Path(fname).absolute()  # force pathlib.Path and absolute path
+    gd_original_fname = gd_fname.resolve()
+
+    gd = None
+    if overwrite_cache:
+        for cache_name in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
+            Path(cache_name).unlink(missing_ok=True)
+
+    # try to read from cache: original file location first, then present location
+    for cache_name in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
+        try:
+            with open(cache_name, 'rb') as file:
+                print(f'Try reading from cache: {cache_name}.')
+                gd = pickle.load(file)
+        except Exception as e:
+            print(f'{e}\nError reading from original cache: {cache_name}.')
+        finally:
+            if gd is not None:
+                return gd  # success, return gd based on cache
+
+    # if cache read is not successful, read from file and update cache
+    for filename in [gd_original_fname, gd_fname]:
+        try:
+            print(f'Try reading from {filename}.')
+            gd = schism_grid(filename)
+            gd.source_file = filename
+        except Exception as e:
+            print(f'{e}\nError reading from original file: {filename}.')
+        finally:
+            if gd is not None:
+                break
+
+    if gd is None:
+        raise Exception(f'Error reading {filename}.')
+
+    # write to cache
+    for cache_fname in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
+        try:
+            with open(cache_fname, 'wb') as file:
+                pickle.dump(gd, file)
+        except Exception as e:
+            print(f'{e}\nError writing cache file {cache_fname}.')  
+
+    if gd.source_file is None:
+        gd.source_file = gd_fname
+
+    return gd
+
+def read_schism_vgrid_cached(vg_filename, overwrite_cache=False):
+    vg_cache_fname = os.path.splitext(vg_filename)[0] + '.pkl'
+    if not overwrite_cache:
+        try:
+            with open(vg_cache_fname, 'rb') as handle:
+                vg = pickle.load(handle)
+        except Exception as e:
+            print(f'{e}\nError reading cache file {vg_cache_fname}.\nReading from original file.')
+            # read original file
+            vg = read_schism_vgrid(vg_filename)
+            with open(vg_cache_fname, 'wb') as handle:
+                pickle.dump(vg, handle, protocol=pickle.HIGHEST_PROTOCOL)
+    else:
+        vg = read_schism_vgrid(vg_filename)
+        with open(vg_cache_fname, 'wb') as handle:
+            pickle.dump(vg, handle, protocol=pickle.HIGHEST_PROTOCOL)
+    return vg
+
 def combine_dataframes(A, B, weights=[1.0, 1.0]):
     import numbers
 
     AB = copy.deepcopy(A)
 
     # warn if B's time period does not contain A's time
     if B.index[0] > A.index[0] or B.index[-1] < A.index[-1]:
@@ -3256,15 +3320,15 @@
         weights_B = vs_B / (vs_A + vs_B)
         AB[common_columns] = weights_A * A[common_columns] + weights_B * B_interpolated[common_columns]
     else:
         raise ValueError('weights must be a list of two numbers or two TimeHistory objects')
 
     return AB
 
-class TimeHistory():
+class TimeHistory:
     """Class for handling SCHISM's *.th file format.
     A *.th file is a simple ascii file containing time series data,
     the 1st column is time in seconds or days,
     the 2nd to last column is data, so each column is a time series.
     However, the *.th file itself lacks information about the time units and start time
     and this class is to bind those information in a dataframe.
     The class also sets the time column as the index of the dataframe
@@ -3450,15 +3514,15 @@
     def __eq__(self, other) -> bool:
         for g1, g2 in zip(self.ele_groups, other.ele_groups):
             if g1.tolist() != g2.tolist():
                 return False
         return True
 
 
-class source_sink():
+class source_sink:
     """
     Class for handling all source/sink inputs:
 
     source_sink.in,
     vsource.th,
     vsink.th,
     msource.th
@@ -3617,32 +3681,32 @@
                 columns=source_sink_in.ele_groups[1]
             )
         
         source_sink = cls(vsource, vsink, msource)
         source_sink.check_consistency()
         return source_sink
     
-    def writer(self, source_dir):
+    def writer(self, output_dir):
         '''
-        Write source/sink files to the source_dir.
+        Write source/sink files to the output_dir.
         '''
-        if not os.path.exists(source_dir):
-            os.makedirs(source_dir)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
 
-        self.source_sink_in.writer(f"{source_dir}/source_sink.in")
+        self.source_sink_in.writer(f"{output_dir}/source_sink.in")
         if self.vsource is not None:
-            self.vsource.writer(f"{source_dir}/vsource.th")
+            self.vsource.writer(f"{output_dir}/vsource.th")
 
             msource_total = self.msource[0].time
             for i in range(self.ntracers):
                 msource_total = np.c_[msource_total, self.msource[i].df.values]
-            np.savetxt(f"{source_dir}/msource.th", msource_total)
+            np.savetxt(f"{output_dir}/msource.th", msource_total)
 
         if self.vsink is not None:
-            self.vsink.writer(f"{source_dir}/vsink.th")
+            self.vsink.writer(f"{output_dir}/vsink.th")
         
     def check_consistency(self):
         # check consistency of source_sink_in and vsource/vsink/msource
         if self.nsource == 0:
             if self.vsource is not None:
                 raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
         else:
@@ -3711,133 +3775,14 @@
                 return False
         for i, [ms_A, ms_B] in enumerate(zip(self.msource, other.msource)):
             if ms_A != ms_B:
                 print('msource {i} not equal')
                 return False
         return True
 
-# -------------------------------------temporarily copied from other files in pylib-------------------------------------
-def signa(x,y):
-    '''
-        compute signed area for triangles along the last dimension (x[...,0:3],y[...,0:3])
-    '''
-    if x.ndim==1:
-        area=((x[0]-x[2])*(y[1]-y[2])-(x[1]-x[2])*(y[0]-y[2]))/2
-    elif x.ndim==2:
-        # area=((x[:,0]-x[:,2])*(y[:,1]-y[:,2])-(x[:,1]-x[:,2])*(y[:,0]-y[:,2]))/2
-        area=((x[...,0]-x[...,2])*(y[...,1]-y[...,2])-(x[...,1]-x[...,2])*(y[...,0]-y[...,2]))/2
-    area=squeeze(area)
-    return area
-
-class zdata:
-    '''
-    self-defined data structure by Zhengui Wang.  Attributes are used to store data
-    '''
-    def __init__(self):
-        pass
-
-    @property
-    def VINFO(self):
-        return get_VINFO(self)
-
-def savez(fname,data,fmt=0):
-    '''
-    save data as self-defined python format
-       fmt=0: save data as *.npz (small filesize, reads slower)
-       fmt=1: save data as *.pkl (large filesize, reads faster)
-    if fname endswith *.npz or *.pkl, then fmt is reset to match fname
-    '''
-
-    #determine format
-    if fname.endswith('.npz'): fmt=0; fname=fname[:-4]
-    if fname.endswith('.pkl'): fmt=1; fname=fname[:-4]
-    if fmt==1: fname=fname+'.pkl'
-
-    #save data
-    if fmt==0:
-       #get all attribute
-       svars=list(data.__dict__.keys())
-       if 'VINFO' in svars: svars.remove('VINFO')
-
-       #check whether there are functions. If yes, change function to string
-       rvars=[]
-       for svar in svars:
-           if hasattr(data.__dict__[svar], '__call__'):
-              import cloudpickle
-              try:
-                 data.__dict__[svar]=cloudpickle.dumps(data.__dict__[svar])
-              except:
-                 print('function {} not saved'.format(svar))
-                 rvars.append(svar)
-       svars=setdiff1d(svars,rvars)
-
-       #check variable types for list,string,int and float
-       lvars=[]; tvars=[]; ivars=[]; fvars=[]
-       for svar in svars:
-           if isinstance(data.__dict__[svar],int): ivars.append(svar)
-           if isinstance(data.__dict__[svar],float): fvars.append(svar)
-           if isinstance(data.__dict__[svar],str): tvars.append(svar)
-           if isinstance(data.__dict__[svar],list):
-              lvars.append(svar)
-              data.__dict__[svar]=array(data.__dict__[svar],dtype='O')
-
-       #constrcut save_string
-       save_str='savez_compressed("{}" '.format(fname)
-       for svar in svars: save_str=save_str+',{}=data.{}'.format(svar,svar)
-       save_str=save_str+',_list_variables=lvars,_str_variables=tvars,_int_variables=ivars,_float_variables=fvars)'
-       exec(save_str)
-    elif fmt==1:
-       fid=open(fname,'wb'); pickle.dump(data,fid,pickle.HIGHEST_PROTOCOL); fid.close()
-
-def loadz(fname,svars=None):
-    '''
-    load self-defined data "fname.npz" or "fname.pkl"
-         svars: list of variables to be read
-    '''
-
-    if fname.endswith('.npz'):
-       #get data info
-       data0=load(fname,allow_pickle=True)
-       keys0=data0.keys() if svars is None else svars
-       ivars=list(data0['_int_variables']) if ('_int_variables' in keys0) else []
-       fvars=list(data0['_float_variables']) if ('_float_variables' in keys0) else []
-       tvars=list(data0['_str_variables']) if ('_str_variables' in keys0) else []
-       lvars=list(data0['_list_variables']) if ('_list_variables' in keys0) else []
-
-       #extract data
-       vdata=zdata()
-       for keyi in keys0:
-           if keyi in ['_list_variables','_str_variables','_int_variables','_float_variables']: continue
-
-           #get variable
-           datai=data0[keyi]
-           if datai.dtype==dtype('O'): datai=datai[()] #restore object
-           if keyi in ivars: datai=int(datai)          #restore int variable
-           if keyi in fvars: datai=float(datai)        #restore int variable
-           if keyi in tvars: datai=str(datai)          #restore str variable
-           if keyi in lvars: datai=datai.tolist()      #restore list variable
-
-           #if value is a function
-           if 'cloudpickle.cloudpickle' in str(datai):
-              import pickle
-              try:
-                 datai=pickle.loads(datai)
-              except:
-                 continue
-           vdata.__dict__[keyi]=datai
-    elif fname.endswith('.pkl'):
-       import pickle
-       vdata=zdata(); fid=open(fname,'rb')
-       data=pickle.load(fid)
-       vdata.__dict__=dcopy(data).__dict__.copy()
-       fid.close()
-    else:
-       sys.exit('unknown format: {}'.format(fname))
-    return vdata
-
 # ---------------------------- unit test ----------------------------
 class test_add_source_sink(unittest.TestCase):
     def test_add_source_sink(self):
         print('*************** test_add_source_sink ****************')
         # read from prepared sample files
         A = source_sink.from_files('/sciclone/data10/feiye/SCHISM_REPOSITORY/schism/src/Utility/Pre-Processing/STOFS-3D-Atl-shadow-VIMS/Pre_processing/Source_sink/Test_data/source_sink_sample1')
         B = source_sink.from_files('/sciclone/data10/feiye/SCHISM_REPOSITORY/schism/src/Utility/Pre-Processing/STOFS-3D-Atl-shadow-VIMS/Pre_processing/Source_sink/Test_data/source_sink_sample2')
```

