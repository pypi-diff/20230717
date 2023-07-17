# Comparing `tmp/pegasusX-0.1.6.tar.gz` & `tmp/pegasusX-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.1.6.tar", last modified: Mon Jul 17 04:15:31 2023, max compression
+gzip compressed data, was "pegasusX-0.1.7.tar", last modified: Mon Jul 17 04:24:34 2023, max compression
```

## Comparing `pegasusX-0.1.6.tar` & `pegasusX-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:15:18.000000 pegasusX-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:15:31.721065 pegasusX-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:15:18.000000 pegasusX-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.717065 pegasusX-0.1.6/pegasus/oceandb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/pegasus/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-17 04:15:18.000000 pegasusX-0.1.6/pegasus/oceandb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:15:31.721065 pegasusX-0.1.6/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:15:31.000000 pegasusX-0.1.6/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:15:31.721065 pegasusX-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:15:18.000000 pegasusX-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.897679 pegasusX-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 04:24:20.000000 pegasusX-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:24:34.893679 pegasusX-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 04:24:20.000000 pegasusX-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.885679 pegasusX-0.1.7/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17618 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.889679 pegasusX-0.1.7/pegasus/oceandb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasus/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-17 04:24:20.000000 pegasusX-0.1.7/pegasus/oceandb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:24:34.893679 pegasusX-0.1.7/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 04:24:34.000000 pegasusX-0.1.7/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:24:34.897679 pegasusX-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 04:24:20.000000 pegasusX-0.1.7/setup.py
```

### Comparing `pegasusX-0.1.6/LICENSE` & `pegasusX-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/PKG-INFO` & `pegasusX-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.6
+Version: 0.1.7
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.6/README.md` & `pegasusX-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/pegasus/main.py` & `pegasusX-0.1.7/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/pegasus/oceandb/__init__.py` & `pegasusX-0.1.7/pegasus/oceandb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,31 @@
         ], f"Setting '{key}' is required when ocean_db_impl={setting}"
 
     if setting == "clickhouse":
         require("clickhouse_host")
         require("clickhouse_port")
         require("persist_directory")
         logger.info("Using Clickhouse for database")
-        import oceandb.db.clickhouse
+        import pegasus.oceandb.db.clickhouse
 
         return oceandb.db.clickhouse.Clickhouse(settings)
     elif setting == "duckdb+parquet":
         require("persist_directory")
         logger.warning(
             f"Using embedded DuckDB with persistence: data will be stored in: {settings.persist_directory}"
         )
-        import oceandb.db.duckdb
+        import pegasus.oceandb.db.duckdb
 
         return oceandb.db.duckdb.PersistentDuckDB(settings)
     elif setting == "duckdb":
         require("persist_directory")
         logger.warning(
             "Using embedded DuckDB without persistence: data will be transient"
         )
-        import oceandb.db.duckdb
+        import pegasus.oceandb.db.duckdb
 
         return oceandb.db.duckdb.DuckDB(settings)
     else:
         raise ValueError(
             f"Expected ocean_db_impl to be one of clickhouse, duckdb, duckdb+parquet, got {setting}"
         )
 
@@ -79,19 +79,19 @@
 
     if setting == "rest":
         require("ocean_server_host")
         require("ocean_server_http_port")
         logger.info(
             "Running Ocean in client mode using REST to connect to remote server"
         )
-        import oceandb.api.fastapi
+        import pegasus.oceandb.api.fastapi
 
         return oceandb.api.fastapi.FastAPI(settings, telemetry_client)
     elif setting == "local":
         logger.info("Running Ocean using direct local API.")
-        import oceandb.api.local
+        import pegasus.oceandb.api.local
 
         return oceandb.api.local.LocalAPI(settings, get_db(settings), telemetry_client)
     else:
         raise ValueError(
             f"Expected ocean_api_impl to be one of rest, local, got {setting}"
         )
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/api/__init__.py` & `pegasusX-0.1.7/pegasus/oceandb/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import ABC, abstractmethod
 from typing import Callable, Sequence, Optional, Dict
 import pandas as pd
 from uuid import UUID
-from oceandb.api.models.Collection import Collection
-from oceandb.api.types import (
+import pegasus.oceandb.api.models.Collection import Collection
+import pegasus.oceandb.api.types import (
     Documents,
     Embeddings,
     IDs,
     Include,
     Metadatas,
     Where,
     QueryResult,
     GetResult,
     WhereDocument,
 )
 
-from oceandb.telemetry import Telemetry
+import pegasus.oceandb.telemetry import Telemetry
 
 
 class API(ABC):
     @abstractmethod
     def __init__(self, telemetry_client: Telemetry):
         pass
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/api/fastapi.py` & `pegasusX-0.1.7/pegasus/oceandb/api/fastapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Dict, List, Optional
-from oceandb.api import API
-from oceandb.api.types import (
+import pegasus.oceandb.api import API
+import pegasus.oceandb.api.types import (
     CrossModalRetrieval,
     Documents,
     Embeddings,
     Embedding,
     IDs,
     Include,
     Metadatas,
@@ -13,17 +13,17 @@
     Where,
     WhereDocument,
 )
 import pandas as pd
 import requests
 import json
 from typing import Sequence, List, Any
-from oceandb.api.models.Collection import Collection
-from oceandb.telemetry import Telemetry
-import oceandb.errors as errors
+import pegasus.oceandb.api.models.Collection import Collection
+import pegasus.oceandb.telemetry import Telemetry
+import pegasus.oceandb.errors as errors
 from uuid import UUID
 
 
 class FastAPI(API):
     def __init__(self, settings, telemetry_client: Telemetry):
         url_prefix = "https" if settings.ocean_server_ssl_enabled else "http"
         self._api_url = f"{url_prefix}://{settings.ocean_server_host}:{settings.ocean_server_http_port}/api/v1"
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/api/local.py` & `pegasusX-0.1.7/pegasus/oceandb/api/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
 import time
 from uuid import UUID
 from typing import Dict, List, Optional, Sequence, Callable, cast
-from oceandb import __version__
-import oceandb.errors as errors
-from oceandb.api import API
-from oceandb.db import DB
-from oceandb.api.types import (
+import pegasus.oceandb import __version__
+import pegasus.oceandb.errors as errors
+import pegasus.oceandb.api import API
+import pegasus.oceandb.db import DB
+import pegasus.oceandb.api.types import (
     Documents,
     Embeddings,
     GetResult,
     IDs,
     Include,
     Metadatas,
     QueryResult,
     Where,
     WhereDocument,
 )
-from oceandb.api.models.Collection import Collection
+import pegasus.oceandb.api.models.Collection import Collection
 
 import re
 
-from oceandb.telemetry import Telemetry
-from oceandb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
+import pegasus.oceandb.telemetry import Telemetry
+import pegasus.oceandb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
 
 
 # mimics s3 bucket requirements for naming
 def check_index_name(index_name):
     msg = (
         "Expected collection name that "
         "(1) contains 3-63 characters, "
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/api/types.py` & `pegasusX-0.1.7/pegasus/oceandb/api/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union, Dict, Sequence, TypeVar, List
 from typing_extensions import Literal, TypedDict, Protocol
-import oceandb.errors as errors
+import pegasus.oceandb.errors as errors
 from abc import ABC, abstractmethod
 import torch.nn as nn
 
 # from ..utils.ImageBind.imagebind_model import ModalityType
 from ..utils.ImageBind.models.imagebind_model import ModalityType
 import numpy as np
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/config.py` & `pegasusX-0.1.7/pegasus/oceandb/config.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/pegasus/oceandb/db/__init__.py` & `pegasusX-0.1.7/pegasus/oceandb/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Dict, List, Sequence, Optional, Tuple
 from uuid import UUID
 import numpy.typing as npt
-from oceandb.api.types import (
+import pegasus.oceandb.api.types import (
     Embeddings,
     Documents,
     IDs,
     Metadatas,
     Where,
     WhereDocument,
 )
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/db/clickhouse.py` & `pegasusX-0.1.7/pegasus/oceandb/db/clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # type: ignore
-from oceandb.api.types import (
+import pegasus.oceandb.api.types import (
     Documents,
     Embeddings,
     IDs,
     Metadatas,
     Where,
     WhereDocument,
 )
-from oceandb.db import DB
-from oceandb.db.index.hnswlib import Hnswlib, delete_all_indexes
-from oceandb.errors import (
+import pegasus.oceandb.db import DB
+import pegasus.oceandb.db.index.hnswlib import Hnswlib, delete_all_indexes
+import pegasus.oceandb.errors import (
     NoDatapointsException,
 )
 import uuid
 import numpy.typing as npt
 import json
 from typing import Dict, Optional, Sequence, List, Tuple, cast
 import clickhouse_connect
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/db/duckdb.py` & `pegasusX-0.1.7/pegasus/oceandb/db/duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from oceandb.api.types import Documents, Embeddings, IDs, Metadatas
-from oceandb.db.clickhouse import (
+import pegasus.oceandb.api.types import Documents, Embeddings, IDs, Metadatas
+import pegasus.oceandb.db.clickhouse import (
     Clickhouse,
     db_array_schema_to_clickhouse_schema,
     EMBEDDING_TABLE_SCHEMA,
     db_schema_to_keys,
     COLLECTION_TABLE_SCHEMA,
 )
 from typing import List, Optional, Sequence, Dict
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/db/index/hnswlib.py` & `pegasusX-0.1.7/pegasus/oceandb/db/index/hnswlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import pickle
 import time
 from typing import Dict
 
-from oceandb.api.types import IndexMetadata
+import pegasus.oceandb.api.types import IndexMetadata
 import hnswlib
-from oceandb.db.index import Index
-from oceandb.errors import (
+import pegasus.oceandb.db.index import Index
+import pegasus.oceandb.errors import (
     NoIndexException,
     InvalidDimensionException,
     NotEnoughElementsException,
 )
 import logging
 import re
 from uuid import UUID
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/errors.py` & `pegasusX-0.1.7/pegasus/oceandb/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/pegasus/oceandb/server/fastapi/__init__.py` & `pegasusX-0.1.7/pegasus/oceandb/server/fastapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from fastapi.responses import JSONResponse
 
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.routing import APIRoute
 from fastapi import HTTPException, status
 from uuid import UUID
 
-import oceandb
-import oceandb.server
-import oceandb.api
-from oceandb.errors import (
+import pegasus.oceandb
+import pegasus.oceandb.server
+import pegasus.oceandb.api
+import pegasus.oceandb.errors import (
     OceanError,
     InvalidUUIDError,
     InvalidDimensionException,
 )
-from oceandb.server.fastapi.types import (
+import pegasus.oceandb.server.fastapi.types import (
     AddEmbedding,
     DeleteEmbedding,
     GetEmbedding,
     QueryEmbedding,
     RawSql,  # Results,
     CreateCollection,
     UpdateCollection,
     UpdateEmbedding,
 )
 from starlette.requests import Request
 
 import logging
-from oceandb.telemetry import ServerContext, Telemetry
+import pegasus.oceandb.telemetry import ServerContext, Telemetry
 
 logger = logging.getLogger(__name__)
 
 
 def use_route_names_as_operation_ids(app: _FastAPI) -> None:
     """
     Simplify operation IDs so that generated API clients have simpler function
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/server/fastapi/types.py` & `pegasusX-0.1.7/pegasus/oceandb/server/fastapi/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel
 from typing import List, Union
-from oceandb.api.types import Include
+import pegasus.oceandb.api.types import Include
 
 
 # type supports single and batch mode
 class AddEmbedding(BaseModel):
     embeddings: List
     metadatas: Union[List, dict] = None
     documents: Union[str, List] = None
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/telemetry/__init__.py` & `pegasusX-0.1.7/pegasus/oceandb/telemetry/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import abstractmethod
 from dataclasses import asdict, dataclass
 import os
 from typing import Callable, ClassVar
 import uuid
 import time
 from threading import Event, Thread
-import oceandb
+import pegasus.oceandb
 from pathlib import Path
-from oceandb.config import TELEMETRY_WHITELISTED_SETTINGS, Settings
+import pegasus.oceandb.config import TELEMETRY_WHITELISTED_SETTINGS, Settings
 from enum import Enum
 
 
 class ServerContext(Enum):
     NONE = "None"
     FASTAPI = "FastAPI"
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/telemetry/events.py` & `pegasusX-0.1.7/pegasus/oceandb/telemetry/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from typing import ClassVar
-from oceandb.telemetry import TelemetryEvent
+import pegasus.oceandb.telemetry import TelemetryEvent
 
 
 @dataclass
 class ClientStartEvent(TelemetryEvent):
     name: ClassVar[str] = "client_start"
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/telemetry/posthog.py` & `pegasusX-0.1.7/pegasus/oceandb/telemetry/posthog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import posthog
 import logging
 import sys
-from oceandb.config import Settings
-from oceandb.telemetry import Telemetry, TelemetryEvent
+import pegasus.oceandb.config import Settings
+import pegasus.oceandb.telemetry import Telemetry, TelemetryEvent
 
 logger = logging.getLogger(__name__)
 
 
 class Posthog(Telemetry):
     def __init__(self, settings: Settings):
         if not settings.anonymized_telemetry or "pytest" in sys.modules:
```

### Comparing `pegasusX-0.1.6/pegasus/oceandb/utils/embedding_functions.py` & `pegasusX-0.1.7/pegasus/oceandb/utils/embedding_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from oceandb.api.types import Documents, EmbeddingFunction, Embeddings
+import pegasus.oceandb.api.types import Documents, EmbeddingFunction, Embeddings
 from typing import Optional
 import torch
 from .ImageBind.models import imagebind_model
 from .ImageBind.models.imagebind_model import ModalityType
 from .ImageBind.data import load_and_transform_text, load_and_transform_vision_data, load_and_transform_audio_data
 
 class SentenceTransformerEmbeddingFunction(EmbeddingFunction):
```

### Comparing `pegasusX-0.1.6/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.1.7/pegasusX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.1.6
+Version: 0.1.7
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.1.6/pegasusX.egg-info/SOURCES.txt` & `pegasusX-0.1.7/pegasusX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusX-0.1.6/setup.py` & `pegasusX-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

