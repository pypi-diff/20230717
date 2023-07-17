# Comparing `tmp/flask_pypprof-0.1.12.tar.gz` & `tmp/flask_pypprof-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pypprof-0.1.12.tar", max compression
+gzip compressed data, was "flask_pypprof-0.1.13.tar", max compression
```

## Comparing `flask_pypprof-0.1.12.tar` & `flask_pypprof-0.1.13.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/LICENSE
--rw-r--r--   0        0        0     1259 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/README.md
--rw-r--r--   0        0        0      141 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/flask_pypprof/__init__.py
--rw-r--r--   0        0        0     1408 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/flask_pypprof/handler.py
--rw-r--r--   0        0        0     1919 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/flask_pypprof/routes.py
--rw-r--r--   0        0        0      499 2023-07-17 16:15:41.777707 flask_pypprof-0.1.12/pyproject.toml
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 flask_pypprof-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/LICENSE
+-rw-r--r--   0        0        0     1788 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/README.md
+-rw-r--r--   0        0        0      141 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/handler.py
+-rw-r--r--   0        0        0     1919 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/routes.py
+-rw-r--r--   0        0        0      481 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/pyproject.toml
+-rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 flask_pypprof-0.1.13/PKG-INFO
```

### Comparing `flask_pypprof-0.1.12/LICENSE` & `flask_pypprof-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.12/README.md` & `flask_pypprof-0.1.13/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flask-pypprof
 
-Blueprint for pprof profiling endpoints a la GO that can be added to python Flask applications. *flask-pypprof* is a wrapper of [pypprof] and based on [django-pypprof] ideas.
+Blueprint for pprof profiling endpoints a la GO's that can be added to python Flask applications. *flask-pypprof* is a wrapper of [pypprof] and based on [django-pypprof] ideas.
 
 ## Installation
 
 ```bash
-pip install flask-pypprof --extra-index-url https://<>/
+pip install flask-pypprof
 ```
 
 ## Usage
 
 To add the pprof endpoints to your application, simply register the blueprint:
 
 ```python
@@ -31,15 +31,34 @@
 
 * `MEMORY_SAMPLE_RATE`: sets the memory profiling sample rate (default: 128 * 1024)
 
 ```bash
 export MEMORY_SAMPLE_RATE = 128 * 1024
 ```
 
+## Fetching profiles from your application
+Fetch a 30 seconds CPU profile:
+
+```bash
+go tool pprof -http=:8088 http://localhost:8081/debug/pprof/profile?seconds=30
+```
+
+Fetch a heap profile:
+
+```bash
+go tool pprof -http=:8088 http://localhost:8081/debug/pprof/heap
+```
+![image_2023-05-09_16-27-22](https://github.com/dpsoft/flask-pypprof/assets/2567525/33f36ed4-0b97-44fc-89e7-2fbbbbb7132a)
+
+
+## Compatibility 
+Python **3.8**, **3.9**, **3.10** and Flask >= **2.0.0** and **Linux** only.
+    
 ## Known issues
 * `zprofile issue with python 3.11`:  https://github.com/timpalpant/zprofile/pull/2 
 
 
 ## License
+This code base is available under the Apache License, version 2.
 
 [pypprof]: https://github.com/timpalpant/pypprof
 [django-pypprof]:https://gitlab.com/prologin/tech/packages/django-pypprof
```

### Comparing `flask_pypprof-0.1.12/flask_pypprof/handler.py` & `flask_pypprof-0.1.13/flask_pypprof/handler.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.12/flask_pypprof/routes.py` & `flask_pypprof-0.1.13/flask_pypprof/routes.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.12/PKG-INFO` & `flask_pypprof-0.1.13/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: flask-pypprof
-Version: 0.1.12
+Version: 0.1.13
 Summary: Pypprof Flask wrapper
 Author: Diego
 Author-email: diegolparra@gmail.com
-Requires-Python: >3.8
+Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: mprofile (==0.0.15)
 Requires-Dist: protobuf (>=3.20,<4.0)
 Requires-Dist: pypprof (==0.0.1)
 Requires-Dist: zprofile (==1.0.12)
 Description-Content-Type: text/markdown
 
 # flask-pypprof
 
-Blueprint for pprof profiling endpoints a la GO that can be added to python Flask applications. *flask-pypprof* is a wrapper of [pypprof] and based on [django-pypprof] ideas.
+Blueprint for pprof profiling endpoints a la GO's that can be added to python Flask applications. *flask-pypprof* is a wrapper of [pypprof] and based on [django-pypprof] ideas.
 
 ## Installation
 
 ```bash
-pip install flask-pypprof --extra-index-url https://<>/
+pip install flask-pypprof
 ```
 
 ## Usage
 
 To add the pprof endpoints to your application, simply register the blueprint:
 
 ```python
@@ -49,16 +49,35 @@
 
 * `MEMORY_SAMPLE_RATE`: sets the memory profiling sample rate (default: 128 * 1024)
 
 ```bash
 export MEMORY_SAMPLE_RATE = 128 * 1024
 ```
 
+## Fetching profiles from your application
+Fetch a 30 seconds CPU profile:
+
+```bash
+go tool pprof -http=:8088 http://localhost:8081/debug/pprof/profile?seconds=30
+```
+
+Fetch a heap profile:
+
+```bash
+go tool pprof -http=:8088 http://localhost:8081/debug/pprof/heap
+```
+![image_2023-05-09_16-27-22](https://github.com/dpsoft/flask-pypprof/assets/2567525/33f36ed4-0b97-44fc-89e7-2fbbbbb7132a)
+
+
+## Compatibility 
+Python **3.8**, **3.9**, **3.10** and Flask >= **2.0.0** and **Linux** only.
+    
 ## Known issues
 * `zprofile issue with python 3.11`:  https://github.com/timpalpant/zprofile/pull/2 
 
 
 ## License
+This code base is available under the Apache License, version 2.
 
 [pypprof]: https://github.com/timpalpant/pypprof
 [django-pypprof]:https://gitlab.com/prologin/tech/packages/django-pypprof
```

