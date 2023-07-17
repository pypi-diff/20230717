# Comparing `tmp/aistudio-cognition-1.0.0.tar.gz` & `tmp/aistudio-cognition-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistudio-cognition-1.0.0.tar", max compression
+gzip compressed data, was "aistudio-cognition-1.0.1.tar", max compression
```

## Comparing `aistudio-cognition-1.0.0.tar` & `aistudio-cognition-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0    13695 2023-07-07 07:29:45.650324 aistudio-cognition-1.0.0/aistudio_cognition/cognibot/models.py
--rwxr-xr-x   0        0        0       46 2023-07-07 05:59:46.616048 aistudio-cognition-1.0.0/aistudio_cognition/models/__init__.py
--rwxr-xr-x   0        0        0      141 2023-07-07 05:59:31.101392 aistudio-cognition-1.0.0/aistudio_cognition/models/response_status.py
--rwxr-xr-x   0        0        0       82 2023-07-07 05:57:55.942375 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/__init__.py
--rwxr-xr-x   0        0        0     7053 2023-07-10 07:13:55.693451 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/luis.py
--rwxr-xr-x   0        0        0       47 2023-07-07 06:00:50.201223 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/models/__init__.py
--rwxr-xr-x   0        0        0      467 2023-07-06 12:49:28.814763 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/models/luis_settings.py
--rwxr-xr-x   0        0        0     2830 2023-07-07 07:48:13.419738 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/prediction.py
--rwxr-xr-x   0        0        0     5207 2023-07-07 07:52:11.957206 aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/rule.py
--rwxr-xr-x   0        0        0      674 2023-07-07 07:45:35.579002 aistudio-cognition-1.0.0/aistudio_cognition/nlu/models.py
--rwxr-xr-x   0        0        0      355 2023-07-10 06:56:35.687128 aistudio-cognition-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 aistudio-cognition-1.0.0/setup.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 aistudio-cognition-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0    13722 2023-07-17 08:16:25.347291 aistudio-cognition-1.0.1/aistudio_cognition/cognibot/models.py
+-rwxr-xr-x   0        0        0       46 2023-07-07 05:59:46.616048 aistudio-cognition-1.0.1/aistudio_cognition/models/__init__.py
+-rwxr-xr-x   0        0        0      141 2023-07-07 05:59:31.101392 aistudio-cognition-1.0.1/aistudio_cognition/models/response_status.py
+-rwxr-xr-x   0        0        0       82 2023-07-07 05:57:55.942375 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/__init__.py
+-rwxr-xr-x   0        0        0     7054 2023-07-10 09:46:56.521943 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/luis.py
+-rwxr-xr-x   0        0        0       47 2023-07-07 06:00:50.201223 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/models/__init__.py
+-rwxr-xr-x   0        0        0      467 2023-07-06 12:49:28.814763 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/models/luis_settings.py
+-rwxr-xr-x   0        0        0     2830 2023-07-07 07:48:13.419738 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/prediction.py
+-rwxr-xr-x   0        0        0     5207 2023-07-07 07:52:11.957206 aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/rule.py
+-rwxr-xr-x   0        0        0      674 2023-07-07 07:45:35.579002 aistudio-cognition-1.0.1/aistudio_cognition/nlu/models.py
+-rwxr-xr-x   0        0        0      355 2023-07-17 08:14:46.033498 aistudio-cognition-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 aistudio-cognition-1.0.1/setup.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 aistudio-cognition-1.0.1/PKG-INFO
```

### Comparing `aistudio-cognition-1.0.0/aistudio_cognition/cognibot/models.py` & `aistudio-cognition-1.0.1/aistudio_cognition/cognibot/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Model class for the chatbot which is pushed to the chatbot webservice.
 """
 import logging
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Optional, Union
 
-from aistudio_cognition.nlu.luis.models.luis_settings import LUIS
 from dataclasses_json import config, dataclass_json
 
+from aistudio_cognition.nlu.luis.models.luis_settings import LUIS
+
 logger = logging.getLogger(__name__)
 
 __version__ = "3.3.3"
 
 
 """ Enumerations
 """
@@ -475,14 +476,15 @@
 @dataclass_json
 @dataclass
 class Dialog:
     name: str
     elements: list[
         Union[Message, Input, Form, Card, Action, Branch, FileInput, SetState, Group]
     ]
+    description: str = ""
     has_feedback: bool = False
 
     def __post_init__(self):
         """
         Apparently, Dialog.from_dict() does not deserialize individual dialog elements.
         This is a workaround to deserialize every element in the Dialog manually.
         """
```

### Comparing `aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/luis.py` & `aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/luis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import logging
 from time import sleep
 from typing import Union
 
 import requests
-from aistudio_cognition.models.response_status import ResponseStatus
 from requests.exceptions import ConnectionError, HTTPError
 
+from aistudio_cognition.models.response_status import ResponseStatus
+
 from .models.luis_settings import LUIS
 from .prediction import format_prediction_response
 
 logger = logging.getLogger(__name__)
 
 
 class AIStudioNLULUIS:
```

### Comparing `aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/prediction.py` & `aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/prediction.py`

 * *Files identical despite different names*

### Comparing `aistudio-cognition-1.0.0/aistudio_cognition/nlu/luis/rule.py` & `aistudio-cognition-1.0.1/aistudio_cognition/nlu/luis/rule.py`

 * *Files identical despite different names*

### Comparing `aistudio-cognition-1.0.0/aistudio_cognition/nlu/models.py` & `aistudio-cognition-1.0.1/aistudio_cognition/nlu/models.py`

 * *Files identical despite different names*

### Comparing `aistudio-cognition-1.0.0/setup.py` & `aistudio-cognition-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dataclasses-json==0.5.6', 'requests==2.31.0']
 
 setup_kwargs = {
     'name': 'aistudio-cognition',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'NLU and KM prediction utility for AIStudio',
     'long_description': 'None',
     'author': 'Ankita Nair',
     'author_email': 'ankita.nair@automationedge.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

