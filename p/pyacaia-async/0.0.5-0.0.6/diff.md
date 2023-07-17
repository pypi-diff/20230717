# Comparing `tmp/pyacaia_async-0.0.5.tar.gz` & `tmp/pyacaia_async-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.5.tar", last modified: Sun Jul 16 06:09:07 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.6.tar", last modified: Mon Jul 17 05:47:52 2023, max compression
```

## Comparing `pyacaia_async-0.0.5.tar` & `pyacaia_async-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 06:09:07.000000 pyacaia_async-0.0.5/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 06:09:07.773082 pyacaia_async-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 06:08:53.000000 pyacaia_async-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/setup.py
```

### Comparing `pyacaia_async-0.0.5/LICENSE` & `pyacaia_async-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.5/PKG-INFO` & `pyacaia_async-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia_async
-Version: 0.0.5
+Version: 0.0.6
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.5/README.md` & `pyacaia_async-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.5/pyacaia_async/acaiascale.py` & `pyacaia_async-0.0.6/pyacaia_async/acaiascale.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,21 +193,23 @@
             self._connected = False
             _LOGGER.debug("Disconnected from Acaia Scale.")
         except Exception as ex:
             _LOGGER.debug("Error disconnecting from device: %s", ex)
 
 
     async def tare(self) -> None:
+        await self.auth()
         await self._queue.put((
                 DEFAULT_CHAR_ID, 
                 self.msg_types["tare"]
             ))
 
 
     async def startStopTimer(self) -> None:
+        await self.auth()
         if not self._timer_running:
             await self._queue.put((      
                     DEFAULT_CHAR_ID, 
                     self.msg_types["startTimer"]
                 ))
             self._timer_running = True
             if not self._timer_start:
@@ -218,14 +220,15 @@
                     self.msg_types["stopTimer"]
                 ))
             self._timer_running = False
             self._timer_stop = time.time()
 
 
     async def resetTimer(self) -> None:
+        await self.auth()
         await self._queue.put((
                 DEFAULT_CHAR_ID, 
                 self.msg_types["resetTimer"]
             ))
         self._timer_start = None
         self._timer_stop = None
```

### Comparing `pyacaia_async-0.0.5/pyacaia_async/decode.py` & `pyacaia_async-0.0.6/pyacaia_async/decode.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.5/pyacaia_async/helpers.py` & `pyacaia_async-0.0.6/pyacaia_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.5/pyacaia_async.egg-info/PKG-INFO` & `pyacaia_async-0.0.6/pyacaia_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia-async
-Version: 0.0.5
+Version: 0.0.6
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.5/setup.py` & `pyacaia_async-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.5",
+    version="0.0.6",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

