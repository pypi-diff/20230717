# Comparing `tmp/yet-another-runner-0.5.0.tar.gz` & `tmp/yet-another-runner-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yet-another-runner-0.5.0.tar", last modified: Fri Oct 26 08:22:57 2018, max compression
+gzip compressed data, was "yet-another-runner-0.6.0.tar", last modified: Sun Jul 16 23:51:05 2023, max compression
```

## Comparing `yet-another-runner-0.5.0.tar` & `yet-another-runner-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)       38 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/setup.cfg
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)      880 2018-10-26 08:18:49.000000 yet-another-runner-0.5.0/setup.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     4657 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/PKG-INFO
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3396 2018-10-14 19:01:10.000000 yet-another-runner-0.5.0/README.md
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/runner/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     2967 2018-10-25 22:35:45.000000 yet-another-runner-0.5.0/runner/proc.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)       51 2018-09-07 23:20:28.000000 yet-another-runner-0.5.0/runner/__init__.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     1582 2018-10-25 22:32:11.000000 yet-another-runner-0.5.0/runner/runner.py
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)        7 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/top_level.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)       45 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/requires.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)        1 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/dependency_links.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)      278 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/SOURCES.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     4657 2018-10-26 08:22:57.000000 yet-another-runner-0.5.0/yet_another_runner.egg-info/PKG-INFO
+drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2023-07-16 23:51:05.352305 yet-another-runner-0.6.0/
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     1071 2018-07-29 19:56:58.000000 yet-another-runner-0.6.0/LICENSE
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3985 2023-07-16 23:51:05.351305 yet-another-runner-0.6.0/PKG-INFO
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3403 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/README.md
+drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2023-07-16 23:51:05.351305 yet-another-runner-0.6.0/runner/
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)       99 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/runner/__init__.py
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3256 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/runner/proc.py
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     1883 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/runner/runner.py
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)       38 2023-07-16 23:51:05.352305 yet-another-runner-0.6.0/setup.cfg
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)      873 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/setup.py
+drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2023-07-16 23:51:05.351305 yet-another-runner-0.6.0/tests/
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     1590 2018-10-14 18:45:58.000000 yet-another-runner-0.6.0/tests/test_lines.py
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)    10362 2023-07-16 23:48:34.000000 yet-another-runner-0.6.0/tests/test_runner.py
+drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2023-07-16 23:51:05.351305 yet-another-runner-0.6.0/yet_another_runner.egg-info/
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3985 2023-07-16 23:51:05.000000 yet-another-runner-0.6.0/yet_another_runner.egg-info/PKG-INFO
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)      327 2023-07-16 23:51:05.000000 yet-another-runner-0.6.0/yet_another_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)        1 2023-07-16 23:51:05.000000 yet-another-runner-0.6.0/yet_another_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)       39 2023-07-16 23:51:05.000000 yet-another-runner-0.6.0/yet_another_runner.egg-info/requires.txt
+-rw-r--r--   0 aragaer   (1000) aragaer   (1000)        7 2023-07-16 23:51:05.000000 yet-another-runner-0.6.0/yet_another_runner.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yet-another-runner-0.5.0/setup.py` & `yet-another-runner-0.6.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="yet-another-runner",
-    version="0.5.0",
+    version="0.6.0",
     author="Ilya Konovalov",
     author_email="aragaer@gmail.com",
     description="Simple process runner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="run command shell socket",
     url="https://github.com/aragaer/runner",
     packages=["runner"],
-    install_requires=["attrs", "yet-another-io-channels-library>=0.2.0"],
+    install_requires=["yet-another-io-channels-library>=0.2.0"],
     classifiers=[
         "Topic :: Utilities",
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ]
 )
```

### Comparing `yet-another-runner-0.5.0/PKG-INFO` & `yet-another-runner-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,108 @@
 Metadata-Version: 2.1
 Name: yet-another-runner
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple process runner
 Home-page: https://github.com/aragaer/runner
 Author: Ilya Konovalov
 Author-email: aragaer@gmail.com
 License: MIT
-Description: # Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![BCH compliance](https://bettercodehub.com/edge/badge/aragaer/runner?branch=master)](https://bettercodehub.com/results/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
-        
-        Simple wrapper around subprocess.Popen.
-        
-        Multiple commands can be configured to be executed. Each command can
-        have some predetermined parameters and additional parameters or
-        overrides can be passed when application is executed. Multiple
-        instances of one application can be running using aliases.
-        
-        To communicate to running processes Channel classes from
-        [yet-another-io-channels-library](https://github.com/aragaer/channels)
-        are used.
-        
-        Examples:
-        
-        Using STDIO.
-        
-            runner = Runner()
-            runner.add("cat", "cat")
-            runner.start('cat')
-            channel = runner.get_channel('cat')
-            channel.write(b'hello, world')
-        	# later
-        	line = channel.read() # Will return b'hello, world'
-        
-        Using UNIX socket.
-        
-            runner = Runner()
-            self._runner.add("socat", "socat SYSTEM:cat UNIX-LISTEN:socket",
-        	                 type="socket", socket="socket")
-            runner.start('socat')
-            channel = runner.get_channel('socat')
-            channel.write(b'hello, world')
-        	# later
-        	line = channel.read() # Will return b'hello, world'
-        
-        ## Classes
-        
-        ### Runner
-        
-        `add(self, name, command, **kwargs)`
-        
-        Add the application to the list of registered applications or update
-        if already added.
-        
-        - `name`: application name
-        - `command`: the command to be executed
-        
-        `**kwargs` can include the following:
-        
-        - `type`: either `stdio` or `socket`. Default is `stdio`
-        - `cwd`: working directory of the process
-        - `socket`: if type is `socket`, this is the name of the UNIX socket file to connect to
-        - `setpgrp`: if `True` the process is moved to a separate process group and will not receive signals sent to main process. Default is `False`
-        - `buffering`: if set to `"line"` the channel is line-buffered for reading
-        
-        `update_config(self, config)`
-        
-        Config must be a dictionary where each key is an alias of an
-        application and value is a dictionary of that application's
-        configuration. `runner.add("app", "command", **kwargs)` is equivalent
-        to `runner.update_config({"app": {"command": "command",
-        **kwargs}})`. Useful for adding multiple applications at once.
-        
-        `ensure_running(self, app_name, alias=None, with_args=None, **kwargs)`
-        
-        `start(self, app_name, alias=None, with_args=None, **kwargs)`
-        
-        Start the process. If the process with the same alias is already
-        running, `start` will raise `ProcessExistsException`, while
-        `ensure_running` will silently do nothing.
-        
-        - `app_name`: application alias, given in the configuration
-        - `alias`: alias that will be given to actual started process. If `None`, application alias will be used
-        - `with_args`: list of additional arguments that will be added to the command
-        - `kwargs`: extend or override parameters in application config
-        
-        `get_channel(self, alias)`
-        
-        Returns the `Channel` object to communicate to the running process.
-        
-        `terminate(self, alias)`
-        
-        Terminates the process.
-        
 Keywords: run command shell socket
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
+
+Simple wrapper around subprocess.Popen.
+
+Multiple commands can be configured to be executed. Each command can
+have some predetermined parameters and additional parameters or
+overrides can be passed when application is executed. Multiple
+instances of one application can be running using aliases.
+
+To communicate to running processes Channel classes from
+[yet-another-io-channels-library](https://github.com/aragaer/channels)
+are used.
+
+Examples:
+
+Using STDIO.
+
+    runner = Runner()
+    runner.add("cat", "cat")
+    runner.start('cat')
+    channel = runner.get_channel('cat')
+    channel.write(b'hello, world')
+	# later
+	line = channel.read() # Will return b'hello, world'
+
+Using UNIX socket.
+
+    runner = Runner()
+    self._runner.add("socat", "socat SYSTEM:cat UNIX-LISTEN:socket",
+	                 type="socket", socket="socket")
+    runner.start('socat')
+    channel = runner.get_channel('socat')
+    channel.write(b'hello, world')
+	# later
+	line = channel.read() # Will return b'hello, world'
+
+## Classes
+
+### Runner
+
+`Runner(*, extra_paths=None)`
+
+Create a new runner object.
+
+- `extra_paths`: List of paths which will be appended to PATH environment variable
+
+`add(self, name, command, **kwargs)`
+
+Add the application to the list of registered applications or update
+if already added.
+
+- `name`: application name
+- `command`: the command to be executed
+
+`**kwargs` can include the following:
+
+- `type`: either `stdio` or `socket`. Default is `stdio`
+- `cwd`: working directory of the process
+- `socket`: if type is `socket`, this is the name of the UNIX socket file to connect to
+- `setpgrp`: if `True` the process is moved to a separate process group and will not receive signals sent to main process. Default is `False`
+- `buffering`: if set to `"line"` the channel is line-buffered for reading
+
+`update_config(self, config)`
+
+Config must be a dictionary where each key is an alias of an
+application and value is a dictionary of that application's
+configuration. `runner.add("app", "command", **kwargs)` is equivalent
+to `runner.update_config({"app": {"command": "command",
+**kwargs}})`. Useful for adding multiple applications at once.
+
+`ensure_running(self, app_name, alias=None, with_args=None, **kwargs)`
+
+`start(self, app_name, alias=None, with_args=None, **kwargs)`
+
+Start the process. If the process with the same alias is already
+running, `start` will raise `ProcessExistsException`, while
+`ensure_running` will silently do nothing.
+
+- `app_name`: application alias, given in the configuration
+- `alias`: alias that will be given to actual started process. If `None`, application alias will be used
+- `with_args`: list of additional arguments that will be added to the command
+- `kwargs`: extend or override parameters in application config
+
+`get_channel(self, alias)`
+
+Returns the `Channel` object to communicate to the running process.
+
+`terminate(self, alias)`
+
+Terminates the process.
```

### Comparing `yet-another-runner-0.5.0/README.md` & `yet-another-runner-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![BCH compliance](https://bettercodehub.com/edge/badge/aragaer/runner?branch=master)](https://bettercodehub.com/results/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
+# Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
 
 Simple wrapper around subprocess.Popen.
 
 Multiple commands can be configured to be executed. Each command can
 have some predetermined parameters and additional parameters or
 overrides can be passed when application is executed. Multiple
 instances of one application can be running using aliases.
@@ -34,14 +34,20 @@
 	# later
 	line = channel.read() # Will return b'hello, world'
 
 ## Classes
 
 ### Runner
 
+`Runner(*, extra_paths=None)`
+
+Create a new runner object.
+
+- `extra_paths`: List of paths which will be appended to PATH environment variable
+
 `add(self, name, command, **kwargs)`
 
 Add the application to the list of registered applications or update
 if already added.
 
 - `name`: application name
 - `command`: the command to be executed
```

### Comparing `yet-another-runner-0.5.0/runner/proc.py` & `yet-another-runner-0.6.0/runner/proc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 import logging
 import os
 import shlex
 import socket
 import subprocess
 import time
 
-from abc import ABCMeta, abstractmethod
+from abc import abstractmethod
+from dataclasses import dataclass
+from typing import Callable, Optional
 
-import attr
 import channels
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class _Proc:
-    proc = attr.ib()
-    channel = attr.ib()
+    proc: subprocess.Popen
+    channel: channels.Channel
 
     def terminate(self):
         self.channel.close()
         self.proc.terminate()
         self.proc.wait()
 
 
-@attr.s
-class _ProcStarter(metaclass=ABCMeta):
-    command = attr.ib()
-    buffering = attr.ib()
-    cwd = attr.ib()
-    preexec_fn = attr.ib(init=False, default=None)
-    proc = attr.ib(init=False)
-    stdin = attr.ib(init=False)
-    stdout = attr.ib(init=False)
+@dataclass
+class _ProcStarter:
+    command: [str]
+    buffering: str = ""
+    cwd: str = None
+    preexec_fn: Optional[Callable] = None
+    proc: _Proc = None
+    stdin = None
+    stdout = None
 
     @abstractmethod
-    def pre_start(self): #pragma: no cover
+    def pre_start(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def get_channel(self): #pragma: no cover
+    def get_channel(self):  # pragma: no cover
         pass
 
-    def start(self):
+    def start(self, paths=None):
         self.pre_start()
+        if paths is None:
+            env = os.environ
+        else:
+            env = {k: v for k, v in os.environ.items()}
+            env["PATH"] = ':'.join(paths)
+            _LOGGER.debug("PATH set to %s", env["PATH"])
         self.proc = subprocess.Popen(self.command,
                                      stdin=self.stdin,
                                      stdout=self.stdout,
                                      preexec_fn=self.preexec_fn,
-                                     cwd=self.cwd)
+                                     cwd=self.cwd,
+                                     env=env)
 
         return _Proc(self.proc, self.get_channel())
 
 
-@attr.s
+@dataclass
 class _PipeProcStarter(_ProcStarter):
 
-    def __attrs_post_init__(self):
+    def __post_init__(self):
         self.stdin = self.stdout = subprocess.PIPE
 
     def get_channel(self):
         return channels.PipeChannel(sink=self.proc.stdin.fileno(),
                                     faucet=self.proc.stdout.fileno(),
                                     buffering=self.buffering)
 
     def pre_start(self):
         pass
 
 
-@attr.s
+@dataclass
 class _SocketProcStarter(_ProcStarter):
-    sockname = attr.ib(init=False)
+    sockname: str = ""
 
-    def __attrs_post_init__(self):
+    def __post_init__(self):
         self.stdin = self.stdout = None
 
     def get_channel(self):
         sock = socket.socket(socket.AF_UNIX)
         _LOGGER.debug("Waiting for socket %s", self.sockname)
         while not os.path.exists(self.sockname):
             time.sleep(0.01)
@@ -105,8 +113,8 @@
         ps = self._ps_class(self._command + list(extra_args),
                             cwd=kwargs.get('cwd'),
                             buffering=kwargs.get('buffering'))
         if kwargs.get('setpgrp', False):
             ps.preexec_fn = os.setpgrp
         if self._ps_class == _SocketProcStarter:
             ps.sockname = kwargs['socket']
-        return ps.start()
+        return ps.start(paths=kwargs.get('paths'))
```

### Comparing `yet-another-runner-0.5.0/runner/runner.py` & `yet-another-runner-0.6.0/runner/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import logging
 
+from os import environ
+
 from .proc import App
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ProcessExistsException(Exception):
     pass
 
 
 class Runner:
 
-    def __init__(self):
+    def __init__(self, *, extra_paths=None):
         self._apps = {}
         self._procs = {}
+        self._paths = environ.get("PATH", "").split(':')
+        if extra_paths is not None:
+            self._paths.extend(extra_paths)
 
     def add(self, app, command, **kwargs):
         self.update_config({app: dict(command=command, **kwargs)})
 
     def update_config(self, config):
         for app, app_config in config.items():
             _LOGGER.debug("Updating config for %s", app)
             self._apps[app] = App(**app_config)
 
     def ensure_running(self, app_name, alias=None, with_args=None, **kwargs):
         if alias is None:
             alias = app_name
         if alias in self._procs:
-            _LOGGER.info("Application alias %s is already taken, not starting %s",
+            _LOGGER.info("Alias %s is already taken, not starting %s",
                          alias, app_name)
             return
         if with_args is None:
             with_args = []
         _LOGGER.info("Starting application %s as %s", app_name, alias)
-        self._procs[alias] = self._apps[app_name].start(*with_args, **kwargs)
+        self._procs[alias] = self._apps[app_name].start(*with_args,
+                                                        paths=self._paths,
+                                                        **kwargs)
         _LOGGER.debug("%s started", alias)
 
     def start(self, app_name, alias=None, with_args=None, **kwargs):
         if alias is None:
             alias = app_name
         if alias in self._procs:
             raise ProcessExistsException
```

### Comparing `yet-another-runner-0.5.0/yet_another_runner.egg-info/PKG-INFO` & `yet-another-runner-0.6.0/yet_another_runner.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,108 @@
 Metadata-Version: 2.1
 Name: yet-another-runner
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple process runner
 Home-page: https://github.com/aragaer/runner
 Author: Ilya Konovalov
 Author-email: aragaer@gmail.com
 License: MIT
-Description: # Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![BCH compliance](https://bettercodehub.com/edge/badge/aragaer/runner?branch=master)](https://bettercodehub.com/results/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
-        
-        Simple wrapper around subprocess.Popen.
-        
-        Multiple commands can be configured to be executed. Each command can
-        have some predetermined parameters and additional parameters or
-        overrides can be passed when application is executed. Multiple
-        instances of one application can be running using aliases.
-        
-        To communicate to running processes Channel classes from
-        [yet-another-io-channels-library](https://github.com/aragaer/channels)
-        are used.
-        
-        Examples:
-        
-        Using STDIO.
-        
-            runner = Runner()
-            runner.add("cat", "cat")
-            runner.start('cat')
-            channel = runner.get_channel('cat')
-            channel.write(b'hello, world')
-        	# later
-        	line = channel.read() # Will return b'hello, world'
-        
-        Using UNIX socket.
-        
-            runner = Runner()
-            self._runner.add("socat", "socat SYSTEM:cat UNIX-LISTEN:socket",
-        	                 type="socket", socket="socket")
-            runner.start('socat')
-            channel = runner.get_channel('socat')
-            channel.write(b'hello, world')
-        	# later
-        	line = channel.read() # Will return b'hello, world'
-        
-        ## Classes
-        
-        ### Runner
-        
-        `add(self, name, command, **kwargs)`
-        
-        Add the application to the list of registered applications or update
-        if already added.
-        
-        - `name`: application name
-        - `command`: the command to be executed
-        
-        `**kwargs` can include the following:
-        
-        - `type`: either `stdio` or `socket`. Default is `stdio`
-        - `cwd`: working directory of the process
-        - `socket`: if type is `socket`, this is the name of the UNIX socket file to connect to
-        - `setpgrp`: if `True` the process is moved to a separate process group and will not receive signals sent to main process. Default is `False`
-        - `buffering`: if set to `"line"` the channel is line-buffered for reading
-        
-        `update_config(self, config)`
-        
-        Config must be a dictionary where each key is an alias of an
-        application and value is a dictionary of that application's
-        configuration. `runner.add("app", "command", **kwargs)` is equivalent
-        to `runner.update_config({"app": {"command": "command",
-        **kwargs}})`. Useful for adding multiple applications at once.
-        
-        `ensure_running(self, app_name, alias=None, with_args=None, **kwargs)`
-        
-        `start(self, app_name, alias=None, with_args=None, **kwargs)`
-        
-        Start the process. If the process with the same alias is already
-        running, `start` will raise `ProcessExistsException`, while
-        `ensure_running` will silently do nothing.
-        
-        - `app_name`: application alias, given in the configuration
-        - `alias`: alias that will be given to actual started process. If `None`, application alias will be used
-        - `with_args`: list of additional arguments that will be added to the command
-        - `kwargs`: extend or override parameters in application config
-        
-        `get_channel(self, alias)`
-        
-        Returns the `Channel` object to communicate to the running process.
-        
-        `terminate(self, alias)`
-        
-        Terminates the process.
-        
 Keywords: run command shell socket
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Runner [![Build Status](https://travis-ci.org/aragaer/runner.svg?branch=master)](https://travis-ci.org/aragaer/runner) [![codecov](https://codecov.io/gh/aragaer/runner/branch/master/graph/badge.svg)](https://codecov.io/gh/aragaer/runner) [![donate using paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=aragaer@gmail.com&lc=RU&item_name=RUNNER&currency_code=USD&bn=PP-DonationsBF:btn_donate_SM.gif:NonHosted)
+
+Simple wrapper around subprocess.Popen.
+
+Multiple commands can be configured to be executed. Each command can
+have some predetermined parameters and additional parameters or
+overrides can be passed when application is executed. Multiple
+instances of one application can be running using aliases.
+
+To communicate to running processes Channel classes from
+[yet-another-io-channels-library](https://github.com/aragaer/channels)
+are used.
+
+Examples:
+
+Using STDIO.
+
+    runner = Runner()
+    runner.add("cat", "cat")
+    runner.start('cat')
+    channel = runner.get_channel('cat')
+    channel.write(b'hello, world')
+	# later
+	line = channel.read() # Will return b'hello, world'
+
+Using UNIX socket.
+
+    runner = Runner()
+    self._runner.add("socat", "socat SYSTEM:cat UNIX-LISTEN:socket",
+	                 type="socket", socket="socket")
+    runner.start('socat')
+    channel = runner.get_channel('socat')
+    channel.write(b'hello, world')
+	# later
+	line = channel.read() # Will return b'hello, world'
+
+## Classes
+
+### Runner
+
+`Runner(*, extra_paths=None)`
+
+Create a new runner object.
+
+- `extra_paths`: List of paths which will be appended to PATH environment variable
+
+`add(self, name, command, **kwargs)`
+
+Add the application to the list of registered applications or update
+if already added.
+
+- `name`: application name
+- `command`: the command to be executed
+
+`**kwargs` can include the following:
+
+- `type`: either `stdio` or `socket`. Default is `stdio`
+- `cwd`: working directory of the process
+- `socket`: if type is `socket`, this is the name of the UNIX socket file to connect to
+- `setpgrp`: if `True` the process is moved to a separate process group and will not receive signals sent to main process. Default is `False`
+- `buffering`: if set to `"line"` the channel is line-buffered for reading
+
+`update_config(self, config)`
+
+Config must be a dictionary where each key is an alias of an
+application and value is a dictionary of that application's
+configuration. `runner.add("app", "command", **kwargs)` is equivalent
+to `runner.update_config({"app": {"command": "command",
+**kwargs}})`. Useful for adding multiple applications at once.
+
+`ensure_running(self, app_name, alias=None, with_args=None, **kwargs)`
+
+`start(self, app_name, alias=None, with_args=None, **kwargs)`
+
+Start the process. If the process with the same alias is already
+running, `start` will raise `ProcessExistsException`, while
+`ensure_running` will silently do nothing.
+
+- `app_name`: application alias, given in the configuration
+- `alias`: alias that will be given to actual started process. If `None`, application alias will be used
+- `with_args`: list of additional arguments that will be added to the command
+- `kwargs`: extend or override parameters in application config
+
+`get_channel(self, alias)`
+
+Returns the `Channel` object to communicate to the running process.
+
+`terminate(self, alias)`
+
+Terminates the process.
```

