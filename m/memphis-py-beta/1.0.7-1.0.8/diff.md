# Comparing `tmp/memphis-py-beta-1.0.7.tar.gz` & `tmp/memphis-py-beta-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-1.0.7.tar", last modified: Sun Jul  9 15:31:27 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.8.tar", last modified: Mon Jul 17 19:59:00 2023, max compression
```

## Comparing `memphis-py-beta-1.0.7.tar` & `memphis-py-beta-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12843 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9588 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13667 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12843 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11224 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13678 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-07-17 19:58:53.000000 memphis-py-beta-1.0.8/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-07-17 19:59:00.000000 memphis-py-beta-1.0.8/setup.py
```

### Comparing `memphis-py-beta-1.0.7/PKG-INFO` & `memphis-py-beta-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.7
+Version: 1.0.8
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.8.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-beta-1.0.7/README.md` & `memphis-py-beta-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/__init__.py` & `memphis-py-beta-1.0.8/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/consumer.py` & `memphis-py-beta-1.0.8/memphis/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,48 @@
         self.t_consume = None
 
     def set_context(self, context):
         """Set a context (dict) that will be passed to each message handler call."""
         self.context = context
 
     def consume(self, callback):
-        """Consume events."""
+        """
+        This method starts consuming events from the specified station and invokes the provided callback function for each batch of messages received.
+
+        Parameters:
+            callback (function): A function that will be called with each batch of messages received. The function should have the following signature:
+                - `callback(messages: List[Message], error: Optional[MemphisError], context: Dict) -> Awaitable[None]`
+                - `messages`: A list of `Message` objects representing the batch of messages received.
+                - `error`: An optional `MemphisError` object if there was an error while consuming the messages.
+                - `context`: A dictionary representing the context that was set using the `set_context()` method.
+
+        Example:
+            import asyncio
+            from memphis import Memphis
+
+            async def message_handler(messages, error, context):
+                if error:
+                    print(f"Error occurred: {error}")
+                    return
+
+                for message in messages:
+                    print(f"Received message: {message}")
+
+            async def main():
+                memphis = Memphis()
+                await memphis.connect(host='localhost', username='user', password='pass')
+                consumer = await memphis.consumer(station_name='my_station', consumer_name='my_consumer', consumer_group='my_group')
+                consumer.set_context({'key': 'value'})
+                consumer.consume(message_handler)
+
+                # Keep the event loop running
+                while True:
+                    await asyncio.sleep(1)
+            asyncio.run(main())
+        """
         self.dls_callback_func = callback
         self.t_consume = asyncio.create_task(self.__consume(callback))
 
     async def __consume(self, callback):
         subject = get_internal_name(self.station_name)
         consumer_group = get_internal_name(self.consumer_group)
         self.psub = await self.connection.broker_connection.pull_subscribe(
@@ -125,15 +158,15 @@
 
         Example:
 
             import asyncio
             
             from memphis import Memphis
 
-            async def main(/, host, username, password, station):
+            async def main(host, username, password, station):
                 memphis = Memphis()
                 await memphis.connect(host=host,
                                       username=username,
                                       password=password)
             
                 consumer = await memphis.consumer(station_name=station,
                                                   consumer_name="test-consumer",
@@ -145,18 +178,18 @@
                     for msg in batch:
                         serialized_record = msg.get_data()
                         print("Message:", serialized_record)
             
                 await memphis.close()
 
             if __name__ == '__main__':
-                asyncio.run(main(host=host,
-                                 username=username,
-                                 password=password,
-                                 station=station))
+                asyncio.run(main(host,
+                                 username,
+                                 password,
+                                 station))
         
         """
         messages = []
         if self.connection.is_connection_active:
             try:
                 if batch_size > self.MAX_BATCH_SIZE:
                     raise MemphisError(
```

### Comparing `memphis-py-beta-1.0.7/memphis/exceptions.py` & `memphis-py-beta-1.0.8/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/headers.py` & `memphis-py-beta-1.0.8/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/memphis.py` & `memphis-py-beta-1.0.8/memphis/memphis.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/message.py` & `memphis-py-beta-1.0.8/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/producer.py` & `memphis-py-beta-1.0.8/memphis/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,21 +261,20 @@
                         + self.producer_name
                         + "\nError:"
                         + str(e),
                         msg_to_send,
                         schemaverse_fail_alert_type,
                     )
             raise e
-        except Exception as e:
+        except Exception as e: # pylint: disable-next=no-member
             if hasattr(e, "status_code") and e.status_code == "503":
                 raise MemphisError(
                     "Produce operation has failed, please check whether Station/Producer still exist"
                 )
-            else:
-                raise MemphisError(str(e)) from e
+            raise MemphisError(str(e)) from e
 
     async def destroy(self):
         """Destroy the producer."""
         try:
             destroy_producer_req = {
                 "name": self.producer_name,
                 "station_name": self.station_name,
```

### Comparing `memphis-py-beta-1.0.7/memphis/station.py` & `memphis-py-beta-1.0.8/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/types.py` & `memphis-py-beta-1.0.8/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis/utils.py` & `memphis-py-beta-1.0.8/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.7/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.8/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.7
+Version: 1.0.8
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.8.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-beta-1.0.7/setup.py` & `memphis-py-beta-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="1.0.7",
+    version="1.0.8",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.8.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

