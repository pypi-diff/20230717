# Comparing `tmp/velikafkaclient-1.0.7.tar.gz` & `tmp/velikafkaclient-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.7.tar", last modified: Mon Jul 17 15:30:40 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.8.tar", last modified: Mon Jul 17 15:33:45 2023, max compression
```

## Comparing `velikafkaclient-1.0.7.tar` & `velikafkaclient-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.040526 velikafkaclient-1.0.7/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:30:40.040408 velikafkaclient-1.0.7/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:30:40.040556 velikafkaclient-1.0.7/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:30:27.000000 velikafkaclient-1.0.7/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.038685 velikafkaclient-1.0.7/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.7/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.039702 velikafkaclient-1.0.7/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.7/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.7/velikafkaclient/killer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.7/velikafkaclient/producer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1216 2023-07-17 15:30:27.000000 velikafkaclient-1.0.7/velikafkaclient/topicmanager.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.040241 velikafkaclient-1.0.7/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.7/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:30:40.039220 velikafkaclient-1.0.7/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:30:40.000000 velikafkaclient-1.0.7/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701773 velikafkaclient-1.0.8/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:33:45.701652 velikafkaclient-1.0.8/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:33:45.701804 velikafkaclient-1.0.8/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:33:36.000000 velikafkaclient-1.0.8/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.700178 velikafkaclient-1.0.8/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.8/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701078 velikafkaclient-1.0.8/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.8/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.8/velikafkaclient/producer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1231 2023-07-17 15:33:33.000000 velikafkaclient-1.0.8/velikafkaclient/topicmanager.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701450 velikafkaclient-1.0.8/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.700656 velikafkaclient-1.0.8/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.7/PKG-INFO` & `velikafkaclient-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.7
+Version: 1.0.8
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.7/readme.md` & `velikafkaclient-1.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/consumer.py` & `velikafkaclient-1.0.8/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/decorators.py` & `velikafkaclient-1.0.8/velikafkaclient/decorators.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.8/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.8/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/producer.py` & `velikafkaclient-1.0.8/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient/topicmanager.py` & `velikafkaclient-1.0.8/velikafkaclient/topicmanager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from confluent_kafka.admin import AdminClient, NewTopic
 
 
-class KafkaTopicAdmin:
+class KafkaTopicManager:
 
     def __init__(self, bootstrap_servers):
         self.bootstrap_servers = bootstrap_servers
         self.client = AdminClient({
             "bootstrap.servers": bootstrap_servers
         })
 
@@ -15,15 +15,15 @@
 
     def create_topics(self, topic_names, num_partitions=1, replication_factor=1):
         topics_list = [NewTopic(tn, num_partitions=num_partitions, replication_factor=replication_factor) for tn in
                        topic_names]
         return self.client.create_topics(topics_list)
 
     def list_topics(self) -> [str]:
-        return self.client.list_topics().topics
+        return list(self.client.list_topics().topics.keys())
 
     def topic_exists(self, topic_name) -> bool:
         return self.client.list_topics().topics.get(topic_name) is not None
 
     def delete_topic(self, topic_name):
         self.client.delete_topics(topics=[topic_name])
```

### Comparing `velikafkaclient-1.0.7/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.8/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.7/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.0.8/velikafkaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.7
+Version: 1.0.8
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.7/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.8/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

