# Comparing `tmp/velikafkaclient-1.0.6.tar.gz` & `tmp/velikafkaclient-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.6.tar", last modified: Wed Jul 12 11:24:51 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.7.tar", last modified: Mon Jul 17 15:30:40 2023, max compression
```

## Comparing `velikafkaclient-1.0.6.tar` & `velikafkaclient-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 11:24:51.571248 velikafkaclient-1.0.6/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-12 11:24:51.571135 velikafkaclient-1.0.6/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:57:42.000000 velikafkaclient-1.0.6/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-12 11:24:51.571278 velikafkaclient-1.0.6/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-12 11:24:44.000000 velikafkaclient-1.0.6/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 11:24:51.569019 velikafkaclient-1.0.6/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.6/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.6/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 11:24:51.570550 velikafkaclient-1.0.6/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.6/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.6/velikafkaclient/killer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.6/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 11:24:51.570944 velikafkaclient-1.0.6/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.6/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 11:24:51.569617 velikafkaclient-1.0.6/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-12 11:24:51.000000 velikafkaclient-1.0.6/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      603 2023-07-12 11:24:51.000000 velikafkaclient-1.0.6/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-12 11:24:51.000000 velikafkaclient-1.0.6/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-12 11:24:51.000000 velikafkaclient-1.0.6/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.040526 velikafkaclient-1.0.7/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:30:40.040408 velikafkaclient-1.0.7/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:30:40.040556 velikafkaclient-1.0.7/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:30:27.000000 velikafkaclient-1.0.7/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.038685 velikafkaclient-1.0.7/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.7/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.039702 velikafkaclient-1.0.7/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.7/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.7/velikafkaclient/producer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1216 2023-07-17 15:30:27.000000 velikafkaclient-1.0.7/velikafkaclient/topicmanager.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.040241 velikafkaclient-1.0.7/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.039220 velikafkaclient-1.0.7/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.6/PKG-INFO` & `velikafkaclient-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.6
+Version: 1.0.7
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.6/readme.md` & `velikafkaclient-1.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/consumer.py` & `velikafkaclient-1.0.7/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/decorators.py` & `velikafkaclient-1.0.7/velikafkaclient/decorators.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.7/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.7/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/producer.py` & `velikafkaclient-1.0.7/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.7/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.6/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.0.7/velikafkaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.6
+Version: 1.0.7
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.6/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.7/velikafkaclient.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 velikafkaclient/__init__.py
 velikafkaclient/consumer.py
 velikafkaclient/decorators.py
 velikafkaclient/eventregistration.py
 velikafkaclient/exceptions.py
 velikafkaclient/killer.py
 velikafkaclient/producer.py
+velikafkaclient/topicmanager.py
 velikafkaclient.egg-info/PKG-INFO
 velikafkaclient.egg-info/SOURCES.txt
 velikafkaclient.egg-info/dependency_links.txt
 velikafkaclient.egg-info/top_level.txt
 velikafkaclient/events/__init__.py
 velikafkaclient/events/base.py
 velikafkaclient/events/triptracker.py
```

