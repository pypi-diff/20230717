# Comparing `tmp/velikafkaclient-1.0.8.tar.gz` & `tmp/velikafkaclient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.8.tar", last modified: Mon Jul 17 15:33:45 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.9.tar", last modified: Mon Jul 17 15:50:16 2023, max compression
```

## Comparing `velikafkaclient-1.0.8.tar` & `velikafkaclient-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701773 velikafkaclient-1.0.8/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:33:45.701652 velikafkaclient-1.0.8/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:33:45.701804 velikafkaclient-1.0.8/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:33:36.000000 velikafkaclient-1.0.8/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.700178 velikafkaclient-1.0.8/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.8/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701078 velikafkaclient-1.0.8/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.8/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.8/velikafkaclient/killer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.8/velikafkaclient/producer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1231 2023-07-17 15:33:33.000000 velikafkaclient-1.0.8/velikafkaclient/topicmanager.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.701450 velikafkaclient-1.0.8/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.8/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:33:45.700656 velikafkaclient-1.0.8/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:33:45.000000 velikafkaclient-1.0.8/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.325369 velikafkaclient-1.0.9/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-17 15:50:16.325235 velikafkaclient-1.0.9/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2787 2023-07-17 15:45:52.000000 velikafkaclient-1.0.9/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-17 15:50:16.325408 velikafkaclient-1.0.9/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-17 15:50:07.000000 velikafkaclient-1.0.9/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.322889 velikafkaclient-1.0.9/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-12 05:57:42.000000 velikafkaclient-1.0.9/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.0.9/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.324483 velikafkaclient-1.0.9/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.0.9/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.0.9/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.9/velikafkaclient/producer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1243 2023-07-17 15:49:44.000000 velikafkaclient-1.0.9/velikafkaclient/topicmanager.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.324992 velikafkaclient-1.0.9/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.9/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-17 15:50:16.323547 velikafkaclient-1.0.9/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-17 15:50:16.000000 velikafkaclient-1.0.9/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.8/PKG-INFO` & `velikafkaclient-1.0.9/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: velikafkaclient
-Version: 1.0.8
-Summary: Veli Kafka Client
-Author: Konstantine
-Author-email: kdvalishvili@veli.store
-Description-Content-Type: text/markdown
-
 ### Kafka Client for VELI.STORE
 
 ### Description
 
 This module is used for producing kafka events, subscribing to kafka topics and consuming kafka events.
 
 ### To remember:
 Each kafka topic event has a predefined structure which you can see in `velikafkaclient/eventregistration`, producer 
 and consumer both have built in validation, meaning that if incorrect object structure is sent to a topic then producer 
 will raise an exception as well as consumer.
 
 
-### How to use:
+### How to use Producer/Consumer:
 
 * Initialize kafka producer:
 
 ```python
 BOOTSTRAP_SERVERS = "kafka bootstrap servers uri"
 kafka_producer: AsyncKafkaEventProducer = AsyncKafkaEventProducer(BOOTSTRAP_SERVERS)
 await kafka_producer.start()
@@ -81,7 +73,43 @@
 
 * To register event structure to a topic go to `kafka-client/velikafkaclient/eventregistration.py` and add:
 ```python
 kafka_topic_events.register_topic_event_model(KafkaTopic.USER_REGISTRATIONS, UserRegistrationEvent)
 ```
 
 Once done follow the instructions in the `veli_libs` readme to update the library on `pyip`
+
+
+### How to manage topics with TopicManager:
+
+```python
+from velikafkaclient.topicmanager import KafkaTopicManager
+
+client = KafkaTopicManager(BOOTSTRAP_SERVERS)
+
+
+# Create Topic
+client.create_topic('topic_name')
+
+
+# Create Multiple Topics
+topics = ['topic_name_1', 'topic_name_2']
+client.create_topics(topics)
+
+
+# List Topics
+print(client.list_topics())
+
+
+# Delete Topic
+client.delete_topic('topic_name')
+
+
+# Delete Multiple Topics
+topics = ['topic_name_1', 'topic_name_2']
+client.delete_topics(topics)
+
+
+# Check if topic exists
+print(client.topic_exists('topic_name'))
+
+```
```

### Comparing `velikafkaclient-1.0.8/velikafkaclient/consumer.py` & `velikafkaclient-1.0.9/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient/decorators.py` & `velikafkaclient-1.0.9/velikafkaclient/decorators.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.9/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.9/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient/producer.py` & `velikafkaclient-1.0.9/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient/topicmanager.py` & `velikafkaclient-1.0.9/velikafkaclient/topicmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
     def __init__(self, bootstrap_servers):
         self.bootstrap_servers = bootstrap_servers
         self.client = AdminClient({
             "bootstrap.servers": bootstrap_servers
         })
 
-    def create_topic(self, topic_name, num_partitions=1, replication_factor=1):
+    def create_topic(self, topic_name: str, num_partitions=1, replication_factor=1):
         topics_list = [NewTopic(topic_name, num_partitions=num_partitions, replication_factor=replication_factor)]
         return self.client.create_topics(topics_list)
 
-    def create_topics(self, topic_names, num_partitions=1, replication_factor=1):
+    def create_topics(self, topic_names: [str], num_partitions=1, replication_factor=1):
         topics_list = [NewTopic(tn, num_partitions=num_partitions, replication_factor=replication_factor) for tn in
                        topic_names]
         return self.client.create_topics(topics_list)
 
     def list_topics(self) -> [str]:
         return list(self.client.list_topics().topics.keys())
```

### Comparing `velikafkaclient-1.0.8/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.9/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.8/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.8
+Version: 1.0.9
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
 
@@ -14,15 +14,15 @@
 
 ### To remember:
 Each kafka topic event has a predefined structure which you can see in `velikafkaclient/eventregistration`, producer 
 and consumer both have built in validation, meaning that if incorrect object structure is sent to a topic then producer 
 will raise an exception as well as consumer.
 
 
-### How to use:
+### How to use Producer/Consumer:
 
 * Initialize kafka producer:
 
 ```python
 BOOTSTRAP_SERVERS = "kafka bootstrap servers uri"
 kafka_producer: AsyncKafkaEventProducer = AsyncKafkaEventProducer(BOOTSTRAP_SERVERS)
 await kafka_producer.start()
@@ -81,7 +81,43 @@
 
 * To register event structure to a topic go to `kafka-client/velikafkaclient/eventregistration.py` and add:
 ```python
 kafka_topic_events.register_topic_event_model(KafkaTopic.USER_REGISTRATIONS, UserRegistrationEvent)
 ```
 
 Once done follow the instructions in the `veli_libs` readme to update the library on `pyip`
+
+
+### How to manage topics with TopicManager:
+
+```python
+from velikafkaclient.topicmanager import KafkaTopicManager
+
+client = KafkaTopicManager(BOOTSTRAP_SERVERS)
+
+
+# Create Topic
+client.create_topic('topic_name')
+
+
+# Create Multiple Topics
+topics = ['topic_name_1', 'topic_name_2']
+client.create_topics(topics)
+
+
+# List Topics
+print(client.list_topics())
+
+
+# Delete Topic
+client.delete_topic('topic_name')
+
+
+# Delete Multiple Topics
+topics = ['topic_name_1', 'topic_name_2']
+client.delete_topics(topics)
+
+
+# Check if topic exists
+print(client.topic_exists('topic_name'))
+
+```
```

### Comparing `velikafkaclient-1.0.8/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.9/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

