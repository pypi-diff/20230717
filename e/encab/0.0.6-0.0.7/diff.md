# Comparing `tmp/encab-0.0.6.tar.gz` & `tmp/encab-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.6.tar", last modified: Thu Jul 13 17:57:16 2023, max compression
+gzip compressed data, was "encab-0.0.7.tar", last modified: Mon Jul 17 16:06:24 2023, max compression
```

## Comparing `encab-0.0.6.tar` & `encab-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.161249 encab-0.0.6/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.6/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-13 17:57:16.157248 encab-0.0.6/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4406 2023-07-13 17:45:41.000000 encab-0.0.6/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-13 17:41:31.000000 encab-0.0.6/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-13 17:57:16.161249 encab-0.0.6/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.149248 encab-0.0.6/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.153248 encab-0.0.6/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.6/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.6/src/encab/__main__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11029 2023-07-12 07:11:39.000000 encab-0.0.6/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-13 17:42:02.000000 encab-0.0.6/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.157248 encab-0.0.6/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.6/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.6/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.6/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.6/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.6/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.6/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-13 17:57:16.157248 encab-0.0.6/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-13 17:57:16.000000 encab-0.0.6/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.7/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-17 16:06:24.729121 encab-0.0.7/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4406 2023-07-17 15:56:26.000000 encab-0.0.7/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-17 15:56:18.000000 encab-0.0.7/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-17 16:06:24.729121 encab-0.0.7/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.717121 encab-0.0.7/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.725121 encab-0.0.7/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.7/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.7/src/encab/__main__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/src/encab/common/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1909 2023-07-16 12:17:22.000000 encab-0.0.7/src/encab/common/log_stream.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4069 2023-07-16 12:33:40.000000 encab-0.0.7/src/encab/common/process.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11826 2023-07-16 12:12:13.000000 encab-0.0.7/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8260 2023-07-17 15:56:44.000000 encab-0.0.7/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.7/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.7/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9609 2023-07-17 15:35:23.000000 encab-0.0.7/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.7/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.7/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5512 2023-07-17 15:17:13.000000 encab-0.0.7/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10183 2023-07-17 15:18:53.000000 encab-0.0.7/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3203 2023-07-16 12:24:46.000000 encab-0.0.7/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.725121 encab-0.0.7/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      585 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.6/LICENSE` & `encab-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.6/PKG-INFO` & `encab-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.6
+Version: 0.0.7
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Encab: A Simple Process Manager
 
 **Encab** is a process manager that simplifies running multiple services in a container or from the command line.
 
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.6
+INFO  encab: encab 0.0.7
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -175,15 +175,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.6/README.md` & `encab-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -89,15 +89,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.6
+INFO  encab: encab 0.0.7
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -160,15 +160,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.6/pyproject.toml` & `encab-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
 description = "Process manager"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "PyYAML >= 6.0, < 7",
```

### Comparing `encab-0.0.6/src/encab/config.py` & `encab-0.0.7/src/encab/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import io
 import os
 import shlex
 import yaml
 import marshmallow_dataclass
 
-from pwd import getpwnam
 from yaml.error import YAMLError
 from typing import Dict, Optional, Union, List, Any
 from dataclasses import dataclass, fields
 from marshmallow.exceptions import MarshmallowError, ValidationError
 from logging import DEBUG, INFO
 from abc import ABC
 
+from .common.process import getUserId, getGroupId
 
 class ConfigError(ValueError):
     """
     Configuration error
     """
 
     pass
@@ -64,14 +64,17 @@
 
     umask: Optional[Union[str, int]]
     """the umask, either as octal string (e.g. "077") or integer"""
 
     user: Optional[Union[str, int]]
     """the user id or user name"""
 
+    group: Optional[Union[str, int]]
+    """the group id or group name"""
+
     join_time: Optional[float]
     """ 
     The join time is the time in seconds encab waits for a program to start/shutdown before 
     it continues with the next. Default: 1 seconds
     """
 
     def _set_umask(self):
@@ -109,23 +112,44 @@
         user = self.user
 
         if user:
             if isinstance(user, int) or user.isnumeric():
                 self.user = int(user)
             else:
                 try:
-                    self.user = getpwnam(user).pw_uid
+                    self.user = getUserId(user)
                 except KeyError:
                     raise ConfigError(f"Unknown user {user}")
 
             if user != os.getuid() and os.getuid() != 0:
                 raise ConfigError(
                     "Encab has to run as root to run it or programs as different user"
                 )
 
+    def set_group(self):
+        """
+        sets the group that runs the program
+
+        steps:
+        - checks wether the group is set.
+        - determines the GID if the user is given as name.
+
+        :raises ConfigError: if the user is unknown or encab is not run as root when needed
+        """
+        group = self.group
+
+        if group:
+            if isinstance(group, int) or group.isnumeric():
+                self.group = int(group)
+            else:
+                try:
+                    self.group = getGroupId(group)
+                except KeyError:
+                    raise ConfigError(f"Unknown group {group}")
+
     def _set_log_level(self):
         """
         selts the log level and turns it into an int if necessary
 
         :raises ConfigError: if an unspecified log level is given
         """
         levels = ["CRITICAL", "FATAL", "ERROR", "WARN", "WARNING", "INFO", "DEBUG"]
@@ -263,23 +287,25 @@
     command: Union[str, List[str], None]
     """the command to be execution as list in POSIX style
         examples:
         
         .. code-block:: yaml
         
             program:
-                command:
-                    echo "Test"
+                main:
+                    command:
+                        echo "Test"
        
         .. code-block:: yaml
         
             program:
-                comand:     
-                    - echo 
-                    - Test
+                main:
+                    command:     
+                        - echo 
+                        - Test
     """
 
     sh: Union[str, List[str], None]
     """the shell script as string or list
     
         examples:
```

### Comparing `encab-0.0.6/src/encab/encab.py` & `encab-0.0.7/src/encab/encab.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 
 from signal import SIGTERM, SIGINT, signal, getsignal
 from typing import Optional, List, Tuple, Dict
 from textwrap import shorten
 from threading import Event
 
+from .common.process import Process
 from .config import Config, ConfigError
 from .program_state import LoggingProgramObserver
 from .program import ExecutionContext
 from .programs import Programs
 from .extensions import extensions, ENCAB
 
 from .ext.log_sanitizer import LogSanitizerExtension
@@ -183,15 +184,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.6", extra=extra)
+        logger.info("encab 0.0.7", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
@@ -205,20 +206,21 @@
         set_up_extensions(config, logger, extra)
 
         if dry_run:
             logger.info("Dry run succeeded. Exiting.", extra=extra)
             return
 
         config.encab.set_user()
+        config.encab.set_group()
 
-        if config.encab.user:
-            os.setuid(int(config.encab.user))
+        assert config.encab.user is None or isinstance(config.encab.user, int)
+        assert config.encab.group is None or isinstance(config.encab.group, int)
+        assert config.encab.umask is None or isinstance(config.encab.umask, int)
 
-        if config.encab.umask and config.encab.umask != -1:
-            os.umask(int(config.encab.umask))
+        Process.update_current(config.encab.user, config.encab.group, config.encab.umask)
 
         program_config = config.programs or {}
 
         if program_config:
             logger.debug("Starting program(s)...", extra=extra)
 
         observer = LoggingProgramObserver(ENCAB, logger, extra)
```

### Comparing `encab-0.0.6/src/encab/ext/log_sanitizer.py` & `encab-0.0.7/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.6/src/encab/ext/startup_script.py` & `encab-0.0.7/src/encab/ext/startup_script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import sys
 import re
 import yaml
 import marshmallow_dataclass
 
 from io import StringIO
-from typing import Dict, List, Any, Optional, Union, IO
-from logging import Logger, getLogger, INFO, ERROR
+from typing import Dict, List, Any, Optional, Union
+from logging import getLogger
 from pluggy import HookimplMarker  # type: ignore
 
 from dataclasses import dataclass
 from marshmallow.exceptions import MarshmallowError, ValidationError
 
 from dotenv import dotenv_values
-from threading import Thread
-from subprocess import Popen, PIPE
+from subprocess import Popen
+
+from encab.common.process import Process
 
 ENCAB = "encab"
 STARTUP_SCRIPT = "startup_script"
 
 mylogger = getLogger(STARTUP_SCRIPT)
 
 
@@ -104,65 +105,14 @@
                 msg = yaml.dump(msg, default_flow_style=False)
 
             raise ConfigError(f"\n\n{STARTUP_SCRIPT}:\n{msg}")
         except MarshmallowError as e:
             raise ConfigError(e.args)
 
 
-class LogStream(object):
-    """
-    Reads from a stream in a background thread and loggs the result line by line
-    """
-
-    def __init__(
-        self, logger: Logger, log_level: int, stream: IO[bytes], extra: Dict[str, str]
-    ) -> None:
-        """
-        :param Logger logger: the logger to which the stream content is written
-        :param int log_level: the log level (see Python logging)
-        :param IOBase stream: the stream that is logged
-        :param Dict[str, str] extra: extra information that is logged each line (see Python logging)
-        """
-        self.logger = logger
-        self.log_level = log_level
-        self.stream = stream
-        self.extra = extra
-        self.thread: Optional[Thread] = None
-
-    def _run(self):
-        try:
-            for line in self.stream:
-                strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
-                self.logger.log(self.log_level, strline, extra=self.extra)
-        except ValueError:
-            pass  # stream was closed
-        except OSError:
-            self.logger.exception(
-                "I/O Error while logging: %s", self.name, extra=self.extra  # type: ignore
-            )
-        except:
-            self.logger.exception(
-                "Something went wrong while logging", extra=self.extra
-            )
-            raise
-
-    def start(self):
-        """starts reading and logging"""
-        program = self.extra.get("program", "")
-        name = f"{program}:{self.log_level}"
-        thread = Thread(target=lambda: self._run(), name=name)
-        thread.daemon = True
-        self.thread = thread
-        thread.start()
-        return self
-
-    def close(self):
-        self.stream.close()
-
-
 class StartupScript:
     """
     Run scripts before the actual programs are started.
     In addition, environman variables can be loaded from a file or generated
     using a script.
     """
 
@@ -274,41 +224,24 @@
         if not sh:
             return
 
         script = "; ".join(sh)
 
         extra = {"program": "startup_script/sh"}
 
-        out: Optional[LogStream] = None
-        err: Optional[LogStream] = None
         try:
-            with Popen(
-                script, stdout=PIPE, stderr=PIPE, env=environment, shell=True
-            ) as process:
-                assert process.stderr
-                assert process.stdout
-
-                err = LogStream(mylogger, ERROR, process.stderr, extra).start()
-                out = LogStream(mylogger, INFO, process.stdout, extra).start()
-
-                process.wait()
-
-                exit_code = process.returncode
-                if exit_code != 0:
-                    raise IOError(
-                        f"{STARTUP_SCRIPT}: Startup script failed with exit code: {exit_code}"
-                    )
+            process = Process(script, environment, shell=True)
+            exit_code = process.execute_and_log(lambda _: None, mylogger, extra)
 
+            if exit_code != 0:
+                raise IOError(
+                    f"{STARTUP_SCRIPT}: Startup script failed with exit code: {exit_code}"
+                )
         except BaseException as e:
             raise IOError(f"{STARTUP_SCRIPT}: Failed to execute startup script: {e}")
-        finally:
-            if out:
-                out.close()
-            if err:
-                err.close()
 
     def buildenv(self, environment: Dict[str, str]):
         """
         runs the buildenv script, processes and updates the current environment
 
         :param environment: the environment
         :type environment: Dict[str, str]
@@ -325,39 +258,32 @@
 
         script = "; ".join(buildenv)
 
         extra = {"program": "startup_script/buildenv"}
 
         mylogger.info("Running buildenv script", extra={"program": ENCAB})
 
-        err: Optional[LogStream] = None
         lines: List[str] = list()
         try:
-            with Popen(
-                script, stderr=PIPE, stdout=PIPE, env=environment, shell=True
-            ) as process:
-                assert process.stdout is not None
-                assert process.stderr is not None
-
-                err = LogStream(mylogger, ERROR, process.stderr, extra).start()
-
-                for line in process.stdout:
-                    strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
-                    lines.append(strline)
-
-                process.wait()
-                exit_code = process.returncode
-                if exit_code != 0:
-                    raise IOError(f"Buildenv script failed with exit code: {exit_code}")
+            def read_lines(process: Popen):
+                assert process.stdout
+                with process.stdout as stdout:
+                    for line in stdout:
+                        strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
+                        lines.append(strline)
+
+            process = Process(script, environment, shell=True)
+
+            exit_code = process.execute_and_log(read_lines, mylogger, extra, log_stdout=False)
+
+            if exit_code != 0:
+                raise IOError(f"Buildenv script failed with exit code: {exit_code}")
 
         except BaseException as e:
             raise IOError(f"{STARTUP_SCRIPT}: Failed to execute buildenv script: {e}")
-        finally:
-            if err:
-                err.close()
 
         self.update_env(environment, stream=StringIO("\n".join(lines)))
 
     def execute(self, environment: Dict[str, str]):
         if self.executed:
             return
```

### Comparing `encab-0.0.6/src/encab/ext/validation.py` & `encab-0.0.7/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.6/src/encab/extensions.py` & `encab-0.0.7/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.6/src/encab/program.py` & `encab-0.0.7/src/encab/program.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,28 @@
-import sys
-
 from copy import deepcopy
 
-from typing import Dict, Optional, IO, Union, List
+from typing import Dict, Optional,Union, List
 
-from subprocess import Popen, PIPE
+from subprocess import Popen
 from threading import Thread
 from signal import SIGINT, SIGTERM
 
-from logging import Logger, INFO, ERROR, getLogger
+from logging import Logger, getLogger
 
+from .common.process import Process
 from .config import ProgramConfig
 from .program_state import (
     ProgramObserver,
     ProgramState,
     ProgramStateHandler,
     ProgramCanceledException,
 )
 from .extensions import extensions
 
 
-class LogStream(object):
-    """
-    Reads from a stream in a background thread and loggs the result line by line
-    """
-
-    def __init__(
-        self, logger: Logger, log_level: int, stream: IO[bytes], extra: Dict[str, str]
-    ) -> None:
-        """
-        :param Logger logger: the logger to which the stream content is written
-        :param int log_level: the log level (see Python logging)
-        :param IOBase stream: the stream that is logged
-        :param Dict[str, str] extra: extra information that is logged each line (see Python logging)
-        """
-        self.logger = logger
-        self.log_level = log_level
-        self.stream = stream
-        self.extra = extra
-        self.thread: Optional[Thread] = None
-
-    def _run(self):
-        try:
-            for line in self.stream:
-                strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
-                self.logger.log(self.log_level, strline, extra=self.extra)
-        except ValueError:
-            pass  # stream was closed
-        except OSError:
-            self.logger.exception(
-                "I/O Error while logging: %s", self.name, extra=self.extra  # type: ignore
-            )
-        except:
-            self.logger.exception(
-                "Something went wrong while logging", extra=self.extra
-            )
-            raise
-
-    def start(self):
-        """starts reading and logging"""
-        program = self.extra.get("program", "")
-        name = f"{program}:{self.log_level}"
-        thread = Thread(target=lambda: self._run(), name=name)
-        thread.daemon = True
-        self.thread = thread
-        thread.start()
-        return self
-
-    def close(self):
-        try:
-            self.stream.flush()
-        except IOError:
-            pass
-        self.stream.close()
-
-
 class ExecutionContext(object):
     """
     The context in which a program is executed
 
     It contains all non-static resources necessary to execute a program,
     such as the logger and the system environment.
     """
@@ -152,27 +96,33 @@
             assert isinstance(self.config.sh, str)
             self.command = [self.config.sh]
 
         observer = self.context.observer
 
         self._observer = observer
         self._state_handler = ProgramStateHandler(observer)
-        self._process: Optional[Popen] = None
+        self._process: Optional[Process] = None
 
     def _run(self) -> None:
         logger = self.logger
         extra = self.extra
+
         command = self.command
         env = self.context.environment
         state = self._state_handler
         observer = self._observer
+
         startup_delay = self.config.startup_delay
+
         umask = self.config.umask
-        out: Optional[LogStream] = None
-        err: Optional[LogStream] = None
+        user = self.config.user
+        group = self.config.group
+
+        assert user is None or isinstance(user, int)
+        assert group is None or isinstance(group, int)
 
         try:
             assert isinstance(startup_delay, float) or isinstance(startup_delay, int)
             assert isinstance(umask, int)
 
             state.wait(float(startup_delay))
 
@@ -181,49 +131,35 @@
 
             shell = self.shell
             args: Union[str, List[str]] = command
 
             if shell:
                 args = command[0]
 
-            process = Popen(
+            def on_run(popen: Popen):
+                state.set(ProgramState.RUNNING)
+                observer.on_run(popen.pid)
+
+            self._process = Process(
                 args,
-                stdout=PIPE,
-                stderr=PIPE,
-                env=env,
-                user=self.config.user,
+                env,
+                user=user,
+                group=group,
                 umask=umask,
                 shell=shell,
                 start_new_session=True,
             )
-            assert process.stdout is not None
-            assert process.stderr is not None
-
-            state.set(ProgramState.RUNNING)
-            self._process = process
-
-            observer.on_run(process.pid)
-
-            err = LogStream(logger, ERROR, process.stderr, extra).start()
-            out = LogStream(logger, INFO, process.stdout, extra).start()
-
-            process.wait()
-            state.handle_exit(process.returncode, self.command)
+            exit_code = self._process.execute_and_log(on_run, logger, extra)
+            state.handle_exit(exit_code, self.command)
         except ProgramCanceledException:
             observer.on_cancel()
             state.set(ProgramState.CANCELED)
         except BaseException as e:
             observer.on_crash(self.command, e)
             state.set(ProgramState.CRASHED)
-        finally:
-            self._process = None
-            if out:
-                out.close()
-            if err:
-                err.close()
 
     def get_state(self) -> int:
         return self._state_handler.get()
 
     def start(self, timeout: Optional[float] = 1) -> int:
         thread = Thread(target=lambda: self._run(), name=self.name)
         thread.daemon = True
@@ -236,14 +172,14 @@
     def join(
         self,
         timeout: Optional[float] = None,
     ) -> ProgramState:
         return self._state_handler.join(timeout)
 
     def interrupt(self) -> None:
-        return self._state_handler.kill(self._process, SIGINT)
+        return self._state_handler.signal(self._process, SIGINT)
 
     def terminate(self) -> None:
-        return self._state_handler.kill(self._process, SIGTERM)  # type: ignore
+        return self._state_handler.signal(self._process, SIGTERM)
 
     def join_wait(self, timeout: Optional[float] = None) -> ProgramState:
         return self._state_handler.join_wait(timeout)
```

### Comparing `encab-0.0.6/src/encab/program_state.py` & `encab-0.0.7/src/encab/program_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import os
-
 from signal import SIGINT
 
 from copy import deepcopy
 
 from typing import Dict, Optional, List, Callable
 from abc import ABC, abstractmethod
 
 from enum import IntEnum
-from subprocess import Popen
 from threading import Condition
 
 from logging import Logger, INFO, ERROR
 
+from .common.process import Process
 from .config import ProgramConfig
 
 
 class ProgramObserver(ABC):
     @abstractmethod
     def get_name(self) -> str:
         pass
@@ -116,14 +114,17 @@
             extra=self.extra,
         )
 
         self.logger.debug("Config: %s", str(config), extra=self.extra)
 
         if config.user:
             self.logger.debug("User id: %d", config.user, extra=self.extra)
+            
+        if config.user:
+            self.logger.debug("Group id: %d", config.group, extra=self.extra)
 
         if config.umask:
             self.logger.debug(
                 "umask: 0o%s", format(config.umask, "o"), extra=self.extra
             )
 
     def on_wait(self, startup_time: float):
@@ -294,29 +295,30 @@
         else:
             self._observer.on_crash(
                 command,
                 ProgramCrashedException(f"State: {state}, exit code {exit_code}"),
             )
             self.set(ProgramState.CRASHED)
 
-    def kill(self, process: Optional[Popen], signal):
+    def signal(self, process: Optional[Process], signal):
         with self._cond:
             if self._state >= ProgramState.CANCELED:
                 return
 
             if self._state == ProgramState.WAITING:
                 self._state = ProgramState.CANCELING
             else:
                 self._state = ProgramState.STOPPING
-                pid = process.pid if process else None
-                if pid:
-                    if signal == SIGINT:
-                        self._observer.on_interrupt(pid)
-                    else:
-                        self._observer.on_terminate(pid)
-
-                    try:
-                        os.kill(pid, signal)
-                    except ProcessLookupError:
-                        pass
+                if process:
+                    pid = process.pid()
+                    if pid:
+                        if signal == SIGINT:
+                            self._observer.on_interrupt(pid)
+                        else:
+                            self._observer.on_terminate(pid)
+
+                        try:
+                            process.signal(signal)
+                        except ProcessLookupError:
+                            pass
 
             self._cond.notify_all()
```

### Comparing `encab-0.0.6/src/encab/programs.py` & `encab-0.0.7/src/encab/programs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         main: Optional[Program] = None
         self.helpers: List[Program] = list()
 
         for name, program_config in program_configs.items():
             if encab_config:
                 program_config.extend(encab_config)
                 program_config.set_user()
+                program_config.set_group()
 
             if name == "main":
                 if args:
                     program_config.command = args
                 main = Program(name, program_config, context)
             else:
                 self.helpers.append(Program(name, program_config, context))
```

### Comparing `encab-0.0.6/src/encab.egg-info/PKG-INFO` & `encab-0.0.7/src/encab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.6
+Version: 0.0.7
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Encab: A Simple Process Manager
 
 **Encab** is a process manager that simplifies running multiple services in a container or from the command line.
 
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.6
+INFO  encab: encab 0.0.7
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -175,15 +175,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.6
+   INFO  encab: encab 0.0.7
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.6/src/encab.egg-info/SOURCES.txt` & `encab-0.0.7/src/encab.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,11 +11,13 @@
 src/encab/programs.py
 src/encab.egg-info/PKG-INFO
 src/encab.egg-info/SOURCES.txt
 src/encab.egg-info/dependency_links.txt
 src/encab.egg-info/entry_points.txt
 src/encab.egg-info/requires.txt
 src/encab.egg-info/top_level.txt
+src/encab/common/log_stream.py
+src/encab/common/process.py
 src/encab/ext/__init__.py
 src/encab/ext/log_sanitizer.py
 src/encab/ext/startup_script.py
 src/encab/ext/validation.py
```

