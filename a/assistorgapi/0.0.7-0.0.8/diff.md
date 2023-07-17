# Comparing `tmp/assistorgapi-0.0.7.tar.gz` & `tmp/assistorgapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistorgapi-0.0.7.tar", last modified: Mon Jul 17 03:05:14 2023, max compression
+gzip compressed data, was "assistorgapi-0.0.8.tar", last modified: Mon Jul 17 03:08:25 2023, max compression
```

## Comparing `assistorgapi-0.0.7.tar` & `assistorgapi-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:05:14.687557 assistorgapi-0.0.7/
--rw-r--r--   0 monte      (501) staff       (20)      188 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/AUTHORS.rst
--rw-r--r--   0 monte      (501) staff       (20)     1086 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/LICENSE
--rw-r--r--   0 monte      (501) staff       (20)      262 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/MANIFEST.in
--rw-r--r--   0 monte      (501) staff       (20)     1472 2023-07-17 03:05:14.687633 assistorgapi-0.0.7/PKG-INFO
--rw-r--r--   0 monte      (501) staff       (20)      665 2023-06-26 18:45:04.000000 assistorgapi-0.0.7/README.md
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:05:14.683723 assistorgapi-0.0.7/assistorgapi/
--rw-r--r--   0 monte      (501) staff       (20)      489 2023-06-28 17:35:49.000000 assistorgapi-0.0.7/assistorgapi/__init__.py
--rw-r--r--   0 monte      (501) staff       (20)      224 2023-06-28 17:40:38.000000 assistorgapi-0.0.7/assistorgapi/academic_years.py
--rw-r--r--   0 monte      (501) staff       (20)      987 2023-06-28 17:40:36.000000 assistorgapi-0.0.7/assistorgapi/agreements.py
--rw-r--r--   0 monte      (501) staff       (20)      524 2023-06-28 17:40:44.000000 assistorgapi-0.0.7/assistorgapi/institutions.py
--rw-r--r--   0 monte      (501) staff       (20)      225 2023-06-28 17:40:47.000000 assistorgapi-0.0.7/assistorgapi/settings.py
--rw-r--r--   0 monte      (501) staff       (20)      850 2023-06-28 17:40:55.000000 assistorgapi-0.0.7/assistorgapi/transferability.py
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:05:14.684616 assistorgapi-0.0.7/assistorgapi.egg-info/
--rw-r--r--   0 monte      (501) staff       (20)     1472 2023-07-17 03:05:14.000000 assistorgapi-0.0.7/assistorgapi.egg-info/PKG-INFO
--rw-r--r--   0 monte      (501) staff       (20)      624 2023-07-17 03:05:14.000000 assistorgapi-0.0.7/assistorgapi.egg-info/SOURCES.txt
--rw-r--r--   0 monte      (501) staff       (20)        1 2023-07-17 03:05:14.000000 assistorgapi-0.0.7/assistorgapi.egg-info/dependency_links.txt
--rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 18:50:13.000000 assistorgapi-0.0.7/assistorgapi.egg-info/not-zip-safe
--rw-r--r--   0 monte      (501) staff       (20)       13 2023-07-17 03:05:14.000000 assistorgapi-0.0.7/assistorgapi.egg-info/top_level.txt
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:05:14.686661 assistorgapi-0.0.7/docs/
--rw-r--r--   0 monte      (501) staff       (20)      619 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/Makefile
--rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/authors.rst
--rw-r--r--   0 monte      (501) staff       (20)     4966 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/conf.py
--rw-r--r--   0 monte      (501) staff       (20)       33 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/contributing.rst
--rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/history.rst
--rw-r--r--   0 monte      (501) staff       (20)      315 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/index.rst
--rw-r--r--   0 monte      (501) staff       (20)     1270 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/installation.rst
--rw-r--r--   0 monte      (501) staff       (20)      774 2023-06-26 18:48:54.000000 assistorgapi-0.0.7/docs/make.bat
--rw-r--r--   0 monte      (501) staff       (20)       27 2023-06-26 03:31:11.000000 assistorgapi-0.0.7/docs/readme.rst
--rw-r--r--   0 monte      (501) staff       (20)       85 2023-06-26 18:48:53.000000 assistorgapi-0.0.7/docs/usage.rst
--rw-r--r--   0 monte      (501) staff       (20)      387 2023-07-17 03:05:14.687903 assistorgapi-0.0.7/setup.cfg
--rw-r--r--   0 monte      (501) staff       (20)     1378 2023-07-17 02:56:41.000000 assistorgapi-0.0.7/setup.py
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:05:14.687332 assistorgapi-0.0.7/tests/
--rw-r--r--   0 monte      (501) staff       (20)       42 2023-06-26 18:49:08.000000 assistorgapi-0.0.7/tests/__init__.py
--rw-r--r--   0 monte      (501) staff       (20)      412 2023-06-26 18:49:29.000000 assistorgapi-0.0.7/tests/test_assist_api_wrapper.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:08:25.587091 assistorgapi-0.0.8/
+-rw-r--r--   0 monte      (501) staff       (20)      188 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/AUTHORS.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1086 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/LICENSE
+-rw-r--r--   0 monte      (501) staff       (20)      262 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/MANIFEST.in
+-rw-r--r--   0 monte      (501) staff       (20)     1472 2023-07-17 03:08:25.587168 assistorgapi-0.0.8/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      665 2023-06-26 18:45:04.000000 assistorgapi-0.0.8/README.md
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:08:25.584677 assistorgapi-0.0.8/assistorgapi/
+-rw-r--r--   0 monte      (501) staff       (20)      489 2023-06-28 17:35:49.000000 assistorgapi-0.0.8/assistorgapi/__init__.py
+-rw-r--r--   0 monte      (501) staff       (20)      224 2023-06-28 17:40:38.000000 assistorgapi-0.0.8/assistorgapi/academic_years.py
+-rw-r--r--   0 monte      (501) staff       (20)      987 2023-06-28 17:40:36.000000 assistorgapi-0.0.8/assistorgapi/agreements.py
+-rw-r--r--   0 monte      (501) staff       (20)      528 2023-07-17 03:07:31.000000 assistorgapi-0.0.8/assistorgapi/institutions.py
+-rw-r--r--   0 monte      (501) staff       (20)      225 2023-06-28 17:40:47.000000 assistorgapi-0.0.8/assistorgapi/settings.py
+-rw-r--r--   0 monte      (501) staff       (20)      850 2023-06-28 17:40:55.000000 assistorgapi-0.0.8/assistorgapi/transferability.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:08:25.585372 assistorgapi-0.0.8/assistorgapi.egg-info/
+-rw-r--r--   0 monte      (501) staff       (20)     1472 2023-07-17 03:08:25.000000 assistorgapi-0.0.8/assistorgapi.egg-info/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      624 2023-07-17 03:08:25.000000 assistorgapi-0.0.8/assistorgapi.egg-info/SOURCES.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-07-17 03:08:25.000000 assistorgapi-0.0.8/assistorgapi.egg-info/dependency_links.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 18:50:13.000000 assistorgapi-0.0.8/assistorgapi.egg-info/not-zip-safe
+-rw-r--r--   0 monte      (501) staff       (20)       13 2023-07-17 03:08:25.000000 assistorgapi-0.0.8/assistorgapi.egg-info/top_level.txt
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:08:25.586718 assistorgapi-0.0.8/docs/
+-rw-r--r--   0 monte      (501) staff       (20)      619 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/Makefile
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/authors.rst
+-rw-r--r--   0 monte      (501) staff       (20)     4966 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/conf.py
+-rw-r--r--   0 monte      (501) staff       (20)       33 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/contributing.rst
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/history.rst
+-rw-r--r--   0 monte      (501) staff       (20)      315 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/index.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1270 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/installation.rst
+-rw-r--r--   0 monte      (501) staff       (20)      774 2023-06-26 18:48:54.000000 assistorgapi-0.0.8/docs/make.bat
+-rw-r--r--   0 monte      (501) staff       (20)       27 2023-06-26 03:31:11.000000 assistorgapi-0.0.8/docs/readme.rst
+-rw-r--r--   0 monte      (501) staff       (20)       85 2023-06-26 18:48:53.000000 assistorgapi-0.0.8/docs/usage.rst
+-rw-r--r--   0 monte      (501) staff       (20)      387 2023-07-17 03:08:25.587444 assistorgapi-0.0.8/setup.cfg
+-rw-r--r--   0 monte      (501) staff       (20)     1378 2023-07-17 03:07:49.000000 assistorgapi-0.0.8/setup.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-07-17 03:08:25.586969 assistorgapi-0.0.8/tests/
+-rw-r--r--   0 monte      (501) staff       (20)       42 2023-06-26 18:49:08.000000 assistorgapi-0.0.8/tests/__init__.py
+-rw-r--r--   0 monte      (501) staff       (20)      412 2023-06-26 18:49:29.000000 assistorgapi-0.0.8/tests/test_assist_api_wrapper.py
```

### Comparing `assistorgapi-0.0.7/LICENSE` & `assistorgapi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/PKG-INFO` & `assistorgapi-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistorgapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assistorgapi
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assistorgapi-0.0.7/README.md` & `assistorgapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/assistorgapi/agreements.py` & `assistorgapi-0.0.8/assistorgapi/agreements.py`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/assistorgapi/institutions.py` & `assistorgapi-0.0.8/assistorgapi/institutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     
     if response.status_code == 200:
         return response.text
     else:
         return None
 
 def get_institutions_academic_years(sendingInstitutionId):
-    url = "https://assist.org/institutions"+sendingInstitutionId+"/transferability/availableAcademicYears"
+    url = "https://assist.org/api/institutions"+sendingInstitutionId+"/transferability/availableAcademicYears"
     response = requests.get(url)
     
     if response.status_code == 200:
         return response.text
     else:
         return None
```

### Comparing `assistorgapi-0.0.7/assistorgapi/transferability.py` & `assistorgapi-0.0.8/assistorgapi/transferability.py`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/assistorgapi.egg-info/PKG-INFO` & `assistorgapi-0.0.8/assistorgapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistorgapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assistorgapi
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assistorgapi-0.0.7/assistorgapi.egg-info/SOURCES.txt` & `assistorgapi-0.0.8/assistorgapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/docs/Makefile` & `assistorgapi-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/docs/conf.py` & `assistorgapi-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/docs/installation.rst` & `assistorgapi-0.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/docs/make.bat` & `assistorgapi-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `assistorgapi-0.0.7/setup.py` & `assistorgapi-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 requirements = []
 
 test_requirements = []
 
 setup(
     name='assistorgapi',
-    version='0.0.7',
+    version='0.0.8',
     description="Unofficial API wrapper for ASSIST.org's API.",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author="Glenn Benedict Montesclaros",
     author_email='montesclarosglennbenedict@gmail.com',
     url='https://github.com/montesclarosglennbenedict/assistorgapi',
     packages=find_packages(include=['assistorgapi', 'assistorgapi.*']),
```

