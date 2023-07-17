# Comparing `tmp/redis-simple-mq-0.5.0.tar.gz` & `tmp/redis_simple_mq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-simple-mq-0.5.0.tar", last modified: Thu Mar 23 22:06:40 2023, max compression
+gzip compressed data, was "redis_simple_mq-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `redis-simple-mq-0.5.0.tar` & `redis_simple_mq-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,6 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 22:06:40.097211 redis-simple-mq-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2021-01-01 20:50:32.000000 redis-simple-mq-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       67 2021-01-01 20:50:32.000000 redis-simple-mq-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-23 22:06:40.097211 redis-simple-mq-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-03-23 21:56:41.000000 redis-simple-mq-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 22:06:40.093211 redis-simple-mq-0.5.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-03-23 20:41:23.000000 redis-simple-mq-0.5.0/examples/hello_world.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-03-23 21:04:46.000000 redis-simple-mq-0.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 22:06:40.097211 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-23 22:06:40.000000 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-03-23 22:06:40.000000 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 22:06:40.000000 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-23 22:06:40.000000 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-23 22:06:40.000000 redis-simple-mq-0.5.0/redis_simple_mq.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-03-23 22:06:40.101211 redis-simple-mq-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 22:06:40.097211 redis-simple-mq-0.5.0/simple_mq/
--rw-rw-rw-   0 root         (0) root         (0)       35 2021-01-01 20:50:32.000000 redis-simple-mq-0.5.0/simple_mq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3297 2023-03-23 21:55:10.000000 redis-simple-mq-0.5.0/simple_mq/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 22:06:40.097211 redis-simple-mq-0.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-23 20:41:23.000000 redis-simple-mq-0.5.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3283 2023-03-23 21:48:29.000000 redis-simple-mq-0.5.0/tests/tests.py
+-rw-r--r--   0        0        0     1070 2021-01-01 20:50:32.254559 redis_simple_mq-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1811 2023-07-17 16:19:11.226710 redis_simple_mq-1.0.0/README.md
+-rw-r--r--   0        0        0     1161 2023-07-17 14:00:15.616042 redis_simple_mq-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-07-17 19:37:55.159872 redis_simple_mq-1.0.0/src/simple_mq/__init__.py
+-rw-r--r--   0        0        0     3373 2023-07-17 19:37:55.159872 redis_simple_mq-1.0.0/src/simple_mq/core.py
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 redis_simple_mq-1.0.0/PKG-INFO
```

### Comparing `redis-simple-mq-0.5.0/LICENSE` & `redis_simple_mq-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-simple-mq-0.5.0/PKG-INFO` & `redis_simple_mq-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: redis-simple-mq
-Version: 0.5.0
-Summary: Simple message queue based on Redis
-Home-page: https://gitlab.com/ErikKalkoken/redis-simple-mq
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Keywords: redis,queue
+Version: 1.0.0
+Summary: Simple message queue based on Redis.
+Keywords: queue,redis
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: redis
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/redis-simple-mq
 
 # redis-simple-mq
 
 A simple message queue for Redis.
 
 [![release](https://img.shields.io/pypi/v/redis-simple-mq?label=release)](https://pypi.org/project/redis-simple-mq/)
 [![python](https://img.shields.io/pypi/pyversions/redis-simple-mq)](https://pypi.org/project/redis-simple-mq/)
 [![pipeline](https://gitlab.com/ErikKalkoken/redis-simple-mq/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/redis-simple-mq/-/pipelines)
-[![codecov](https://codecov.io/gl/ErikKalkoken/redis-simple-mq/branch/\x6d6173746572/graph/badge.svg?token=M1IBQV97BE)](https://codecov.io/gl/ErikKalkoken/redis-simple-mq)
+[![codecov](https://codecov.io/gl/ErikKalkoken/redis-simple-mq/branch/master/graph/badge.svg?token=M1IBQV97BE)](https://codecov.io/gl/ErikKalkoken/redis-simple-mq)
+[![Documentation Status](https://readthedocs.org/projects/redis-simple-mq/badge/?version=latest)](https://redis-simple-mq.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/redis-simple-mq/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Description
 
@@ -54,7 +54,8 @@
 q = SimpleMQ(conn)
 q.enqueue('Hello, World!')
 message = q.dequeue()
 print(message)
 ```
 
 See also the examples folder for examples.
+
```

### Comparing `redis-simple-mq-0.5.0/README.md` & `redis_simple_mq-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # redis-simple-mq
 
 A simple message queue for Redis.
 
 [![release](https://img.shields.io/pypi/v/redis-simple-mq?label=release)](https://pypi.org/project/redis-simple-mq/)
 [![python](https://img.shields.io/pypi/pyversions/redis-simple-mq)](https://pypi.org/project/redis-simple-mq/)
 [![pipeline](https://gitlab.com/ErikKalkoken/redis-simple-mq/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/redis-simple-mq/-/pipelines)
-[![codecov](https://codecov.io/gl/ErikKalkoken/redis-simple-mq/branch/\x6d6173746572/graph/badge.svg?token=M1IBQV97BE)](https://codecov.io/gl/ErikKalkoken/redis-simple-mq)
+[![codecov](https://codecov.io/gl/ErikKalkoken/redis-simple-mq/branch/master/graph/badge.svg?token=M1IBQV97BE)](https://codecov.io/gl/ErikKalkoken/redis-simple-mq)
+[![Documentation Status](https://readthedocs.org/projects/redis-simple-mq/badge/?version=latest)](https://redis-simple-mq.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/redis-simple-mq/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Description
```

### Comparing `redis-simple-mq-0.5.0/simple_mq/core.py` & `redis_simple_mq-1.0.0/src/simple_mq/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Core logic for simple mq."""
+
 import secrets
 import string
 from typing import Iterable, List, Optional
 
 from redis import Redis
 
 
@@ -36,33 +38,34 @@
 
     def _redis_key(self) -> str:
         """Full key used to locate this queue on redis."""
         return f"{self.REDIS_KEY_PREFIX}_{self.name}"
 
     @property
     def conn(self) -> Redis:
+        """Return redis connection."""
         return self._conn
 
     @property
     def name(self) -> str:
+        """Return name."""
         return self._name
 
     def size(self) -> int:
         """Current number of messages in the queue"""
         return int(self.conn.llen(self._redis_key()))
 
     def clear(self) -> int:
         """Purge all messages from the queue and return count of cleared messages."""
         total = 0
         while True:
             message = self.dequeue()
             if message is None:
                 break
-            else:
-                total += 1
+            total += 1
         return total
 
     def enqueue(self, message: str) -> int:
         """Enqueue one message into the queue
         and return size of the queue after enqueuing.
         """
         return self.conn.rpush(self._redis_key(), str(message))
@@ -80,30 +83,28 @@
     def dequeue(self) -> Optional[str]:
         """Dequeue one message from the queue. Return None if queue was empty."""
         value = self.conn.lpop(self._redis_key())
         if value is not None:
             return value.decode("utf8")
         return None
 
-    def dequeue_bulk(self, max: Optional[int] = None) -> List[str]:
+    def dequeue_bulk(self, max_messages: Optional[int] = None) -> List[str]:
         """Dequeue a list of message from the queue.
 
         Return no more than max message from queue
         or return all messages if max is not specified.
         Returns an empty list if queue is empty.
         """
-        if max is not None and int(max) < 0:
-            raise ValueError("max can not be negative")
+        if max_messages is not None and int(max_messages) < 0:
+            raise ValueError("max_messages can not be negative")
 
         messages = []
-        n = 0
+        i = 0
         while True:
-            if max is not None and n == int(max):
+            if max_messages is not None and i == int(max_messages):
+                break
+            i += 1
+            data = self.dequeue()
+            if data is None:
                 break
-            else:
-                n += 1
-                x = self.dequeue()
-                if x is None:
-                    break
-                else:
-                    messages.append(x)
+            messages.append(data)
         return messages
```

