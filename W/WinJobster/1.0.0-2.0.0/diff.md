# Comparing `tmp/WinJobster-1.0.0.tar.gz` & `tmp/WinJobster-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinJobster-1.0.0.tar", last modified: Sat Jul 15 22:44:35 2023, max compression
+gzip compressed data, was "WinJobster-2.0.0.tar", last modified: Sun Jul 16 21:21:54 2023, max compression
```

## Comparing `WinJobster-1.0.0.tar` & `WinJobster-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:35.854077 WinJobster-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 22:44:22.000000 WinJobster-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 22:44:35.854077 WinJobster-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-15 22:44:22.000000 WinJobster-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-15 22:44:22.000000 WinJobster-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:22.000000 WinJobster-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:44:35.854077 WinJobster-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:35.854077 WinJobster-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:35.854077 WinJobster-1.0.0/src/WinJobster/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/WinJobster/Process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/WinJobster/WinJobsterCallFailedException.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/WinJobster/WinJobsterLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/WinJobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/WinJobster/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:35.854077 WinJobster-1.0.0/src/WinJobster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 22:44:35.000000 WinJobster-1.0.0/src/WinJobster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-15 22:44:35.000000 WinJobster-1.0.0/src/WinJobster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:44:35.000000 WinJobster-1.0.0/src/WinJobster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 22:44:35.000000 WinJobster-1.0.0/src/WinJobster.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:44:35.854077 WinJobster-1.0.0/src/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-15 22:44:28.000000 WinJobster-1.0.0/src/libs/WinJobster-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-07-15 22:44:28.000000 WinJobster-1.0.0/src/libs/WinJobster-x86.dll
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-15 22:44:22.000000 WinJobster-1.0.0/src/libs/get_dlls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:54.764735 WinJobster-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 21:21:38.000000 WinJobster-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-16 21:21:54.764735 WinJobster-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-16 21:21:38.000000 WinJobster-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-16 21:21:38.000000 WinJobster-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:38.000000 WinJobster-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 21:21:54.764735 WinJobster-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:54.760735 WinJobster-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:54.760735 WinJobster-2.0.0/src/WinJobster/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/WinJobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/WinJobster/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/WinJobster/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/WinJobster/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/WinJobster/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:54.764735 WinJobster-2.0.0/src/WinJobster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-16 21:21:54.000000 WinJobster-2.0.0/src/WinJobster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-16 21:21:54.000000 WinJobster-2.0.0/src/WinJobster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:21:54.000000 WinJobster-2.0.0/src/WinJobster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 21:21:54.000000 WinJobster-2.0.0/src/WinJobster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:21:54.764735 WinJobster-2.0.0/src/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-07-16 21:21:47.000000 WinJobster-2.0.0/src/libs/WinJobster-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    19968 2023-07-16 21:21:47.000000 WinJobster-2.0.0/src/libs/WinJobster-x86.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-16 21:21:38.000000 WinJobster-2.0.0/src/libs/get_dlls.py
```

### Comparing `WinJobster-1.0.0/LICENSE.md` & `WinJobster-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `WinJobster-1.0.0/PKG-INFO` & `WinJobster-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: WinJobster
-Version: 1.0.0
+Version: 2.0.0
 Summary: WinJobster is a library, which can start processes in a Windows job, monitor their state (dead or alive) and kill them all at once, including their children, children of their children... you know where I'm going...
 Author: MaxBQb, SemperSolus0x3d
 License: GPL-3.0 license
+Project-URL: Homepage, https://github.com/SemperSolus0x3d/WinJobster.py
+Project-URL: Bug Tracker, https://github.com/SemperSolus0x3d/WinJobster.py/issues
 Keywords: windows,windows-jobs,winapi,process,process-groups
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,23 +32,21 @@
 
 ## Installation
 ```cmd
 pip install WinJobster
 ```
 
 ## Usage
+
 ```py
 import WinJobster
 
-
 cmdline = "notepad.exe"  # Path to any app, which can also start other app
-process = WinJobster.Process()
-process.start(cmdline)
-print(process.is_alive)  # True
-process.kill()  # Will close original app and everything which was started by it
+job = WinJobster.Job()
+print(job.is_alive)  # False, no alive processes found
+job.start_process(cmdline)
+print(job.is_alive)  # True, 1 alive process found
+job.terminate()  # Will close original app and everything which was started by it
 ```
 
-> By default, script root dir will be used as working directory for any started app,
-> to avoid this use `start_in_base_dir` method or set working directory explicitly in `start`
-
-> `process.start`'s first argument can be path, 
-> or any string interpreted as console input (Windows will expand path for you) 
+> `job.start_process`' first argument can be path, 
+> or any string interpreted as console input (Windows will expand %PATH% values for you)
```

### Comparing `WinJobster-1.0.0/README.md` & `WinJobster-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 
 ## Installation
 ```cmd
 pip install WinJobster
 ```
 
 ## Usage
+
 ```py
 import WinJobster
 
-
 cmdline = "notepad.exe"  # Path to any app, which can also start other app
-process = WinJobster.Process()
-process.start(cmdline)
-print(process.is_alive)  # True
-process.kill()  # Will close original app and everything which was started by it
+job = WinJobster.Job()
+print(job.is_alive)  # False, no alive processes found
+job.start_process(cmdline)
+print(job.is_alive)  # True, 1 alive process found
+job.terminate()  # Will close original app and everything which was started by it
 ```
 
-> By default, script root dir will be used as working directory for any started app,
-> to avoid this use `start_in_base_dir` method or set working directory explicitly in `start`
-
-> `process.start`'s first argument can be path, 
-> or any string interpreted as console input (Windows will expand path for you) 
+> `job.start_process`' first argument can be path, 
+> or any string interpreted as console input (Windows will expand %PATH% values for you)
```

### Comparing `WinJobster-1.0.0/pyproject.toml` & `WinJobster-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,12 +23,15 @@
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: Microsoft :: Windows",
 ]
+[project.urls]
+"Homepage" = "https://github.com/SemperSolus0x3d/WinJobster.py"
+"Bug Tracker" = "https://github.com/SemperSolus0x3d/WinJobster.py/issues"
 [tool.setuptools.package-data]
 "*" = ["*.dll"]
 [tool.setuptools.dynamic]
 version = {attr = "WinJobster._meta.__version__"}
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `WinJobster-1.0.0/src/WinJobster/Process.py` & `WinJobster-2.0.0/src/WinJobster/job.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,96 @@
 import ctypes as c
-import functools
+import shutil
 import typing
 from pathlib import Path
+from typing import Optional, Union
 
-from .WinJobsterLoader import WinJobsterLoader
+from .loader import LibLoader
 
 
-_F = typing.TypeVar('_F', bound=typing.Callable[..., typing.Any])
-
-
-def _cleanup_on_fail(func: _F) -> _F:
-
-    @functools.wraps(func)
-    def wrapper(self, *args, **kwargs):
-        try:
-            return func(self, *args, **kwargs)
-        except:
-            self._cleanup()
-            raise
+class Job:
+    _library = None
 
-    return wrapper
+    class AppLocal:
+        pass
 
-
-class Process:
-    _library = None
+    APP_LOCAL = AppLocal()
 
     @classmethod
     def _init(cls):
         if cls._library is None:
-            cls._library = WinJobsterLoader().load()
+            cls._library = LibLoader().load()
 
     def __init__(self):
-        self._handle = None
         self._init()
+        self._handle = self._library.CreateJob()
+
+    def start_process(
+        self,
+        path: Union[str, Path],
+        call_params: str = "",
+        working_directory: Union[str, Path, AppLocal, None] = APP_LOCAL,
+    ):
+        if isinstance(working_directory, Job.AppLocal):
+            resolved_path = shutil.which(str(path))
+            if resolved_path is None:
+                resolved_path = path
+            working_directory = Path(resolved_path).parent
+
+        cmdline = str(path)
+        if call_params:
+            cmdline += " " + call_params
 
-    def start_in_base_dir(self, cmdline: typing.Union[str, Path]):
-        cmdline = Path(cmdline)
-        self.start(cmdline, cmdline.parent)
-
-    @_cleanup_on_fail
-    def start(self, cmdline: typing.Union[str, Path], working_directory: typing.Union[str, Path, None] = None):
-        cmdline = str(cmdline)
         if working_directory is not None:
             working_directory = str(working_directory)
-        self._handle = c.c_void_p(None)
+
+        self._start_process(cmdline, working_directory)
+
+    def _start_process(self, cmdline: str, working_directory: Optional[str] = None):
         self._library.StartProcess(
             cmdline,
             working_directory,
-            c.byref(self._handle))
+            self._handle,
+        )
 
     @property
-    @_cleanup_on_fail
     def is_alive(self) -> bool:
         if self._handle is None:
             return False
 
         return self._library.IsAlive(self._handle)
 
-    @_cleanup_on_fail
-    def kill(self):
+    def terminate(self, gracefully=True):
         if self._handle is None:
             return
 
-        self._library.Kill(self._handle)
+        if gracefully:
+            self._library.Terminate(self._handle)
+        else:
+            self._library.Kill(self._handle)
+
+        # TODO: This part should be moved to CPP library
+        self._cleanup()
+        self._handle = self._library.CreateJob()
+
+    @property
+    def process_ids(self) -> typing.Set[int]:
+        if self._handle is None:
+            return set()
+
+        ids = c.POINTER(c.c_uint64)()
+        size = c.c_size_t()
+
+        self._library.GetProcessIds(self._handle, c.byref(ids), c.byref(size))
+
+        result = {int(ids[i]) for i in range(size.value)}
+
+        self._library.FreeMemory(ids)
+        return result
 
     def _cleanup(self):
         if self._handle is not None:
-            self._library.Cleanup(self._handle)
+            self._library.DestroyJob(self._handle)
             self._handle = None
 
     def __del__(self):
         self._cleanup()
```

### Comparing `WinJobster-1.0.0/src/WinJobster/WinJobsterCallFailedException.py` & `WinJobster-2.0.0/src/WinJobster/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 class ErrorCode(IntEnum):
     Success = 0
     JobObjectCreationFailed = 1
     CompletionPortCreationFailed = 2
     FailedToAssociateJobWithCompletionPort = 3
     ProcessCreationFailed = 4
+    QueryJobObjectInformationFailed = 5
 
     @classmethod
     def of(cls, code: int):
         if code not in tuple(cls):
             return None
         return ErrorCode(code)
 
     @property
     def message(self):
         if self == ErrorCode.Success:
             return None
         return self.name
 
 
-class WinJobsterCallFailedException(Exception):
+class CallFailedException(Exception):
     ERROR_CODES = tuple(ErrorCode)
 
     def __init__(self, error_code):
         self.error_code_value = error_code
         self.error_code = ErrorCode.of(error_code)
         self.message = self.get_error_message()
         super().__init__(self.message, self.error_code, self.error_code_value)
```

### Comparing `WinJobster-1.0.0/src/WinJobster.egg-info/PKG-INFO` & `WinJobster-2.0.0/src/WinJobster.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: WinJobster
-Version: 1.0.0
+Version: 2.0.0
 Summary: WinJobster is a library, which can start processes in a Windows job, monitor their state (dead or alive) and kill them all at once, including their children, children of their children... you know where I'm going...
 Author: MaxBQb, SemperSolus0x3d
 License: GPL-3.0 license
+Project-URL: Homepage, https://github.com/SemperSolus0x3d/WinJobster.py
+Project-URL: Bug Tracker, https://github.com/SemperSolus0x3d/WinJobster.py/issues
 Keywords: windows,windows-jobs,winapi,process,process-groups
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,23 +32,21 @@
 
 ## Installation
 ```cmd
 pip install WinJobster
 ```
 
 ## Usage
+
 ```py
 import WinJobster
 
-
 cmdline = "notepad.exe"  # Path to any app, which can also start other app
-process = WinJobster.Process()
-process.start(cmdline)
-print(process.is_alive)  # True
-process.kill()  # Will close original app and everything which was started by it
+job = WinJobster.Job()
+print(job.is_alive)  # False, no alive processes found
+job.start_process(cmdline)
+print(job.is_alive)  # True, 1 alive process found
+job.terminate()  # Will close original app and everything which was started by it
 ```
 
-> By default, script root dir will be used as working directory for any started app,
-> to avoid this use `start_in_base_dir` method or set working directory explicitly in `start`
-
-> `process.start`'s first argument can be path, 
-> or any string interpreted as console input (Windows will expand path for you) 
+> `job.start_process`' first argument can be path, 
+> or any string interpreted as console input (Windows will expand %PATH% values for you)
```

### Comparing `WinJobster-1.0.0/src/libs/get_dlls.py` & `WinJobster-2.0.0/src/libs/get_dlls.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     logging.basicConfig(
         format="[%(asctime)s][%(levelname)s] %(message)s",
         datefmt='%H:%M:%S',
         level=logging.INFO
     )
     check_and_download_updates(
         GitHubRepo("SemperSolus0x3d", "WinJobster.cpp", os.environ.get("GITHUB_TOKEN")),
-        SimpleSpec("~1"),
+        SimpleSpec("~2"),
         assets_mask=re.compile(".*\\.dll"),
     )
 
 
 if __name__ == '__main__':
     main()
```

