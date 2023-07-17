# Comparing `tmp/cachetory-2.7.0.tar.gz` & `tmp/cachetory-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.7.0.tar", max compression
+gzip compressed data, was "cachetory-2.8.0.tar", max compression
```

## Comparing `cachetory-2.7.0.tar` & `cachetory-2.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11355 2023-07-12 15:16:14.500930 cachetory-2.7.0/LICENSE
--rw-r--r--   0        0        0    14352 2023-07-12 15:16:14.500930 cachetory-2.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     2385 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/django.py
--rw-r--r--   0        0        0     1520 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1718 2023-07-12 15:16:14.500930 cachetory-2.7.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2476 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0     1266 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     2220 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/django.py
--rw-r--r--   0        0        0     1408 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2340 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2201 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     4241 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     3665 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3959 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3489 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      481 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      909 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-07-12 15:16:14.504930 cachetory-2.7.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3235 2023-07-12 15:16:28.077126 cachetory-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    15899 1970-01-01 00:00:00.000000 cachetory-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-17 14:32:17.842513 cachetory-2.8.0/LICENSE
+-rw-r--r--   0        0        0    14352 2023-07-17 14:32:17.842513 cachetory-2.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     2385 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/django.py
+-rw-r--r--   0        0        0     1520 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1718 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2476 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0     1266 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     2220 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/django.py
+-rw-r--r--   0        0        0     1408 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2340 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2201 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     4241 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3665 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3959 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3489 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      481 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3234 2023-07-17 14:32:30.802511 cachetory-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    15890 1970-01-01 00:00:00.000000 cachetory-2.8.0/PKG-INFO
```

### Comparing `cachetory-2.7.0/LICENSE` & `cachetory-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/README.md` & `cachetory-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/async_/__init__.py` & `cachetory-2.8.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/async_/django.py` & `cachetory-2.8.0/cachetory/backends/async_/django.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/async_/dummy.py` & `cachetory-2.8.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/async_/memory.py` & `cachetory-2.8.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/async_/redis.py` & `cachetory-2.8.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/sync/__init__.py` & `cachetory-2.8.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/sync/django.py` & `cachetory-2.8.0/cachetory/backends/sync/django.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/sync/dummy.py` & `cachetory-2.8.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/sync/memory.py` & `cachetory-2.8.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/backends/sync/redis.py` & `cachetory-2.8.0/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/caches/async_.py` & `cachetory-2.8.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/caches/sync.py` & `cachetory-2.8.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/decorators/async_.py` & `cachetory-2.8.0/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/decorators/shared.py` & `cachetory-2.8.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/decorators/sync.py` & `cachetory-2.8.0/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.8.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/interfaces/backends/private.py` & `cachetory-2.8.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.8.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/interfaces/serializers.py` & `cachetory-2.8.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/private/functools.py` & `cachetory-2.8.0/cachetory/private/functools.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/chained.py` & `cachetory-2.8.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.8.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/compressors/zstd.py` & `cachetory-2.8.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/json.py` & `cachetory-2.8.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/msgpack.py` & `cachetory-2.8.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/noop.py` & `cachetory-2.8.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/cachetory/serializers/pickle.py` & `cachetory-2.8.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.7.0/pyproject.toml` & `cachetory-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.7.0"
+version = "2.8.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -31,15 +31,15 @@
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
 django = {version = "^4.0.0", optional = true}
 ormsgpack = {version = "^1.2.6", optional = true, markers = "platform_python_implementation == 'CPython'"}
-pydantic = "^1.10.4"
+pydantic = "<3.0.0"
 python = "^3.8.0"
 redis = {version = "^4.4.2", optional = true}
 typing-extensions = "^4.4.0"
 zstd = {version = "^1.5.2.6", optional = true}
 
 [tool.poetry.extras]
 django = ["django"]
```

### Comparing `cachetory-2.7.0/PKG-INFO` & `cachetory-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.7.0
+Version: 2.8.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -24,15 +24,15 @@
 Classifier: Typing :: Typed
 Provides-Extra: django
 Provides-Extra: ormsgpack
 Provides-Extra: redis
 Provides-Extra: zstd
 Requires-Dist: django (>=4.0.0,<5.0.0) ; extra == "django"
 Requires-Dist: ormsgpack (>=1.2.6,<2.0.0) ; (platform_python_implementation == "CPython") and (extra == "ormsgpack")
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (<3.0.0)
 Requires-Dist: redis (>=4.4.2,<5.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: zstd (>=1.5.2.6,<2.0.0.0) ; extra == "zstd"
 Project-URL: Repository, https://github.com/kpn/cachetory
 Description-Content-Type: text/markdown
 
 # Cachetory
```

