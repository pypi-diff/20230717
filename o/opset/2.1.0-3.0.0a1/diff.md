# Comparing `tmp/opset-2.1.0.tar.gz` & `tmp/opset-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opset-2.1.0.tar", last modified: Wed Oct  7 16:55:34 2020, max compression
+gzip compressed data, was "opset-3.0.0a1.tar", max compression
```

## Comparing `opset-2.1.0.tar` & `opset-3.0.0a1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0    11357 2020-02-27 17:57:55.829661 opset-2.1.0/LICENSE
--rw-r--r--   0        0        0    24719 2020-10-07 16:54:19.850296 opset-2.1.0/README.md
--rw-r--r--   0        0        0    40960 2020-10-07 13:28:04.452997 opset-2.1.0/opset/.configurator.py.swo
--rw-r--r--   0        0        0      328 2020-02-27 17:57:55.873624 opset-2.1.0/opset/__init__.py
--rw-r--r--   0        0        0    24343 2020-10-07 16:54:19.857024 opset-2.1.0/opset/configurator.py
--rw-r--r--   0        0        0        0 2020-06-09 18:49:49.334121 opset-2.1.0/opset/py.typed
--rw-r--r--   0        0        0     4037 2020-09-11 18:06:03.887283 opset-2.1.0/opset/utils.py
--rw-r--r--   0        0        0     1300 2020-10-07 16:54:19.862462 opset-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    26063 2020-10-07 16:55:36.089285 opset-2.1.0/setup.py
--rw-r--r--   0        0        0    25685 2020-10-07 16:55:36.092338 opset-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 16:21:49.415760 opset-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0    24719 2023-07-17 16:21:49.415760 opset-3.0.0a1/README.md
+-rw-r--r--   0        0        0      328 2023-07-17 16:21:49.415760 opset-3.0.0a1/opset/__init__.py
+-rw-r--r--   0        0        0    24214 2023-07-17 17:20:51.727956 opset-3.0.0a1/opset/configurator.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:21:49.415760 opset-3.0.0a1/opset/py.typed
+-rw-r--r--   0        0        0     3981 2023-07-17 16:59:01.186916 opset-3.0.0a1/opset/utils.py
+-rw-r--r--   0        0        0     1665 2023-07-17 18:27:53.372084 opset-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    25663 1970-01-01 00:00:00.000000 opset-3.0.0a1/PKG-INFO
```

### Comparing `opset-2.1.0/LICENSE` & `opset-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `opset-2.1.0/README.md` & `opset-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `opset-2.1.0/opset/configurator.py` & `opset-3.0.0a1/opset/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,19 +116,15 @@
 
         return tentative_path
 
     def _read_yaml_config(self, config_name: str, raise_not_found: bool = True) -> Dict[str, Dict]:
         config_path = self._get_config_file_path(config_name)
         try:
             with open(config_path, "r") as config_file:
-                if hasattr(yaml, "FullLoader"):
-                    # pyyaml 5.1+
-                    return yaml.load(config_file, Loader=yaml.FullLoader) or {}
-                # pyyaml 3.13
-                return yaml.load(config_file) or {}
+                return yaml.load(config_file, Loader=yaml.FullLoader) or {}
         except FileNotFoundError:
             warnings.warn(f"WARNING: Config not found at {config_path}")
             if raise_not_found:
                 raise
             return {}
 
     def _build_critical_setting_exception(self, missing_settings: List[List[str]]) -> CriticalSettingException:
@@ -503,27 +499,29 @@
         custom_processors = custom_processors or []
         if use_hostname_processor:
             custom_processors.append(HostNameProcessor())
 
     pre_processors = [
         structlog.stdlib.filter_by_level,
     ]
-    shared_processors = [
+    shared_processors: Any = [
         structlog.stdlib.add_log_level,
         structlog.processors.StackInfoRenderer(),
         structlog.processors.format_exc_info,
         structlog.processors.TimeStamper(fmt=config.logging.date_format, utc=config.logging.use_utc),
         structlog.processors.UnicodeDecoder(),
         structlog.stdlib.add_logger_name,
     ] + custom_processors
     post_processors = [structlog.stdlib.ProcessorFormatter.wrap_for_formatter]
 
+    processors: Any = pre_processors + shared_processors + post_processors
+
     structlog.reset_defaults()
     structlog.configure(
-        processors=pre_processors + shared_processors + post_processors,
+        processors=processors,
         logger_factory=structlog.stdlib.LoggerFactory(),
         cache_logger_on_first_use=True,
         wrapper_class=structlog.stdlib.BoundLogger,
     )
 
     use_colors = getattr(config.logging, "colors", False)
```

### Comparing `opset-2.1.0/opset/utils.py` & `opset-3.0.0a1/opset/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # __init__.py
 # Emilio Assuncao, 2019-01-24
 # Copyright (c) Element AI Inc. All rights not expressly granted hereunder are reserved.
 
 from contextlib import contextmanager
 from copy import copy
-from tempfile import NamedTemporaryFile, _TemporaryFileWrapper  # type: ignore
+from tempfile import NamedTemporaryFile, _TemporaryFileWrapper  # noqa
 from typing import Any, Dict, Generator, Optional
 from unittest.mock import patch
 
 import pkg_resources
 import yaml
-from munch import Munch  # noqa
 
 from opset.configurator import Config, config
 
 
 @contextmanager
 def mock_config(config_values: Dict[str, Dict[str, Any]]) -> Generator:
     """Inject a fake config into the interpreter.
@@ -69,15 +68,15 @@
     default_temp_file = NamedTemporaryFile()
 
     def save_as_tmp(_config: Dict[str, Dict[str, Any]], temp_file: _TemporaryFileWrapper) -> str:
         if not _config:
             return "this-is-not-a-valid-path.yml"
         with open(temp_file.name, "w") as file_buffer:
             yaml.dump(_config, file_buffer)
-        return temp_file.name  # type: ignore
+        return temp_file.name
 
     configs = {"default.yml": save_as_tmp(default_values, default_temp_file)}
 
     if local_values:
         local_temp_file = NamedTemporaryFile()
         configs["local.yml"] = save_as_tmp(local_values, local_temp_file)
```

### Comparing `opset-2.1.0/setup.py` & `opset-3.0.0a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,562 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: opset
+Version: 3.0.0a1
+Summary: A library for simplifying the configuration of Python applications at all stages of deployment.
+Home-page: https://github.com/MarcDufresne/opset
+License: Apache-2.0
+Keywords: config,management,configuration,logging,setup
+Author: Marc-André Dufresne
+Author-email: marc.andre.dufresne@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4,<0.5)
+Requires-Dist: munch (>=4.0,<5.0)
+Requires-Dist: pytz (>=2023.3)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: structlog (>=23.1,<24.0)
+Project-URL: Documentation, https://github.com/MarcDufresne/opset
+Project-URL: Repository, https://github.com/MarcDufresne/opset
+Description-Content-Type: text/markdown
 
-packages = \
-['opset']
+# Opset
 
-package_data = \
-{'': ['*']}
+[![Coverage Status](https://coveralls.io/repos/github/ElementAI/opset/badge.svg)](https://coveralls.io/github/ElementAI/opset)
 
-install_requires = \
-['colorama>=0.4.1,<0.5.0',
- 'munch>=2.3,<3.0',
- 'pytz>=2018.9',
- 'pyyaml>=3.13,<6',
- 'structlog>=19.1,<21']
-
-setup_kwargs = {
-    'name': 'opset',
-    'version': '2.1.0',
-    'description': 'A library for simplifying the configuration of Python applications at all stages of deployment.',
-    'long_description': '# Opset\n\n[![Coverage Status](https://coveralls.io/repos/github/ElementAI/opset/badge.svg)](https://coveralls.io/github/ElementAI/opset)\n\nA library for simplifying the configuration of Python applications at all stages of deployment.\n\nOpset is a config manager that let you manage your configuration via YAML file or environment variables.\nThe general principle of Opset is that you want to hold your secrets and manage your configurations via\nconfiguration files when doing local development and via environment variables when your app is deployed. It is however\npossible to also handle local development through environment variables if the developer sees fit.\n\nWith Opset you define everything that can be tweaked with your application in one specific\nfile (`default.yml`). This way the developers and integrators working with your code will know exactly what setting they\ncan change on your code base. You can then overwrite the default config with a local config stored in a file called\n`local.yml`, this file is aimed to be used for local development by your developers and let them easily manage a\nconfiguration file that fits their development need. Finally, you can also have environment variables that have a\nmatching name to your config that will overwrite your config, letting you use your config in a deployed environment\nwithout having your secret written down in a config file. Opset aims to reconcile the ease of use of a\nconfig file with the added security of environment variables.\n\nThis library is available on PyPI under the name Opset. You can install with pip by running `pip install opset`.\n\n# Table of Contents\n\n1. [Lexicon](#lexicon)\n1. [Architecture Overview](#architecture-overview)\n    1. [Loading the config for unit tests](#loading-the-config-for-unit-tests)\n    1. [Safeguards](#safeguards)\n        1. [Settings not declared in default.yml are not loaded](#settings-not-declared-in-defaultyml-are-not-loaded)\n        1. [Forcing all default settings to have values](#forcing-all-default-settings-to-have-values)\n1. [Usage Guide](#usage-guide)\n    1. [Making the difference between null and empty](#making-the-difference-between-null-and-empty)\n1. [Example of Usage](#example-of-usage)\n    1. [Opset + Environment Variables](#Opset--environment-variables)\n    1. [Naming your config sections](#naming-your-config-sections)\n    1. [Controlling your entry points](#controlling-your-entry-points)\n1. [Example Configuration file](#example-configuration-file)\n    1. [default.yml](#defaultyml)\n    1. [local.yml](#localyml)\n    1. [unit_test.yml](#unit_testyml)\n    1. [Example Logging Configuration values](#example-logging-configuration-values)\n    1. [Log Processors](#log-processors)\n1. [Support for unit tests](#support-for-unit-tests)\n    1. [setup_unit_test_config](#setup_unit_test_config)\n        1. [Usage example of setup_unit_test_config](#usage-example-of-setup_unit_test_config)\n    1. [mock_config](#mock_config)\n        1. [Usage example of mock_config](#usage-example-of-mock_config)\n1. [Contributing and getting set up for local development](#contributing-and-getting-set-up-for-local-development)\n\n## Lexicon\n\n| Term | Definition |\n|--- | --- |\n| config |\tA configuration file (format: YAML). |\n| section\t| A section within a configuration file, a section tend to group different settings together under a logical block. For example a section named redis would encompass all settings related specifically to redis. |\n| setting\t| A key within a section in a configuration file. A value is associated with a key and querying the config for a setting within a section will return the value associated with it. |\n\n![Lexicon](https://github.com/ElementAI/opset/raw/master/doc/lexicon.png)\n\n## Architecture Overview\n\nThere are three possible config files\n\n| Config Name | Purpose |\n| --- | --- |\n| default.yml | This is the base config, `default.yml` needs to have the declaration of all sections and settings. |\n| local.yml | This is a local config that overwrites the default config, this file is not committed to the repository and is meant to be used in a local development environment. |\n| unit_test.yml | This is a local config that overwrites the default config during unit tests, this file is not committed to the repository and is meant to be used in a local development environment. When the config is initialized for unit tests, if a `unit_test.yml` file is present it will be loaded, otherwise the environment variables will be loaded on top of the default config. |\n\nThe content of the default config is loaded first, and if any settings are redefined in `local.yml`, the values from\n`default.yml` are overwritten by `local.yml`.\n\nEnvironment variables will apply after the `local.yml` overwrite of the config settings if they have a matching name. To\ndo so, the environment variable must be named in the following way:\n\n> `{APP_NAME_ALL_CAPS}_{SECTION}_{SETTING}`\n\nSo for the application `my-small-project` if we wanted to overwrite the setting `port` from the section `app`, your\nenvironment variable would need to be named like this:\n\n> `MY_SMALL_PROJECT_APP_PORT`\n\nIt is also possible to have nested sections, so following the example above, if you wanted to override the value of\n`api.weather.host` you could do so using the following environment variable:\n\n> `MY_SMALL_PROJECT_API_WEATHER_HOST`\n\n![Order](https://github.com/ElementAI/opset/raw/master/doc/setup_config_overwrite_order.png)\n\n### Loading the config for unit tests\n\nOpset provides a specific function to load the config when performing unit testing that provides the\ndeveloper with some additional tool to better handle the reality of unit testing. When initializing the config for\nunit tests, the content of the default config is loaded first, and if the `unit_test.yml` file is present and has\nvalues, the values from `default.yml` are overwritten by `unit_test.yml`. Then the values from the environment variables\napply and if you need some config values to be specific to your unit tests you have the option to pass config values\nwhen loading the unit tests that will overwrite all other sources.\n\n![Order](https://github.com/ElementAI/opset/raw/master/doc/setup_config_unit_test_overwrite_order.png)\n\n### Safeguards\n\nThere are two safeguards in the code to try to prevent developer mistakes.\n\n#### Settings not declared in `default.yml` are not loaded\n\nYour `default.yml` is what defines what can be tweaked in your application, it is made to be the one place to look at if\nyou are wondering what can be changed in the configuration of your application.\n\nWhen loading the configuration a warning will be raised if a setting is detected from the local config, environment\nvariables or unit tests values that is not present in `default.yml`. This means that if your `local.yml`\nconfig looks like this:\n\n```\napp:\n  host: 127.0.0.1\n  port: 7777\n  ham_level: 7\n  api_key: 332d5c3e-a7a3-41db-aa5c-c0dfbac8f3d2\n```\n\nAnd your default config looks like this:\n\n```\napp:\n  host: 127.0.0.1\n  port: 7777\n  debug: False\n  api_key: null\n```\n\nA warning will be issued when the config is loaded because the setting `ham_level` from the section `app` is not known to\nthe default config. The setting and value of `ham_level` will not be loaded in the config and will not be usable in the\napplication if it\'s not present in `default.yml`. As per the example above, you are not forced to set a value for\nsettings in the default config (see `api_key`), but the setting needs to be there.\n\n#### Forcing all default settings to have values\n\nThere is a special flag called `critical_settings` that is passed to the function `setup_config` from the module.\nThis flag is set to `True` by default and will make Opset raise an error if there is no\nvalue defined for a setting in `default.yml` after having applied all possible configuration files and environment\nvariables.\n\n## Usage Guide\n\nYou interact with the library through the function `opset.setup_config` to set up the config and with the\nsingleton object `opset.config` to read config values. Optionally Opset can also manage your\napplication logging via the function `opset.load_logging_config` or the argument `setup_logging` from the\nfunction `opset.setup_config`. The `opset.config` object is a singleton which means that no matter where\nit is accessed in the code and the loading order, as long as it has been initiated with `opset.setup_config` it\nwill hold the same configuration values in all of your application.\n\nThe library expects that your project will contain [YAML](https://yaml.org/) files named `default.yml` and\n(optionally) `local.yml` and `unit_test.yml`. You will be able to point to the location of those config files when\ninvoking `opset.setup_config` as the second positional argument. The file `default.yml` should be committed and follow your\nproject and should not contain any secrets. The files `local.yml` and `unit_test.yml` should be added to your\n`.gitignore` to avoid having them committed by accident as those files can contain secrets.\n\nThe `opset.setup_config` function will handle everything from reading the YAML file containing your project\'s config values,\nto loading them into your environment being mindful not to overwrite ENV variables already present. It needs to be\npassed the name of your application along with the python style path (eg. `module.submodule`) to where the\n`default.yml`, `local.yml` or `unit_test.yml` files are located in the project.\n\nTo initialize the configuration, use the function `opset.setup_config` and that\'s it. After that you can import\nthe variable `opset.config` from the module to use the config. You can safely import the config variable before\ninitializing it because access to the config object attributes is dynamic. It is important to note that the config is\nbuilt to be read-only, it gets populated when `opset.setup_config` and from then on you just read the values from\nthe config as needed in your implementation.\n\nThe function setup_config takes the following arguments:\n\n| Parameter | Description | Default value | Example\n| --- | --- | --- | --- |\n| `app_name` | The name of the application, usually the name of the repo. Ex: `myproject-example`. This will be used for finding the prefix to the environment variables. The name of the app will be uppercased and dashes will be replaced by underscores. | | `myproject-example` |\n| `config_path` | A python path to where the configuration files are. Relative to the application. Ex: `tasks.config` would mean that the config files are located in the directory config of the directory tasks from the root of the repo. | | `tasks.config` |\n| `critical_settings` | A boolean to specify how null settings in `default.yml` should be handled. If set to `True`, the function will raise an exception when a key in `default.yml` is not defined in `local.yml` or in an environment variable. | `True` | `True` |\n| `setup_logging` | Whether the logging config should be loaded immediately after the config has been loaded. Default to `True`. | `True` | `True` |\n\n### Making the difference between null and empty\n\nThe configuration is stored in YAML and follows the YAML standard. As such, it makes a distinction between `null` keys\nand empty keys. \n\n```\napp:\n  # this setting\'s value is declared but not defined\n  # it will be set to None when accessed unless it is overwritten in local.yml or in an environment variable\n  api_key: null\n  # this setting\'s value is set to an empty string\n  log_prefix: \n```\n\n### Controlling your entry points\n\nThe config object is initiated once you call the function `opset.setup_config`, before that, trying to get read\na value from the config will throw an exception. It is very important to have a good idea of what the entry points\nare in your application and to call `opset.setup_config` as early as possible in your application to avoid issues.\n\nTo avoid duplicating calls to `opset.setup_config` we recommend you add the call to `opset.setup_config`\nin a function that is called whenever you need to start your application, you can then safely call this function\nwhenever you create a new entry points in your application.\n\nBe mindful about reading values from the config object at module level. If you need to import modules before you can\ncall `opset.setup_config` and one of those modules has a module-level call to read the config, Opset\nwill raise an error when importing because the code will be read at import time and the config will not have been\ninitiated.\n\nFor a more concrete example, avoid doing something like this:\n\n```python\nfrom opset import config\n\nFULL_DB_URI = f"{config.db.scheme}{config.db.user}:{config.db.password}@{config.db.host}:{config.db.port}"\n```\n\nAnd do something like this instead:\n\n```python\nfrom opset import config\n\ndef get_full_db_uri():\n    return f"{config.db.scheme}{config.db.user}:{config.db.password}@{config.db.host}:{config.db.port}"\n```\n\nLast thing, remember that it is safe to import the config object before the config has been initiated. The config\nobject is a singleton and will be populated after `opset.setup_config` has been called, even if it was imported\nfirst.\n\n## Example Of Usage\n\nHere is a little example of how to use the opset features in a simple Flask app.\n\n```python\nfrom flask import Flask, jsonify\nfrom opset import config, setup_config\n\n\nsetup_config("myproject-example", "myproject-example.config")\n \napp = Flask(config.app.name)\n\n@app.route("/")\ndef hello():\n    return jsonify({"Hello and welcome to": config.app.welcome_message})\n```\n\nThis example will leverage the config values stored under the `myproject-example/config` folder, with the following content:\n\n```yaml\napp:\n  welcome_message: Hi lads\n```\n\n### Opset + Environment Variables\n\nOne of the features of Opset is how it handles the interaction between the config values in your projects\' YAML\nfiles and the values that might already be set in your environment. Values already in your environment have higher\npriority and will overwrite any values in your config files. In order to compare against the environment variables,\nOpset builds the names for config values using `<APP_NAME>_<SECTION_NAME>_<SETTING_NAME>` as a template.\nThis means that if your environment contains the value `MYPROJECT_EXAMPLE_DATABASE_HOST`, and your application is named\n`myproject-example` it will overwrite the value of the database host from the following config file:\n\n```yaml\ndatabase:\n  host: 89.22.102.02\n```\n\nThe conversion to python types from the YAML config file is handled by `pyyaml` but for environment variables\nOpset does its own conversion depending on the value:\n\n- `true`, `t`, `yes`, `y` (case-insensitive) will be converted to a `True` `bool`\n- `false`, `f`, `no`, `n` (case-insensitive) will be converted to a `False` `bool`\n- Any number-only string will be converted to an `int` if they have no decimals and `float` if they do\n- A JSON-valid array will be converted to a `list`\n- A JSON-valid object will be converted to a `dict`\n- Any other value will remain a `str`\n\nNOTE: Be sure to respect JSON conventions when defining arrays and objects, use lower-case booleans, double quotes, etc.\n\n## Example Configuration file\n\n### default.yml\n\nDeclare in the `default.yml` file all the settings that the app will require. For each of the keys,\nyou can define a default value. If there is no sensible defaults for a setting, leave it blank (which\nis equivalent to setting it to `null`).\n\nAs a rule of thumb, a default value should be equally good and safe for local, staging or prod environments.\nFor example, setting `app.debug` above to `True` would be an error as it may cause prod to run with debug\nmessages enabled if prod is not overriding it. The opposite is also true. A default value pointing to a production\nsystem can easily wipe or overload it during testing if tests do not overwrite the defaults properly. When in doubt,\nprefer a `null` value.\n\nAlso, secrets should _NEVER_ be added to this file.\n\n### local.yml\n\nThis file is typically defined by developers for their own development and local usage of the app. This file\nmay contain secrets and as such it must be added to the `.gitignore` file.\n\n### unit_test.yml\n\nThis file is used to handle configuration values when running unit tests locally by developers. The content of this\nfile is only used when initiating the config through `opset.setup_unit_test_config` and is discussed in more\ndetails in the section of the documentation dedicated to unit testing. This file may contain secrets and as such it\nmust be added to the `.gitignore` file.\n\n### Example Logging Configuration values\n\nOpset also provides functionality for configuring the logging handlers for your project, this uses\n`structlog` in the background. This is provided through the aforementioned `load_logging_config` function. If you\nchoose to use this functionality, you will need to add some more values to your configuration files, and you can find\nan example of such values here:\n\n```yaml\nlogging:\n  date_format: "iso"  # strftime-valid date format, e.g.: "%Y-%M-%d", or "iso" to use the standard ISO format\n  use_utc: True  # Use UTC timezone if true, or local otherwise\n  min_level: DEBUG  # Minimum level to display log for\n  colors: False  # Use colors for log display, defaults to False\n  disable_processors: False  # Disables log processors (additional info at the end of the log record)\n  logger_overrides:  # overwrite min log level of third party loggers\n    googleapiclient: ERROR\n  json_format: False  # Whether the logs should be formatted as json. Defaults to False.\n```\n\n### Log Processors\n\nSince we are using `structlog` you can use the Processor feature to add additional info to your log records, this\ncan be useful to add a request ID, or the hostname of the machine to all your log records without having to pass\nanything to your logging calls.\n\nTo use this simply define any processors you want by inheriting from the `BaseProcessor` class of `opset`\nand pass an instance to the `load_logging_config` call:\n\n```python\nimport logging\n\nfrom flask import Flask\nfrom opset import BaseProcessor, load_logging_config, setup_config\n\nfrom my_app.request_context import get_request_id\n\n\nclass RequestContextProcessor(BaseProcessor):\n    def __call__(self, logger, name, event_dict):\n        event_dict["request_id"] = get_request_id()\n        return event_dict\n\n\nsetup_config("my_app", "my_app.config", setup_logging=False)  # Defer the logging setup\nload_logging_config(custom_processors=[RequestContextProcessor()])  # Pass your custom processors\n\napp = Flask(__name__)\n\n@app.route("/")\ndef root():\n    logging.info("This will include the request ID!")\n    return "OK"\n```\n\nA processor receives the logger object, the logger name and most importantly the `event_dict` which contains all the\ninfo of the log record. So simply add to the `event_dict` in your processor and return it.\n\nIn local development processors can add some unnecessary noise to the log output, so they can be disabled by setting\n`logging.disable_processors` to `True` in your `local.yml`.\n\nBy default, Opset enables the built-in `HostNameProcessor`, which adds the machine hostname to log records.\nIt can be disabled by passing `use_hostname_processor=False` in the `load_logging_config` call.\n\n### Log Handlers\n\nSince we are using python\'s `logging` library, you can use custom log handlers to customize how and where the\ninformation is logged when using the logger.\n\nTo use this simply define any log handlers you want by inheriting from the `Handler` class of `logging` and overwriting\nthe `emit` method, and pass an instance to the `load_logging_config` call:\n\n```python\nimport logging\n\nfrom flask import Flask\nfrom opset import load_logging_config, setup_config\nfrom logging import Handler\nimport json\n\nclass LocalFileHandler(Handler):\n    def __init__(self):\n        Handler.__init__(self)\n\n    def emit(self, record):\n        """\n        Will log the record in the root log.json file\n        """\n        with open("log.json", "w") as fp:\n            json.dump(record.msg, fp)\n\n\nsetup_config("my_app", "my_app.config", setup_logging=False)  # Defer the logging setup\nload_logging_config(custom_handlers=[LocalFileHandler()])  # Pass your custom handlers\n\napp = Flask(__name__)\n\n@app.route("/")\ndef root():\n    logging.info("Log me in a local file!")\n    return "OK"\n```\n\nThe handler receives the record object, containing all the log information that was processed by the\nprocessors. The handler can chose what to do with that information, should it be to log it in a local file,\nsend it to a blob storage, send it to an external tool (ex: Sentry)\n\n## Support for unit tests\n\nOpset support unit testing to make sure you can handle the special cases that may come up in your\napplication configuration during unit testing.\n\n### setup_unit_test_config\n\nThe function `opset.setup_unit_test_config` is made to replace `opset.setup_config` when running unit\ntests. Remember to control your entry points and call this function as early as possible when running the unit tests.\nIf you are using pytest it is recommended to add it to a\n[conftest.py](https://docs.pytest.org/en/2.7.3/plugins.html?highlight=re#conftest-py-plugins) module set at the root of\nyour unit tests package.\n\n`opset.setup_unit_test_config` works in the same way as `opset.setup_config` but will load the YAML\nconfig file `unit_test.yml` if present instead of `local.yml`. It also accepts an additional parameter called\n`config_values` that is a dictionary representation of a config file that will have the highest priority when doing\noverwrites.\n\n| Parameter | Description | Default value | Example\n| --- | --- | --- | --- |\n| `app_name` | The name of the application, usually the name of the repo. Ex: myproject-example. This will be used for finding the prefix to the environment variables. The name of the app will be uppercased and dashes will be replaced by underscores. | | `myproject-example` |\n| `config_path` | A python path to where the configuration files are. Relative to the application. Ex: `tasks.config` would mean that the config files are located in the directory config of the directory tasks from the root of the repo. | | `tasks.config` |\n| `config_values` | A dictionary mimicking the structure of the config files, to be applied as an overwrite on top of default + unit_test config (if available) and env variables. | | `{"app": {"debug": False}}` |\n\n#### Usage example of setup_unit_test_config\n\nIn `default.yml`:\n\n```yaml\ndb:\n  user: \n  password:\n  name: staging\n```\n\nIn `unit_test.yml`:\n\n```yaml\ndb:\n  user: serge\n  password: mystrongpassword\n```\n\nIn the `conftest.py` module a the root of your unit tests package:\n\n```python\nfrom opset import config, setup_unit_test_config\n\nsetup_unit_test_config("myproject-example", "myproject-example.config", config_values={"db": {"name": "test"}})\n```\n\nAfter running `opset.setup_unit_test_config` the config will hold the following values:\n\n```\n>>> config.db.user\n\'serge\'\n\n>>> config.db.password\n\'mystrongpassword\'\n\n>>> config.db.name\n\'test\' \n```\n\n### mock_config\n\nThe function `opset.mock_config` is a context manager that lets you overwrite config values from the config\nobject for the time of a unit tests. If your unit test requires for the time of a test to have your config hold a\nspecial temporary value, `opset.mock_config` is there for you. It takes the parameter `config_values` which\nis identical to what `opset.setup_unit_test_config` uses.\n\nYour config object will be duplicated for the duration of your context manager and overwritten by the values you send\nto the parameter `config_values`. Once you exit the context manager the copy of the config disappears and your\napplication resumes with the config object being in the same state as it was before entering the context manager.\n\n#### Usage example of mock_config\n\nIn your module to be tested:\n\n```python\nfrom opset import config\n\ndef is_admin(user_name: str) -> bool:\n    return user_name in config.app.admin_list\n```\n\nIn your `default.yml`:\n```yaml\napp:\n  admin_list: \n```\n\nIn your `unit_test.yml`:\n```yaml\napp:\n  admin_list:\n    - "jotaro kujo"\n```\n\nIn your unit test module:\n```python\nfrom opset import mock_config\n\nfrom my_package.my_module import is_admin\n\n\ndef test_is_admin():\n    # Test true\n    assert is_admin("jotaro kujo")\n    \n    # Test false\n    with mock_config(config_values={"app": {"admin_list": []}}):\n        assert not is_admin("jotaro kujo")\n```\n\n\n## Contributing and getting set up for local development\n\nTo set yourself up for development on Opset, make sure you are using\n[poetry](https://poetry.eustace.io/docs/) and simply run the following commands from the root directory:\n\n```bash\nmake bootstrap\nmake install\n```\n',
-    'author': 'Element AI Inc.',
-    'author_email': 'hello@elementai.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ElementAI/opset',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+A library for simplifying the configuration of Python applications at all stages of deployment.
 
+Opset is a config manager that let you manage your configuration via YAML file or environment variables.
+The general principle of Opset is that you want to hold your secrets and manage your configurations via
+configuration files when doing local development and via environment variables when your app is deployed. It is however
+possible to also handle local development through environment variables if the developer sees fit.
+
+With Opset you define everything that can be tweaked with your application in one specific
+file (`default.yml`). This way the developers and integrators working with your code will know exactly what setting they
+can change on your code base. You can then overwrite the default config with a local config stored in a file called
+`local.yml`, this file is aimed to be used for local development by your developers and let them easily manage a
+configuration file that fits their development need. Finally, you can also have environment variables that have a
+matching name to your config that will overwrite your config, letting you use your config in a deployed environment
+without having your secret written down in a config file. Opset aims to reconcile the ease of use of a
+config file with the added security of environment variables.
+
+This library is available on PyPI under the name Opset. You can install with pip by running `pip install opset`.
+
+# Table of Contents
+
+1. [Lexicon](#lexicon)
+1. [Architecture Overview](#architecture-overview)
+    1. [Loading the config for unit tests](#loading-the-config-for-unit-tests)
+    1. [Safeguards](#safeguards)
+        1. [Settings not declared in default.yml are not loaded](#settings-not-declared-in-defaultyml-are-not-loaded)
+        1. [Forcing all default settings to have values](#forcing-all-default-settings-to-have-values)
+1. [Usage Guide](#usage-guide)
+    1. [Making the difference between null and empty](#making-the-difference-between-null-and-empty)
+1. [Example of Usage](#example-of-usage)
+    1. [Opset + Environment Variables](#Opset--environment-variables)
+    1. [Naming your config sections](#naming-your-config-sections)
+    1. [Controlling your entry points](#controlling-your-entry-points)
+1. [Example Configuration file](#example-configuration-file)
+    1. [default.yml](#defaultyml)
+    1. [local.yml](#localyml)
+    1. [unit_test.yml](#unit_testyml)
+    1. [Example Logging Configuration values](#example-logging-configuration-values)
+    1. [Log Processors](#log-processors)
+1. [Support for unit tests](#support-for-unit-tests)
+    1. [setup_unit_test_config](#setup_unit_test_config)
+        1. [Usage example of setup_unit_test_config](#usage-example-of-setup_unit_test_config)
+    1. [mock_config](#mock_config)
+        1. [Usage example of mock_config](#usage-example-of-mock_config)
+1. [Contributing and getting set up for local development](#contributing-and-getting-set-up-for-local-development)
+
+## Lexicon
+
+| Term | Definition |
+|--- | --- |
+| config |	A configuration file (format: YAML). |
+| section	| A section within a configuration file, a section tend to group different settings together under a logical block. For example a section named redis would encompass all settings related specifically to redis. |
+| setting	| A key within a section in a configuration file. A value is associated with a key and querying the config for a setting within a section will return the value associated with it. |
+
+![Lexicon](https://github.com/ElementAI/opset/raw/master/doc/lexicon.png)
+
+## Architecture Overview
+
+There are three possible config files
+
+| Config Name | Purpose |
+| --- | --- |
+| default.yml | This is the base config, `default.yml` needs to have the declaration of all sections and settings. |
+| local.yml | This is a local config that overwrites the default config, this file is not committed to the repository and is meant to be used in a local development environment. |
+| unit_test.yml | This is a local config that overwrites the default config during unit tests, this file is not committed to the repository and is meant to be used in a local development environment. When the config is initialized for unit tests, if a `unit_test.yml` file is present it will be loaded, otherwise the environment variables will be loaded on top of the default config. |
+
+The content of the default config is loaded first, and if any settings are redefined in `local.yml`, the values from
+`default.yml` are overwritten by `local.yml`.
+
+Environment variables will apply after the `local.yml` overwrite of the config settings if they have a matching name. To
+do so, the environment variable must be named in the following way:
+
+> `{APP_NAME_ALL_CAPS}_{SECTION}_{SETTING}`
+
+So for the application `my-small-project` if we wanted to overwrite the setting `port` from the section `app`, your
+environment variable would need to be named like this:
+
+> `MY_SMALL_PROJECT_APP_PORT`
+
+It is also possible to have nested sections, so following the example above, if you wanted to override the value of
+`api.weather.host` you could do so using the following environment variable:
+
+> `MY_SMALL_PROJECT_API_WEATHER_HOST`
+
+![Order](https://github.com/ElementAI/opset/raw/master/doc/setup_config_overwrite_order.png)
+
+### Loading the config for unit tests
+
+Opset provides a specific function to load the config when performing unit testing that provides the
+developer with some additional tool to better handle the reality of unit testing. When initializing the config for
+unit tests, the content of the default config is loaded first, and if the `unit_test.yml` file is present and has
+values, the values from `default.yml` are overwritten by `unit_test.yml`. Then the values from the environment variables
+apply and if you need some config values to be specific to your unit tests you have the option to pass config values
+when loading the unit tests that will overwrite all other sources.
+
+![Order](https://github.com/ElementAI/opset/raw/master/doc/setup_config_unit_test_overwrite_order.png)
+
+### Safeguards
+
+There are two safeguards in the code to try to prevent developer mistakes.
+
+#### Settings not declared in `default.yml` are not loaded
+
+Your `default.yml` is what defines what can be tweaked in your application, it is made to be the one place to look at if
+you are wondering what can be changed in the configuration of your application.
+
+When loading the configuration a warning will be raised if a setting is detected from the local config, environment
+variables or unit tests values that is not present in `default.yml`. This means that if your `local.yml`
+config looks like this:
+
+```
+app:
+  host: 127.0.0.1
+  port: 7777
+  ham_level: 7
+  api_key: 332d5c3e-a7a3-41db-aa5c-c0dfbac8f3d2
+```
+
+And your default config looks like this:
+
+```
+app:
+  host: 127.0.0.1
+  port: 7777
+  debug: False
+  api_key: null
+```
+
+A warning will be issued when the config is loaded because the setting `ham_level` from the section `app` is not known to
+the default config. The setting and value of `ham_level` will not be loaded in the config and will not be usable in the
+application if it's not present in `default.yml`. As per the example above, you are not forced to set a value for
+settings in the default config (see `api_key`), but the setting needs to be there.
+
+#### Forcing all default settings to have values
+
+There is a special flag called `critical_settings` that is passed to the function `setup_config` from the module.
+This flag is set to `True` by default and will make Opset raise an error if there is no
+value defined for a setting in `default.yml` after having applied all possible configuration files and environment
+variables.
+
+## Usage Guide
+
+You interact with the library through the function `opset.setup_config` to set up the config and with the
+singleton object `opset.config` to read config values. Optionally Opset can also manage your
+application logging via the function `opset.load_logging_config` or the argument `setup_logging` from the
+function `opset.setup_config`. The `opset.config` object is a singleton which means that no matter where
+it is accessed in the code and the loading order, as long as it has been initiated with `opset.setup_config` it
+will hold the same configuration values in all of your application.
+
+The library expects that your project will contain [YAML](https://yaml.org/) files named `default.yml` and
+(optionally) `local.yml` and `unit_test.yml`. You will be able to point to the location of those config files when
+invoking `opset.setup_config` as the second positional argument. The file `default.yml` should be committed and follow your
+project and should not contain any secrets. The files `local.yml` and `unit_test.yml` should be added to your
+`.gitignore` to avoid having them committed by accident as those files can contain secrets.
+
+The `opset.setup_config` function will handle everything from reading the YAML file containing your project's config values,
+to loading them into your environment being mindful not to overwrite ENV variables already present. It needs to be
+passed the name of your application along with the python style path (eg. `module.submodule`) to where the
+`default.yml`, `local.yml` or `unit_test.yml` files are located in the project.
+
+To initialize the configuration, use the function `opset.setup_config` and that's it. After that you can import
+the variable `opset.config` from the module to use the config. You can safely import the config variable before
+initializing it because access to the config object attributes is dynamic. It is important to note that the config is
+built to be read-only, it gets populated when `opset.setup_config` and from then on you just read the values from
+the config as needed in your implementation.
+
+The function setup_config takes the following arguments:
+
+| Parameter | Description | Default value | Example
+| --- | --- | --- | --- |
+| `app_name` | The name of the application, usually the name of the repo. Ex: `myproject-example`. This will be used for finding the prefix to the environment variables. The name of the app will be uppercased and dashes will be replaced by underscores. | | `myproject-example` |
+| `config_path` | A python path to where the configuration files are. Relative to the application. Ex: `tasks.config` would mean that the config files are located in the directory config of the directory tasks from the root of the repo. | | `tasks.config` |
+| `critical_settings` | A boolean to specify how null settings in `default.yml` should be handled. If set to `True`, the function will raise an exception when a key in `default.yml` is not defined in `local.yml` or in an environment variable. | `True` | `True` |
+| `setup_logging` | Whether the logging config should be loaded immediately after the config has been loaded. Default to `True`. | `True` | `True` |
+
+### Making the difference between null and empty
+
+The configuration is stored in YAML and follows the YAML standard. As such, it makes a distinction between `null` keys
+and empty keys. 
+
+```
+app:
+  # this setting's value is declared but not defined
+  # it will be set to None when accessed unless it is overwritten in local.yml or in an environment variable
+  api_key: null
+  # this setting's value is set to an empty string
+  log_prefix: 
+```
+
+### Controlling your entry points
+
+The config object is initiated once you call the function `opset.setup_config`, before that, trying to get read
+a value from the config will throw an exception. It is very important to have a good idea of what the entry points
+are in your application and to call `opset.setup_config` as early as possible in your application to avoid issues.
+
+To avoid duplicating calls to `opset.setup_config` we recommend you add the call to `opset.setup_config`
+in a function that is called whenever you need to start your application, you can then safely call this function
+whenever you create a new entry points in your application.
+
+Be mindful about reading values from the config object at module level. If you need to import modules before you can
+call `opset.setup_config` and one of those modules has a module-level call to read the config, Opset
+will raise an error when importing because the code will be read at import time and the config will not have been
+initiated.
+
+For a more concrete example, avoid doing something like this:
+
+```python
+from opset import config
+
+FULL_DB_URI = f"{config.db.scheme}{config.db.user}:{config.db.password}@{config.db.host}:{config.db.port}"
+```
+
+And do something like this instead:
+
+```python
+from opset import config
+
+def get_full_db_uri():
+    return f"{config.db.scheme}{config.db.user}:{config.db.password}@{config.db.host}:{config.db.port}"
+```
+
+Last thing, remember that it is safe to import the config object before the config has been initiated. The config
+object is a singleton and will be populated after `opset.setup_config` has been called, even if it was imported
+first.
+
+## Example Of Usage
+
+Here is a little example of how to use the opset features in a simple Flask app.
+
+```python
+from flask import Flask, jsonify
+from opset import config, setup_config
+
+
+setup_config("myproject-example", "myproject-example.config")
+ 
+app = Flask(config.app.name)
+
+@app.route("/")
+def hello():
+    return jsonify({"Hello and welcome to": config.app.welcome_message})
+```
+
+This example will leverage the config values stored under the `myproject-example/config` folder, with the following content:
+
+```yaml
+app:
+  welcome_message: Hi lads
+```
+
+### Opset + Environment Variables
+
+One of the features of Opset is how it handles the interaction between the config values in your projects' YAML
+files and the values that might already be set in your environment. Values already in your environment have higher
+priority and will overwrite any values in your config files. In order to compare against the environment variables,
+Opset builds the names for config values using `<APP_NAME>_<SECTION_NAME>_<SETTING_NAME>` as a template.
+This means that if your environment contains the value `MYPROJECT_EXAMPLE_DATABASE_HOST`, and your application is named
+`myproject-example` it will overwrite the value of the database host from the following config file:
+
+```yaml
+database:
+  host: 89.22.102.02
+```
+
+The conversion to python types from the YAML config file is handled by `pyyaml` but for environment variables
+Opset does its own conversion depending on the value:
+
+- `true`, `t`, `yes`, `y` (case-insensitive) will be converted to a `True` `bool`
+- `false`, `f`, `no`, `n` (case-insensitive) will be converted to a `False` `bool`
+- Any number-only string will be converted to an `int` if they have no decimals and `float` if they do
+- A JSON-valid array will be converted to a `list`
+- A JSON-valid object will be converted to a `dict`
+- Any other value will remain a `str`
+
+NOTE: Be sure to respect JSON conventions when defining arrays and objects, use lower-case booleans, double quotes, etc.
+
+## Example Configuration file
+
+### default.yml
+
+Declare in the `default.yml` file all the settings that the app will require. For each of the keys,
+you can define a default value. If there is no sensible defaults for a setting, leave it blank (which
+is equivalent to setting it to `null`).
+
+As a rule of thumb, a default value should be equally good and safe for local, staging or prod environments.
+For example, setting `app.debug` above to `True` would be an error as it may cause prod to run with debug
+messages enabled if prod is not overriding it. The opposite is also true. A default value pointing to a production
+system can easily wipe or overload it during testing if tests do not overwrite the defaults properly. When in doubt,
+prefer a `null` value.
+
+Also, secrets should _NEVER_ be added to this file.
+
+### local.yml
+
+This file is typically defined by developers for their own development and local usage of the app. This file
+may contain secrets and as such it must be added to the `.gitignore` file.
+
+### unit_test.yml
+
+This file is used to handle configuration values when running unit tests locally by developers. The content of this
+file is only used when initiating the config through `opset.setup_unit_test_config` and is discussed in more
+details in the section of the documentation dedicated to unit testing. This file may contain secrets and as such it
+must be added to the `.gitignore` file.
+
+### Example Logging Configuration values
+
+Opset also provides functionality for configuring the logging handlers for your project, this uses
+`structlog` in the background. This is provided through the aforementioned `load_logging_config` function. If you
+choose to use this functionality, you will need to add some more values to your configuration files, and you can find
+an example of such values here:
+
+```yaml
+logging:
+  date_format: "iso"  # strftime-valid date format, e.g.: "%Y-%M-%d", or "iso" to use the standard ISO format
+  use_utc: True  # Use UTC timezone if true, or local otherwise
+  min_level: DEBUG  # Minimum level to display log for
+  colors: False  # Use colors for log display, defaults to False
+  disable_processors: False  # Disables log processors (additional info at the end of the log record)
+  logger_overrides:  # overwrite min log level of third party loggers
+    googleapiclient: ERROR
+  json_format: False  # Whether the logs should be formatted as json. Defaults to False.
+```
+
+### Log Processors
+
+Since we are using `structlog` you can use the Processor feature to add additional info to your log records, this
+can be useful to add a request ID, or the hostname of the machine to all your log records without having to pass
+anything to your logging calls.
+
+To use this simply define any processors you want by inheriting from the `BaseProcessor` class of `opset`
+and pass an instance to the `load_logging_config` call:
+
+```python
+import logging
+
+from flask import Flask
+from opset import BaseProcessor, load_logging_config, setup_config
+
+from my_app.request_context import get_request_id
+
+
+class RequestContextProcessor(BaseProcessor):
+    def __call__(self, logger, name, event_dict):
+        event_dict["request_id"] = get_request_id()
+        return event_dict
+
+
+setup_config("my_app", "my_app.config", setup_logging=False)  # Defer the logging setup
+load_logging_config(custom_processors=[RequestContextProcessor()])  # Pass your custom processors
+
+app = Flask(__name__)
+
+@app.route("/")
+def root():
+    logging.info("This will include the request ID!")
+    return "OK"
+```
+
+A processor receives the logger object, the logger name and most importantly the `event_dict` which contains all the
+info of the log record. So simply add to the `event_dict` in your processor and return it.
+
+In local development processors can add some unnecessary noise to the log output, so they can be disabled by setting
+`logging.disable_processors` to `True` in your `local.yml`.
+
+By default, Opset enables the built-in `HostNameProcessor`, which adds the machine hostname to log records.
+It can be disabled by passing `use_hostname_processor=False` in the `load_logging_config` call.
+
+### Log Handlers
+
+Since we are using python's `logging` library, you can use custom log handlers to customize how and where the
+information is logged when using the logger.
+
+To use this simply define any log handlers you want by inheriting from the `Handler` class of `logging` and overwriting
+the `emit` method, and pass an instance to the `load_logging_config` call:
+
+```python
+import logging
+
+from flask import Flask
+from opset import load_logging_config, setup_config
+from logging import Handler
+import json
+
+class LocalFileHandler(Handler):
+    def __init__(self):
+        Handler.__init__(self)
+
+    def emit(self, record):
+        """
+        Will log the record in the root log.json file
+        """
+        with open("log.json", "w") as fp:
+            json.dump(record.msg, fp)
+
+
+setup_config("my_app", "my_app.config", setup_logging=False)  # Defer the logging setup
+load_logging_config(custom_handlers=[LocalFileHandler()])  # Pass your custom handlers
+
+app = Flask(__name__)
+
+@app.route("/")
+def root():
+    logging.info("Log me in a local file!")
+    return "OK"
+```
+
+The handler receives the record object, containing all the log information that was processed by the
+processors. The handler can chose what to do with that information, should it be to log it in a local file,
+send it to a blob storage, send it to an external tool (ex: Sentry)
+
+## Support for unit tests
+
+Opset support unit testing to make sure you can handle the special cases that may come up in your
+application configuration during unit testing.
+
+### setup_unit_test_config
+
+The function `opset.setup_unit_test_config` is made to replace `opset.setup_config` when running unit
+tests. Remember to control your entry points and call this function as early as possible when running the unit tests.
+If you are using pytest it is recommended to add it to a
+[conftest.py](https://docs.pytest.org/en/2.7.3/plugins.html?highlight=re#conftest-py-plugins) module set at the root of
+your unit tests package.
+
+`opset.setup_unit_test_config` works in the same way as `opset.setup_config` but will load the YAML
+config file `unit_test.yml` if present instead of `local.yml`. It also accepts an additional parameter called
+`config_values` that is a dictionary representation of a config file that will have the highest priority when doing
+overwrites.
+
+| Parameter | Description | Default value | Example
+| --- | --- | --- | --- |
+| `app_name` | The name of the application, usually the name of the repo. Ex: myproject-example. This will be used for finding the prefix to the environment variables. The name of the app will be uppercased and dashes will be replaced by underscores. | | `myproject-example` |
+| `config_path` | A python path to where the configuration files are. Relative to the application. Ex: `tasks.config` would mean that the config files are located in the directory config of the directory tasks from the root of the repo. | | `tasks.config` |
+| `config_values` | A dictionary mimicking the structure of the config files, to be applied as an overwrite on top of default + unit_test config (if available) and env variables. | | `{"app": {"debug": False}}` |
+
+#### Usage example of setup_unit_test_config
+
+In `default.yml`:
+
+```yaml
+db:
+  user: 
+  password:
+  name: staging
+```
+
+In `unit_test.yml`:
+
+```yaml
+db:
+  user: serge
+  password: mystrongpassword
+```
+
+In the `conftest.py` module a the root of your unit tests package:
+
+```python
+from opset import config, setup_unit_test_config
+
+setup_unit_test_config("myproject-example", "myproject-example.config", config_values={"db": {"name": "test"}})
+```
+
+After running `opset.setup_unit_test_config` the config will hold the following values:
+
+```
+>>> config.db.user
+'serge'
+
+>>> config.db.password
+'mystrongpassword'
+
+>>> config.db.name
+'test' 
+```
+
+### mock_config
+
+The function `opset.mock_config` is a context manager that lets you overwrite config values from the config
+object for the time of a unit tests. If your unit test requires for the time of a test to have your config hold a
+special temporary value, `opset.mock_config` is there for you. It takes the parameter `config_values` which
+is identical to what `opset.setup_unit_test_config` uses.
+
+Your config object will be duplicated for the duration of your context manager and overwritten by the values you send
+to the parameter `config_values`. Once you exit the context manager the copy of the config disappears and your
+application resumes with the config object being in the same state as it was before entering the context manager.
+
+#### Usage example of mock_config
+
+In your module to be tested:
+
+```python
+from opset import config
+
+def is_admin(user_name: str) -> bool:
+    return user_name in config.app.admin_list
+```
+
+In your `default.yml`:
+```yaml
+app:
+  admin_list: 
+```
+
+In your `unit_test.yml`:
+```yaml
+app:
+  admin_list:
+    - "jotaro kujo"
+```
+
+In your unit test module:
+```python
+from opset import mock_config
+
+from my_package.my_module import is_admin
+
+
+def test_is_admin():
+    # Test true
+    assert is_admin("jotaro kujo")
+    
+    # Test false
+    with mock_config(config_values={"app": {"admin_list": []}}):
+        assert not is_admin("jotaro kujo")
+```
+
+
+## Contributing and getting set up for local development
+
+To set yourself up for development on Opset, make sure you are using
+[poetry](https://poetry.eustace.io/docs/) and simply run the following commands from the root directory:
+
+```bash
+make bootstrap
+make install
+```
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

