# Comparing `tmp/pynisher-1.0.5.tar.gz` & `tmp/pynisher-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynisher-1.0.5.tar", last modified: Sun Mar 19 16:43:10 2023, max compression
+gzip compressed data, was "pynisher-1.0.6.tar", last modified: Mon Jul 17 09:42:30 2023, max compression
```

## Comparing `pynisher-1.0.5.tar` & `pynisher-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-03-19 16:43:10.570834 pynisher-1.0.5/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.5/LICENSE
--rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.5/MANIFEST.in
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-03-19 16:43:10.570834 pynisher-1.0.5/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)    13803 2023-03-13 20:53:22.000000 pynisher-1.0.5/README.md
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-03-19 16:43:10.570834 pynisher-1.0.5/pynisher/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/exceptions.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-03-19 16:43:10.570834 pynisher-1.0.5/pynisher/limiters/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/limiters/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    11795 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/limiters/limiter.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2602 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/limiters/linux.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3214 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/limiters/mac.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4996 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/limiters/windows.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/py.typed
--rw-r--r--   0 skantify  (1000) skantify  (1000)    26449 2023-03-19 16:40:33.000000 pynisher-1.0.5/pynisher/pynisher.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/support.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.5/pynisher/util.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.5/pynisher/win_errcodes.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-03-19 16:43:10.570834 pynisher-1.0.5/pynisher.egg-info/
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-03-19 16:43:10.000000 pynisher-1.0.5/pynisher.egg-info/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-03-19 16:43:10.000000 pynisher-1.0.5/pynisher.egg-info/SOURCES.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-03-19 16:43:10.000000 pynisher-1.0.5/pynisher.egg-info/dependency_links.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-03-19 16:43:10.000000 pynisher-1.0.5/pynisher.egg-info/requires.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-03-19 16:43:10.000000 pynisher-1.0.5/pynisher.egg-info/top_level.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-03-13 20:53:22.000000 pynisher-1.0.5/pyproject.toml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-03-19 16:43:10.570834 pynisher-1.0.5/setup.cfg
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-03-19 16:40:45.000000 pynisher-1.0.5/setup.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.6/LICENSE
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.6/MANIFEST.in
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-07-17 09:42:29.996314 pynisher-1.0.6/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    13803 2023-03-13 20:53:22.000000 pynisher-1.0.6/README.md
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/exceptions.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher/limiters/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/limiters/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    11791 2023-07-17 09:27:44.000000 pynisher-1.0.6/pynisher/limiters/limiter.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2625 2023-07-17 09:31:11.000000 pynisher-1.0.6/pynisher/limiters/linux.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3214 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/limiters/mac.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4995 2023-07-17 09:27:44.000000 pynisher-1.0.6/pynisher/limiters/windows.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/py.typed
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    26577 2023-07-17 09:14:39.000000 pynisher-1.0.6/pynisher/pynisher.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/support.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.6/pynisher/util.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/win_errcodes.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher.egg-info/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/SOURCES.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/dependency_links.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/requires.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/top_level.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-07-17 09:28:49.000000 pynisher-1.0.6/pyproject.toml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-07-17 09:42:29.996314 pynisher-1.0.6/setup.cfg
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-07-17 09:14:50.000000 pynisher-1.0.6/setup.py
```

### Comparing `pynisher-1.0.5/LICENSE` & `pynisher-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/PKG-INFO` & `pynisher-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.5
+Version: 1.0.6
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pynisher-1.0.5/README.md` & `pynisher-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/__init__.py` & `pynisher-1.0.6/pynisher/__init__.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/exceptions.py` & `pynisher-1.0.6/pynisher/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/limiters/limiter.py` & `pynisher-1.0.6/pynisher/limiters/limiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
             Arguments to the function
 
         Returns
         -------
         None
         """
         try:
-
             if self.cpu_time is not None:
                 self.limit_cpu_time(self.cpu_time)
 
             if self.memory is not None:
                 # We should probably warn if we exceed the memory usage before
                 # any limitation is set
                 memusage = Monitor().memory("B")
@@ -249,15 +248,14 @@
         ...
 
     def _raise_warning(self, msg: str) -> None:
         if self.warnings is True:
             print(msg, file=sys.stderr)
 
     def _wrap_error(self, err: Exception, *args: Any, **kwargs: Any) -> Exception:
-
         _wrap_message = f"Wrapped Exception {type(err).__name__} - {err}"
 
         # Catch memory errors first, these don't count as `wrap_errors=False`
         # as we need to catch memory errors that occur due to limits
         if self.memory and (
             isinstance(err, MemoryError)
             or (
@@ -295,17 +293,15 @@
                 return CpuTimeoutException(_wrap_message)
 
         if self.wall_time is not None and "wall_time" in mapping:
             if any(is_err(err, err_type) for err_type in mapping["wall_time"]):
                 return WallTimeoutException(_wrap_message)
 
         if self.memory is not None and "memory" in mapping:
-
             for t in mapping["memory"]:
-
                 # Windows specific errors
                 if isinstance(t, tuple) and len(t) == 3:
                     errT, errno, winerr = t
 
                     is_type = is_err(err, errT)
                     has_errno = getattr(err, "errno", None) == errno
                     has_winerr = getattr(err, "winerr", None) == winerr
```

### Comparing `pynisher-1.0.5/pynisher/limiters/linux.py` & `pynisher-1.0.6/pynisher/limiters/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+"""Set limits for Linux.
+
 For documentation on `setrlimit` and how to limit resources for Linux
 ** `setrlimit` **
 https://man7.org/linux/man-pages/man2/setrlimit.2.html
 
 For documentation on Linux specific signal alarms:
 ** `signals` **
 https://man7.org/linux/man-pages/man7/signal.7.html
@@ -15,15 +16,15 @@
 import resource
 
 from pynisher.limiters.limiter import Limiter
 
 
 class LimiterLinux(Limiter):
     def limit_memory(self, memory: int) -> None:
-        """Limit the addressable memory
+        """Limit the addressable memory.
 
         This could technically raise `SIGSEGV` (segmentation fault) but
         we instead catch a python `MemoryError` as indication that memory
         time was exceeded. This lets us give back the traceback.
 
         Parameters
         ----------
```

### Comparing `pynisher-1.0.5/pynisher/limiters/mac.py` & `pynisher-1.0.6/pynisher/limiters/mac.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/limiters/windows.py` & `pynisher-1.0.6/pynisher/limiters/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         Returns
         -------
         WIN32JOB
             A Windows job which consists of one or more processes. In this case
             we just have the one process
         """
         if not hasattr(self, "_job"):
-
             # First try to import stuff, an easy exception to catch and give good
             # information about
             try:
                 import win32api
                 import win32job
                 import winerror
             except ModuleNotFoundError as e:
```

### Comparing `pynisher-1.0.5/pynisher/pynisher.py` & `pynisher-1.0.6/pynisher/pynisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import psutil
 from typing_extensions import Literal, ParamSpec
 
 from pynisher.exceptions import (
     CpuTimeoutException,
     MemoryLimitException,
-    TimeoutException,
     PynisherException,
+    TimeoutException,
     WallTimeoutException,
 )
 from pynisher.limiters import Limiter
 from pynisher.support import contexts as valid_contexts
 from pynisher.support import supports
 from pynisher.util import callstring, memconvert, terminate_process, timeconvert
 from pynisher.win_errcodes import WIN_CPUTIMEOUT_EXITCODES, WIN_MEMORY_EXITCODES
@@ -235,15 +235,15 @@
 
         if _wall_time is not None and not _wall_time >= 1:
             raise ValueError(f"`wall_time` {wall_time} must be >= 1 second")
 
         if _memory is not None and not _memory >= 1:
             raise ValueError(f"`memory` {memory} must be >= 1 Byte")
 
-        if context is not None and context not in valid_contexts:
+        if isinstance(context, str) and context not in valid_contexts:
             raise ValueError(f"`context` {context} must be in {valid_contexts}")
 
         if isinstance(wrap_errors, dict):
             valid_keys = {"memory", "wall_time", "cpu_time", "pynisher"}
             keys = list(wrap_errors.keys())
             if not all(key in valid_keys for key in keys):
                 raise ValueError(
@@ -253,15 +253,19 @@
 
         self.func = func
         self.name = name
         self.cpu_time = _cpu_time
         self.memory = _memory
         self.wall_time = _wall_time
         self.raises = raises
-        self.context = multiprocessing.get_context(context)
+        self.context = (
+            multiprocessing.get_context(context)
+            if isinstance(context, str) or context is None
+            else context
+        )
         self.warnings = warnings
         self.wrap_errors = wrap_errors
         self.terminate_child_processes = terminate_child_processes
         self.forceful_keyboard_interrupt = forceful_keyboard_interrupt
 
         # Set once the function is running
         self._process: psutil.Process | None = None
@@ -334,15 +338,15 @@
             warnings=self.warnings,
             wrap_errors=self.wrap_errors,
             terminate_child_processes=self.terminate_child_processes,
         )
 
         # We now create the subprocess and let it know that it should call the limiter's
         # __call__ with the args and kwargs for the function being limited
-        subprocess = self.context.Process(
+        subprocess = self.context.Process(  # type: ignore
             target=limiter.__call__,
             args=args,  # type: ignore
             kwargs=kwargs,  # type: ignore
             daemon=False,
             name=self.name,
         )
 
@@ -432,15 +436,14 @@
 
         # Cleanup pipes
         receive_pipe.close()
         send_pipe.close()
 
         # We got a result or an error
         if result is not EMPTY or err is not None:
-
             # If an error, the result must be empty
             if err is not None:
                 result = EMPTY
 
             return self._handle_return(result=result, err=err, tb=tb)
 
         # Process ended gracefully but no result?
```

### Comparing `pynisher-1.0.5/pynisher/support.py` & `pynisher-1.0.6/pynisher/support.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/util.py` & `pynisher-1.0.6/pynisher/util.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher/win_errcodes.py` & `pynisher-1.0.6/pynisher/win_errcodes.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/pynisher.egg-info/PKG-INFO` & `pynisher-1.0.6/pynisher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.5
+Version: 1.0.6
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pynisher-1.0.5/pyproject.toml` & `pynisher-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.5/setup.py` & `pynisher-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = Path(__file__).parent / "README.md"
 
 with readme.open("r") as fh:
     long_description = fh.read()
 
 setup(
     name="pynisher",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(where=".", include=["pynisher*"], exclude=["test*"]),
     include_package_data=True,
     install_requires=[
         "psutil",
         "typing_extensions",
         "pywin32; platform_system=='Windows'",
     ],
```

