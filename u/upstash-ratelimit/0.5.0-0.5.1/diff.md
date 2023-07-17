# Comparing `tmp/upstash_ratelimit-0.5.0.tar.gz` & `tmp/upstash_ratelimit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.5.0.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.5.1.tar", max compression
```

## Comparing `upstash_ratelimit-0.5.0.tar` & `upstash_ratelimit-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/LICENSE
--rw-r--r--   0        0        0     8060 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/README.md
--rw-r--r--   0        0        0     1331 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0      253 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     4481 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/asyncio/ratelimit.py
--rw-r--r--   0        0        0    14777 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0     4244 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/ratelimit.py
--rw-r--r--   0        0        0      138 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/typing.py
--rw-r--r--   0        0        0     1123 2023-07-10 10:44:19.023758 upstash_ratelimit-0.5.0/upstash_ratelimit/utils.py
--rw-r--r--   0        0        0     9253 1970-01-01 00:00:00.000000 upstash_ratelimit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-17 10:57:03.774984 upstash_ratelimit-0.5.1/LICENSE
+-rw-r--r--   0        0        0     8062 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/README.md
+-rw-r--r--   0        0        0     1331 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     4482 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/ratelimit.py
+-rw-r--r--   0        0        0    14777 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0     4245 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/ratelimit.py
+-rw-r--r--   0        0        0      138 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/typing.py
+-rw-r--r--   0        0        0     1123 2023-07-17 10:57:03.778984 upstash_ratelimit-0.5.1/upstash_ratelimit/utils.py
+-rw-r--r--   0        0        0     9255 1970-01-01 00:00:00.000000 upstash_ratelimit-0.5.1/PKG-INFO
```

### Comparing `upstash_ratelimit-0.5.0/LICENSE` & `upstash_ratelimit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.0/README.md` & `upstash_ratelimit-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 # Create a new ratelimiter, that allows 10 requests per 10 seconds
 ratelimit = Ratelimit(
     redis=Redis.from_env(),
     limiter=FixedWindow(max_requests=10, window=10),
     # Optional prefix for the keys used in Redis. This is useful
     # if you want to share a Redis instance with other applications
     # and want to avoid key collisions. The default prefix is
-    # "upstash-ratelimit"
-    prefix="upstash-ratelimit",
+    # "@upstash/ratelimit"
+    prefix="@upstash/ratelimit",
 )
 
 # Use a constant string to limit all requests with a single ratelimit
 # Or use a user ID, API key or IP address for individual limits.
 identifier = "api"
 response = ratelimit.limit(identifier)
```

### Comparing `upstash_ratelimit-0.5.0/pyproject.toml` & `upstash_ratelimit-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upstash-ratelimit"
-version = "0.5.0"
+version = "0.5.1"
 description = "Serverless ratelimiting package from Upstash"
 authors = ["Upstash <support@upstash.com>", "Zgîmbău Tudor <tudor.zgimbau@gmail.com>"]
 maintainers = ["Upstash <support@upstash.com>"]
 readme = "README.md"
 repository = "https://github.com/upstash/ratelimit-python"
 keywords = ["ratelimit", "rate limit", "Upstash rate limit", "Redis rate limit"]
 classifiers = [
```

### Comparing `upstash_ratelimit-0.5.0/upstash_ratelimit/asyncio/ratelimit.py` & `upstash_ratelimit-0.5.1/upstash_ratelimit/asyncio/ratelimit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Ratelimit:
     """
     Provides means of ratelimitting over the HTTP-based
     Upstash Redis client.
     """
 
     def __init__(
-        self, redis: Redis, limiter: Limiter, prefix: str = "upstash-ratelimit"
+        self, redis: Redis, limiter: Limiter, prefix: str = "@upstash/ratelimit"
     ) -> None:
         """
         :param redis: Upstash Redis instance to use.
         :param limiter: Ratelimiter to use. Available limiters are \
             `FixedWindow`, `SlidingWindow`, and `TokenBucket` which are provided \
             in the `limiter` module. 
         :param prefix: Prefix to distinguish the keys used in the ratelimit \
```

### Comparing `upstash_ratelimit-0.5.0/upstash_ratelimit/limiter.py` & `upstash_ratelimit-0.5.1/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.0/upstash_ratelimit/ratelimit.py` & `upstash_ratelimit-0.5.1/upstash_ratelimit/ratelimit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Ratelimit:
     """
     Provides means of ratelimitting over the HTTP-based
     Upstash Redis client.
     """
 
     def __init__(
-        self, redis: Redis, limiter: Limiter, prefix: str = "upstash-ratelimit"
+        self, redis: Redis, limiter: Limiter, prefix: str = "@upstash/ratelimit"
     ) -> None:
         """
         :param redis: Upstash Redis instance to use.
         :param limiter: Ratelimiter to use. Available limiters are \
             `FixedWindow`, `SlidingWindow`, and `TokenBucket` which are provided \
             in the `limiter` module. 
         :param prefix: Prefix to distinguish the keys used in the ratelimit \
```

### Comparing `upstash_ratelimit-0.5.0/upstash_ratelimit/utils.py` & `upstash_ratelimit-0.5.1/upstash_ratelimit/utils.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.5.0/PKG-INFO` & `upstash_ratelimit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.5.0
+Version: 0.5.1
 Summary: Serverless ratelimiting package from Upstash
 Home-page: https://github.com/upstash/ratelimit-python
 Keywords: ratelimit,rate limit,Upstash rate limit,Redis rate limit
 Author: Upstash
 Author-email: support@upstash.com
 Maintainer: Upstash
 Maintainer-email: support@upstash.com
@@ -87,16 +87,16 @@
 # Create a new ratelimiter, that allows 10 requests per 10 seconds
 ratelimit = Ratelimit(
     redis=Redis.from_env(),
     limiter=FixedWindow(max_requests=10, window=10),
     # Optional prefix for the keys used in Redis. This is useful
     # if you want to share a Redis instance with other applications
     # and want to avoid key collisions. The default prefix is
-    # "upstash-ratelimit"
-    prefix="upstash-ratelimit",
+    # "@upstash/ratelimit"
+    prefix="@upstash/ratelimit",
 )
 
 # Use a constant string to limit all requests with a single ratelimit
 # Or use a user ID, API key or IP address for individual limits.
 identifier = "api"
 response = ratelimit.limit(identifier)
```

