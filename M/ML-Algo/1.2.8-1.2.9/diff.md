# Comparing `tmp/ML-Algo-1.2.8.tar.gz` & `tmp/ML-Algo-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.8.tar", last modified: Fri Jul 14 05:31:55 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.9.tar", last modified: Mon Jul 17 06:14:03 2023, max compression
```

## Comparing `ML-Algo-1.2.8.tar` & `ML-Algo-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.976147 ML-Algo-1.2.8/
-drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.950105 ML-Algo-1.2.8/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.8/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1909 2023-07-14 05:26:01.000000 ML-Algo-1.2.8/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.8/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.8/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.8/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0     2517 2023-07-13 11:01:26.000000 ML-Algo-1.2.8/ML_Algo/TestRun.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.8/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.970139 ML-Algo-1.2.8/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0     2198 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2198 2023-07-14 05:31:55.974136 ML-Algo-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 05:31:55.977141 ML-Algo-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-07-14 05:31:30.000000 ML-Algo-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:14:03.397946 ML-Algo-1.2.9/
+drwxrwxrwx   0        0        0        0 2023-07-17 06:14:03.386409 ML-Algo-1.2.9/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.9/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     2364 2023-07-17 06:12:40.000000 ML-Algo-1.2.9/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.9/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.9/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.9/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0     2517 2023-07-13 11:01:26.000000 ML-Algo-1.2.9/ML_Algo/TestRun.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.9/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:14:03.394960 ML-Algo-1.2.9/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0     2239 2023-07-17 06:14:03.000000 ML-Algo-1.2.9/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-17 06:14:03.000000 ML-Algo-1.2.9/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:14:03.000000 ML-Algo-1.2.9/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 06:14:03.000000 ML-Algo-1.2.9/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-17 06:14:03.000000 ML-Algo-1.2.9/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2239 2023-07-17 06:14:03.396944 ML-Algo-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:14:03.397946 ML-Algo-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-17 06:12:54.000000 ML-Algo-1.2.9/setup.py
```

### Comparing `ML-Algo-1.2.8/ML_Algo/DataCleaning.py` & `ML-Algo-1.2.9/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.8/ML_Algo/FetchData.py` & `ML-Algo-1.2.9/ML_Algo/FetchData.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,29 @@
 def getData(date):  
     url =  'http://192.168.0.35:5060/ldat'
     param =  {
         "id": "10751",
         "reqdate": date
          # 04-06-2023
     }   
+    dat = ''
     try:
-        response = requests.post(url,json=param, verify=False, timeout=20)
-    
+        response = requests.post(url,json=param, verify=False, timeout=300)
+        dat = response.text
     except:
         print('server busy')
-    dat = response.text
+        dat = {'data':
+                {'10751': [
+                    {'ts': '0/0/0000 12:00:00 AM','value': '0000','status': 'OK'},
+                    {'ts': '0/0/0000 12:00:00 AM','value': '0000','status': 'OK'},
+                    {'ts': '0/0/0000 12:00:00 AM','value': '0000','status': 'OK'},
+                    {'ts': '0/0/0000 12:00:00 AM','value': '0000','status': 'OK'},
+                    ]
+                }
+        }
     dt = json.loads(dat)
     return dt
 
 def get_live_data(yesterday,today,interval=15,manual_override=0,ct=0):
     if manual_override == 0:
         t = calculate_completed_intervals(interval)
     else:
```

### Comparing `ML-Algo-1.2.8/ML_Algo/Predictions.py` & `ML-Algo-1.2.9/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.8/ML_Algo/Series_Data.py` & `ML-Algo-1.2.9/ML_Algo/Series_Data.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.8/ML_Algo/Series_Time.py` & `ML-Algo-1.2.9/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.8/ML_Algo/TestRun.py` & `ML-Algo-1.2.9/ML_Algo/TestRun.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.8/ML_Algo.egg-info/PKG-INFO` & `ML-Algo-1.2.9/ML_Algo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -48,11 +48,12 @@
 Please ensure that you adhere to the code style and format used in the project.
 License
 
 ML-Algo is licensed under the MIT License. See the LICENSE file for more information.
 Contact
 
 `Changes Made as 14/07/2023 at 10:57am`
+`Changes Made as 17/07/2023 at 11:43am`
 
 If you have any questions, suggestions, or issues, please feel free to reach out to the project maintainer, Arunraj, at <a href="mailto:srvnn_arunraj@gmail.com." target="_new">srvnn_arunraj@gmail.com.</a>
 
 <a href="https://pypi.org/project/ml-algo/" target="_new"><img src="https://img.shields.io/pypi/v/ml-algo.svg" alt="PyPI Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.8 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.9 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -17,10 +17,10 @@
 contribute, please follow these guidelines: Fork the repository and clone it
 locally. Create a new branch for your feature or bug fix. Make your changes and
 ensure that the code passes all tests. Write tests for any new functionality
 you add. Commit your changes and push them to your fork. Submit a pull request,
 describing your changes in detail. Please ensure that you adhere to the code
 style and format used in the project. License ML-Algo is licensed under the MIT
 License. See the LICENSE file for more information. Contact `Changes Made as
-14/07/2023 at 10:57am` If you have any questions, suggestions, or issues,
-please feel free to reach out to the project maintainer, Arunraj, at
-srvnn_arunraj@gmail.com. [PyPI_Version]
+14/07/2023 at 10:57am` `Changes Made as 17/07/2023 at 11:43am` If you have any
+questions, suggestions, or issues, please feel free to reach out to the project
+maintainer, Arunraj, at srvnn_arunraj@gmail.com. [PyPI_Version]
```

### Comparing `ML-Algo-1.2.8/PKG-INFO` & `ML-Algo-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -48,11 +48,12 @@
 Please ensure that you adhere to the code style and format used in the project.
 License
 
 ML-Algo is licensed under the MIT License. See the LICENSE file for more information.
 Contact
 
 `Changes Made as 14/07/2023 at 10:57am`
+`Changes Made as 17/07/2023 at 11:43am`
 
 If you have any questions, suggestions, or issues, please feel free to reach out to the project maintainer, Arunraj, at <a href="mailto:srvnn_arunraj@gmail.com." target="_new">srvnn_arunraj@gmail.com.</a>
 
 <a href="https://pypi.org/project/ml-algo/" target="_new"><img src="https://img.shields.io/pypi/v/ml-algo.svg" alt="PyPI Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.8 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.9 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -17,10 +17,10 @@
 contribute, please follow these guidelines: Fork the repository and clone it
 locally. Create a new branch for your feature or bug fix. Make your changes and
 ensure that the code passes all tests. Write tests for any new functionality
 you add. Commit your changes and push them to your fork. Submit a pull request,
 describing your changes in detail. Please ensure that you adhere to the code
 style and format used in the project. License ML-Algo is licensed under the MIT
 License. See the LICENSE file for more information. Contact `Changes Made as
-14/07/2023 at 10:57am` If you have any questions, suggestions, or issues,
-please feel free to reach out to the project maintainer, Arunraj, at
-srvnn_arunraj@gmail.com. [PyPI_Version]
+14/07/2023 at 10:57am` `Changes Made as 17/07/2023 at 11:43am` If you have any
+questions, suggestions, or issues, please feel free to reach out to the project
+maintainer, Arunraj, at srvnn_arunraj@gmail.com. [PyPI_Version]
```

### Comparing `ML-Algo-1.2.8/setup.py` & `ML-Algo-1.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ML-Algo',
-    version='1.2.8',
+    version='1.2.9',
     author='Mr Raj',
     author_email='arunraj14092002@gmail.com',
     description='A package for calculating Series Time Data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['ML_Algo'],
     install_requires=['pandas','requests'],
```

