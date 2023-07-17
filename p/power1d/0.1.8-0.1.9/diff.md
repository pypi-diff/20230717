# Comparing `tmp/power1d-0.1.8.tar.gz` & `tmp/power1d-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power1d-0.1.8.tar", last modified: Sun Jul  9 08:09:11 2023, max compression
+gzip compressed data, was "power1d-0.1.9.tar", last modified: Mon Jul 10 22:07:09 2023, max compression
```

## Comparing `power1d-0.1.8.tar` & `power1d-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.873253 power1d-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-09 08:09:00.000000 power1d-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-09 08:09:11.873253 power1d-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-09 08:09:00.000000 power1d-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-09 08:09:00.000000 power1d-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 08:09:11.873253 power1d-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.869253 power1d-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.869253 power1d-0.1.8/src/power1d/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.869253 power1d-0.1.8/src/power1d/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.873253 power1d-0.1.8/src/power1d/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/data/weather/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/data/weather/daily.m
--rw-r--r--   0 runner    (1001) docker     (123)    44350 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/data/weather/daily.mat
--rw-r--r--   0 runner    (1001) docker     (123)   102942 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/data/weather/daily.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-09 08:09:00.000000 power1d-0.1.8/src/power1d/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.869253 power1d-0.1.8/src/power1d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-09 08:09:11.000000 power1d-0.1.8/src/power1d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 08:09:11.000000 power1d-0.1.8/src/power1d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:09:11.000000 power1d-0.1.8/src/power1d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 08:09:11.000000 power1d-0.1.8/src/power1d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 08:09:11.000000 power1d-0.1.8/src/power1d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:09:11.873253 power1d-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-09 08:09:00.000000 power1d-0.1.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-09 08:09:00.000000 power1d-0.1.8/tests/test_data_sample_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-09 08:09:00.000000 power1d-0.1.8/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-09 08:09:00.000000 power1d-0.1.8/tests/test_samplesize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.599899 power1d-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-10 22:06:57.000000 power1d-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-10 22:07:09.599899 power1d-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-10 22:06:57.000000 power1d-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-10 22:06:57.000000 power1d-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:07:09.599899 power1d-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.595899 power1d-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.595899 power1d-0.1.9/src/power1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.595899 power1d-0.1.9/src/power1d/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.599899 power1d-0.1.9/src/power1d/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/data/weather/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/data/weather/daily.m
+-rw-r--r--   0 runner    (1001) docker     (123)    44350 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/data/weather/daily.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   102942 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/data/weather/daily.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-10 22:06:57.000000 power1d-0.1.9/src/power1d/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.599899 power1d-0.1.9/src/power1d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-10 22:07:09.000000 power1d-0.1.9/src/power1d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-10 22:07:09.000000 power1d-0.1.9/src/power1d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:07:09.000000 power1d-0.1.9/src/power1d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 22:07:09.000000 power1d-0.1.9/src/power1d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 22:07:09.000000 power1d-0.1.9/src/power1d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:07:09.599899 power1d-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-10 22:06:57.000000 power1d-0.1.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-10 22:06:57.000000 power1d-0.1.9/tests/test_data_sample_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-10 22:06:57.000000 power1d-0.1.9/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-10 22:06:57.000000 power1d-0.1.9/tests/test_samplesize.py
```

### Comparing `power1d-0.1.8/LICENSE.txt` & `power1d-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/PKG-INFO` & `power1d-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power1d
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical Power Estimates for One-Dimensional Continua
 Author-email: Todd Pataky <0todd0@gmail.com>
 Project-URL: Homepage, https://www.spm1d.org/power1d
 Project-URL: Source, https://github.com/0todd0000/power1d
 Project-URL: Bug Reports, https://github.com/0todd0000/power1d/issues
 Keywords: statistics,probability,hypothesis testing,functional data analysis,time series analysis,continuum data analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `power1d-0.1.8/README.md` & `power1d-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/pyproject.toml` & `power1d-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "power1d"
-version         = "0.1.8"
+version         = "0.1.9"
 description     = "Numerical Power Estimates for One-Dimensional Continua"
 readme          = "README.md"
 requires-python = ">=3.7"
 # license         = "GPL version 3"
 # license = {file = "LICENSE.txt"}
 
 keywords        = [
```

### Comparing `power1d-0.1.8/src/power1d/__init__.py` & `power1d-0.1.9/src/power1d/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://peerj.com/articles/cs-125/
 
 
 Copyright (C) 2023  Todd Pataky
 '''
 
 
-__version__ = '0.1.8 (2023-07-09)'
+__version__ = '0.1.9 (2023-07-11)'
 
 
 __all__ = ['geom', 'models', 'noise', 'roi', 'stats']
 
 
 
 from . import data
```

### Comparing `power1d-0.1.8/src/power1d/_base.py` & `power1d-0.1.9/src/power1d/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 	def dump(self, fpath):
 		import pickle
 		with open(fpath, 'wb') as f:
 			pickle.dump(self, f)
 	
 	def plot(self, ax=None, q=None, *args, **kwdargs):
 		plotter = DataPlotter(ax)
-		plotter.plot( q, self.value, *args, **kwdargs )
+		return plotter.plot( q, self.value, *args, **kwdargs )
 	
 	def toarray(self):
 		return self.value.copy()
 
 
 
 class _Continuum1D(_ContniuumObject):
@@ -298,15 +298,15 @@
 		self.value = self.value[-1::-1]
 	def flipud(self, datum=0):
 		self.value = -(self.value-datum) + datum
 
 
 	def plot(self, ax=None, q=None, *args, **kwdargs):
 		plotter = DataPlotter(ax)
-		plotter.plot( q, self.value, *args, **kwdargs )
+		return plotter.plot( q, self.value, *args, **kwdargs )
 		
 		
 	def save(self, fpath):
 		from gzip import GzipFile
 		with GzipFile( fpath, 'w') as f:
 			np.save(file=f, arr=self.value)
 
@@ -355,15 +355,15 @@
 		assert self.J == other.J
 		assert self.Q == other.Q
 		assert self.value  == pytest.approx(other.value,  abs=tol)
 	
 	
 	def plot(self, ax=None, q=None, *args, **kwdargs):
 		plotter = DataPlotter(ax)
-		plotter.plot( q, self.value.T, *args, **kwdargs )
+		return plotter.plot( q, self.value.T, *args, **kwdargs )
 
 	def set_sample_size(self, J):
 		self._assert_J( J )
 		self.J      = J
 
 	def set_value(self, y):
 		self.value  = y
```

### Comparing `power1d-0.1.8/src/power1d/_plot.py` & `power1d-0.1.9/src/power1d/_plot.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/data/weather/README.txt` & `power1d-0.1.9/src/power1d/data/weather/README.txt`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/data/weather/daily.m` & `power1d-0.1.9/src/power1d/data/weather/daily.m`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/data/weather/daily.mat` & `power1d-0.1.9/src/power1d/data/weather/daily.mat`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/data/weather/daily.npz` & `power1d-0.1.9/src/power1d/data/weather/daily.npz`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/data.py` & `power1d-0.1.9/src/power1d/data.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/geom.py` & `power1d-0.1.9/src/power1d/geom.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/io.py` & `power1d-0.1.9/src/power1d/io.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/models.py` & `power1d-0.1.9/src/power1d/models.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/noise.py` & `power1d-0.1.9/src/power1d/noise.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/prob.py` & `power1d-0.1.9/src/power1d/prob.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/random.py` & `power1d-0.1.9/src/power1d/random.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/results.py` & `power1d-0.1.9/src/power1d/results.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/roi.py` & `power1d-0.1.9/src/power1d/roi.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d/stats.py` & `power1d-0.1.9/src/power1d/stats.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/src/power1d.egg-info/PKG-INFO` & `power1d-0.1.9/src/power1d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power1d
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical Power Estimates for One-Dimensional Continua
 Author-email: Todd Pataky <0todd0@gmail.com>
 Project-URL: Homepage, https://www.spm1d.org/power1d
 Project-URL: Source, https://github.com/0todd0000/power1d
 Project-URL: Bug Reports, https://github.com/0todd0000/power1d/issues
 Keywords: statistics,probability,hypothesis testing,functional data analysis,time series analysis,continuum data analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `power1d-0.1.8/src/power1d.egg-info/SOURCES.txt` & `power1d-0.1.9/src/power1d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/tests/test_basic.py` & `power1d-0.1.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/tests/test_data_sample_modeling.py` & `power1d-0.1.9/tests/test_data_sample_modeling.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/tests/test_power.py` & `power1d-0.1.9/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `power1d-0.1.8/tests/test_samplesize.py` & `power1d-0.1.9/tests/test_samplesize.py`

 * *Files identical despite different names*

