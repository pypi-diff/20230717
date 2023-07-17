# Comparing `tmp/envappconfig-2023.4.988.tar.gz` & `tmp/envappconfig-2023.5.1022.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envappconfig-2023.4.988.tar", max compression
+gzip compressed data, was "envappconfig-2023.5.1022.tar", max compression
```

## Comparing `envappconfig-2023.4.988.tar` & `envappconfig-2023.5.1022.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11350 2023-01-04 16:28:21.751134 envappconfig-2023.4.988/LICENSE
--rw-r--r--   0        0        0     3092 2023-01-04 16:28:21.751134 envappconfig-2023.4.988/README.md
--rw-r--r--   0        0        0       97 2023-01-04 16:28:21.751134 envappconfig-2023.4.988/envappconfig/__init__.py
--rw-r--r--   0        0        0     5447 2023-01-04 16:28:21.751134 envappconfig-2023.4.988/envappconfig/envappconfig.py
--rw-r--r--   0        0        0       49 2023-01-04 16:28:21.751134 envappconfig-2023.4.988/envappconfig/exceptions.py
--rw-r--r--   0        0        0     1066 2023-01-04 16:28:35.659152 envappconfig-2023.4.988/pyproject.toml
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 envappconfig-2023.4.988/setup.py
--rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 envappconfig-2023.4.988/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-01-05 17:02:04.136932 envappconfig-2023.5.1022/LICENSE
+-rw-r--r--   0        0        0     2597 2023-01-05 17:02:04.136932 envappconfig-2023.5.1022/README.md
+-rw-r--r--   0        0        0       97 2023-01-05 17:02:04.136932 envappconfig-2023.5.1022/envappconfig/__init__.py
+-rw-r--r--   0        0        0     3896 2023-01-05 17:02:04.136932 envappconfig-2023.5.1022/envappconfig/envappconfig.py
+-rw-r--r--   0        0        0       49 2023-01-05 17:02:04.136932 envappconfig-2023.5.1022/envappconfig/exceptions.py
+-rw-r--r--   0        0        0     1067 2023-01-05 17:02:17.953127 envappconfig-2023.5.1022/pyproject.toml
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 envappconfig-2023.5.1022/setup.py
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 envappconfig-2023.5.1022/PKG-INFO
```

### Comparing `envappconfig-2023.4.988/LICENSE` & `envappconfig-2023.5.1022/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 Spectric Labs, Inc.
+   Copyright 2023 Spectric Labs, Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `envappconfig-2023.4.988/README.md` & `envappconfig-2023.5.1022/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 envappconfig is intended to provide simple configuration via environment variables, in the same spirit as argparse.
 
 Features:
 * Autogenerates usage output if an environment variable is missing
 * Default settings for missing environment variables
 * Functions that transform the environment variable string to the value you need
 * Environment variable prefixes
-* Optional dictionary of the config
 
 ## Basic example
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(description='Amazing app')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.add_env('mirror', help='The URL to mirror')
-config.configure()
+env = EnvAppConfig(description='Amazing app')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+env.add_env('mirror', help='The URL to mirror')
+config = env.configure()
 
 # Returns PORT from os.environ transformed to an int,
 # or 1234 if PORT does not exist.
 config.port
 
 # Returns MIRROR from os.environ,
 # or displays usage if MIRROR does not exist, then exits.
@@ -31,18 +30,18 @@
 ## Adding a prefix
 
 If all the environment variables for the app have the same prefix, it can be specified with the `prefix` parameter.
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(prefix='MYAPP', description='Amazing app')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.add_env('mirror', help='The URL to mirror')
-config.configure()
+env = EnvAppConfig(prefix='MYAPP', description='Amazing app')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+env.add_env('mirror', help='The URL to mirror')
+config = env.configure()
 
 # Returns MYAPP_PORT from os.environ transformed to an int,
 # or 1234 if MYAPP_PORT does not exist.
 config.port
 
 # Returns MYAPP_MIRROR from os.environ,
 # or displays usage if MYAPP_MIRROR does not exist, then exits.
@@ -50,47 +49,31 @@
 ```
 
 ## Custom transforms
 
 The `transform` parameter can be used to specify normal transforms, like `int` or `float` (the default is `str`), but it can also take custom transform functions.  The transform function must take a single parameter, which will be filled in with the string value from the environment variable.
 
 ```python
-config = EnvAppConfig(description='Amazing app')
+env = EnvAppConfig(description='Amazing app')
 
 # Double the timeout specified in the TIMEOUT environment variable,
 # or default to 60.
-config.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')
+env.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')
 ...
 ```
 
 ## Adding more config values
 
-Additional config values can be added to an existing EnvAppConfig, which can be helpful when there's a config value that needs to be calculated based on other config values.
+Additional config values can be added to an existing namespace, which can be helpful when there's a config value that needs to be calculated based on other config values.
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(description='Amazing app')
-config.add_env('bind', help='IP address to bind to')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.configure()
-config.add_conf('listen', f'{config.bind}:{config.port}')
+env = EnvAppConfig(description='Amazing app')
+env.add_env('bind', help='IP address to bind to')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+config = env.configure()
+config.listen = f'{config.bind}:{config.port}'
 
 # Returns the combined bind:port string.
 config.listen
 ```
-
-## Getting a config dictionary
-
-The EnvAppConfig instance is also available as a dictionary.
-
-```python
-from envappconfig import EnvAppConfig
-
-config = EnvAppConfig(description='Amazing app')
-config.add_env('bind', help='IP address to bind to')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.configure()
-
-# Returns a dictionary containing {'bind': '1.2.3.4', 'port': 1234}
-config.asdict()
-```
```

### Comparing `envappconfig-2023.4.988/envappconfig/envappconfig.py` & `envappconfig-2023.5.1022/envappconfig/envappconfig.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from argparse import Namespace
 from collections import OrderedDict
-from copy import copy
 from typing import Any, Callable, Dict, Iterable, Optional, Union
 
 import os
 import re
 import sys
 
 from .exceptions import EnvAppConfigException
@@ -59,107 +59,71 @@
 
 class EnvAppConfig:
     def __init__(
         self,
         prefix: Optional[str]=None,
         description: Optional[str]=None,
     ) -> None:
-        self.existing_attributes = ('add_conf', 'add_env', 'asdict', 'configure', 'usage')
-        self.configure_called = False
         self.prefix = prefix.strip() if type(prefix) is str else None
         self.description = description.strip() if type(description) is str else None
         self.full_names = set()
         self.envs = OrderedDict()
-        self.confs = {}
 
         if self.prefix is not None and not valid_name(self.prefix):
             raise EnvAppConfigException(f'{self.prefix} is not a valid prefix')
 
     def add_env(
         self,
         name: str,
         default: Optional[Any]=None,
         help: str='Description not provided',  # pylint: disable=redefined-builtin
         transform=str,
     ) -> None:
-        self.configure_called = False
         name = name.strip().lower()
 
-        # Can't use hasattr(self, name) here because it will call __getattr__(),
-        # which raises an exception if configure() hasn't been called yet.
-        if name in self.existing_attributes:
-            raise EnvAppConfigException(f'{name} is already an attribute of EnvAppConfig')
-
         if not valid_name(name):
             raise EnvAppConfigException(f'{name} is not a valid environment variable name')
 
-        if name in self.envs or name in self.confs:
+        if name in self.envs:
             raise EnvAppConfigException(f'{name} already specified in EnvAppConfig')
 
         full_name = apply_prefix(self.prefix, name)
         self.full_names.add(full_name)
         self.envs[name] = Env(full_name, default, help, transform)
 
-    def __getattr__(self, name):
-        if not self.configure_called:
-            raise EnvAppConfigException('configure() needs to be called before config values are available')
-
-        if name not in self.confs:
-            raise AttributeError(f'{name} not available in config')
-
-        return self.confs[name]
-
-    def asdict(self):
-        if not self.configure_called:
-            raise EnvAppConfigException('configure() needs to be called before config values are available')
-
-        return copy(self.confs)
-
-    def configure(self, environ: Optional[Union[os._Environ, Dict[str, str]]]=None) -> None:
+    def configure(self, environ: Optional[Union[os._Environ, Dict[str, str]]]=None) -> Namespace:
         if environ is None:
             environ = os.environ
 
         is_missing_envs = False
+        confs = {}
 
         for name, env in self.envs.items():
             try:
-                self.confs[name] = env.configure(environ)
+                confs[name] = env.configure(environ)
             except EnvAppConfigException:
                 print(f'Error: {env.name} not available in environment')
                 is_missing_envs = True
             except Exception:
                 print(f'Error while trying transform {env.name} value "{env.raw_value(environ)}"')
                 self.usage()
                 raise
 
         if is_missing_envs:
             self.usage()
             sys.exit(1)
 
-        self.configure_called = True
+        return Namespace(**confs)
 
     def usage(self) -> None:
         print('\nusage:\n')
 
         if self.description:
             print(f'{self.description}\n')
 
         if len(self.envs.keys()) > 0:
             print('Config Environment Variables:')
 
         longest_name_len = longest_str_len(self.full_names)
 
         for env in self.envs.values():
             env.usage(1, longest_name_len)
-
-    def add_conf(self, name: str, value: Any) -> None:
-        name = name.strip()
-
-        # Can't use hasattr(self, name) here because it will call __getattr__(),
-        # which raises an exception if configure() hasn't been called yet.
-        if name in self.existing_attributes:
-            raise EnvAppConfigException(f'{name} is already an attribute of EnvAppConfig')
-
-        if name in self.envs or name in self.confs:
-            raise EnvAppConfigException(f'{name} already specified in EnvAppConfig')
-
-        self.confs[name] = value
```

### Comparing `envappconfig-2023.4.988/pyproject.toml` & `envappconfig-2023.5.1022/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envappconfig"
-version = "2023.4.988"
+version = "2023.5.1022"
 description = "Simple app configuration via environment variables, in the spirit of argparse."
 authors = ["Spectric Labs <foss@spectric.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/spectriclabs/envappconfig"
 
 [tool.poetry.dependencies]
```

### Comparing `envappconfig-2023.4.988/setup.py` & `envappconfig-2023.5.1022/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['envappconfig']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'envappconfig',
-    'version': '2023.4.988',
+    'version': '2023.5.1022',
     'description': 'Simple app configuration via environment variables, in the spirit of argparse.',
-    'long_description': "# envappconfig\n\nenvappconfig is intended to provide simple configuration via environment variables, in the same spirit as argparse.\n\nFeatures:\n* Autogenerates usage output if an environment variable is missing\n* Default settings for missing environment variables\n* Functions that transform the environment variable string to the value you need\n* Environment variable prefixes\n* Optional dictionary of the config\n\n## Basic example\n\n```python\nfrom envappconfig import EnvAppConfig\n\nconfig = EnvAppConfig(description='Amazing app')\nconfig.add_env('port', default=1234, transform=int, help='The listen port')\nconfig.add_env('mirror', help='The URL to mirror')\nconfig.configure()\n\n# Returns PORT from os.environ transformed to an int,\n# or 1234 if PORT does not exist.\nconfig.port\n\n# Returns MIRROR from os.environ,\n# or displays usage if MIRROR does not exist, then exits.\nconfig.mirror\n```\n\n## Adding a prefix\n\nIf all the environment variables for the app have the same prefix, it can be specified with the `prefix` parameter.\n\n```python\nfrom envappconfig import EnvAppConfig\n\nconfig = EnvAppConfig(prefix='MYAPP', description='Amazing app')\nconfig.add_env('port', default=1234, transform=int, help='The listen port')\nconfig.add_env('mirror', help='The URL to mirror')\nconfig.configure()\n\n# Returns MYAPP_PORT from os.environ transformed to an int,\n# or 1234 if MYAPP_PORT does not exist.\nconfig.port\n\n# Returns MYAPP_MIRROR from os.environ,\n# or displays usage if MYAPP_MIRROR does not exist, then exits.\nconfig.mirror\n```\n\n## Custom transforms\n\nThe `transform` parameter can be used to specify normal transforms, like `int` or `float` (the default is `str`), but it can also take custom transform functions.  The transform function must take a single parameter, which will be filled in with the string value from the environment variable.\n\n```python\nconfig = EnvAppConfig(description='Amazing app')\n\n# Double the timeout specified in the TIMEOUT environment variable,\n# or default to 60.\nconfig.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')\n...\n```\n\n## Adding more config values\n\nAdditional config values can be added to an existing EnvAppConfig, which can be helpful when there's a config value that needs to be calculated based on other config values.\n\n```python\nfrom envappconfig import EnvAppConfig\n\nconfig = EnvAppConfig(description='Amazing app')\nconfig.add_env('bind', help='IP address to bind to')\nconfig.add_env('port', default=1234, transform=int, help='The listen port')\nconfig.configure()\nconfig.add_conf('listen', f'{config.bind}:{config.port}')\n\n# Returns the combined bind:port string.\nconfig.listen\n```\n\n## Getting a config dictionary\n\nThe EnvAppConfig instance is also available as a dictionary.\n\n```python\nfrom envappconfig import EnvAppConfig\n\nconfig = EnvAppConfig(description='Amazing app')\nconfig.add_env('bind', help='IP address to bind to')\nconfig.add_env('port', default=1234, transform=int, help='The listen port')\nconfig.configure()\n\n# Returns a dictionary containing {'bind': '1.2.3.4', 'port': 1234}\nconfig.asdict()\n```\n",
+    'long_description': "# envappconfig\n\nenvappconfig is intended to provide simple configuration via environment variables, in the same spirit as argparse.\n\nFeatures:\n* Autogenerates usage output if an environment variable is missing\n* Default settings for missing environment variables\n* Functions that transform the environment variable string to the value you need\n* Environment variable prefixes\n\n## Basic example\n\n```python\nfrom envappconfig import EnvAppConfig\n\nenv = EnvAppConfig(description='Amazing app')\nenv.add_env('port', default=1234, transform=int, help='The listen port')\nenv.add_env('mirror', help='The URL to mirror')\nconfig = env.configure()\n\n# Returns PORT from os.environ transformed to an int,\n# or 1234 if PORT does not exist.\nconfig.port\n\n# Returns MIRROR from os.environ,\n# or displays usage if MIRROR does not exist, then exits.\nconfig.mirror\n```\n\n## Adding a prefix\n\nIf all the environment variables for the app have the same prefix, it can be specified with the `prefix` parameter.\n\n```python\nfrom envappconfig import EnvAppConfig\n\nenv = EnvAppConfig(prefix='MYAPP', description='Amazing app')\nenv.add_env('port', default=1234, transform=int, help='The listen port')\nenv.add_env('mirror', help='The URL to mirror')\nconfig = env.configure()\n\n# Returns MYAPP_PORT from os.environ transformed to an int,\n# or 1234 if MYAPP_PORT does not exist.\nconfig.port\n\n# Returns MYAPP_MIRROR from os.environ,\n# or displays usage if MYAPP_MIRROR does not exist, then exits.\nconfig.mirror\n```\n\n## Custom transforms\n\nThe `transform` parameter can be used to specify normal transforms, like `int` or `float` (the default is `str`), but it can also take custom transform functions.  The transform function must take a single parameter, which will be filled in with the string value from the environment variable.\n\n```python\nenv = EnvAppConfig(description='Amazing app')\n\n# Double the timeout specified in the TIMEOUT environment variable,\n# or default to 60.\nenv.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')\n...\n```\n\n## Adding more config values\n\nAdditional config values can be added to an existing namespace, which can be helpful when there's a config value that needs to be calculated based on other config values.\n\n```python\nfrom envappconfig import EnvAppConfig\n\nenv = EnvAppConfig(description='Amazing app')\nenv.add_env('bind', help='IP address to bind to')\nenv.add_env('port', default=1234, transform=int, help='The listen port')\nconfig = env.configure()\nconfig.listen = f'{config.bind}:{config.port}'\n\n# Returns the combined bind:port string.\nconfig.listen\n```\n",
     'author': 'Spectric Labs',
     'author_email': 'foss@spectric.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/spectriclabs/envappconfig',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `envappconfig-2023.4.988/PKG-INFO` & `envappconfig-2023.5.1022/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envappconfig
-Version: 2023.4.988
+Version: 2023.5.1022
 Summary: Simple app configuration via environment variables, in the spirit of argparse.
 Home-page: https://github.com/spectriclabs/envappconfig
 License: Apache-2.0
 Author: Spectric Labs
 Author-email: foss@spectric.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,25 +22,24 @@
 envappconfig is intended to provide simple configuration via environment variables, in the same spirit as argparse.
 
 Features:
 * Autogenerates usage output if an environment variable is missing
 * Default settings for missing environment variables
 * Functions that transform the environment variable string to the value you need
 * Environment variable prefixes
-* Optional dictionary of the config
 
 ## Basic example
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(description='Amazing app')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.add_env('mirror', help='The URL to mirror')
-config.configure()
+env = EnvAppConfig(description='Amazing app')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+env.add_env('mirror', help='The URL to mirror')
+config = env.configure()
 
 # Returns PORT from os.environ transformed to an int,
 # or 1234 if PORT does not exist.
 config.port
 
 # Returns MIRROR from os.environ,
 # or displays usage if MIRROR does not exist, then exits.
@@ -50,18 +49,18 @@
 ## Adding a prefix
 
 If all the environment variables for the app have the same prefix, it can be specified with the `prefix` parameter.
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(prefix='MYAPP', description='Amazing app')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.add_env('mirror', help='The URL to mirror')
-config.configure()
+env = EnvAppConfig(prefix='MYAPP', description='Amazing app')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+env.add_env('mirror', help='The URL to mirror')
+config = env.configure()
 
 # Returns MYAPP_PORT from os.environ transformed to an int,
 # or 1234 if MYAPP_PORT does not exist.
 config.port
 
 # Returns MYAPP_MIRROR from os.environ,
 # or displays usage if MYAPP_MIRROR does not exist, then exits.
@@ -69,48 +68,32 @@
 ```
 
 ## Custom transforms
 
 The `transform` parameter can be used to specify normal transforms, like `int` or `float` (the default is `str`), but it can also take custom transform functions.  The transform function must take a single parameter, which will be filled in with the string value from the environment variable.
 
 ```python
-config = EnvAppConfig(description='Amazing app')
+env = EnvAppConfig(description='Amazing app')
 
 # Double the timeout specified in the TIMEOUT environment variable,
 # or default to 60.
-config.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')
+env.add_env('timeout', default=60, transform=lambda x: int(x) * 2, help='Timeout in seconds')
 ...
 ```
 
 ## Adding more config values
 
-Additional config values can be added to an existing EnvAppConfig, which can be helpful when there's a config value that needs to be calculated based on other config values.
+Additional config values can be added to an existing namespace, which can be helpful when there's a config value that needs to be calculated based on other config values.
 
 ```python
 from envappconfig import EnvAppConfig
 
-config = EnvAppConfig(description='Amazing app')
-config.add_env('bind', help='IP address to bind to')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.configure()
-config.add_conf('listen', f'{config.bind}:{config.port}')
+env = EnvAppConfig(description='Amazing app')
+env.add_env('bind', help='IP address to bind to')
+env.add_env('port', default=1234, transform=int, help='The listen port')
+config = env.configure()
+config.listen = f'{config.bind}:{config.port}'
 
 # Returns the combined bind:port string.
 config.listen
 ```
 
-## Getting a config dictionary
-
-The EnvAppConfig instance is also available as a dictionary.
-
-```python
-from envappconfig import EnvAppConfig
-
-config = EnvAppConfig(description='Amazing app')
-config.add_env('bind', help='IP address to bind to')
-config.add_env('port', default=1234, transform=int, help='The listen port')
-config.configure()
-
-# Returns a dictionary containing {'bind': '1.2.3.4', 'port': 1234}
-config.asdict()
-```
-
```

