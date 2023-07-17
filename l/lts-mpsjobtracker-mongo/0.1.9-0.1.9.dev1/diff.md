# Comparing `tmp/lts-mpsjobtracker-mongo-0.1.9.tar.gz` & `tmp/lts-mpsjobtracker-mongo-0.1.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsjobtracker-mongo-0.1.9.tar", last modified: Wed Nov 16 17:34:21 2022, max compression
+gzip compressed data, was "dist/lts-mpsjobtracker-mongo-0.1.9.dev1.tar", last modified: Wed Nov 16 17:34:50 2022, max compression
```

## Comparing `lts-mpsjobtracker-mongo-0.1.9.tar` & `lts-mpsjobtracker-mongo-0.1.9.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.789186 lts-mpsjobtracker-mongo-0.1.9/
--rw-r--r--   0 dougsimon   (502) staff       (20)       81 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/MANIFEST.in
--rw-r--r--   0 dougsimon   (502) staff       (20)     6214 2022-11-16 17:34:21.788724 lts-mpsjobtracker-mongo-0.1.9/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     4740 2022-10-20 15:19:44.000000 lts-mpsjobtracker-mongo-0.1.9/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.777071 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6214 2022-11-16 17:34:21.000000 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      630 2022-11-16 17:34:21.000000 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2022-11-16 17:34:21.000000 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       40 2022-11-16 17:34:21.000000 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       14 2022-11-16 17:34:21.000000 lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.778071 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     6441 2022-11-16 17:04:59.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/job_monitor.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.782233 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/json_templates/
--rw-r--r--   0 dougsimon   (502) staff       (20)      276 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/json_templates/job_tracker_init.json
--rw-r--r--   0 dougsimon   (502) staff       (20)      744 2022-10-20 15:19:44.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/json_templates/main_step_list.json
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.783305 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/schemas/
--rw-r--r--   0 dougsimon   (502) staff       (20)     3081 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/schemas/job.json
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.784624 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 19:25:01.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     9870 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/tests/test_job_tracker.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:21.787785 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 19:25:01.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    19276 2022-10-24 20:50:02.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/jobtracker.py
--rw-r--r--   0 dougsimon   (502) staff       (20)      529 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/validator.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2022-11-16 17:34:21.789328 lts-mpsjobtracker-mongo-0.1.9/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      834 2022-11-16 17:34:15.000000 lts-mpsjobtracker-mongo-0.1.9/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.491068 lts-mpsjobtracker-mongo-0.1.9.dev1/
+-rw-r--r--   0 dougsimon   (502) staff       (20)       81 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/MANIFEST.in
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6219 2022-11-16 17:34:50.490696 lts-mpsjobtracker-mongo-0.1.9.dev1/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4740 2022-10-20 15:19:44.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.485890 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6219 2022-11-16 17:34:50.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      630 2022-11-16 17:34:50.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2022-11-16 17:34:50.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       40 2022-11-16 17:34:50.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       14 2022-11-16 17:34:50.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.486664 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6441 2022-11-16 17:04:59.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/job_monitor.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.487533 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/json_templates/
+-rw-r--r--   0 dougsimon   (502) staff       (20)      276 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/json_templates/job_tracker_init.json
+-rw-r--r--   0 dougsimon   (502) staff       (20)      744 2022-10-20 15:19:44.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/json_templates/main_step_list.json
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.488060 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/schemas/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     3081 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/schemas/job.json
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.488797 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 19:25:01.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     9870 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/tests/test_job_tracker.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2022-11-16 17:34:50.490119 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 19:25:01.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    19276 2022-10-24 20:50:02.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/jobtracker.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)      529 2021-11-12 19:48:26.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/validator.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2022-11-16 17:34:50.491187 lts-mpsjobtracker-mongo-0.1.9.dev1/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      839 2022-11-16 17:34:32.000000 lts-mpsjobtracker-mongo-0.1.9.dev1/setup.py
```

### Comparing `lts-mpsjobtracker-mongo-0.1.9/PKG-INFO` & `lts-mpsjobtracker-mongo-0.1.9.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsjobtracker-mongo
-Version: 0.1.9
+Version: 0.1.9.dev1
 Summary: A job tracker management module
 Home-page: https://github.huit.harvard.edu/LTS/mps-jobtracker
 Author: Katie Amaral
 Author-email: kathryn_amaral@harvard.edu
 License: UNKNOWN
 Description: # mps_mongo_prototype
         Prototype for mongo instance to be used for IIIF job tracking
```

### Comparing `lts-mpsjobtracker-mongo-0.1.9/README.md` & `lts-mpsjobtracker-mongo-0.1.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/PKG-INFO` & `lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsjobtracker-mongo
-Version: 0.1.9
+Version: 0.1.9.dev1
 Summary: A job tracker management module
 Home-page: https://github.huit.harvard.edu/LTS/mps-jobtracker
 Author: Katie Amaral
 Author-email: kathryn_amaral@harvard.edu
 License: UNKNOWN
 Description: # mps_mongo_prototype
         Prototype for mongo instance to be used for IIIF job tracking
```

### Comparing `lts-mpsjobtracker-mongo-0.1.9/lts_mpsjobtracker_mongo.egg-info/SOURCES.txt` & `lts-mpsjobtracker-mongo-0.1.9.dev1/lts_mpsjobtracker_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/job_monitor.py` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/job_monitor.py`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/json_templates/main_step_list.json` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/json_templates/main_step_list.json`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/schemas/job.json` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/schemas/job.json`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/tests/test_job_tracker.py` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/tests/test_job_tracker.py`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/jobtracker.py` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/jobtracker.py`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/mpsjobtracker/trackers/validator.py` & `lts-mpsjobtracker-mongo-0.1.9.dev1/mpsjobtracker/trackers/validator.py`

 * *Files identical despite different names*

### Comparing `lts-mpsjobtracker-mongo-0.1.9/setup.py` & `lts-mpsjobtracker-mongo-0.1.9.dev1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsjobtracker-mongo",
-    version="0.1.9",
+    version="0.1.9.dev1",
     author="Katie Amaral",
     author_email="kathryn_amaral@harvard.edu",
     description="A job tracker management module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-jobtracker",
     packages=setuptools.find_packages(),
```

