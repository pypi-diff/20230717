# Comparing `tmp/ztfidr-0.9.4.tar.gz` & `tmp/ztfidr-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.4.tar", last modified: Mon Jun  5 13:32:46 2023, max compression
+gzip compressed data, was "ztfidr-0.9.5.tar", last modified: Mon Jul 17 14:08:19 2023, max compression
```

## Comparing `ztfidr-0.9.4.tar` & `ztfidr-0.9.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739952 ztfidr-0.9.4/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.4/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-06-05 13:32:46.739821 ztfidr-0.9.4/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.4/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-06-05 13:32:46.739991 ztfidr-0.9.4/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-06-05 13:32:25.000000 ztfidr-0.9.4/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739021 ztfidr-0.9.4/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-06-05 13:32:21.000000 ztfidr-0.9.4/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14949 2023-06-04 13:51:50.000000 ztfidr-0.9.4/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.4/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.4/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10098 2023-06-04 12:12:27.000000 ztfidr-0.9.4/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.4/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    29089 2023-06-04 14:04:07.000000 ztfidr-0.9.4/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.4/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.4/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.4/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.4/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.4/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.4/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739670 ztfidr-0.9.4/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-17 14:08:19.709574 ztfidr-0.9.5/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.5/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-07-17 14:08:19.709441 ztfidr-0.9.5/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.5/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-07-17 14:08:19.709611 ztfidr-0.9.5/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-07-17 11:47:52.000000 ztfidr-0.9.5/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-17 14:08:19.708592 ztfidr-0.9.5/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      126 2023-07-17 13:36:44.000000 ztfidr-0.9.5/ztfidr/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5542 2023-07-17 14:06:04.000000 ztfidr-0.9.5/ztfidr/host.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    16159 2023-07-13 12:05:49.000000 ztfidr-0.9.5/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22735 2023-07-17 11:50:09.000000 ztfidr-0.9.5/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.5/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    25901 2023-07-13 12:46:52.000000 ztfidr-0.9.5/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1091 2023-06-18 10:58:06.000000 ztfidr-0.9.5/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    25280 2023-06-20 08:13:19.000000 ztfidr-0.9.5/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.5/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.5/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.5/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.5/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.5/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4225 2023-07-05 21:38:13.000000 ztfidr-0.9.5/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-17 14:08:19.709258 ztfidr-0.9.5/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-07-17 14:08:19.000000 ztfidr-0.9.5/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      392 2023-07-17 14:08:19.000000 ztfidr-0.9.5/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-07-17 14:08:19.000000 ztfidr-0.9.5/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-07-17 14:08:19.000000 ztfidr-0.9.5/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.4/LICENSE` & `ztfidr-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/README.md` & `ztfidr-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/setup.py` & `ztfidr-0.9.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.9.4'
+VERSION = '0.9.5'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.9.4/ztfidr/io.py` & `ztfidr-0.9.5/ztfidr/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,40 @@
            "get_autotyping"]
     
 # ================== #
 #                    #
 #   TOP LEVEL        #
 #                    #
 # ================== #
-def get_targets_data():
-    """ """
+def get_targets_data(saltmodel="default"):
+    """ 
+    Returns
+    -------
+    pandas.DataFrame, string
+        - dataframe containing targets parameters (incl lc fit parameters)
+        - name of the lc fit model.
+    """
     redshifts = get_redshif_data()[["redshift","redshift_err", "source"]]
-    salt2params = get_salt2params()
+    saltparams, saltmodel = get_saltparams(which=saltmodel)
     coords = get_coords_data()
     
     # merging
-    data_ = pandas.merge(redshifts,salt2params, left_index=True, right_index=True,
+    data_ = pandas.merge(redshifts,saltparams, left_index=True, right_index=True,
                      suffixes=("","_salt"), how="outer")
     data_ = pandas.merge(data_, coords, left_index=True, right_index=True,
                          how="outer")
     
     # force limit to target to use
     target_list = get_targetlist()
     data_ = data_.loc[target_list["ztfname"]]
 
     # adding classification
     typing = get_target_typing()
     data_ = data_.join(typing["classification"], how="left")
-
-
-    
-    return data_
+    return data_, saltmodel
 
 def get_localhost_data(local_nkpc=2, which="mag"):
     """ """
     hostlocal = get_host_local(nkpc=2, which="mag")
     hostcoords = get_host_coords()
     dlr = get_host_mags().xs("global", axis=1)["host_dlr"]
     hostcoords = hostcoords.merge(dlr, left_index=True, right_index=True)
@@ -217,28 +220,58 @@
     filepath = os.path.join(IDR_PATH, "tables",
                             "ztfdr2_coordinates.csv")
     if not load:
         return filepath
     return pandas.read_csv(filepath, index_col=index_col, **kwargs)
 
 # SALT
-def get_salt2params(load=True, default=True, **kwargs):
-    """ """
-    filename = "ztfdr2_salt2_params.csv" if default else\
-      "ztfdr2_salt2_params_phase-15to30_color-0.4to0.8.csv"
-    filepath = os.path.join(IDR_PATH, "tables",
-                                filename)
+def get_saltparams(load=True, which="default", **kwargs):
+    """ 
 
+    Parameters
+    ----------
+    which: string
+        name of the salt2 fit file to load. 
+        If 'default': ztfdr2_salt2_params.csv is used
+        
+    Returns
+    -------
+    pandas.DataFrame, string
+        - dataframe containing targets lc fit parameters
+        - name of the lc fit model.
+    """
+    if which == "default":
+        filename = "ztfdr2_salt2_params.csv"
+    else:
+        filename = os.path.join(".dataset_creation/lc_fits", which)
+
+    filepath = os.path.join(IDR_PATH, "tables", filename)
+    saltmodel = _parse_salt2filename(filepath)
+    
+    
     if not load:
-        return filepath
+        return filepath, saltmodel
     
     return pandas.read_csv(filepath, **kwargs
                           ).rename({"z":"redshift"}, axis=1
-                          ).set_index("ztfname")
+                          ).set_index("ztfname"), saltmodel
+
 
+def _parse_salt2filename(filename):
+    """ """
+    basename = os.path.basename(filename)
+    saltmodel, *version = basename.split("_")[1].split("params")[0].split("-")
+    saltmodel = saltmodel.strip()
+    version = None if len(version) ==0 else version[0].strip()
+    if version is None:
+        if saltmodel == "salt2": # so name is salt2 only:
+            return f"{saltmodel} v=T21" # default version T21
+        return saltmodel
+    
+    return f"{saltmodel} v={version}"
 
 # ================== #
 #                    #
 #   HOST             #
 #                    #
 # ================== #
 def get_host_coords(load=True, **kwargs):
@@ -308,23 +341,26 @@
                           keys=["2kpc", "4kpc", "global"])
     
 # ================== #
 #                    #
 #   LIGHTCURVES      #
 #                    #
 # ================== #
-def get_target_lc(target, test_exist=True):
+def get_target_lightcurve(target, test_exist=True, load=True):
     """ """
     fullpath = os.path.join(IDR_PATH, "lightcurves", f"{target}_LC.csv")
     if test_exist:
         if not os.path.isfile(fullpath):
             warnings.warn(f"No lc file for {target} ; {fullpath}")
             return None
-
-    return fullpath
+        
+    if not load:
+        return fullpath
+    
+    return pandas.read_csv(fullpath,  delim_whitespace=True, comment='#')
 
 
 def get_phase_coverage(load=True, warn=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables", "phase_coverage.parquet")
     if not load:
         return filepath
```

### Comparing `ztfidr-0.9.4/ztfidr/lightcurve.py` & `ztfidr-0.9.5/ztfidr/lightcurve.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,98 +6,121 @@
 
 
 __all__ =["get_target_lightcurve"]
 
 
 
 ZTFCOLOR = { # ZTF
-        "p48r":dict(marker="o",ms=7,  mfc="C3"),
-        "p48g":dict(marker="o",ms=7,  mfc="C2"),
-        "p48i":dict(marker="o",ms=7, mfc="C1")
+        "ztfr":dict(marker="o",ms=7,  mfc="C3"),
+        "ztfg":dict(marker="o",ms=7,  mfc="C2"),
+        "ztfi":dict(marker="o",ms=7, mfc="C1")
 }
 
 BAD_ZTFCOLOR = { # ZTF
-        "p48r":dict(marker="o",ms=6,  mfc="None", mec="C3"),
-        "p48g":dict(marker="o",ms=6,  mfc="None", mec="C2"),
-        "p48i":dict(marker="o",ms=6,  mfc="None", mec="C1")
+        "ztfr":dict(marker="o",ms=6,  mfc="None", mec="C3"),
+        "ztfg":dict(marker="o",ms=6,  mfc="None", mec="C2"),
+        "ztfi":dict(marker="o",ms=6,  mfc="None", mec="C1")
 }
 
 
-def get_target_lightcurve(name, load_salt2param=True, **kwargs):
+def get_target_lightcurve(name, saltparam=None, **kwargs):
     """ load the lightcurve object for the given target. """
-    return LightCurve.from_name(name, load_salt2param=load_salt2param, **kwargs)
+    return LightCurve.from_name(name, saltparam=saltparam, **kwargs)
+
+
+def get_target_lcresiduals(name, phase_range=None, mjd_range=None, saltparam=None,
+                               which_model=None, **kwargs):
+    """ shortcut to get the target lc residuals """
+    data = LightCurve.from_name(name, saltparam=saltparam).get_model_residual(which=which_model, **kwargs)
+    if phase_range is not None:
+        data = data[data["phase"].between(*phase_range)]
+
+    if mjd_range is not None:
+        data = data[data["mjd"].between(*mjd_range)]
+
+    return data
+
+def get_saltmodel(which="salt2.4", **params):
+    """ """
+    import sncosmo    
+    if which is None or which in ["salt2.4"]:
+        which = "salt2 v=2.4"
     
+    # parsing model version
+    source_name, *version = which.split("v=")
+    source_name = source_name.strip()
+    version = None if len(version)==0 else version[0].strip()
+    source = sncosmo.get_source(source_name, version=version, copy=True)
+    
+    dust  = sncosmo.CCM89Dust()
+    model = sncosmo.Model(source, effects=[dust],
+                              effect_names=['mw'],
+                              effect_frames=['obs'])
+    model.set(**params)
+    return model
+
 # ================== #
 #                    #
 #   LIGHTCURVES      #
 #                    #
 # ================== #
     
 class LightCurve( object ):
 
-    def __init__(self, data, meta=None, salt2param=None, use_dask=False):
+    def __init__(self, data, meta=None, saltparam=None, saltmodel=None, use_dask=False):
         """ likely, this is not how you should load the data. 
         See from_name() or from_filename() class methods.
         """
         self.set_data(data)
         self.set_meta(meta)
-        self.set_salt2param(salt2param)
+        self.set_saltparam(saltparam)
         self._use_dask = use_dask
+        self._saltmodel = saltmodel
         
     @classmethod
-    def from_filename(cls, filename, use_dask=False):
+    def from_filename(cls, filename, saltparam=None, use_dask=False, saltmodel=None, **kwargs):
         """  load a Lightcurve object from a given file. """
         if use_dask:
             from dask import delayed
             # This is faster than dd.read_cvs and does what we need here
             lc = delayed(pandas.read_csv)(filename,  delim_whitespace=True, comment='#')
         else:
             lc = pandas.read_csv(filename,  delim_whitespace=True, comment='#')
             
         meta = pandas.Series([os.path.basename(filename).split("_")[0]], 
                              index=["name"])
-        return cls(lc, meta=meta, use_dask=use_dask)
+        return cls(lc, meta=meta, use_dask=use_dask,
+                       saltparam=saltparam, saltmodel=saltmodel,
+                       **kwargs)
 
     @classmethod
-    def from_name(cls, targetname, use_dask=False, load_salt2param=True, **kwargs):
+    def from_name(cls, targetname, use_dask=False, saltparam=None, saltmodel=None, **kwargs):
         """ """
-        filename = io.get_target_lc(targetname)
-        this = cls.from_filename(filename, use_dask=use_dask, **kwargs)
-        this._targetname = targetname
-        if load_salt2param:
-            this.load_salt2param()
-            
+        filename = io.get_target_lightcurve(targetname, load=False)
+        this = cls.from_filename(filename, use_dask=use_dask, saltparam=saltparam, saltmodel=saltmodel, **kwargs)
+        this._targetname = targetname            
         return this
+    
     # ================ #
     #    Method        #
     # ================ #
     # --------- #
     #  LOADER   #
     # --------- #
-    def load_salt2param(self):
-        """ """
-        targetname = self.targetname
-        if targetname is None:
-            warnings.warn("Unknown targetname (=None) ; use manually set_salt2param()")
-            return None
-        
-        from .salt2 import get_target_salt2param
-        salt2param = get_target_salt2param(targetname)
-        self.set_salt2param(salt2param)
-        
+
     # --------- #
     #  SETTER   #
     # --------- #
     def set_data(self, data):
         """ """
         self._data = data
 
-    def set_salt2param(self, salt2param):
+    def set_saltparam(self, saltparam):
         """ """
-        self._salt2param = salt2param
+        self._saltparam = saltparam
         
     def set_meta(self, meta):
         """ """
         self._meta = meta  
 
     # --------- #
     #  GETTER   #
@@ -110,31 +133,31 @@
         """
         lcdata = self.get_lcdata(min_detection=min_detection, **kwargs)
         if groupby is None:
             return lcdata["phase"]
         
         return lcdata.groupby(groupby)["phase"].apply( list )
         
-    def get_saltmodel(self):
+    def get_saltmodel(self, which=None):
         """ """
-        from .salt2 import get_saltmodel
-        return get_saltmodel(**self.salt2param.rename({"redshift":"z"}
-                                                     )[["z","t0","x0","x1","c",
-                                                        "mwebv"]].to_dict()
-                            )
+        if which is None:
+            which = self._saltmodel
+        propmodel = self.saltparam.rename({"redshift":"z"})[["z","t0","x0","x1","c","mwebv"]].to_dict()
+        return get_saltmodel(which=which, **propmodel)
+    
     def get_lcdata(self, zp=None, in_mjdrange=None,
                        min_detection=None,
                        filters=None,
                        flagout=[1,2,4,8,16]):
         """ 
         filters: [string, None or list]
             list of filters 
             - None/'*' or 'all': no filter selection/
-            - string: just this filter (e.g. 'p48g')
-            - list of string: just these filters (e.g. ['p48g','p48r'])
+            - string: just this filter (e.g. 'ztfg')
+            - list of string: just these filters (e.g. ['ztfg','ztfr'])
 
         flagout: [list of int or string]
             flag == 0 means all good, but in details:
             
             0: no warning 
             1: flux_err==0 Remove unphysical errors 
             2: chi2dof>3: Remove extreme outliers 
@@ -149,30 +172,27 @@
 
         """
         from .utils import flux_to_mag
 
         if flagout in ["all","any","*"]:
             data = self.data[self.data["flag"]==0]
             
-        if flagout in ["all","any","*"]:
-            data = self.data[self.data["flag"]==0]
         elif flagout is None:
             data = self.data.copy()
         else:
             flag_ = np.all([(self.data.flag&i_==0) for i_ in np.atleast_1d(flagout)], axis=0)
             data = self.data[flag_]            
             
 
         if zp is None:
             zp = data["ZP"].values
             coef = 1. 
         else:
             coef = 10 ** (-(data["ZP"].values - zp) / 2.5)
 
-            
         flux  = data["flux"] * coef
         error = data["flux_err"] * coef
         detection = flux/error
             
         
         lcdata = data[["mjd","mag","mag_err","filter","field_id","x_pos","y_pos", "flag"]]
         additional = pandas.DataFrame(np.asarray([zp, flux, error, detection]).T,
@@ -182,36 +202,35 @@
         additional["mag_lim"], _ = flux_to_mag(error*5, None, zp=zp)
         
         lcdata = pandas.merge(lcdata, additional, left_index=True, right_index=True)
 #        lcdata.loc["zp",:] = zp
 #        lcdata["flux"] = flux
 #        lcdata["error"] = error
 #        lcdata["detection"] = detection
-        lcdata["filter"] = lcdata["filter"].replace("ztfg","p48g").replace("ztfr","p48r").replace("ztfi","p48i") 
+        lcdata["filter"] = lcdata["filter"].replace("ztf","ztf")
         
         
-        if self.has_salt2param():
-            lcdata["phase"] = lcdata["mjd"]-self.salt2param['t0']
+        if self.has_saltparam():
+            lcdata["phase"] = lcdata["mjd"]-self.saltparam['t0']
         else:
             lcdata["phase"] = np.NaN
             
         if in_mjdrange is not None:
             lcdata = lcdata[lcdata["mjd"].between(*in_mjdrange)]
 
         if min_detection is not None:
             lcdata = lcdata[lcdata["detection"]>min_detection]
 
         if filters is not None and filters not in ["*","all"]:
             lcdata = lcdata[lcdata["filter"].isin(np.atleast_1d(filters))]
             
         return lcdata
 
-
-    def get_model_residual(self, model=None, modelprop={}, 
-                           intrinsic_error=None,
+    def get_model_residual(self, model=None, which=None,
+                           intrinsic_error=None, 
                            **kwargs):
         """ get a dataframe with lightcurve data, model and residuals information.
 
         Parameters
         ----------
         model: [sncosmo.Model or None] -optional-
             provide the sncosmo model from which the model flux can be obtained.
@@ -231,101 +250,95 @@
         
         **kwargs goes to get_lcdata()
 
         Returns
         -------
         DataFrame
         """
-        basedata = self.get_lcdata(**kwargs)[["mjd","flux", "error","phase", "filter","flag"]]
+        basedata = self.get_lcdata(**kwargs)[["mjd","flux", "error","phase", "filter","flag"]].copy()
         if model is None:
-            model = self.get_saltmodel()
-            if modelprop is not None:
-                # Does nothing if empty dict
-                model.set(**modelprop) 
+            model = self.get_saltmodel(which)
 
         # Model
         basedata["model"] = model.bandflux(basedata["filter"], basedata["mjd"], 
                                             zp=self.flux_zp, zpsys="ab")
         # Residual    
         basedata["residual"] = basedata["flux"] - basedata["model"]
 
         # Error    
         basedata["error_int"] = intrinsic_error if intrinsic_error is not None else 0
         total_error = np.sqrt(basedata["error"]**2 + basedata["error_int"]**2)
         # Pull    
         basedata["pull"] = basedata["residual"]/total_error
         return basedata
-
     
-    def get_sncosmotable(self, min_detection=5,  phase_range=[-10,30], filters=["p48r","p48g"], **kwargs):
+    def get_sncosmotable(self, min_detection=5,  phase_range=[-10,30], filters=["ztfr","ztfg"], **kwargs):
         """ """
         from .utils import mag_to_flux
         
-        t0 = self.salt2param["t0"]
+        t0 = self.saltparam["t0"]
         to_fit = self.get_lcdata(min_detection=min_detection, in_mjdrange= t0 + phase_range,
                                  filters=filters, **kwargs)
         sncosmo_lc = to_fit.rename({"mjd":"time", "filter":"band"}, axis=1)[["time","band","zp","mag","mag_err"]]
         sncosmo_lc["zpsys"] = "ab"
         sncosmo_lc["flux"], sncosmo_lc["flux_err"] = mag_to_flux(sncosmo_lc["mag"],
                                                                  sncosmo_lc["mag_err"],
                                                                  zp=sncosmo_lc["zp"])
         return sncosmo_lc
 
     def fit_salt(self, free_parameters=['t0', 'x0', 'x1', 'c'],
-                       min_detection=5, phase_range=[-10,30], filters=["p48r","p48g"],
-                       as_dataframe=False,
+                       min_detection=5, phase_range=[-10,30], filters=["ztfr","ztfg"],
+                       as_dataframe=False, which=None,
                        **kwargs):
         """ """
         import sncosmo
         from astropy import table
         from .salt2 import salt2result_to_dataframe
-        model = self.get_saltmodel()
+        model = self.get_saltmodel(which=which)
         sncosmo_df = self.get_sncosmotable(min_detection=min_detection, 
                                            phase_range=phase_range, 
                                            filters=filters)
         fitted_data = table.Table.from_pandas(sncosmo_df)
         (result, fitted_model) = sncosmo.fit_lc(fitted_data, model,
                                             vparam_names=free_parameters,  **kwargs)
         if as_dataframe:
             return salt2result_to_dataframe(result)
         
         return (fitted_data,model), (result, fitted_model)
 
-    def fit_salt_perfilter(lc, filters=["p48g",'p48r','p48i'],
+    def fit_salt_perfilter(lc, filters=["ztfg",'ztfr','ztfi'],
                            min_detection=5, free_parameters=['t0','x0', 'x1'],
                            phase_range=[-10, 30], t0_range=[-2,+2]):
         """ """
         results = []
         for filter_ in filters:
             try:
                 result  = lc.fit_salt(min_detection=min_detection,
                                       filters=filter_,
                                       free_parameters=free_parameters,
                                       phase_range=phase_range,
-                                      bounds={"t0":lc.salt2param['t0']+t0_range},
+                                      bounds={"t0":lc.saltparam['t0']+t0_range},
                                       as_dataframe=True
                                       )
             except:
                 warnings.warn(f"failed for filter {filter_}")
                 result = pandas.DataFrame()
 
             results.append(result)
             
         return pandas.concat(results, keys=filters)
         
-    
-    
-
     # --------- #
     #  PLOTTER  #
     # --------- #
     def show(self, ax=None, figsize=None, zp=None, formattime=True, zeroline=True,
-                 incl_salt2=True, autoscale_salt=True, clear_yticks=True,
-                 phase_range=[-30,100],
-                 zprop={}, inmag=False, ulength=0.1, ualpha=0.1, notplt=False, **kwargs):
+                 incl_salt=True, which_model=None, autoscale_salt=True, clear_yticks=True,
+                 phase_range=[-30,100], as_phase=False, t0=None, 
+                 zprop={}, inmag=False, ulength=0.1, ualpha=0.1, notplt=False,
+                 rm_flags=True, **kwargs):
         """ """
         from matplotlib import dates as mdates
         from astropy.time import Time
         
         self._compute()
         # - Axes Definition
         if ax is None:
@@ -338,80 +351,85 @@
         # - End axes definition
         # -- 
         # - Data
         base_prop = dict(ls="None", mec="0.9", mew=0.5, ecolor="0.7", zorder=7)
         bad_prop  = dict(ls="None", mew=1, ecolor="0.7", zorder=6)        
         lineprop  = dict(color="0.7", zorder=1, lw=0.5)
 
-        if incl_salt2:
-            saltmodel = self.get_saltmodel()
+        if incl_salt:
+            saltmodel = self.get_saltmodel(which=which_model)
         else:
              saltmodel = None
              autoscale_salt = False
              
-        modeltime = self.salt2param.t0 + np.linspace(-15,50,100)
-        t0 = self.salt2param.t0
+        modeltime = self.saltparam.t0 + np.linspace(-15,50,100)
+        t0 = self.saltparam.t0
         if phase_range is not None:
-            timerange = [t0-30, t0+100]
+            timerange = [t0+phase_range[0], t0+phase_range[1]]
         else:
             timerange = None
-            
-        lightcurves = self.get_lcdata(zp=zp, in_mjdrange=timerange)        
+
+        if not rm_flags:
+            prop = {"flagout":None}
+        else:
+            prop = {}
+        lightcurves = self.get_lcdata(zp=zp, in_mjdrange=timerange, **prop)
         bands = np.unique(lightcurves["filter"])
         
-        # flag goods
-        flag_good = (lightcurves.flag&1==0) & (lightcurves.flag&2==0) & (lightcurves.flag&4==0) & (lightcurves.flag&8==0)
 
         max_saltlc = 0
         min_saltlc = 100
         # Loop over bands
         for band_ in bands:
             if band_ not in ZTFCOLOR:
                 warnings.warn(f"WARNING: Unknown instrument: {band_} | magnitude not shown")
                 continue
 
             flagband   = (lightcurves["filter"]==band_)
             
             bdata = lightcurves[flagband]
-            flag_good_ = flag_good[flagband]
+#            flag_good_ = flag_good[flagband]
             
             # IN FLUX
             if not inmag:
                 # - Data
                 datatime = Time(bdata["mjd"], format="mjd").datetime
                 y, dy = bdata["flux"], bdata["error"]
                 # - Salt
                 if saltmodel is not None:
-                    saltdata = saltmodel.bandflux(band_, modeltime, zp=self.flux_zp, zpsys="ab") if saltmodel is not None else None
+                    saltdata = saltmodel.bandflux(band_, modeltime, zp=self.flux_zp, zpsys="ab") \
+                      if saltmodel is not None else None
                 else:
                     saltdata = None
                     
             # IN MAG                                
             else:
                 flag_det = (lightcurves["mag"]<99)
                 # - Data                
                 bdata = bdata[flag_det]
-                flag_good_ = flag_good_[flag_det]
+                #flag_good_ = flag_good_[flag_det]
                 datatime = Time(bdata["mjd"], format="mjd").datetime
                 y, dy = bdata["mag"], bdata["mag_err"]
                 # - Salt
                 if saltmodel is not None:
                     saltdata = saltmodel.bandmag(band_, "ab",modeltime) if saltmodel is not None else None
                 else:
                     saltdata = None
             
             # -> good
-            ax.errorbar(datatime[flag_good_],
-                            y[flag_good_],  yerr=dy[flag_good_], 
+            ax.errorbar(datatime,#[flag_good_],
+                            y,#[flag_good_],
+                            yerr=dy,#[flag_good_], 
                             label=band_, 
                             **{**base_prop, **ZTFCOLOR[band_],**kwargs}
                             )
             # -> bad
-            ax.errorbar(datatime[~flag_good_],
-                            y[~flag_good_],  yerr=dy[~flag_good_], 
+            ax.errorbar(datatime,#[~flag_good_],
+                            y,#[~flag_good_],
+                            yerr=dy,#[~flag_good_], 
                             label=band_, 
                             **{**bad_prop, **BAD_ZTFCOLOR[band_],**kwargs}
                             )
         
             if saltdata is not None:
                 ax.plot(Time(modeltime, format="mjd").datetime,
                         saltdata,
@@ -427,16 +445,14 @@
                 datatime = Time(bdata["mjd"], format="mjd").datetime
                 y = bdata["mag_lim"]
                 ax.errorbar(datatime, y,
                                  yerr=ulength, lolims=True, alpha=ualpha,
                                  color=ZTFCOLOR[band_]["mfc"], 
                                  ls="None",  label="_no_legend_")
                                  
-                                 
-                
         if formattime:
             locator = mdates.AutoDateLocator()
             formatter = mdates.ConciseDateFormatter(locator)
             ax.xaxis.set_major_locator(locator)
             ax.xaxis.set_major_formatter(formatter)
 
         lunit = "flux" if not inmag else "mag"
@@ -503,26 +519,24 @@
             if self.meta is not None:
                 return self.meta.get("name",None)
             
             return None
         
         return self._targetname
     
-
-    def has_salt2param(self):
+    def has_saltparam(self):
         """" """
-        return self.salt2param is not None
+        return self.saltparam is not None
     
     @property
-    def salt2param(self):
+    def saltparam(self):
         """ """
-        if not hasattr(self,"_salt2param"):
+        if not hasattr(self,"_saltparam"):
             return None
-        return self._salt2param
-
+        return self._saltparam
 
     @property
     def flux_zp(self):
         """ """
         zp = self.data["ZP"]
         if len(np.unique(zp)) == 1:
             return float(zp[0])
```

### Comparing `ztfidr-0.9.4/ztfidr/linefitter.py` & `ztfidr-0.9.5/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/sample.py` & `ztfidr-0.9.5/ztfidr/sample.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,34 +21,35 @@
     n_points_i = phase_df.xs("ztfi", level=1).groupby(level=0).size().to_frame(f"n_{prefix}points_ztfi")
     dfs = [n_points, n_bands, n_points_g, n_points_r, n_points_i]
     return pandas.concat(dfs, axis=1).fillna(0).astype( int )
 
 class Sample():
 
     
-    def __init__(self, data=None):
+    def __init__(self, data=None, saltmodel=None):
         """ """
         self.set_data(data)
-    
+        self._saltmodel = saltmodel
+        
     @classmethod
-    def load(cls, redshift_range=None, target_list=None, has_spectra=True):
+    def load(cls, redshift_range=None, target_list=None, has_spectra=True, saltmodel="default", **kwargs):
         """ Load a Sample instance building it from io.get_targets_data() """
-        data = io.get_targets_data()
+        data, saltmodel = io.get_targets_data(saltmodel=saltmodel, **kwargs)
         
         if redshift_range is not None:
             data = data[data["redshift"].between(*redshift_range)]
 
         if target_list is not None:
             data = data.loc[target_list]
 
         if has_spectra:
             specfile = io.get_spectra_datafile(data=data)
             data = data[data.index.isin(specfile["ztfname"])]
             
-        return cls(data=data)
+        return cls(data=data, saltmodel=saltmodel)
 
     # ------- #
     # LOADER  #
     # ------- #
     def load_hostdata(self):
         """ load the host data using io.get_host_data(). This is made automatically upon hostdata call. """
         self.set_hostdata( io.get_host_data() )
@@ -294,26 +295,30 @@
         if query:
             data = data.query(query)
             
         return data
 
     def get_phases(self, one_per_day=False,
                          phase_range=None,
-                         detection=5):
+                         detection=5,
+                         in_targetlist=None):
         """ """
         if detection is not None:
             phase_df = self.phase_df[(self.phase_df["detection"]>detection)]["phase"].copy()
         else:
             phase_df = self.phase_df["phase"]
         
         if one_per_day:
             phase_df = phase_df.astype(int).reset_index().drop_duplicates().set_index(["ztfname","filter"])["phase"]
             
         if phase_range is not None:
-            phase_df = phase_df[phase_df.between(*phase_df)]
+            phase_df = phase_df[phase_df.between(*phase_range)]
+
+        if in_targetlist:
+            phase_df = phase_df[phase_df.index.get_level_values(0).isin(np.atleast_1d(in_targetlist))]
             
         return phase_df
                                     
     
     # Target | High level
     def get_target(self, name):
         """ """
@@ -325,51 +330,87 @@
 
     def get_target_typing(self, name=None):
         """ """
         if name is None:
             return self.data["classification"].copy()
         
         return self.data.loc[np.atleast_1d(name)]["classification"].copy()
-    
+
+    # model
+    def get_target_saltmodel(self, name):
+        """ """
+        from .lightcurve import get_saltmodel
+        propmodel = self.data.loc[name].rename({"redshift":"z"})[["z","t0","x0","x1","c","mwebv"]].to_dict()
+        return get_saltmodel(which=self._saltmodel, **propmodel)
+        
+        
     # LightCurve
     def get_target_lightcurve(self, name, **kwargs):
         """ Get the {name} LightCurve object """
         from . import lightcurve
-        return lightcurve.LightCurve.from_name(name)
+        return lightcurve.LightCurve.from_name(name, saltparam=self.data.loc[name], saltmodel=self._saltmodel)
 
+    def get_target_lightcurve_residual(self, name, phase_range=None, mjd_range=None, **kwargs):
+        """ fet the {name} lightcurve residuals given the target's salt model. 
+        
+        Parameters
+        ----------
+        name: str
+            target's name
+
+        phase_range: [float, float]
+            limit phase range (days to maximum of light t0): [start, end]
+        
+        **kwargs goes to lightcurve.LightCurve.get_model_residual
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
+        from . import lightcurve
+        return lightcurve.get_target_lcresiduals(name, phase_range,
+                                                     mjd_range=mjd_range,
+                                                     saltparam=self.data.loc[name],
+                                                     which_model=self._saltmodel,
+                                                     **kwargs)
+    
     # Spectrum
     def get_target_spectra(self, name, **kwargs):
         """ Get a list with all the Spectra for the given object """
         from . import spectroscopy
         return spectroscopy.Spectrum.from_name(name, **kwargs)
 
     # Extra
     def get_goodcoverage_targets(self, premax_range = [-15,0],
                                        postmax_range = [0,45],
                                        phase_range = [-15,45],
+                                       detection=5, one_per_day=True,
                                       **kwargs):
         """ kwargs should have the same format as the n_early_point='>=2' for instance.
         None means no constrain, like n_bands=None means 'n_bands' is not considered.
         """
         query = {**dict(n_late_bands=">=2", n_points=">=7", n_early_points=">=2"),
                  **kwargs}
         df_query = " and ".join([f"{k}{v}" for k,v in query.items() if v is not None])
 
         phase_coverage = self.get_phase_coverage(premax_range = premax_range,
                                                  postmax_range = postmax_range,
-                                                 phase_range = phase_range)
+                                                 phase_range = phase_range,
+                                                detection=5, one_per_day=True)
+        
         return phase_coverage.query(df_query).index.astype("string")
     
     def get_phase_coverage(self, premax_range = [-15,0],
                                  postmax_range = [0,45],
                                  phase_range = [-15,45],
-                                 one_per_day=True):
+                                 one_per_day=True,
+                                 detection=5):
         """ """
 
-        phase_df = self.get_phases(one_per_day)
+        phase_df = self.get_phases(one_per_day, detection=detection)
         
         dfs = _get_coverage_( phase_df[phase_df.between(*phase_range)] )
         dfs_early = _get_coverage_(phase_df[phase_df.between(*premax_range)], prefix="early_")
         dfs_late = _get_coverage_(phase_df[phase_df.between(*postmax_range)], prefix="late_")
         return pandas.concat([dfs, dfs_early, dfs_late], axis=1).reindex(self.data.index).fillna(0).astype(int)
         
     def build_phase_coverage(self, groupby='filter', client=None, store=True, **kwargs):
@@ -377,26 +418,24 @@
         time: 
         - Dask: 45s on a normal laptop | 4 cores 
         - No Dask: 60s on a normal laptop | 4 cores 
         """
         warnings.warn("building phase coverage takes ~30s.")
         
         import pandas
-        import dask
-        from . import lightcurve
         from . import io
         phases = []
         data = self.get_data()
         
         lcdata = io.get_lightcurve_datafile().set_index("ztfname").loc[data.index]
         dfs = pandas.concat([pandas.read_csv(f_, delim_whitespace=True, comment='#') for f_ in lcdata["fullpath"]],
                                 keys=data.index)
         dfs["phase"] = dfs["mjd"] - data["t0"].reindex(dfs.index, level=0)
         dfs["detection"] = dfs["flux"]/dfs["flux_err"]
-        phase_df = dfs.reset_index().set_index(["ztfname","filter"])[["phase","detection"]]
+        phase_df = dfs.reset_index().set_index(["ztfname","filter"])[["phase","detection","flag","in_baseline"]]
         if store:
             filepath = io.get_phase_coverage(load=False)
             phase_df.to_parquet(filepath)
             
         return phase_df
     
     
@@ -598,161 +637,15 @@
     #        ax.set_title("ZTF-1 Ia Statistics")
         ax.set_ylabel("Number of Type Ia Supernovae")
         ax.set_ylim(bottom=0)
         ax.tick_params("y", labelsize="small")
         return fig
 
 
-    def show_npoints_distribution_perband(self, phase_coverage=[-20, 40],
-                                                ax=None, clearaxes=True,
-                                          add_pantheon=True):
-        """ """
-        phase_cov = self.get_phase_coverage( premax_range=[phase_coverage[0], 0],
-                                               postmax_range=[0, phase_coverage[1]],
-                                               phase_range=phase_coverage,)
-
-
-        from matplotlib.colors import to_rgba
-        if ax is None:
-            import matplotlib.pyplot as plt
-            fig = plt.figure(figsize=[7, 4.5])
-            axb = fig.add_axes([0.08, 0.15, 0.87, 0.35])
-            axt = fig.add_axes([0.08, 0.6, 0.87, 0.35])
-
-        else:
-            fig = ax.figure
-            axb, axt = fig.axew
 
-        prop = dict(bins=np.logspace(0,3, 15), density=False, log=False)
-
-        # -------------
-        weights = np.ones(len(phase_cov))*1
-        axt.hist(phase_cov["n_early_points_p48g"]+phase_cov["n_late_points_p48g"], histtype="step", 
-                fill=True, 
-                edgecolor=to_rgba("tab:green", 1), lw=1., ls="--",
-                facecolor=to_rgba("tab:green", 0.05), 
-                label=f"ztf:g", weights=weights,
-                zorder=2, **prop)
-
-        axt.hist(phase_cov["n_early_points_p48r"]+phase_cov["n_late_points_p48r"], histtype="step", 
-                fill=True, 
-                edgecolor=to_rgba("tab:red", 1), lw=1., ls="-",
-                facecolor=to_rgba("tab:red", 0.05), 
-                label=f"ztf:r",weights=weights,
-                zorder=3, **prop)
-
-        axt.hist(phase_cov["n_early_points_p48i"]+phase_cov["n_late_points_p48i"], histtype="step", 
-                fill=True, 
-                edgecolor=to_rgba("tab:orange", 1), lw=1., ls=":",
-                facecolor=to_rgba("tab:orange", 0.05), 
-                label=f"ztf:i",weights=weights,
-                zorder=5, **prop)
-
-
-        # --------------
-        weights = np.ones(len(phase_cov))*1
-
-        axb.hist(phase_cov["n_points"], histtype="step", color="k", lw=1.5,
-                label=f"any phase",
-                weights=weights,
-                zorder=5, **prop)
-
-        axb.hist(phase_cov["n_early_points"], histtype="step", 
-                fill=True, 
-                edgecolor=to_rgba("0.5", 1), lw=1., ls="-",
-                facecolor=to_rgba("0.5", 0.), 
-                label="pre-max",
-                weights=weights,            
-                zorder=3, **prop)
-
-        axb.hist(phase_cov["n_late_points"], histtype="step", 
-                fill=True, 
-                edgecolor=to_rgba("0.5", 1), lw=0., 
-                facecolor=to_rgba("0.5", 0.3), 
-                label="post-max",
-                weights=weights,
-                zorder=4, **prop)
-
-        # --------------
-
-        axb.set_xlabel("number of detected point", fontsize="large")
-        axb.set_xscale("log")
-        axt.set_xscale("log")
-
-        if clearaxes:
-            clearwhich = ["left","right","top"] # "bottom"
-            for ax in [axb, axt]:
-                [ax.spines[which].set_visible(False) for which in clearwhich]
-                ax.tick_params(axis="y", labelsize="small", 
-                           labelcolor="0.5", color="0.5")
-
-        axt.legend(fontsize="medium", frameon=False)#, loc="upper left")
-        axb.legend(fontsize="medium", frameon=False)
-
-        axt.set_xlim(*axb.get_xlim())
-        return fig
-
-
-    def show_firstdet_distributions(self, ax=None, restrict_to=[-25,60]):
-        """ """
-        phases = self.get_phases(phase_range=restrict_to)
-        goodlc = self.get_goodcoverage_targets()
-
-        from matplotlib.colors import to_rgba
-        if ax is None:
-            import matplotlib.pyplot as plt
-            fig = plt.figure(figsize=[7, 2.5])
-            ax = fig.add_axes([0.08, 0.1, 0.87, 0.8])
-        else:
-            fig = ax.figure
-
-        first_det_per_band = phases.groupby(level=[0,1]).min()
-        first_det = first_det_per_band.unstack().min(axis=1)
-
-        prop = dict(range=[-21,30], bins=50, histtype="step", fill=True)
-
-        # ---- Any band
-
-        _ = ax.hist(first_det, facecolor="None", zorder=5,
-                    color="k", label="all Type Ia", **prop)
-
-        _ = ax.hist(first_det.loc[goodlc], zorder=4,
-                    facecolor="0.7", lw=0,
-                     label="good sampling", **prop)
-        # ---- Per filter
-
-        #ax.legend(frameon=False)
-
-        for band, color, label in zip(["p48g","p48r","p48i"],
-                              ["tab:green","tab:red","tab:orange"],
-                              ["ztf:g","ztf:r","ztf:i"]):
-            band_fdet = first_det_per_band.xs(band, level=1)
-            band_fdet_good = band_fdet.loc[band_fdet.index.isin(goodlc)]
-
-
-            _ = ax.hist(band_fdet_good, 
-                        facecolor=to_rgba(color, 0.0), #zorder=2,
-                        edgecolor=color,
-                        weights = np.ones(len(band_fdet_good))*-1, 
-                        label=label, **prop)
-
-        ax.spines["bottom"].set_position(('data',0))
-        ax.spines["bottom"].set_zorder(10)
-
-        clearwhich = ["left","right","top"] # "bottom"
-        [ax.spines[which].set_visible(False) for which in clearwhich]
-        ax.tick_params(axis="y", labelsize="small", 
-                   labelcolor="0.5", color="0.5")
-        ax.tick_params(axis="x", pad=2, zorder=10)
-        ax.set_xlabel("First detection phase [days]", loc="right")
-
-
-        #ax.legend(["all", "good"], frameon=False)
-        ax.legend(frameon=False, ncol=3)
-        return fig
         
     # =============== #
     #   Properties    #
     # =============== #
     @property
     def data(self):
         """ """
```

### Comparing `ztfidr-0.9.4/ztfidr/script.py` & `ztfidr-0.9.5/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/snid.py` & `ztfidr-0.9.5/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/spectroscopy.py` & `ztfidr-0.9.5/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/target.py` & `ztfidr-0.9.5/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/typing.py` & `ztfidr-0.9.5/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.4/ztfidr/utils.py` & `ztfidr-0.9.5/ztfidr/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import numpy as np
 
+
+def nmad(*args, **kwargs):
+    """ stats.median_abs_deviation forcing scale='normal' """
+    from scipy import stats
+    return stats.median_abs_deviation(*args, scale="normal", **kwargs)
+
+
 def mag_to_flux(mag, magerr=None, units="zp", zp=25.0, wavelength=None):
     """converts magnitude into flux
     Parameters
     ----------
     mag: [float or array]
         AB magnitude(s)
     magerr: [float or array] -optional-
```

