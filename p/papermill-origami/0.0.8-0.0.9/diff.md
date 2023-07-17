# Comparing `tmp/papermill_origami-0.0.8.tar.gz` & `tmp/papermill_origami-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermill_origami-0.0.8.tar", max compression
+gzip compressed data, was "papermill_origami-0.0.9.tar", max compression
```

## Comparing `papermill_origami-0.0.8.tar` & `papermill_origami-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1516 2022-10-29 04:24:12.537602 papermill_origami-0.0.8/LICENSE
--rw-r--r--   0        0        0     3323 2022-10-29 04:24:12.537602 papermill_origami-0.0.8/README.md
--rw-r--r--   0        0        0      116 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/__init__.py
--rw-r--r--   0        0        0       18 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/_version.py
--rw-r--r--   0        0        0    26133 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/engine.py
--rw-r--r--   0        0        0     3323 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/iorw.py
--rw-r--r--   0        0        0     4863 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/manager.py
--rw-r--r--   0        0        0      834 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/__init__.py
--rw-r--r--   0        0        0    14450 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/assets.py
--rw-r--r--   0        0        0     2818 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/context.py
--rw-r--r--   0        0        0      405 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/engine.py
--rw-r--r--   0        0        0    17852 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/ops.py
--rw-r--r--   0        0        0     2383 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/translator.py
--rw-r--r--   0        0        0      217 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_flytekit/__init__.py
--rw-r--r--   0        0        0     4750 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/noteable_flytekit/tasks.py
--rw-r--r--   0        0        0      934 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/tests/noteable_dagstermill/__init__.py
--rw-r--r--   0        0        0    12543 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/tests/test_engine.py
--rw-r--r--   0        0        0     1079 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/tests/test_iorw.py
--rw-r--r--   0        0        0      684 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/tests/test_papermill_registration.py
--rw-r--r--   0        0        0     1350 2022-10-29 04:24:12.541603 papermill_origami-0.0.8/papermill_origami/util.py
--rw-r--r--   0        0        0     3069 2022-10-29 04:24:12.545603 papermill_origami-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4843 1970-01-01 00:00:00.000000 papermill_origami-0.0.8/setup.py
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 papermill_origami-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3875 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/README.md
+-rw-r--r--   0        0        0      116 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/__init__.py
+-rw-r--r--   0        0        0       18 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/_version.py
+-rw-r--r--   0        0        0    26130 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/engine.py
+-rw-r--r--   0        0        0     3322 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/iorw.py
+-rw-r--r--   0        0        0     4862 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/manager.py
+-rw-r--r--   0        0        0      834 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/__init__.py
+-rw-r--r--   0        0        0    14450 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/assets.py
+-rw-r--r--   0        0        0     2818 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/context.py
+-rw-r--r--   0        0        0      405 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/engine.py
+-rw-r--r--   0        0        0    17852 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/ops.py
+-rw-r--r--   0        0        0     2383 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/translator.py
+-rw-r--r--   0        0        0      217 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_flytekit/__init__.py
+-rw-r--r--   0        0        0     4750 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/noteable_flytekit/tasks.py
+-rw-r--r--   0        0        0        0 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/__init__.py
+-rw-r--r--   0        0        0      932 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/noteable_dagstermill/__init__.py
+-rw-r--r--   0        0        0    12542 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/test_engine.py
+-rw-r--r--   0        0        0     1079 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/test_iorw.py
+-rw-r--r--   0        0        0      684 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/tests/test_papermill_registration.py
+-rw-r--r--   0        0        0     1350 2022-11-02 16:48:14.826987 papermill_origami-0.0.9/papermill_origami/util.py
+-rw-r--r--   0        0        0     3070 2022-11-02 16:48:14.830987 papermill_origami-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 papermill_origami-0.0.9/setup.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 papermill_origami-0.0.9/PKG-INFO
```

### Comparing `papermill_origami-0.0.8/LICENSE` & `papermill_origami-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/engine.py` & `papermill_origami-0.0.9/papermill_origami/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 import nbformat
 import orjson
 from jupyter_client.utils import run_sync
 from nbclient.exceptions import CellExecutionError
 from nbformat import NotebookNode
 from origami.client import NoteableClient, SkipCallback
-from origami.types.files import NotebookFile
-from origami.types.jobs import (
+from origami.defs.files import NotebookFile
+from origami.defs.jobs import (
     CustomerJobDefinitionReferenceInput,
     CustomerJobInstanceReferenceInput,
     JobInstanceAttempt,
     JobInstanceAttemptStatus,
 )
-from origami.types.rtu import (
+from origami.defs.rtu import (
     AppendOutputEventSchema,
     BulkCellStateMessage,
     DisplayHandlerUpdateEventSchema,
     KernelOutput,
     KernelOutputType,
     UpdateOutputCollectionEventSchema,
 )
```

### Comparing `papermill_origami-0.0.8/papermill_origami/iorw.py` & `papermill_origami-0.0.9/papermill_origami/iorw.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from urllib.parse import urlparse
 
 import httpx
 import structlog
 from jupyter_client.utils import run_sync
 from origami.client import NoteableClient
-from origami.types.files import FileVersion
+from origami.defs.files import FileVersion
 
 from papermill_origami.util import parse_noteable_file_id
 
 logger = structlog.get_logger(__name__)
 
 
 def _ensure_client(func):
```

### Comparing `papermill_origami-0.0.8/papermill_origami/manager.py` & `papermill_origami-0.0.9/papermill_origami/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import functools
 from typing import Optional
 
 from jupyter_client.managerabc import KernelManagerABC
 from jupyter_client.utils import run_sync
 from origami.client import NoteableClient
-from origami.types.files import NotebookFile
+from origami.defs.files import NotebookFile
 
 
 class NoteableKernelManager(KernelManagerABC):
     """KernelManager for Noteable client interactions"""
 
     def _requires_client_context(func):
         """A helper for checking if one is in a websocket context or not"""
```

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/__init__.py` & `papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/__init__.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/assets.py` & `papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/assets.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/context.py` & `papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/context.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/ops.py` & `papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/ops.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_dagstermill/translator.py` & `papermill_origami-0.0.9/papermill_origami/noteable_dagstermill/translator.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/noteable_flytekit/tasks.py` & `papermill_origami-0.0.9/papermill_origami/noteable_flytekit/tasks.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/tests/conftest.py` & `papermill_origami-0.0.9/papermill_origami/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from datetime import datetime, timezone
 
 import nbformat.v4
 import pytest
-from origami.types.access_levels import Visibility
-from origami.types.files import FileType, NotebookFile
+from origami.defs.access_levels import Visibility
+from origami.defs.files import FileType, NotebookFile
 
 
 @pytest.fixture
 def file_content():
     return nbformat.v4.new_notebook(cells=[nbformat.v4.new_code_cell("1 + 1") for _ in range(10)])
```

### Comparing `papermill_origami-0.0.8/papermill_origami/tests/test_engine.py` & `papermill_origami-0.0.9/papermill_origami/tests/test_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import uuid
 from datetime import datetime
 from unittest.mock import ANY
 
 import nbformat
 import pytest
-from origami.types.rtu import (
+from origami.defs.rtu import (
     CellStateMessageData,
     KernelOutput,
     KernelOutputContent,
     KernelOutputType,
 )
 from orjson import orjson
```

### Comparing `papermill_origami-0.0.8/papermill_origami/tests/test_iorw.py` & `papermill_origami-0.0.9/papermill_origami/tests/test_iorw.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/tests/test_papermill_registration.py` & `papermill_origami-0.0.9/papermill_origami/tests/test_papermill_registration.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/papermill_origami/util.py` & `papermill_origami-0.0.9/papermill_origami/util.py`

 * *Files identical despite different names*

### Comparing `papermill_origami-0.0.8/pyproject.toml` & `papermill_origami-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "papermill-origami"
-version = "0.0.8"
+version = "0.0.9"
 description = "The noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/papermill-origami"
 # old setup.cfg had a bdist_wheel option.
@@ -30,15 +30,15 @@
 
 [[tool.poetry.source]]
 name = "papermill-origami"
 url = "https://pypi.org"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-noteable-origami = "^0.0.9"
+noteable-origami = "^0.0.11"
 papermill = "^2.4.0"
 dagstermill = {version = "^1.0.5", optional = true}
 cloudpickle = "^2.2.0"
 flytekit = {version = "^1.2.1", optional = true}
 flytekitplugins-papermill = {version = "^1.2.1", optional = true}
 
 [tool.poetry.dev-dependencies]
```

### Comparing `papermill_origami-0.0.8/setup.py` & `papermill_origami-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
  'papermill_origami.tests.noteable_dagstermill']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cloudpickle>=2.2.0,<3.0.0',
- 'noteable-origami>=0.0.9,<0.0.10',
+ 'noteable-origami>=0.0.11,<0.0.12',
  'papermill>=2.4.0,<3.0.0']
 
 extras_require = \
 {'dagster': ['dagstermill>=1.0.5,<2.0.0'],
  'flyte': ['flytekit>=1.2.1,<2.0.0', 'flytekitplugins-papermill>=1.2.1,<2.0.0']}
 
 entry_points = \
 {'papermill.engine': ['noteable = papermill_origami.engine:NoteableEngine'],
  'papermill.io': ['https:// = papermill_origami.iorw:NoteableHandler',
                   'noteable:// = papermill_origami.iorw:NoteableHandler']}
 
 setup_kwargs = {
     'name': 'papermill-origami',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'The noteable API interface',
-    'long_description': '# papermill-origami\nA papermill engine for running Noteable notebooks\n\n<p align="center">\n<a href="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml">\n    <img src="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml/badge.svg" alt="CI" />\n</a>\n<img alt="PyPI - License" src="https://img.shields.io/pypi/l/papermill-origami" />\n<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/papermill-origami" />\n<img alt="PyPI" src="https://img.shields.io/pypi/v/papermill-origami">\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n</p>\n\n---------\n\n[Install](#installation) | [Getting Started](#getting-started) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)\n\n## Requirements\n\nPython 3.8+\n\n## Installation\n\n### Poetry\n\n```shell\npoetry add papermill-origami\n```\n\n\n### Pip\n```shell\npip install papermill-origami\n```\n\n## Getting Started\n\n### API Token\n\nGet your access token from your User Settings -> API Tokens\n\nor alternatively you can generate a post request to generate a new token\n\n```\ncurl -X \'POST\' \\\n  \'https://app.noteable.io/gate/api/v1/tokens\' \\\n  -H \'accept: application/json\' \\\n  -H \'Content-Type: application/json\' \\\n  -d \'{\n  "ttl": 31536000,\n  "name": "my_token"\n}\'\n```\n\n### Engine Registration\n\nThe `noteable` engine keyword will use the following environment variables by default:\n\n```bash\nNOTEABLE_DOMAIN = app.noteable.io\nNOTEABLE_TOKEN = MY_TOKEN_VALUE_HERE\n```\n\nThen the engine is enabled by running papermill as normal. But now you have access to\nthe `noteable://` scheme as well as the ability to tell papermill to use Noteable as\nthe execution location for your notebook.\n\n```python\nimport papermill as pm\n\nfile_id = \'...\'\n\npm.execute_notebook(\n    f\'noteable://{file_id}\',\n    None, # Set no particular output notebook, but a log of the resulting exeuction link still prints\n    # This turns on the Noteable API interface\n    engine_name=\'noteable\', # exclude this kwarg to run the Notebook locally\n)\n```\n\n#### Advanced Setup\n\nFor more advanced control or reuse of a NoteableClient SDK object you can use\nthe async await pattern around a client constructor. This reuses the connection\nthroughout the life cycle of the context block.\n\n```python\nimport papermill as pm\nfrom papermill.iorw import papermill_io\nfrom papermill_origami import ClientConfig, NoteableClient, NoteableHandler \n\n\ndomain = \'app.noteable.io\'\ntoken = MY_TOKEN_VALUE_HERE\nfile_id = \'...\'\n\nasync with NoteableClient(token, config=ClientConfig(domain=domain)) as client:\n    file = await client.get_notebook(file_id)\n    papermill_io.register("noteable://", NoteableHandler(client))\n    pm.execute_notebook(\n        f\'noteable://{file_id}\',\n        None,\n        engine_name=\'noteable\',\n        # Noteable-specific kwargs\n        file=file,\n        client=client,\n    )\n```\n\n## Contributing\n\nSee [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n-------\n\n<p align="center">Open sourced with ❤️ by <a href="https://noteable.io">Noteable</a> for the community.</p>\n\n<img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">\n',
+    'long_description': '# papermill-origami\n    A papermill engine for running Noteable notebooks\n\n<p align="center">\n<a href="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml">\n    <img src="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml/badge.svg" alt="CI" />\n</a>\n<img alt="PyPI - License" src="https://img.shields.io/pypi/l/papermill-origami" />\n<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/papermill-origami" />\n<img alt="PyPI" src="https://img.shields.io/pypi/v/papermill-origami">\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n</p>\n\n---------\n\n[Install](#installation) | [Getting Started](#getting-started) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)\n\n<!-- --8<-- [start:intro] -->\n## Intro to Papermill-Origami\n\nPapermill-Origami is the bridge library between the [Origami Noteable SDK](https://noteable-origami.readthedocs.io/en/latest/) and [Papermill](https://papermill.readthedocs.io/en/latest/). It build a papermill engine that can talk to Noteable APIs to run Notebooks. \n<!-- --8<-- [end:intro] -->\n\n<!-- --8<-- [start:requirements] -->\n## Requirements\n\nPython 3.8+\n<!-- --8<-- [end:requirements] -->\n\n<!-- --8<-- [start:install] -->\n## Installation\n\n### Poetry\n\n```shell\npoetry add papermill-origami\n```\n\n### Pip\n```shell\npip install papermill-origami\n```\n<!-- --8<-- [end:install] -->\n\n<!-- --8<-- [start:start] -->\n## Getting Started\n\n### API Token\n\nGet your access token from your User Settings -> API Tokens\n\nor alternatively you can generate a post request to generate a new token\n\n```\ncurl -X \'POST\' \\\n  \'https://app.noteable.io/gate/api/v1/tokens\' \\\n  -H \'accept: application/json\' \\\n  -H \'Content-Type: application/json\' \\\n  -d \'{\n  "ttl": 31536000,\n  "name": "my_token"\n}\'\n```\n\n### Engine Registration\n\nThe `noteable` engine keyword will use the following environment variables by default:\n\n```bash\nNOTEABLE_DOMAIN = app.noteable.io\nNOTEABLE_TOKEN = MY_TOKEN_VALUE_HERE\n```\n\nThen the engine is enabled by running papermill as normal. But now you have access to\nthe `noteable://` scheme as well as the ability to tell papermill to use Noteable as\nthe execution location for your notebook.\n\n```python\nimport papermill as pm\n\nfile_id = \'...\'\n\npm.execute_notebook(\n    f\'noteable://{file_id}\',\n    None, # Set no particular output notebook, but a log of the resulting exeuction link still prints\n    # This turns on the Noteable API interface\n    engine_name=\'noteable\', # exclude this kwarg to run the Notebook locally\n)\n```\n\n#### Advanced Setup\n\nFor more advanced control or reuse of a NoteableClient SDK object you can use\nthe async await pattern around a client constructor. This reuses the connection\nthroughout the life cycle of the context block.\n\n```python\nimport papermill as pm\nfrom papermill.iorw import papermill_io\nfrom papermill_origami import ClientConfig, NoteableClient, NoteableHandler \n\n\ndomain = \'app.noteable.io\'\ntoken = MY_TOKEN_VALUE_HERE\nfile_id = \'...\'\n\nasync with NoteableClient(token, config=ClientConfig(domain=domain)) as client:\n    file = await client.get_notebook(file_id)\n    papermill_io.register("noteable://", NoteableHandler(client))\n    pm.execute_notebook(\n        f\'noteable://{file_id}\',\n        None,\n        engine_name=\'noteable\',\n        # Noteable-specific kwargs\n        file=file,\n        client=client,\n    )\n```\n<!-- --8<-- [end:start] -->\n\n## Contributing\n\nSee [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n-------\n\n<p align="center">Open sourced with ❤️ by <a href="https://noteable.io">Noteable</a> for the community.</p>\n\n<img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">\n',
     'author': 'Matt Seal',
     'author_email': 'matt@noteable.io',
     'maintainer': 'Matt Seal',
     'maintainer_email': 'matt@noteable.io',
     'url': 'https://github.com/noteable-io/papermill-origami',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,33 +1,38 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['papermill_origami', 'papermill_origami.noteable_dagstermill',
 'papermill_origami.noteable_flytekit', 'papermill_origami.tests',
 'papermill_origami.tests.noteable_dagstermill'] package_data = \ {'': ['*']}
 install_requires = \ ['cloudpickle>=2.2.0,<3.0.0', 'noteable-
-origami>=0.0.9,<0.0.10', 'papermill>=2.4.0,<3.0.0'] extras_require = \
+origami>=0.0.11,<0.0.12', 'papermill>=2.4.0,<3.0.0'] extras_require = \
 {'dagster': ['dagstermill>=1.0.5,<2.0.0'], 'flyte': ['flytekit>=1.2.1,<2.0.0',
 'flytekitplugins-papermill>=1.2.1,<2.0.0']} entry_points = \
 {'papermill.engine': ['noteable = papermill_origami.engine:NoteableEngine'],
 'papermill.io': ['https:// = papermill_origami.iorw:NoteableHandler',
 'noteable:// = papermill_origami.iorw:NoteableHandler']} setup_kwargs =
-{ 'name': 'papermill-origami', 'version': '0.0.8', 'description': 'The noteable
-API interface', 'long_description': '# papermill-origami\nA papermill engine
+{ 'name': 'papermill-origami', 'version': '0.0.9', 'description': 'The noteable
+API interface', 'long_description': '# papermill-origami\n A papermill engine
 for running Noteable notebooks\n\n
  \n\n_[CI]\n\n[PyPI - License]\n[PyPI - Python Version]\n[PyPI]\n[Code_style:
                                    black]\n
 \n\n---------\n\n[Install](#installation) | [Getting Started](#getting-started)
 | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) |
-[Contributing](./CONTRIBUTING.md)\n\n## Requirements\n\nPython 3.8+\n\n##
-Installation\n\n### Poetry\n\n```shell\npoetry add papermill-
-origami\n```\n\n\n### Pip\n```shell\npip install papermill-origami\n```\n\n##
-Getting Started\n\n### API Token\n\nGet your access token from your User
-Settings -> API Tokens\n\nor alternatively you can generate a post request to
-generate a new token\n\n```\ncurl -X \'POST\' \\\n \'https://app.noteable.io/
-gate/api/v1/tokens\' \\\n -H \'accept: application/json\' \\\n -H \'Content-
-Type: application/json\' \\\n -d \'{\n "ttl": 31536000,\n "name":
+[Contributing](./CONTRIBUTING.md)\n\n\n## Intro to Papermill-
+Origami\n\nPapermill-Origami is the bridge library between the [Origami
+Noteable SDK](https://noteable-origami.readthedocs.io/en/latest/) and
+[Papermill](https://papermill.readthedocs.io/en/latest/). It build a papermill
+engine that can talk to Noteable APIs to run Notebooks. \n\n\n\n##
+Requirements\n\nPython 3.8+\n\n\n\n## Installation\n\n###
+Poetry\n\n```shell\npoetry add papermill-origami\n```\n\n### Pip\n```shell\npip
+install papermill-origami\n```\n\n\n\n## Getting Started\n\n### API
+Token\n\nGet your access token from your User Settings -> API Tokens\n\nor
+alternatively you can generate a post request to generate a new
+token\n\n```\ncurl -X \'POST\' \\\n \'https://app.noteable.io/gate/api/v1/
+tokens\' \\\n -H \'accept: application/json\' \\\n -H \'Content-Type:
+application/json\' \\\n -d \'{\n "ttl": 31536000,\n "name":
 "my_token"\n}\'\n```\n\n### Engine Registration\n\nThe `noteable` engine
 keyword will use the following environment variables by default:
 \n\n```bash\nNOTEABLE_DOMAIN = app.noteable.io\nNOTEABLE_TOKEN =
 MY_TOKEN_VALUE_HERE\n```\n\nThen the engine is enabled by running papermill as
 normal. But now you have access to\nthe `noteable://` scheme as well as the
 ability to tell papermill to use Noteable as\nthe execution location for your
 notebook.\n\n```python\nimport papermill as pm\n\nfile_id =
@@ -42,15 +47,15 @@
 papermill_io\nfrom papermill_origami import ClientConfig, NoteableClient,
 NoteableHandler \n\n\ndomain = \'app.noteable.io\'\ntoken =
 MY_TOKEN_VALUE_HERE\nfile_id = \'...\'\n\nasync with NoteableClient(token,
 config=ClientConfig(domain=domain)) as client:\n file = await
 client.get_notebook(file_id)\n papermill_io.register("noteable://",
 NoteableHandler(client))\n pm.execute_notebook(\n f\'noteable://{file_id}\',\n
 None,\n engine_name=\'noteable\',\n # Noteable-specific kwargs\n file=file,\n
-client=client,\n )\n```\n\n## Contributing\n\nSee [CONTRIBUTING.md](./
+client=client,\n )\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md](./
 CONTRIBUTING.md).\n\n-------\n\n
             Open sourced with â¤ï¸ by Noteable for the community.
 \n\n[Boost Data Collaboration with Notebooks]\n', 'author': 'Matt Seal',
 'author_email': 'matt@noteable.io', 'maintainer': 'Matt Seal',
 'maintainer_email': 'matt@noteable.io', 'url': 'https://github.com/noteable-io/
 papermill-origami', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
```

### Comparing `papermill_origami-0.0.8/PKG-INFO` & `papermill_origami-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermill-origami
-Version: 0.0.8
+Version: 0.0.9
 Summary: The noteable API interface
 Home-page: https://github.com/noteable-io/papermill-origami
 License: BSD-3-Clause
 Keywords: notebook,api,noteable
 Author: Matt Seal
 Author-email: matt@noteable.io
 Maintainer: Matt Seal
@@ -23,21 +23,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dagster
 Provides-Extra: flyte
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: dagstermill (>=1.0.5,<2.0.0); extra == "dagster"
 Requires-Dist: flytekit (>=1.2.1,<2.0.0); extra == "flyte"
 Requires-Dist: flytekitplugins-papermill (>=1.2.1,<2.0.0); extra == "flyte"
-Requires-Dist: noteable-origami (>=0.0.9,<0.0.10)
+Requires-Dist: noteable-origami (>=0.0.11,<0.0.12)
 Requires-Dist: papermill (>=2.4.0,<3.0.0)
 Project-URL: Repository, https://github.com/noteable-io/papermill-origami
 Description-Content-Type: text/markdown
 
 # papermill-origami
-A papermill engine for running Noteable notebooks
+    A papermill engine for running Noteable notebooks
 
 <p align="center">
 <a href="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml">
     <img src="https://github.com/noteable-io/papermill-origami/actions/workflows/ci.yaml/badge.svg" alt="CI" />
 </a>
 <img alt="PyPI - License" src="https://img.shields.io/pypi/l/papermill-origami" />
 <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/papermill-origami" />
@@ -45,32 +45,42 @@
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ---------
 
 [Install](#installation) | [Getting Started](#getting-started) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)
 
+<!-- --8<-- [start:intro] -->
+## Intro to Papermill-Origami
+
+Papermill-Origami is the bridge library between the [Origami Noteable SDK](https://noteable-origami.readthedocs.io/en/latest/) and [Papermill](https://papermill.readthedocs.io/en/latest/). It build a papermill engine that can talk to Noteable APIs to run Notebooks. 
+<!-- --8<-- [end:intro] -->
+
+<!-- --8<-- [start:requirements] -->
 ## Requirements
 
 Python 3.8+
+<!-- --8<-- [end:requirements] -->
 
+<!-- --8<-- [start:install] -->
 ## Installation
 
 ### Poetry
 
 ```shell
 poetry add papermill-origami
 ```
 
-
 ### Pip
 ```shell
 pip install papermill-origami
 ```
+<!-- --8<-- [end:install] -->
 
+<!-- --8<-- [start:start] -->
 ## Getting Started
 
 ### API Token
 
 Get your access token from your User Settings -> API Tokens
 
 or alternatively you can generate a post request to generate a new token
@@ -136,14 +146,15 @@
         None,
         engine_name='noteable',
         # Noteable-specific kwargs
         file=file,
         client=client,
     )
 ```
+<!-- --8<-- [end:start] -->
 
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md).
 
 -------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: papermill-origami Version: 0.0.8 Summary: The
+Metadata-Version: 2.1 Name: papermill-origami Version: 0.0.9 Summary: The
 noteable API interface Home-page: https://github.com/noteable-io/papermill-
 origami License: BSD-3-Clause Keywords: notebook,api,noteable Author: Matt Seal
 Author-email: matt@noteable.io Maintainer: Matt Seal Maintainer-email:
 matt@noteable.io Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -10,44 +10,48 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Provides-Extra: dagster
 Provides-Extra: flyte Requires-Dist: cloudpickle (>=2.2.0,<3.0.0) Requires-
 Dist: dagstermill (>=1.0.5,<2.0.0); extra == "dagster" Requires-Dist: flytekit
 (>=1.2.1,<2.0.0); extra == "flyte" Requires-Dist: flytekitplugins-papermill
 (>=1.2.1,<2.0.0); extra == "flyte" Requires-Dist: noteable-origami
-(>=0.0.9,<0.0.10) Requires-Dist: papermill (>=2.4.0,<3.0.0) Project-URL:
+(>=0.0.11,<0.0.12) Requires-Dist: papermill (>=2.4.0,<3.0.0) Project-URL:
 Repository, https://github.com/noteable-io/papermill-origami Description-
 Content-Type: text/markdown # papermill-origami A papermill engine for running
 Noteable notebooks
    [CI] [PyPI - License] [PyPI - Python Version] [PyPI] [Code_style:_black]
 --------- [Install](#installation) | [Getting Started](#getting-started) |
 [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing]
-(./CONTRIBUTING.md) ## Requirements Python 3.8+ ## Installation ### Poetry
-```shell poetry add papermill-origami ``` ### Pip ```shell pip install
-papermill-origami ``` ## Getting Started ### API Token Get your access token
-from your User Settings -> API Tokens or alternatively you can generate a post
-request to generate a new token ``` curl -X 'POST' \ 'https://app.noteable.io/
-gate/api/v1/tokens' \ -H 'accept: application/json' \ -H 'Content-Type:
-application/json' \ -d '{ "ttl": 31536000, "name": "my_token" }' ``` ### Engine
-Registration The `noteable` engine keyword will use the following environment
-variables by default: ```bash NOTEABLE_DOMAIN = app.noteable.io NOTEABLE_TOKEN
-= MY_TOKEN_VALUE_HERE ``` Then the engine is enabled by running papermill as
-normal. But now you have access to the `noteable://` scheme as well as the
-ability to tell papermill to use Noteable as the execution location for your
-notebook. ```python import papermill as pm file_id = '...' pm.execute_notebook
-( f'noteable://{file_id}', None, # Set no particular output notebook, but a log
-of the resulting exeuction link still prints # This turns on the Noteable API
-interface engine_name='noteable', # exclude this kwarg to run the Notebook
-locally ) ``` #### Advanced Setup For more advanced control or reuse of a
-NoteableClient SDK object you can use the async await pattern around a client
-constructor. This reuses the connection throughout the life cycle of the
-context block. ```python import papermill as pm from papermill.iorw import
-papermill_io from papermill_origami import ClientConfig, NoteableClient,
-NoteableHandler domain = 'app.noteable.io' token = MY_TOKEN_VALUE_HERE file_id
-= '...' async with NoteableClient(token, config=ClientConfig(domain=domain)) as
-client: file = await client.get_notebook(file_id) papermill_io.register
-("noteable://", NoteableHandler(client)) pm.execute_notebook( f'noteable://
-{file_id}', None, engine_name='noteable', # Noteable-specific kwargs file=file,
-client=client, ) ``` ## Contributing See [CONTRIBUTING.md](./CONTRIBUTING.md).
--------
+(./CONTRIBUTING.md)  ## Intro to Papermill-Origami Papermill-Origami is the
+bridge library between the [Origami Noteable SDK](https://noteable-
+origami.readthedocs.io/en/latest/) and [Papermill](https://
+papermill.readthedocs.io/en/latest/). It build a papermill engine that can talk
+to Noteable APIs to run Notebooks.   ## Requirements Python 3.8+   ##
+Installation ### Poetry ```shell poetry add papermill-origami ``` ### Pip
+```shell pip install papermill-origami ```   ## Getting Started ### API Token
+Get your access token from your User Settings -> API Tokens or alternatively
+you can generate a post request to generate a new token ``` curl -X 'POST' \
+'https://app.noteable.io/gate/api/v1/tokens' \ -H 'accept: application/json' \
+-H 'Content-Type: application/json' \ -d '{ "ttl": 31536000, "name": "my_token"
+}' ``` ### Engine Registration The `noteable` engine keyword will use the
+following environment variables by default: ```bash NOTEABLE_DOMAIN =
+app.noteable.io NOTEABLE_TOKEN = MY_TOKEN_VALUE_HERE ``` Then the engine is
+enabled by running papermill as normal. But now you have access to the
+`noteable://` scheme as well as the ability to tell papermill to use Noteable
+as the execution location for your notebook. ```python import papermill as pm
+file_id = '...' pm.execute_notebook( f'noteable://{file_id}', None, # Set no
+particular output notebook, but a log of the resulting exeuction link still
+prints # This turns on the Noteable API interface engine_name='noteable', #
+exclude this kwarg to run the Notebook locally ) ``` #### Advanced Setup For
+more advanced control or reuse of a NoteableClient SDK object you can use the
+async await pattern around a client constructor. This reuses the connection
+throughout the life cycle of the context block. ```python import papermill as
+pm from papermill.iorw import papermill_io from papermill_origami import
+ClientConfig, NoteableClient, NoteableHandler domain = 'app.noteable.io' token
+= MY_TOKEN_VALUE_HERE file_id = '...' async with NoteableClient(token,
+config=ClientConfig(domain=domain)) as client: file = await client.get_notebook
+(file_id) papermill_io.register("noteable://", NoteableHandler(client))
+pm.execute_notebook( f'noteable://{file_id}', None, engine_name='noteable', #
+Noteable-specific kwargs file=file, client=client, ) ```  ## Contributing See
+[CONTRIBUTING.md](./CONTRIBUTING.md). -------
             Open sourced with â¤ï¸ by Noteable for the community.
 [Boost Data Collaboration with Notebooks]
```

