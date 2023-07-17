# Comparing `tmp/krakatoa-0.0.6.post2.tar.gz` & `tmp/krakatoa-0.0.6.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.6.post2.tar", last modified: Mon Jul 10 20:08:00 2023, max compression
+gzip compressed data, was "krakatoa-0.0.6.post3.tar", last modified: Mon Jul 17 17:56:56 2023, max compression
```

## Comparing `krakatoa-0.0.6.post2.tar` & `krakatoa-0.0.6.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 20:08:00.000000 krakatoa-0.0.6.post2/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 20:08:00.348557 krakatoa-0.0.6.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-10 20:07:50.000000 krakatoa-0.0.6.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/krakatoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/krakatoa/future/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/future/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/future/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/future/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/future/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/krakatoa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/_getmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/krakatoa/models/quick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/krakatoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 17:56:56.000000 krakatoa-0.0.6.post3/krakatoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 17:56:56.000000 krakatoa-0.0.6.post3/krakatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:56:56.000000 krakatoa-0.0.6.post3/krakatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 17:56:56.000000 krakatoa-0.0.6.post3/krakatoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 17:56:56.000000 krakatoa-0.0.6.post3/krakatoa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 17:56:56.750945 krakatoa-0.0.6.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 17:56:44.000000 krakatoa-0.0.6.post3/setup.py
```

### Comparing `krakatoa-0.0.6.post2/LICENSE` & `krakatoa-0.0.6.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/PKG-INFO` & `krakatoa-0.0.6.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post2
+Version: 0.0.6.post3
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post3.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post2/krakatoa/future/analysis.py` & `krakatoa-0.0.6.post3/krakatoa/future/analysis.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/future/evaluate.py` & `krakatoa-0.0.6.post3/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/future/experiment.py` & `krakatoa-0.0.6.post3/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/future/preprocess.py` & `krakatoa-0.0.6.post3/krakatoa/future/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 '''
 
 #============================================================
 # Imports
 #============================================================
 
 import pandas as pd
-from pandas.api.types import is_string_dtype, is_numeric_dtype, is_categorical_dtype
+from pandas.api.types import is_string_dtype, is_numeric_dtype, is_object_dtype, is_categorical_dtype, is_datetime64_dtype, is_float_dtype, is_integer_dtype
 import numpy as np
 
 
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import MinMaxScaler, StandardScaler, RobustScaler, MaxAbsScaler
 from krakatoa.future.evaluate import countNull
-from sklearn.preprocessing import OneHotEncoder
+from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder, LabelEncoder
 
 #============================================================
 def changeColType(df, columns, newType):
     
     for col in columns:
         df[col] = df[col].astype(newType)
         
@@ -50,14 +50,39 @@
     dataset[columns] = cur_scaler.fit_transform(dataset[columns])
     
     return {
         "scaler" : cur_scaler,
         "dataset" : dataset
     }
 
+def encode(dataset, column, encoder='one_hot_encoder', **kwargs):
+    encoders = {
+        'one_hot_encoder' : OneHotEncoder(**kwargs),
+        'label_encoder' : LabelEncoder(),
+        'ordinal_encoder' : OrdinalEncoder(**kwargs)
+        }
+    
+    cur_encoder = encoders.get(encoder, None)
+
+    if cur_encoder is None:
+        raise ValueError(f'Encoder is not valid! Choose one of the following: {list(encoders.keys())}')
+
+    if encoder == 'one_hot_encoder':
+        transformed = cur_encoder.fit_transform(dataset[[column]])
+        new_df = pd.DataFrame(transformed.toarray(), columns=cur_encoder.get_feature_names_out())
+        dataset = dataset.join(new_df)
+        dataset.drop(columns=[column], inplace=True)
+
+    else:
+        dataset[column] = cur_encoder.fit_transform(dataset[[column]])
+    
+    return {
+        "encoder" : cur_encoder,
+        "dataset" : dataset
+    }
 
 # Class designed to dataset management   
 class DataClean():
 
     def __init__(self, target=None):
         self.dataset = pd.DataFrame()
         self.originalDataset = pd.DataFrame()
@@ -87,42 +112,57 @@
         # TODO precisamos ainda identificar colunas de outros tipos , como data e quando é numerica e categorica
         catCols = []
         numCols = []
         datCols = []
         floatCols = []
         intCols = []
         otherCols = []
+        dtype = {}
 
         for k, v in self.dataset.dtypes.items():
             # Check for non numeric
-            if v in ['object', 'category']:
+            # if v in ['object', 'category']:
+            if is_categorical_dtype(self.dataset[k]) or is_object_dtype(self.dataset[k]):
                 # Try to set datetime data
                 try:
                     # self.dataset[k] = pd.to_datetime(self.dataset[k], format='%d-%m-%Y %H:%M:%S.%f')
                     self.dataset[k] = pd.to_datetime(self.dataset[k], infer_datetime_format=True)
                     datCols.append(k)
+                    dtype[k] = 'datetime'
                 except:
-                    pass
                     catCols.append(k)
+                    dtype[k] = 'string'
+
+            # elif is_numeric_dtype(self.dataset[k]):
+            #     numCols.append(k)
+                # if v in ['float64', 'float32']:
+            elif is_float_dtype(self.dataset[k]):
+                floatCols.append(k)
+                numCols.append(k)
+                dtype[k] = 'float'
+                # elif v in ['int64', 'int32', 'int16', 'int8', 'uint64', 'uint32', 'uint16', 'uint8']:
+            elif is_integer_dtype(self.dataset[k]):
+                intCols.append(k)
+                numCols.append(k)
+                dtype[k] = 'integer'
+                    
+            elif is_datetime64_dtype(self.dataset[k]):
+                datCols.append(k)
+                dtype[k] = 'datetime'
             else:
-                if v in ['float64', 'float32']:
-                    floatCols.append(k)
-                    numCols.append(k)
-                elif v in ['int64', 'int32', 'int16', 'int8', 'uint64', 'uint32', 'uint16', 'uint8']:
-                    intCols.append(k)
-                    numCols.append(k)
-                else:
-                    otherCols.append(k)
+                otherCols.append(k)
+                dtype[k] = 'other'
                 
         self.category_cols = catCols
         self.numeric_cols = numCols
         self.integer_cols = intCols
         self.float_cols = floatCols
         self.other_cols = otherCols
         self.datetime_cols = datCols
+        self.dtype = dtype
         if self.target is not None:
             self.target_col = [self.target]
         else:
             self.target_col = []
 
     def splitTrainTest(self):
 
@@ -203,14 +243,26 @@
 
 
         # refresh column data in self
         self.getColType()
 
         return self.dataset
 
+    def encodeColumns(self, columns, encoder='one_hot_encoder'):
+        
+        for col in columns:
+
+            res_encoder = encode(self.dataset, column=col, encoder=encoder)
+
+        self.dataset = res_encoder["dataset"]
+        self.encoder = res_encoder["encoder"]
+
+        return self.dataset
+    
+
     def getDummies(self):
 
         # self.dataset = pd.get_dummies(self.dataset)
         # return self.dataset
         self.dataset.reset_index(inplace=True, drop=True)
 
         cat_cols = self.category_cols
```

### Comparing `krakatoa-0.0.6.post2/krakatoa/models/_config.py` & `krakatoa-0.0.6.post3/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/models/_getmodels.py` & `krakatoa-0.0.6.post3/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/models/_metrics.py` & `krakatoa-0.0.6.post3/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/models/autotune.py` & `krakatoa-0.0.6.post3/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa/models/quick.py` & `krakatoa-0.0.6.post3/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/krakatoa.egg-info/PKG-INFO` & `krakatoa-0.0.6.post3/krakatoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post2
+Version: 0.0.6.post3
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post3.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post2/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.6.post3/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post2/setup.py` & `krakatoa-0.0.6.post3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.6post2',      
+  version = '0.0.6post3',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
   long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post2.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post3.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
           'scikit-learn',
           'numpy',
           'pandas',
           'xgboost',
           'seaborn'
```

